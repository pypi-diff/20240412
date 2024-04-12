# Comparing `tmp/bbrc-pyxnat-1.6.2.tar.gz` & `tmp/bbrc-pyxnat-1.6.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbrc-pyxnat-1.6.2.tar", last modified: Mon Jan 29 09:17:37 2024, max compression
+gzip compressed data, was "bbrc-pyxnat-1.6.3.dev1.tar", last modified: Fri Apr 12 09:02:58 2024, max compression
```

## Comparing `bbrc-pyxnat-1.6.2.tar` & `bbrc-pyxnat-1.6.3.dev1.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxrwxrwx   0        0        0        0 2024-01-29 09:17:37.534489 bbrc-pyxnat-1.6.2/
--rw-rw-rw-   0        0        0     1663 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/LICENSE
--rw-rw-rw-   0        0        0     5449 2024-01-29 09:17:37.533490 bbrc-pyxnat-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     4424 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-01-29 09:17:37.531493 bbrc-pyxnat-1.6.2/bbrc_pyxnat.egg-info/
--rw-rw-rw-   0        0        0     5449 2024-01-29 09:17:36.000000 bbrc-pyxnat-1.6.2/bbrc_pyxnat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2230 2024-01-29 09:17:36.000000 bbrc-pyxnat-1.6.2/bbrc_pyxnat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-29 09:17:36.000000 bbrc-pyxnat-1.6.2/bbrc_pyxnat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-01-29 09:17:36.000000 bbrc-pyxnat-1.6.2/bbrc_pyxnat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-01-29 09:17:36.000000 bbrc-pyxnat-1.6.2/bbrc_pyxnat.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-29 09:17:36.797481 bbrc-pyxnat-1.6.2/bin/
--rw-rw-rw-   0        0        0    25198 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/bin/sessionmirror.py
-drwxrwxrwx   0        0        0        0 2024-01-29 09:17:36.807412 bbrc-pyxnat-1.6.2/pyxnat/
--rw-rw-rw-   0        0        0      695 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 09:17:37.084115 bbrc-pyxnat-1.6.2/pyxnat/core/
--rw-rw-rw-   0        0        0      153 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/__init__.py
--rw-rw-rw-   0        0        0     9938 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/array.py
--rw-rw-rw-   0        0        0     6300 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/attributes.py
-drwxrwxrwx   0        0        0        0 2024-01-29 09:17:37.264579 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/
--rw-rw-rw-   0        0        0     1758 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/__init__.py
--rw-rw-rw-   0        0        0     1026 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/ashs.py
--rw-rw-rw-   0        0        0     7798 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/bamos.py
--rw-rw-rw-   0        0        0     2649 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/basil.py
--rw-rw-rw-   0        0        0     1195 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/cat12.py
--rw-rw-rw-   0        0        0      587 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/dicom.py
--rw-rw-rw-   0        0        0      194 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/donsurf.py
--rw-rw-rw-   0        0        0      614 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/dtifit.py
--rw-rw-rw-   0        0        0     6651 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/freesurfer.py
--rw-rw-rw-   0        0        0     2159 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/freesurfer7_extras.py
--rw-rw-rw-   0        0        0     1083 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/mrtrix3.py
--rw-rw-rw-   0        0        0     1065 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/pet_fdg.py
--rw-rw-rw-   0        0        0      488 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/pet_ftm.py
--rw-rw-rw-   0        0        0      930 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/qsxmt.py
--rw-rw-rw-   0        0        0     1136 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/spm12.py
--rw-rw-rw-   0        0        0     3381 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/validator.py
--rw-rw-rw-   0        0        0      828 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/xcp_d.py
--rw-rw-rw-   0        0        0     7954 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/downloadutils.py
--rw-rw-rw-   0        0        0     3517 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/errors.py
--rw-rw-rw-   0        0        0    22552 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/help.py
--rw-rw-rw-   0        0        0      597 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/httputil.py
--rw-rw-rw-   0        0        0    20139 2024-01-27 17:34:57.000000 bbrc-pyxnat-1.6.2/pyxnat/core/interfaces.py
--rw-rw-rw-   0        0        0     9999 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/jsonutil.py
--rw-rw-rw-   0        0        0    10873 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/manage.py
--rw-rw-rw-   0        0        0      775 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/pathutil.py
--rw-rw-rw-   0        0        0    14803 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/pipelines.py
--rw-rw-rw-   0        0        0    10017 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/provenance.py
--rw-rw-rw-   0        0        0    88934 2024-01-27 17:34:57.000000 bbrc-pyxnat-1.6.2/pyxnat/core/resources.py
--rw-rw-rw-   0        0        0     5281 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/schema.py
--rw-rw-rw-   0        0        0    26480 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/search.py
--rw-rw-rw-   0        0        0    11899 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/select.py
--rw-rw-rw-   0        0        0     3633 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/tags.py
--rw-rw-rw-   0        0        0     4272 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/uriutil.py
--rw-rw-rw-   0        0        0     2506 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/users.py
--rw-rw-rw-   0        0        0     2094 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/xpass.py
--rw-rw-rw-   0        0        0     5038 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/core/xpath_store.py
-drwxrwxrwx   0        0        0        0 2024-01-29 09:17:37.529498 bbrc-pyxnat-1.6.2/pyxnat/tests/
--rw-rw-rw-   0        0        0      605 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/__init__.py
--rw-rw-rw-   0        0        0     2666 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/array_test.py
--rw-rw-rw-   0        0        0     3591 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/attributes_test.py
--rw-rw-rw-   0        0        0     1150 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/custom_variables_test.py
--rw-rw-rw-   0        0        0      501 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/downloadutils_test.py
--rw-rw-rw-   0        0        0      378 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/experiments_test.py
--rw-rw-rw-   0        0        0      514 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/graphdata_test.py
--rw-rw-rw-   0        0        0      269 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/inspector_test.py
--rw-rw-rw-   0        0        0     2584 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/interfaces_test.py
--rw-rw-rw-   0        0        0     1437 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/jsonutil_test.py
--rw-rw-rw-   0        0        0      779 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/manage_test.py
--rw-rw-rw-   0        0        0      123 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/pathutil_test.py
--rw-rw-rw-   0        0        0     1843 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/pipelines_test.py
--rw-rw-rw-   0        0        0      570 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/prearchive_test.py
--rw-rw-rw-   0        0        0      288 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/project_manager_test.py
--rw-rw-rw-   0        0        0     1125 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/provenance_test.py
--rw-rw-rw-   0        0        0     5081 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/repr_test.py
--rw-rw-rw-   0        0        0    11631 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/resources_test.py
--rw-rw-rw-   0        0        0      383 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/scans_test.py
--rw-rw-rw-   0        0        0     3084 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/search_test.py
--rw-rw-rw-   0        0        0     3263 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/select_test.py
--rw-rw-rw-   0        0        0     1714 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/sessionmirror_test.py
--rw-rw-rw-   0        0        0     7672 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/test_resource_functions.py
--rw-rw-rw-   0        0        0     1782 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/uriutil_test.py
--rw-rw-rw-   0        0        0     7271 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/user_and_project_management_test.py
--rw-rw-rw-   0        0        0     1504 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/xpass_test.py
--rw-rw-rw-   0        0        0      973 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/tests/xpath_test.py
--rw-rw-rw-   0        0        0       19 2024-01-26 14:26:27.000000 bbrc-pyxnat-1.6.2/pyxnat/version.py
--rw-rw-rw-   0        0        0      295 2024-01-29 09:17:37.543466 bbrc-pyxnat-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0     2420 2024-01-29 09:15:38.000000 bbrc-pyxnat-1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:02:58.162367 bbrc-pyxnat-1.6.3.dev1/
+-rw-rw-rw-   0        0        0     1631 2022-09-16 14:24:20.000000 bbrc-pyxnat-1.6.3.dev1/LICENSE
+-rw-rw-rw-   0        0        0     5454 2024-04-12 09:02:58.159782 bbrc-pyxnat-1.6.3.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     4424 2023-08-16 13:20:38.000000 bbrc-pyxnat-1.6.3.dev1/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-12 09:02:58.154502 bbrc-pyxnat-1.6.3.dev1/bbrc_pyxnat.egg-info/
+-rw-rw-rw-   0        0        0     5454 2024-04-12 09:02:57.000000 bbrc-pyxnat-1.6.3.dev1/bbrc_pyxnat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2263 2024-04-12 09:02:57.000000 bbrc-pyxnat-1.6.3.dev1/bbrc_pyxnat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 09:02:57.000000 bbrc-pyxnat-1.6.3.dev1/bbrc_pyxnat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-04-12 09:02:57.000000 bbrc-pyxnat-1.6.3.dev1/bbrc_pyxnat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-12 09:02:57.000000 bbrc-pyxnat-1.6.3.dev1/bbrc_pyxnat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 09:02:57.838575 bbrc-pyxnat-1.6.3.dev1/bin/
+-rw-rw-rw-   0        0        0    25198 2024-04-08 14:41:00.000000 bbrc-pyxnat-1.6.3.dev1/bin/sessionmirror.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:02:57.847811 bbrc-pyxnat-1.6.3.dev1/pyxnat/
+-rw-rw-rw-   0        0        0      666 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:02:57.942332 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/
+-rw-rw-rw-   0        0        0      148 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/__init__.py
+-rw-rw-rw-   0        0        0     9682 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/array.py
+-rw-rw-rw-   0        0        0     6300 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/attributes.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:02:58.016050 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/
+-rw-rw-rw-   0        0        0      520 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/3dasl.py
+-rw-rw-rw-   0        0        0     1758 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/__init__.py
+-rw-rw-rw-   0        0        0     1026 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/ashs.py
+-rw-rw-rw-   0        0        0     7798 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/bamos.py
+-rw-rw-rw-   0        0        0     2649 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/basil.py
+-rw-rw-rw-   0        0        0     1195 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/cat12.py
+-rw-rw-rw-   0        0        0      587 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/dicom.py
+-rw-rw-rw-   0        0        0      194 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/donsurf.py
+-rw-rw-rw-   0        0        0      614 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/dtifit.py
+-rw-rw-rw-   0        0        0     6651 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/freesurfer.py
+-rw-rw-rw-   0        0        0     2159 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/freesurfer7_extras.py
+-rw-rw-rw-   0        0        0     1083 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/mrtrix3.py
+-rw-rw-rw-   0        0        0     1065 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/pet_fdg.py
+-rw-rw-rw-   0        0        0      488 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/pet_ftm.py
+-rw-rw-rw-   0        0        0      930 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/qsxmt.py
+-rw-rw-rw-   0        0        0     1136 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/spm12.py
+-rw-rw-rw-   0        0        0     3381 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/validator.py
+-rw-rw-rw-   0        0        0      828 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/xcp_d.py
+-rw-rw-rw-   0        0        0     7751 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/downloadutils.py
+-rw-rw-rw-   0        0        0     3517 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/errors.py
+-rw-rw-rw-   0        0        0    21861 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/help.py
+-rw-rw-rw-   0        0        0      576 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/httputil.py
+-rw-rw-rw-   0        0        0    20139 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/interfaces.py
+-rw-rw-rw-   0        0        0     9999 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/jsonutil.py
+-rw-rw-rw-   0        0        0    10565 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/manage.py
+-rw-rw-rw-   0        0        0      745 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/pathutil.py
+-rw-rw-rw-   0        0        0    14803 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/pipelines.py
+-rw-rw-rw-   0        0        0     9708 2024-01-24 17:01:35.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/provenance.py
+-rw-rw-rw-   0        0        0    88934 2024-01-26 16:56:07.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/resources.py
+-rw-rw-rw-   0        0        0     5281 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/schema.py
+-rw-rw-rw-   0        0        0    26480 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/search.py
+-rw-rw-rw-   0        0        0    11517 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/select.py
+-rw-rw-rw-   0        0        0     3509 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/tags.py
+-rw-rw-rw-   0        0        0     4113 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/uriutil.py
+-rw-rw-rw-   0        0        0     2424 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/users.py
+-rw-rw-rw-   0        0        0     2094 2023-08-16 13:20:38.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/xpass.py
+-rw-rw-rw-   0        0        0     4876 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/core/xpath_store.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:02:58.147551 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/
+-rw-rw-rw-   0        0        0      605 2024-01-22 14:58:16.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/__init__.py
+-rw-rw-rw-   0        0        0     2666 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/array_test.py
+-rw-rw-rw-   0        0        0     3591 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/attributes_test.py
+-rw-rw-rw-   0        0        0     1150 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/custom_variables_test.py
+-rw-rw-rw-   0        0        0      511 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/downloadutils_test.py
+-rw-rw-rw-   0        0        0      378 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/experiments_test.py
+-rw-rw-rw-   0        0        0      514 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/graphdata_test.py
+-rw-rw-rw-   0        0        0      269 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/inspector_test.py
+-rw-rw-rw-   0        0        0     2584 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/interfaces_test.py
+-rw-rw-rw-   0        0        0     1384 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/jsonutil_test.py
+-rw-rw-rw-   0        0        0      779 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/manage_test.py
+-rw-rw-rw-   0        0        0      119 2024-01-17 15:10:29.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/pathutil_test.py
+-rw-rw-rw-   0        0        0     1843 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/pipelines_test.py
+-rw-rw-rw-   0        0        0      570 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/prearchive_test.py
+-rw-rw-rw-   0        0        0      288 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/project_manager_test.py
+-rw-rw-rw-   0        0        0     1125 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/provenance_test.py
+-rw-rw-rw-   0        0        0     5081 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/repr_test.py
+-rw-rw-rw-   0        0        0    11631 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/resources_test.py
+-rw-rw-rw-   0        0        0      383 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/scans_test.py
+-rw-rw-rw-   0        0        0     3009 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/search_test.py
+-rw-rw-rw-   0        0        0     3199 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/select_test.py
+-rw-rw-rw-   0        0        0     1714 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/sessionmirror_test.py
+-rw-rw-rw-   0        0        0     8214 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/test_resource_functions.py
+-rw-rw-rw-   0        0        0     1731 2022-09-16 14:24:22.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/uriutil_test.py
+-rw-rw-rw-   0        0        0     7271 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/user_and_project_management_test.py
+-rw-rw-rw-   0        0        0     1504 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/xpass_test.py
+-rw-rw-rw-   0        0        0      973 2024-01-26 16:46:14.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/xpath_test.py
+-rw-rw-rw-   0        0        0       24 2024-04-12 08:58:52.000000 bbrc-pyxnat-1.6.3.dev1/pyxnat/version.py
+-rw-rw-rw-   0        0        0      295 2024-04-12 09:02:58.180377 bbrc-pyxnat-1.6.3.dev1/setup.cfg
+-rw-rw-rw-   0        0        0     2420 2024-04-12 07:57:20.000000 bbrc-pyxnat-1.6.3.dev1/setup.py
```

### Comparing `bbrc-pyxnat-1.6.2/LICENSE` & `bbrc-pyxnat-1.6.3.dev1/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-This software is OSI Certified Open Source Software.
-OSI Certified is a certification mark of the Open Source Initiative.
-
-Copyright (c) 2010-2011, Yannick Schwartz
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice,
-  this list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of Yannick Schwartz. nor the names of other pyxnat
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-**This software is provided by the copyright holders and contributors
-"as is" and any express or implied warranties, including, but not
-limited to, the implied warranties of merchantability and fitness for
-a particular purpose are disclaimed. In no event shall the copyright
-owner or contributors be liable for any direct, indirect, incidental,
-special, exemplary, or consequential damages (including, but not
-limited to, procurement of substitute goods or services; loss of use,
-data, or profits; or business interruption) however caused and on any
-theory of liability, whether in contract, strict liability, or tort
-(including negligence or otherwise) arising in any way out of the use
-of this software, even if advised of the possibility of such
-damage.**
+This software is OSI Certified Open Source Software.
+OSI Certified is a certification mark of the Open Source Initiative.
+
+Copyright (c) 2010-2011, Yannick Schwartz
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice,
+  this list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of Yannick Schwartz. nor the names of other pyxnat
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+**This software is provided by the copyright holders and contributors
+"as is" and any express or implied warranties, including, but not
+limited to, the implied warranties of merchantability and fitness for
+a particular purpose are disclaimed. In no event shall the copyright
+owner or contributors be liable for any direct, indirect, incidental,
+special, exemplary, or consequential damages (including, but not
+limited to, procurement of substitute goods or services; loss of use,
+data, or profits; or business interruption) however caused and on any
+theory of liability, whether in contract, strict liability, or tort
+(including negligence or otherwise) arising in any way out of the use
+of this software, even if advised of the possibility of such
+damage.**
```

### Comparing `bbrc-pyxnat-1.6.2/PKG-INFO` & `bbrc-pyxnat-1.6.3.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbrc-pyxnat
-Version: 1.6.2
+Version: 1.6.3.dev1
 Summary: XNAT in Python
 Home-page: https://github.com/pyxnat/pyxnat
 Author: Yannick Schwartz
 Author-email: yannick.schwartz@cea.fr
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bbrc-pyxnat-1.6.2/README.rst` & `bbrc-pyxnat-1.6.3.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/bbrc_pyxnat.egg-info/PKG-INFO` & `bbrc-pyxnat-1.6.3.dev1/bbrc_pyxnat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbrc-pyxnat
-Version: 1.6.2
+Version: 1.6.3.dev1
 Summary: XNAT in Python
 Home-page: https://github.com/pyxnat/pyxnat
 Author: Yannick Schwartz
 Author-email: yannick.schwartz@cea.fr
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bbrc-pyxnat-1.6.2/bbrc_pyxnat.egg-info/SOURCES.txt` & `bbrc-pyxnat-1.6.3.dev1/bbrc_pyxnat.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 pyxnat/core/search.py
 pyxnat/core/select.py
 pyxnat/core/tags.py
 pyxnat/core/uriutil.py
 pyxnat/core/users.py
 pyxnat/core/xpass.py
 pyxnat/core/xpath_store.py
+pyxnat/core/derivatives/3dasl.py
 pyxnat/core/derivatives/__init__.py
 pyxnat/core/derivatives/ashs.py
 pyxnat/core/derivatives/bamos.py
 pyxnat/core/derivatives/basil.py
 pyxnat/core/derivatives/cat12.py
 pyxnat/core/derivatives/dicom.py
 pyxnat/core/derivatives/donsurf.py
```

### Comparing `bbrc-pyxnat-1.6.2/bin/sessionmirror.py` & `bbrc-pyxnat-1.6.3.dev1/bin/sessionmirror.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/__init__.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/__init__.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-"""
-PyXNAT
-======
-
-:mod:`pyxnat` provides an API to access data on XNAT servers
-(see http://xnat.org).
-
-Visit https://pyxnat.github.io/pyxnat for more information.
-"""
-
-from .version import VERSION as __version__
-
-from .core import Interface
-from .core import SearchManager
-from .core import Select
-from .core import Inspector
-from .core import Users
-from .core import attributes
-from .core import help
-from .core import interfaces
-from .core import resources
-from .core import manage
-from .core import schema
-from .core import select
-from .core import users
-from .core import jsonutil
-from .core import uriutil
-from .core import xpass
-from .core import xpath_store
+"""
+PyXNAT
+======
+
+:mod:`pyxnat` provides an API to access data on XNAT servers
+(see http://xnat.org).
+
+Visit https://pyxnat.github.io/pyxnat for more information.
+"""
+
+from .version import VERSION as __version__
+
+from .core import Interface
+from .core import SearchManager
+from .core import Select
+from .core import Inspector
+from .core import Users
+from .core import attributes
+from .core import help
+from .core import interfaces
+from .core import resources
+from .core import manage
+from .core import schema
+from .core import select
+from .core import users
+from .core import jsonutil
+from .core import uriutil
+from .core import xpass
+from .core import xpath_store
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/array.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/array.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,256 +1,256 @@
-from .jsonutil import JsonTable
-
-
-class ArrayData(object):
-
-    def __init__(self, interface):
-        self._intf = interface
-
-    def _get_array(self, query_string, project_id=None,
-                   subject_id=None, subject_label=None,
-                   experiment_id=None, experiment_label=None,
-                   experiment_type='xnat:subjectAssessorData',
-                   columns=None, constraints=None
-                   ):
-
-        if constraints is None:
-            constraints = {}
-
-        uri = '%s/experiments?xsiType=%s' % (self._intf._get_entry_point(),
-                                             experiment_type)
-
-        if project_id is not None:
-            uri += '&project=%s' % project_id
-
-        if subject_id is not None:
-            uri += '&%s/subject_id=%s' % (experiment_type, subject_id)
-
-        # Subject Label is only held in the xnat:subjectData so look for it
-        # there. This should join against whatever the experiment type is.
-        if subject_label is not None:
-            uri += '&xnat:subjectData/label=%s' % (subject_label)
-
-        if experiment_id is not None:
-            uri += '&ID=%s' % experiment_id
-
-        if experiment_label is not None:
-            uri += '&label=%s' % experiment_label
-
-        uri += query_string
-
-        if constraints != {}:
-            uri += ',' + ','.join(constraints.keys())
-
-        if columns is not None:
-            uri += ',' + ','.join(columns)
-
-        c = {}
-
-        [c.setdefault(key.lower(), value)
-         for key, value in constraints.items()
-         ]
-
-        return JsonTable(self._intf._get_json(uri)).where(**c)
-
-    def experiments(self, project_id=None, subject_id=None, subject_label=None,
-                    experiment_id=None, experiment_label=None,
-                    experiment_type='xnat:subjectAssessorData',
-                    columns=None,
-                    constraints=None):
-
-        """ Returns a list of all visible experiment IDs of the specified
-            type, filtered by optional constraints.
-
-            Parameters
-            ----------
-            project_id: string
-                Name pattern to filter by project ID.
-            subject_id: string
-                Name pattern to filter by subject ID.
-            subject_label: string
-                Name pattern to filter by subject ID.
-            experiment_id: string
-                Name pattern to filter by experiment ID.
-            experiment_label: string
-                Name pattern to filter by experiment ID.
-            experiment_type: string
-                xsi path type; e.g. 'xnat:mrSessionData'
-            columns: list
-                Values to return.
-            constraints: dict
-                Dictionary of xsi_type (key--) and parameter (--value)
-                pairs by which to filter.
-            """
-
-        query_string = '&columns=ID,project,%s/subject_id' % experiment_type
-
-        return self._get_array(query_string, project_id,
-                               subject_id, subject_label,
-                               experiment_id, experiment_label,
-                               experiment_type, columns, constraints
-                               )
-
-    def mrsessions(self, project_id=None, subject_id=None, subject_label=None,
-                   experiment_id=None, experiment_label=None,
-                   columns=None,
-                   constraints=None):
-
-        """ Returns a list of all MR sessions, filtered by optional constraints.
-
-            Parameters
-            ----------
-            project_id: string
-                Name pattern to filter by project ID.
-            subject_id: string
-                Name pattern to filter by subject ID.
-            subject_label: string
-                Name pattern to filter by subject ID.
-            experiment_id: string
-                Name pattern to filter by experiment ID.
-            experiment_label: string
-                Name pattern to filter by experiment ID.
-            columns: list
-                Values to return.
-            constraints: dict
-                Dictionary of xsi_type (key--) and parameter (--value)
-                pairs by which to filter.
-            """
-
-        return self.experiments(project_id, subject_id, subject_label,
-                                experiment_id, experiment_label,
-                                'xnat:mrSessionData', columns, constraints
-                                )
-
-    def scans(self, project_id=None, subject_id=None, subject_label=None,
-              experiment_id=None, experiment_label=None,
-              experiment_type='xnat:imageSessionData',
-              scan_type='xnat:imageScanData',
-              columns=None,
-              constraints=None
-              ):
-
-        """ Returns a list of all visible scan IDs of the specified type,
-            filtered by optional constraints.
-
-            Parameters
-            ----------
-            project_id: string
-                Name pattern to filter by project ID.
-            subject_id: string
-                Name pattern to filter by subject ID.
-            subject_label: string
-                Name pattern to filter by subject ID.
-            experiment_id: string
-                Name pattern to filter by experiment ID.
-            experiment_label: string
-                Name pattern to filter by experiment ID.
-            experiment_type: string
-                xsi path type; e.g. 'xnat:mrSessionData'
-            scan_type: string
-                xsi path type; e.g. 'xnat:mrScanData', etc.
-            columns: list
-                Values to return.
-            constraints: dict
-                Dictionary of xsi_type (key--) and parameter (--value)
-                pairs by which to filter.
-            """
-
-        query_string = '&columns=ID,project,%s/subject_id,%s/ID' % (
-            experiment_type, scan_type)
-
-        array = self._get_array(query_string, project_id,
-                                subject_id, subject_label,
-                                experiment_id, experiment_label,
-                                experiment_type, columns, constraints)
-        id_key = ('%s/ID' % scan_type).lower()
-        return JsonTable([i for i in array if i[id_key]])
-
-    def mrscans(self, project_id=None, subject_id=None, subject_label=None,
-                experiment_id=None, experiment_label=None,
-                columns=None,
-                constraints=None):
-
-        """ Returns a list of all MR scans, filtered by optional constraints.
-
-            Parameters
-            ----------
-            project_id: string
-                Name pattern to filter by project ID.
-            subject_id: string
-                Name pattern to filter by subject ID.
-            subject_label: string
-                Name pattern to filter by subject ID.
-            experiment_id: string
-                Name pattern to filter by experiment ID.
-            experiment_label: string
-                Name pattern to filter by experiment ID.
-            columns: list
-                Values to return.
-            constraints: dict
-                Dictionary of xsi_type (key--) and parameter (--value)
-                pairs by which to filter.
-            """
-
-        return self.scans(project_id, subject_id, subject_label,
-                          experiment_id, experiment_label,
-                          'xnat:mrSessionData', 'xnat:mrScanData',
-                          columns, constraints
-                          )
-
-    def search_experiments(self,
-                           project_id=None,
-                           subject_id=None,
-                           subject_label=None,
-                           experiment_type='xnat:subjectAssessorData',
-                           columns=None,
-                           constraints=None
-                           ):
-
-        """ Returns a list of all visible experiment IDs of the
-            specified type, filtered by optional constraints. This
-            function is a shortcut using the search engine.
-
-            Parameters
-            ----------
-            project_id: string
-                Name pattern to filter by project ID.
-            subject_id: string
-                Name pattern to filter by subject ID.
-            subject_label: string
-                Name pattern to filter by subject ID.
-            experiment_type: string
-                xsi path type must be a leaf session type.
-                defaults to 'xnat:mrSessionData'
-            columns: List[string]
-                list of xsi paths for names of columns to return.
-            constraints: list[(tupple)]
-                List of tupples for comparison in the form (key, comparison,
-                value) valid comparisons are: =, <, <=,>,>=, LIKE
-            """
-
-        if columns is None:
-            columns = []
-
-        where_clause = []
-
-        if project_id is not None:
-            item = ('%s/project' % experiment_type, "=", project_id)
-            where_clause.append(item)
-        if subject_id is not None:
-            where_clause.append(('xnat:subjectData/ID', "=", subject_id))
-        if subject_label is not None:
-            where_clause.append(('xnat:subjectData/LABEL', "=", subject_label))
-
-        if constraints is not None:
-            where_clause.extend(constraints)
-
-        if where_clause != []:
-            where_clause.append('AND')
-
-        if where_clause != []:
-            sel = self._intf.select(experiment_type, columns=columns)
-            table = sel.where(where_clause)
-            return table
-        else:
-            table = self._intf.select(experiment_type, columns=columns)
-            return table.all()
+from .jsonutil import JsonTable
+
+
+class ArrayData(object):
+
+    def __init__(self, interface):
+        self._intf = interface
+
+    def _get_array(self, query_string, project_id=None,
+                   subject_id=None, subject_label=None,
+                   experiment_id=None, experiment_label=None,
+                   experiment_type='xnat:subjectAssessorData',
+                   columns=None, constraints=None
+                   ):
+
+        if constraints is None:
+            constraints = {}
+
+        uri = '%s/experiments?xsiType=%s' % (self._intf._get_entry_point(),
+                                             experiment_type)
+
+        if project_id is not None:
+            uri += '&project=%s' % project_id
+
+        if subject_id is not None:
+            uri += '&%s/subject_id=%s' % (experiment_type, subject_id)
+
+        # Subject Label is only held in the xnat:subjectData so look for it
+        # there. This should join against whatever the experiment type is.
+        if subject_label is not None:
+            uri += '&xnat:subjectData/label=%s' % (subject_label)
+
+        if experiment_id is not None:
+            uri += '&ID=%s' % experiment_id
+
+        if experiment_label is not None:
+            uri += '&label=%s' % experiment_label
+
+        uri += query_string
+
+        if constraints != {}:
+            uri += ',' + ','.join(constraints.keys())
+
+        if columns is not None:
+            uri += ',' + ','.join(columns)
+
+        c = {}
+
+        [c.setdefault(key.lower(), value)
+         for key, value in constraints.items()
+         ]
+
+        return JsonTable(self._intf._get_json(uri)).where(**c)
+
+    def experiments(self, project_id=None, subject_id=None, subject_label=None,
+                    experiment_id=None, experiment_label=None,
+                    experiment_type='xnat:subjectAssessorData',
+                    columns=None,
+                    constraints=None):
+
+        """ Returns a list of all visible experiment IDs of the specified
+            type, filtered by optional constraints.
+
+            Parameters
+            ----------
+            project_id: string
+                Name pattern to filter by project ID.
+            subject_id: string
+                Name pattern to filter by subject ID.
+            subject_label: string
+                Name pattern to filter by subject ID.
+            experiment_id: string
+                Name pattern to filter by experiment ID.
+            experiment_label: string
+                Name pattern to filter by experiment ID.
+            experiment_type: string
+                xsi path type; e.g. 'xnat:mrSessionData'
+            columns: list
+                Values to return.
+            constraints: dict
+                Dictionary of xsi_type (key--) and parameter (--value)
+                pairs by which to filter.
+            """
+
+        query_string = '&columns=ID,project,%s/subject_id' % experiment_type
+
+        return self._get_array(query_string, project_id,
+                               subject_id, subject_label,
+                               experiment_id, experiment_label,
+                               experiment_type, columns, constraints
+                               )
+
+    def mrsessions(self, project_id=None, subject_id=None, subject_label=None,
+                   experiment_id=None, experiment_label=None,
+                   columns=None,
+                   constraints=None):
+
+        """ Returns a list of all MR sessions, filtered by optional constraints.
+
+            Parameters
+            ----------
+            project_id: string
+                Name pattern to filter by project ID.
+            subject_id: string
+                Name pattern to filter by subject ID.
+            subject_label: string
+                Name pattern to filter by subject ID.
+            experiment_id: string
+                Name pattern to filter by experiment ID.
+            experiment_label: string
+                Name pattern to filter by experiment ID.
+            columns: list
+                Values to return.
+            constraints: dict
+                Dictionary of xsi_type (key--) and parameter (--value)
+                pairs by which to filter.
+            """
+
+        return self.experiments(project_id, subject_id, subject_label,
+                                experiment_id, experiment_label,
+                                'xnat:mrSessionData', columns, constraints
+                                )
+
+    def scans(self, project_id=None, subject_id=None, subject_label=None,
+              experiment_id=None, experiment_label=None,
+              experiment_type='xnat:imageSessionData',
+              scan_type='xnat:imageScanData',
+              columns=None,
+              constraints=None
+              ):
+
+        """ Returns a list of all visible scan IDs of the specified type,
+            filtered by optional constraints.
+
+            Parameters
+            ----------
+            project_id: string
+                Name pattern to filter by project ID.
+            subject_id: string
+                Name pattern to filter by subject ID.
+            subject_label: string
+                Name pattern to filter by subject ID.
+            experiment_id: string
+                Name pattern to filter by experiment ID.
+            experiment_label: string
+                Name pattern to filter by experiment ID.
+            experiment_type: string
+                xsi path type; e.g. 'xnat:mrSessionData'
+            scan_type: string
+                xsi path type; e.g. 'xnat:mrScanData', etc.
+            columns: list
+                Values to return.
+            constraints: dict
+                Dictionary of xsi_type (key--) and parameter (--value)
+                pairs by which to filter.
+            """
+
+        query_string = '&columns=ID,project,%s/subject_id,%s/ID' % (
+            experiment_type, scan_type)
+
+        array = self._get_array(query_string, project_id,
+                                subject_id, subject_label,
+                                experiment_id, experiment_label,
+                                experiment_type, columns, constraints)
+        id_key = ('%s/ID' % scan_type).lower()
+        return JsonTable([i for i in array if i[id_key]])
+
+    def mrscans(self, project_id=None, subject_id=None, subject_label=None,
+                experiment_id=None, experiment_label=None,
+                columns=None,
+                constraints=None):
+
+        """ Returns a list of all MR scans, filtered by optional constraints.
+
+            Parameters
+            ----------
+            project_id: string
+                Name pattern to filter by project ID.
+            subject_id: string
+                Name pattern to filter by subject ID.
+            subject_label: string
+                Name pattern to filter by subject ID.
+            experiment_id: string
+                Name pattern to filter by experiment ID.
+            experiment_label: string
+                Name pattern to filter by experiment ID.
+            columns: list
+                Values to return.
+            constraints: dict
+                Dictionary of xsi_type (key--) and parameter (--value)
+                pairs by which to filter.
+            """
+
+        return self.scans(project_id, subject_id, subject_label,
+                          experiment_id, experiment_label,
+                          'xnat:mrSessionData', 'xnat:mrScanData',
+                          columns, constraints
+                          )
+
+    def search_experiments(self,
+                           project_id=None,
+                           subject_id=None,
+                           subject_label=None,
+                           experiment_type='xnat:subjectAssessorData',
+                           columns=None,
+                           constraints=None
+                           ):
+
+        """ Returns a list of all visible experiment IDs of the
+            specified type, filtered by optional constraints. This
+            function is a shortcut using the search engine.
+
+            Parameters
+            ----------
+            project_id: string
+                Name pattern to filter by project ID.
+            subject_id: string
+                Name pattern to filter by subject ID.
+            subject_label: string
+                Name pattern to filter by subject ID.
+            experiment_type: string
+                xsi path type must be a leaf session type.
+                defaults to 'xnat:mrSessionData'
+            columns: List[string]
+                list of xsi paths for names of columns to return.
+            constraints: list[(tupple)]
+                List of tupples for comparison in the form (key, comparison,
+                value) valid comparisons are: =, <, <=,>,>=, LIKE
+            """
+
+        if columns is None:
+            columns = []
+
+        where_clause = []
+
+        if project_id is not None:
+            item = ('%s/project' % experiment_type, "=", project_id)
+            where_clause.append(item)
+        if subject_id is not None:
+            where_clause.append(('xnat:subjectData/ID', "=", subject_id))
+        if subject_label is not None:
+            where_clause.append(('xnat:subjectData/LABEL', "=", subject_label))
+
+        if constraints is not None:
+            where_clause.extend(constraints)
+
+        if where_clause != []:
+            where_clause.append('AND')
+
+        if where_clause != []:
+            sel = self._intf.select(experiment_type, columns=columns)
+            table = sel.where(where_clause)
+            return table
+        else:
+            table = self._intf.select(experiment_type, columns=columns)
+            return table.all()
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/attributes.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/attributes.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/__init__.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/__init__.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/ashs.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/ashs.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/bamos.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/bamos.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/basil.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/basil.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/cat12.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/cat12.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/dicom.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/dicom.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/dtifit.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/dtifit.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/freesurfer.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/freesurfer.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/freesurfer7_extras.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/freesurfer7_extras.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/mrtrix3.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/mrtrix3.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/pet_fdg.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/pet_fdg.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/qsxmt.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/qsxmt.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/spm12.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/spm12.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/validator.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/validator.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/derivatives/xcp_d.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/derivatives/xcp_d.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/downloadutils.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/downloadutils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-import os.path as op
-import zipfile
-import sys
-
-from .schema import class_name
-from . import uriutil
-
-DEBUG = False
-
-
-def unzip(fzip,
-          dest_dir,
-          check={'run': lambda z, d: True, 'desc': ""}):
-    """
-    Extracts the given zip file to the given directory, but only if all members
-    of the archive pass the given check.
-
-        Parameters
-        ----------
-        src: fzip
-            zipfile
-        dest_dir: string
-            directory into which to extract the archive
-        check: dict
-            An dictionary that has the keys:
-                 'run' : A function that takes a filename and parent directory
-                     and returns Bool. By default this function always returns
-                     True.
-                 'dest' : A string description of this test. By default this
-                     is empty.
-
-        Returns a tuple of type (bool,[string]) where if the extraction ran
-        successfully the first is true and the second is a list of files that
-        were extracted, and if not the first is false and the second is the
-        name of the failing member.
-    """
-    for member in fzip.namelist():
-        if not check['run'](member, dest_dir):
-            return (False, member)
-
-    fzip.extractall(path=dest_dir)
-    return (True, map(lambda f: op.join(dest_dir, f), fzip.namelist()))
-
-
-def download(dest_dir, instance=None, type="ALL", name=None, extract=False,
-             safe=False, removeZip=False):
-    """
-    Download all the files at this level that match the given constraint as a
-    zip archive. Should not be called directly but from a instance of class
-    that supports bulk downloading eg. "Scans"
-
-        Parameters
-        ----------
-        instance : 'object
-             The instance that contains local values needed by this function
-             eg. instance._cbase stores the URI.
-        dest_dir : string
-             directory into which to place the downloaded archive.
-        type: string
-             a comma separated list of file types, eg. "T1,T2". Default is
-             "ALL".
-        name: string
-             the name of the zip archive. Defaults to None. See below for the
-             default naming scheme.
-        extract: bool
-             If True, the files are left extracted in the parent directory.
-             Default is False.
-        safe: bool
-             If true, run safety checks on the files before extracting,
-             eg. check that the file doesn't exist in the parent directory
-             before overwriting it. Default is False.
-
-        Default Zip Name
-        ----------------
-        Given the project "p", subject "s" and experiment "e", and that the
-        "Scans" (as opposed to "Assessors" or "Reconstructions") are being
-        downloaded, and the scan types are constrained to "T1,T2", the name of
-        the zip file defaults to:
-          "p_s_e_scans_T1_T2.zip"
-
-        Exceptions
-        ----------
-        A generic Exception will be raised if any of the following happen:
-         - This function is called directly and not from an instance of a
-            class that supports bulk downloading eg."Scans"
-         - The destination directory is unspecified
-        A LookupError is raised if there are no resources to download
-        A ValueError is raised if any of the following happen:
-         - The project, subject and experiment names could not be extracted
-            from the URI
-         - The type constraint "ALL" is used with other constraints.
-            eg. "ALL,T1,T2"
-         - The URI associated with this class contains wildcards
-            eg. /projects/proj/subjects/*/experiments/scans
-        An EnvironmentError is raised if any of the following happen:
-         - If "safe" is true, and (a) a zip file with the same name exists in
-            given destination directory or
-           (b) extracting the archive overrides an existing file. In the second
-            case the downloaded archive
-           is left in the parent directory.
-
-        Return
-        ------
-        A path to the zip archive if "extract" is False, and a list of
-        extracted files if True.
-    """
-
-    if instance is None:
-        raise Exception('This function should be called directly but from an'
-                        'instance of a class that supports bulk downloading, '
-                        'eg. "Scans"')
-    if dest_dir is None:
-        raise Exception('Destination directory is unspecified')
-
-    # the URI must be fully qualified with a project,subject and experiment
-    if '%2A' in instance._cbase:
-        raise ValueError('URI contains wildcards :' + instance._cbase)
-
-    # Check that there are resources at this level
-    available = instance.get()
-    if len(available) == 0:
-        raise LookupError(
-            'There are no %s to download' % class_name(instance).lower())
-
-    pse = uriutil.extract_uri(instance._cbase)
-    if pse is None:
-        raise ValueError("Could not extract project, subject and experiment "
-                         "from the uri: " + instance._cbase)
-
-    # Extract the desired scan types. Clean up whitespace and remove dupes
-    types = {}
-    for t in type.split(','):
-        cleaned = t.strip()
-        if cleaned != "":
-            types[cleaned] = cleaned
-
-    # Make sure the user hasn't asked us to download ALL the scans and then
-    # asked for them to be constrained to a type.
-    if len(types) > 1 and 'ALL' in types:
-        raise ValueError('The \"ALL\" scan type constraint cannot be used with'
-                         ' any other constraint')
-
-    (p, s, e) = pse
-
-    # Make the name of the zip file
-    default_zip_name = lambda: '%s_%s_%s_%s_%s' % (
-        p, s, e, class_name(instance).lower(), '_'.join(types.values()))
-
-    zip_name = name if name is not None else default_zip_name()
-    zip_location = op.join(dest_dir, zip_name + '.zip')
-
-    if safe:
-        if op.exists(zip_location):
-            raise EnvironmentError("Unable to download to " + zip_location +
-                                   " because this file already exists.")
-
-    # Download from the server
-    with open(zip_location, 'wb') as f:
-        response = instance._intf.get(uriutil.join_uri(
-            instance._cbase, ','.join(types.values())) + '/files?format=zip',
-            stream=True)
-        try:
-            count = 0
-            for chunk in response.iter_content(chunk_size=1024):
-                if chunk:  # filter out keep-alive new chunks
-                    f.write(chunk)
-                    count += 1
-                    if count % 10 == 0:
-                        # flush the buffer every once in a while.
-                        f.flush()
-            f.flush()  # and one last flush.
-        except Exception as e:
-            sys.stderr.write(e)
-        finally:
-            response.close()
-
-    if DEBUG:
-        print(zip_location)
-
-    ##
-
-    # Extract the archive
-    fzip = zipfile.ZipFile(zip_location, 'r')
-    if extract:
-        check = {'run': lambda f, d: not op.exists(op.join(dest_dir, f)),
-                 'desc': 'File does not exist in the parent directory'}
-        safeUnzip = lambda: unzip(fzip, dest_dir, check) \
-            if safe else lambda: unzip(fzip, dest_dir)
-        (unzipped, paths) = safeUnzip()()
-        if not unzipped:
-            fzip.close()
-            msg = "Unable to extract " + zip_location + " because file " +\
-                paths + " failed the following test: " + check['desc']
-            raise EnvironmentError(msg)
-        else:
-            if removeZip:
-                fzip.close()
-                import os
-                os.remove(zip_location)
-            return paths
-    else:
-        fzip.close()
-        return zip_location
+import os.path as op
+import zipfile
+import sys
+
+from .schema import class_name
+from . import uriutil
+
+DEBUG = False
+
+
+def unzip(fzip,
+          dest_dir,
+          check={'run': lambda z, d: True, 'desc': ""}):
+    """
+    Extracts the given zip file to the given directory, but only if all members
+    of the archive pass the given check.
+
+        Parameters
+        ----------
+        src: fzip
+            zipfile
+        dest_dir: string
+            directory into which to extract the archive
+        check: dict
+            An dictionary that has the keys:
+                 'run' : A function that takes a filename and parent directory
+                     and returns Bool. By default this function always returns
+                     True.
+                 'dest' : A string description of this test. By default this
+                     is empty.
+
+        Returns a tuple of type (bool,[string]) where if the extraction ran
+        successfully the first is true and the second is a list of files that
+        were extracted, and if not the first is false and the second is the
+        name of the failing member.
+    """
+    for member in fzip.namelist():
+        if not check['run'](member, dest_dir):
+            return (False, member)
+
+    fzip.extractall(path=dest_dir)
+    return (True, map(lambda f: op.join(dest_dir, f), fzip.namelist()))
+
+
+def download(dest_dir, instance=None, type="ALL", name=None, extract=False,
+             safe=False, removeZip=False):
+    """
+    Download all the files at this level that match the given constraint as a
+    zip archive. Should not be called directly but from a instance of class
+    that supports bulk downloading eg. "Scans"
+
+        Parameters
+        ----------
+        instance : 'object
+             The instance that contains local values needed by this function
+             eg. instance._cbase stores the URI.
+        dest_dir : string
+             directory into which to place the downloaded archive.
+        type: string
+             a comma separated list of file types, eg. "T1,T2". Default is
+             "ALL".
+        name: string
+             the name of the zip archive. Defaults to None. See below for the
+             default naming scheme.
+        extract: bool
+             If True, the files are left extracted in the parent directory.
+             Default is False.
+        safe: bool
+             If true, run safety checks on the files before extracting,
+             eg. check that the file doesn't exist in the parent directory
+             before overwriting it. Default is False.
+
+        Default Zip Name
+        ----------------
+        Given the project "p", subject "s" and experiment "e", and that the
+        "Scans" (as opposed to "Assessors" or "Reconstructions") are being
+        downloaded, and the scan types are constrained to "T1,T2", the name of
+        the zip file defaults to:
+          "p_s_e_scans_T1_T2.zip"
+
+        Exceptions
+        ----------
+        A generic Exception will be raised if any of the following happen:
+         - This function is called directly and not from an instance of a
+            class that supports bulk downloading eg."Scans"
+         - The destination directory is unspecified
+        A LookupError is raised if there are no resources to download
+        A ValueError is raised if any of the following happen:
+         - The project, subject and experiment names could not be extracted
+            from the URI
+         - The type constraint "ALL" is used with other constraints.
+            eg. "ALL,T1,T2"
+         - The URI associated with this class contains wildcards
+            eg. /projects/proj/subjects/*/experiments/scans
+        An EnvironmentError is raised if any of the following happen:
+         - If "safe" is true, and (a) a zip file with the same name exists in
+            given destination directory or
+           (b) extracting the archive overrides an existing file. In the second
+            case the downloaded archive
+           is left in the parent directory.
+
+        Return
+        ------
+        A path to the zip archive if "extract" is False, and a list of
+        extracted files if True.
+    """
+
+    if instance is None:
+        raise Exception('This function should be called directly but from an'
+                        'instance of a class that supports bulk downloading, '
+                        'eg. "Scans"')
+    if dest_dir is None:
+        raise Exception('Destination directory is unspecified')
+
+    # the URI must be fully qualified with a project,subject and experiment
+    if '%2A' in instance._cbase:
+        raise ValueError('URI contains wildcards :' + instance._cbase)
+
+    # Check that there are resources at this level
+    available = instance.get()
+    if len(available) == 0:
+        raise LookupError(
+            'There are no %s to download' % class_name(instance).lower())
+
+    pse = uriutil.extract_uri(instance._cbase)
+    if pse is None:
+        raise ValueError("Could not extract project, subject and experiment "
+                         "from the uri: " + instance._cbase)
+
+    # Extract the desired scan types. Clean up whitespace and remove dupes
+    types = {}
+    for t in type.split(','):
+        cleaned = t.strip()
+        if cleaned != "":
+            types[cleaned] = cleaned
+
+    # Make sure the user hasn't asked us to download ALL the scans and then
+    # asked for them to be constrained to a type.
+    if len(types) > 1 and 'ALL' in types:
+        raise ValueError('The \"ALL\" scan type constraint cannot be used with'
+                         ' any other constraint')
+
+    (p, s, e) = pse
+
+    # Make the name of the zip file
+    default_zip_name = lambda: '%s_%s_%s_%s_%s' % (
+        p, s, e, class_name(instance).lower(), '_'.join(types.values()))
+
+    zip_name = name if name is not None else default_zip_name()
+    zip_location = op.join(dest_dir, zip_name + '.zip')
+
+    if safe:
+        if op.exists(zip_location):
+            raise EnvironmentError("Unable to download to " + zip_location +
+                                   " because this file already exists.")
+
+    # Download from the server
+    with open(zip_location, 'wb') as f:
+        response = instance._intf.get(uriutil.join_uri(
+            instance._cbase, ','.join(types.values())) + '/files?format=zip',
+            stream=True)
+        try:
+            count = 0
+            for chunk in response.iter_content(chunk_size=1024):
+                if chunk:  # filter out keep-alive new chunks
+                    f.write(chunk)
+                    count += 1
+                    if count % 10 == 0:
+                        # flush the buffer every once in a while.
+                        f.flush()
+            f.flush()  # and one last flush.
+        except Exception as e:
+            sys.stderr.write(e)
+        finally:
+            response.close()
+
+    if DEBUG:
+        print(zip_location)
+
+    ##
+
+    # Extract the archive
+    fzip = zipfile.ZipFile(zip_location, 'r')
+    if extract:
+        check = {'run': lambda f, d: not op.exists(op.join(dest_dir, f)),
+                 'desc': 'File does not exist in the parent directory'}
+        safeUnzip = lambda: unzip(fzip, dest_dir, check) \
+            if safe else lambda: unzip(fzip, dest_dir)
+        (unzipped, paths) = safeUnzip()()
+        if not unzipped:
+            fzip.close()
+            msg = "Unable to extract " + zip_location + " because file " +\
+                paths + " failed the following test: " + check['desc']
+            raise EnvironmentError(msg)
+        else:
+            if removeZip:
+                fzip.close()
+                import os
+                os.remove(zip_location)
+            return paths
+    else:
+        fzip.close()
+        return zip_location
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/errors.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/help.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/help.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,691 +1,691 @@
-try:
-    import networkx as nx
-    from networkx.drawing.nx_agraph import graphviz_layout
-    import matplotlib.pyplot as plt
-    _DRAW_GRAPHS = True
-except Exception:
-    _DRAW_GRAPHS = False
-
-from . import schema
-from .jsonutil import get_column
-from .search import Search
-
-
-class Inspector(object):
-    """ Database introspection interface.
-    """
-
-    def __init__(self, interface):
-        """
-            Parameters
-            ----------
-            interface:
-                :class:`Interface` Object
-        """
-        self._intf = interface
-        self._get_json = interface._get_json
-        self._auto = True
-        self._tick = 30
-
-        self.schemas = SchemasInspector(interface)
-
-    def __call__(self):
-        for name in ['experiment', 'assessor', 'scan', 'reconstruction']:
-            self._resource_struct(name)
-
-    def set_autolearn(self, auto=None, tick=None):
-        """ Once in a while queries will persist additional
-            information on the server. This information is available
-            through the following methods of this class:
-
-                - experiment_types
-                - assessor_types
-                - scan_types
-                - reconstruction_types
-
-            It is also transparently used in insert operations.
-
-            Parameters
-            ----------
-            auto: boolean
-                True to enable auto learn. False to disable.
-            tick: int
-                Every 'tick' seconds, if a query is issued, additional
-                information will be persisted.
-
-            See Also
-            --------
-            :func:`EObject.insert`
-        """
-        if auto is not None:
-            self._auto = auto
-        if tick is not None:
-            self._tick = tick
-
-    def datatypes(self, pattern='*', fields_pattern=None):
-        """ Discovers the datatypes and datafields of the database.
-
-            Parameters
-            ----------
-            pattern: string
-                Pattern for the datatype. May include wildcards.
-            fields_pattern: string
-                - Pattern for the datafields -- may include wildcards.
-                - If specified, datafields will be returned instead of
-                  datatypes.
-
-            Returns
-            -------
-            list : datatypes or datafields depending on the argument usage.
-        """
-        self._intf._get_entry_point()
-
-        search_els = self._get_json('%s/search/elements?format=json' %
-                                    self._intf._get_entry_point())
-
-        if not fields_pattern and ('*' in pattern or '?' in pattern):
-            return get_column(search_els, 'ELEMENT_NAME', pattern)
-
-        else:
-            fields = []
-            for datatype in get_column(search_els, 'ELEMENT_NAME', pattern):
-                df = self._datafields(datatype, fields_pattern or '*', True)
-                fields.extend(df)
-
-            return fields
-
-    def _datafields(self, datatype, pattern='*', prepend_type=True):
-        self._intf._get_entry_point()
-
-        search_fds = self._get_json('%s/search/elements/%s?format=json' %
-                                    (self._intf._get_entry_point(),
-                                        datatype))
-
-        fields = get_column(search_fds, 'FIELD_ID', pattern)
-
-        return ['%s/%s' % (datatype, field)
-                if prepend_type else field
-                for field in fields
-                if '=' not in field and 'SHARINGSHAREPROJECT' not in field
-                ]
-
-    def experiment_types(self):
-        """ Returns the datatypes used at the experiment level in this
-            database.
-
-            See Also
-            --------
-            :func:`Inspector.set_autolearn`
-        """
-        return self._resource_types('experiment')
-
-    def assessor_types(self):
-        """ Returns the datatypes used at the assessor level in this
-            database.
-
-            See Also
-            --------
-            :func:`Inspector.set_autolearn`
-        """
-        return self._resource_types('assessor')
-
-    def reconstruction_types(self):
-        """ Returns the datatypes used at the reconstruction level in this
-            database.
-
-            See Also
-            --------
-            :func:`Inspector.set_autolearn`
-        """
-        return self._resource_types('reconstruction')
-
-    def scan_types(self):
-        """ Returns the datatypes used at the scan level in this
-            database.
-
-            See Also
-            --------
-            :func:`Inspector.set_autolearn`
-        """
-        return self._resource_types('scan')
-
-    def field_values(self, field_name):
-        """ Look for the values a specific datafield takes in the database.
-        """
-        self._intf._get_entry_point()
-
-        search_tbl = Search(field_name.split('/')[0],
-                            [field_name], self._intf
-                            )
-
-        criteria = [('%s/ID' % field_name.split('/')[0], 'LIKE', '%'), 'AND']
-
-        return list(set([val
-                         for entry in search_tbl.where(criteria)
-                         for val in entry.values()
-                         ])
-                    )
-
-    def project_values(self):
-        """ Look for the values a the project level in the database.
-
-            .. note::
-                Is equivalent to interface.select.projects().get()
-        """
-        self._intf._get_entry_point()
-
-        return get_column(self._get_json(
-                '%s/projects' % self._intf._entry), 'ID')
-
-    def subject_values(self, project=None):
-        """ Look for the values a the subject level in the database.
-
-            .. note::
-                Is equivalent to interface.select('//subjects').get()
-        """
-        self._intf._get_entry_point()
-
-        uri = '%s/subjects?columns=ID' % self._intf._entry
-
-        if project is not None:
-            uri += '&project=%s' % project
-
-        return get_column(self._get_json(uri), 'ID')
-
-    def experiment_values(self, datatype, project=None):
-        """ Look for the values a the experiment level for a given datatype
-            in the database.
-
-            .. note::
-                The  datatype should be one of Inspector.experiment_types()
-
-            Parameters
-            ----------
-            datatype: string
-                An experiment type. eg: xnat:mrsessiondata
-            project: string
-                Optional. Restrict operation to a project.
-        """
-        self._intf._get_entry_point()
-
-        uri = '%s/experiments?columns=ID' % self._intf._entry
-        if datatype is not None:
-            uri += '&xsiType=%s' % datatype
-        if project is not None:
-            uri += '&project=%s' % project
-
-        return get_column(self._get_json(uri), 'ID')
-
-    def assessor_values(self, experiment_type, project=None):
-        """ Look for the values at the assessor level for a given experiment
-            type in the database.
-
-            .. note::
-               The experiment type should be one of
-               Inspector.experiment_types()
-
-            .. warning::
-                Depending on the number of elements the operation may
-                take a while.
-
-            Parameters
-            ----------
-            datatype: string
-                An experiment type. eg: xnat:mrsessiondata
-            project: string
-                Optional. Restrict operation to a project.
-        """
-        return self._sub_experiment_values('assessor',
-                                           project, experiment_type)
-
-    def scan_values(self, experiment_type, project=None):
-        """ Look for the values at the scan level for a given experiment
-            type in the database.
-
-            .. note::
-               The experiment type should be one of
-               Inspector.experiment_types()
-
-            .. warning::
-                Depending on the number of elements the operation may
-                take a while.
-
-            Parameters
-            ----------
-            datatype: string
-                An experiment type.
-            project: string
-                Optional. Restrict operation to a project.
-        """
-        return self._sub_experiment_values('scan', project, experiment_type)
-
-    def reconstruction_values(self, experiment_type, project=None):
-        """ Look for the values at the reconstruction level for a given
-            experiment type in the database.
-
-            .. note::
-               The experiment type should be one of
-               Inspector.experiment_types()
-
-            .. warning::
-                Depending on the number of elements the operation may
-                take a while.
-
-            Parameters
-            ----------
-            datatype: string
-                An experiment type.
-            project: string
-                Optional. Restrict operation to a project.
-        """
-        return self._sub_experiment_values('reconstruction',
-                                           project, experiment_type)
-
-    def structure(self):
-        """ Displays the keywords structure used in XNAT REST API.
-        """
-        def traverse(coll, lvl):
-            for key in schema.resources_tree[coll]:
-                print('%s+%s' % (' ' * lvl, key.upper()))
-
-                datatypes = set([
-                        self._intf._struct[uri]
-                        for uri in self._intf._struct.keys()
-                        if uri.split('/')[-2] == key
-                        ])
-
-                if datatypes != set():
-                    print('%s  %s' % (' ' * lvl, '-' * len(key)))
-
-                for datatype in datatypes:
-                    print('%s- %s' % (' ' * lvl, datatype))
-
-                if key in schema.resources_tree.keys():
-                    traverse(key, lvl + 4)
-
-        print('- %s' % 'PROJECTS')
-        traverse('projects', 4)
-
-    def _sub_experiment_values(self, sub_exp, project, experiment_type):
-        self._intf._get_entry_point()
-
-        values = []
-
-        column = '%s/%ss/%s/id' % \
-            (experiment_type.lower(), sub_exp, sub_exp)
-
-        sub_exps = '%s/experiments?columns=ID,%s' % (self._intf._entry,
-                                                     column
-                                                     )
-
-        if project is not None:
-            sub_exps += '&project=%s' % project
-
-        values = get_column(self._get_json(sub_exps), column)
-
-        return list(set(values))
-
-    def _resource_struct(self, name):
-
-        return self._intf._struct
-
-    def _resource_types(self, name):
-        return list(set(self._resource_struct(name).values()))
-
-
-class GraphData(object):
-    def __init__(self, interface):
-        self._intf = interface
-        self._struct = interface._struct
-
-    # def link(self, subjects, fields):
-
-    #     criteria = [('xnat:subjectData/SUBJECT_ID', '=', _id)
-    #                 for _id in subjects
-    #                 ]
-    #     criteria += ['OR']
-    #     # variables = ['xnat:subjectData/SUBJECT_ID'] + fields
-
-    #     subject_id = 'xnat:subjectData/SUBJECT_ID'
-
-    #     for field in fields:
-
-    #         field_tbl = self._intf.select('xnat:subjectData',
-    #                                       [subject_id, field]
-    #                                       ).where(criteria)
-    #         head = field_tbl.headers()
-    #         head.remove('subject_id')
-    #         head = head[0]
-    #         possible = set(field_tbl.get(head))
-
-    #         groups = {}
-
-    #         for val in possible:
-    #             groups[val] = field_tbl.where(**{head:val}
-    #                                             ).select('subject_id')
-
-    #     return groups
-
-    def datatypes(self, pattern='*'):
-        graph = nx.DiGraph()
-        graph.add_node('datatypes')
-        graph.labels = {'datatypes': 'datatypes'}
-        graph.weights = {'datatypes': 100.0}
-
-        datatypes = self._intf.inspect.datatypes(pattern)
-        namespaces = set([dat.split(':')[0] for dat in datatypes])
-
-        for ns in namespaces:
-            graph.add_edge('datatypes', ns)
-            graph.weights[ns] = 70.0
-
-            for dat in datatypes:
-                if dat.startswith(ns):
-                    graph.add_edge(ns, dat)
-                    graph.weights[dat] = 40.0
-
-        return graph
-
-    def rest_resource(self, name):
-        resource_types = self._intf.inspect._resource_types(name)
-
-        graph = nx.DiGraph()
-        graph.add_node(name)
-        graph.labels = {name: name}
-        graph.weights = {name: 100.0}
-
-        namespaces = set([exp.split(':')[0] for exp in resource_types])
-
-        for ns in namespaces:
-            graph.add_edge(name, ns)
-            graph.weights[ns] = 70.0
-
-            for exp in resource_types:
-                if exp.startswith(ns):
-                    graph.add_edge(ns, exp)
-                    graph.weights[exp] = 40.0
-
-        return graph
-
-    def field_values(self, field_name):
-
-        search_tbl = Search(field_name.split('/')[0],
-                            [field_name], self._intf
-                            )
-
-        criteria = [('%s/ID' % field_name.split('/')[0], 'LIKE', '%'), 'AND']
-
-        dist = {}
-
-        for entry in search_tbl.where(criteria):
-            for val in entry.values():
-                dist.setdefault(val, 1.0)
-                dist[val] += 1
-
-        graph = nx.Graph()
-        graph.add_node(field_name)
-        graph.weights = dist
-        graph.weights[field_name] = 100.0
-
-        for val in dist.keys():
-            graph.add_edge(field_name, val)
-
-        return graph
-
-    def architecture(self, with_datatypes=True):
-        graph = nx.DiGraph()
-        graph.add_node('projects')
-        graph.labels = {'projects': 'projects'}
-        graph.weights = {'projects': 100.0}
-
-        def traverse(lkw, as_lkw):
-
-            for key in schema.resources_tree[lkw]:
-                as_key = '%s_%s' % (as_lkw, key)
-                weight = (1 - len(as_key*2)/100.0) * 100
-                graph.add_edge(as_lkw, as_key)
-                graph.labels[as_key] = key
-                graph.weights[as_key] = weight
-
-                if with_datatypes:
-                    for uri in self._struct.keys():
-                        if uri.split('/')[-2] == key:
-                            datatype = self._struct[uri]
-                            graph.add_edge(as_key, datatype)
-                            graph.weights[datatype] = 10
-                            graph.labels[datatype] = datatype
-
-                traverse(key, as_key)
-
-        traverse('projects', 'projects')
-
-        return graph
-
-
-class PaintGraph(object):
-    def __init__(self, interface):
-        self._intf = interface
-        self.get_graph = interface._get_graph
-
-    def architecture(self, with_datatypes=True, save=None):
-        graph = self.get_graph.architecture(with_datatypes)
-
-        plt.figure(figsize=(8, 8))
-        pos = graphviz_layout(graph, prog='twopi', args='')
-
-        # node_size = [(float(graph.degree(v)) * 5)**3 for v in graph]
-        # node_size = [graph.weights[v] ** 2 for v in graph]
-        # node_color = [float(graph.degree(v)) for v in graph]
-        # node_color = [graph.weights[v] ** 2 for v in graph]
-
-        cost = lambda v: float(graph.degree(v)) ** 3 + \
-            graph.weights[v] ** 2
-
-        costs = norm_costs([cost(v) for v in graph], 10000)
-
-        nx.draw(graph, pos, labels=graph.labels,
-                node_size=costs, node_color=costs,
-                font_size=13, font_color='orange',
-                font_weight='bold', with_labels=True
-                )
-
-        plt.axis('off')
-
-        if save is not None:
-            plt.savefig(save)
-
-        plt.show()
-
-    def experiments(self, save=None):
-        graph = self.get_graph.rest_resource('experiments')
-        self._draw_rest_resource(graph, save=None)
-
-    def assessors(self, save=None):
-        graph = self.get_graph.rest_resource('assessors')
-        self._draw_rest_resource(graph, save=None)
-
-    def reconstructions(self, save=None):
-        graph = self.get_graph.rest_resource('reconstructions')
-        self._draw_rest_resource(graph, save=None)
-
-    def scans(self):
-        graph = self.get_graph.rest_resource('scans')
-        self._draw_rest_resource(graph)
-
-    def _draw_rest_resource(self, graph, save=None):
-        plt.figure(figsize=(8, 8))
-        pos = graphviz_layout(graph, prog='twopi', args='')
-
-        cost = lambda v: float(graph.degree(v)) ** 3 + \
-            graph.weights[v] ** 2
-
-        node_size = [cost(v) for v in graph]
-        # node_size = [graph.weights[v] ** 2 for v in graph]
-        # node_color = [float(graph.degree(v)) for v in graph]
-        node_color = [cost(v) for v in graph]
-
-        nx.draw(graph, pos,
-                node_size=node_size, node_color=node_color,
-                font_size=13, font_color='green', font_weight='bold'
-                )
-
-        plt.axis('off')
-
-        if save is not None:
-            plt.savefig(save)
-
-        plt.show()
-
-    def datatypes(self, pattern='*', save=None):
-        graph = self.get_graph.datatypes(pattern)
-
-        plt.figure(figsize=(8, 8))
-        pos = graphviz_layout(graph, prog='twopi', args='')
-
-        cost = lambda v: float(graph.degree(v)) ** 3 + \
-            graph.weights[v] ** 2
-
-        node_size = [cost(v) for v in graph]
-        # node_size = [graph.weights[v] ** 2 for v in graph]
-        # node_color = [float(graph.degree(v)) for v in graph]
-        node_color = [cost(v) for v in graph]
-
-        nx.draw(graph, pos,
-                node_size=node_size, node_color=node_color,
-                font_size=13, font_color='green', font_weight='bold',
-                with_labels=True
-                )
-
-        plt.axis('off')
-
-        if save is not None:
-            plt.savefig(save)
-
-        plt.show()
-
-    def field_values(self, field_name, save=None):
-        graph = self.get_graph.field_values(field_name)
-
-        plt.figure(figsize=(8, 8))
-        pos = graphviz_layout(graph, prog='twopi', args='')
-
-        cost = lambda v: graph.weights[v]
-
-        graph.weights[field_name] = max([cost(v) for v in graph]) / 2.0
-
-        costs = norm_costs([cost(v) for v in graph], 10000)
-
-        nx.draw(graph, pos,
-                node_size=costs, node_color=costs,
-                font_size=13, font_color='black',
-                font_weight='bold', with_labels=True
-                )
-
-        plt.axis('off')
-
-        if save is not None:
-            plt.savefig(save)
-
-        plt.show()
-
-
-def norm_costs(costs, norm=1000):
-    max_cost = max(costs)
-
-    return [(cost / max_cost) * norm for cost in costs]
-
-
-# class GraphDrawer(object):
-#     def __init__(self, interface):
-#         self._intf = interface
-
-#     def datatypes(self, project):
-#         self._intf.connection.set_strategy('offline')
-
-#         experiments_types = self._intf.inspect.datatypes.experiments(project)
-
-#         labels = {project:project, 'Experiments':'Experiments'}
-
-#         g = nx.Graph()
-
-#         g.add_edge(project, 'Experiments', {'weight':1})
-
-#         for exp_type in experiments_types:
-#             g.add_edge('Experiments', exp_type, {'weight':8})
-#             labels[exp_type] = exp_type
-
-#         pos = nx.graphviz_layout(g, prog='twopi', args='')
-
-#         nx.draw_networkx_nodes(g, pos,
-#                                nodelist=[project],
-#                                node_color='green', alpha=0.7,
-#                                node_size=2500, node_shape='s')
-
-#         nx.draw_networkx_nodes(g, pos,
-#                                nodelist=['Experiments'],
-#                                node_color='blue', alpha=0.7,
-#                                node_size=2000, node_shape='p')
-
-#         nx.draw_networkx_nodes(g, pos,
-#                                nodelist=experiments_types,
-#                                node_color='red', alpha=0.7,
-#                                node_size=1500, node_shape='o')
-
-#         nx.draw_networkx_edges(g, pos, width=2, alpha=0.5,
-#                                edge_color='black')
-
-#         nx.draw_networkx_labels(g, pos, labels,
-#                                 alpha=0.9, font_size=8,
-#                                 font_color='black', font_weight='bold')
-
-#         plt.axis('off')
-#         plt.show()
-
-#         self._intf.connection.revert_strategy()
-
-class SchemasInspector(object):
-    def __init__(self, interface):
-        self._intf = interface
-
-    def __call__(self):
-        self._intf.manage.schemas()
-
-        for xsd in self._intf.manage.schemas():
-            print('-'*40)
-            print(xsd.upper())
-            print('-'*40)
-            print()
-
-            trees = self._intf.manage.schemas._trees[xsd]
-            for datatype in schema.datatypes(trees):
-                print('[%s]' % datatype)
-                print()
-
-                for path in schema.datatype_attributes(trees, datatype):
-                    print(path)
-
-                print()
-
-    def look_for(self, element_name, datatype_name=None):
-        paths = []
-        self._intf.manage.schemas._init()
-
-        if ':' in element_name:
-            for root in self._intf.manage.schemas._trees.values():
-                paths.extend(schema.datatype_attributes(root, element_name))
-            return paths
-
-        for xsd in self._intf.manage.schemas():
-            # nsmap = self._intf.manage.schemas._trees[xsd].nsmap
-            trees = self._intf.manage.schemas._trees[xsd]
-            if datatype_name is not None:
-                datatypes = [datatype_name]
-            else:
-                datatypes = schema.datatypes(trees)
-
-            for datatype in datatypes:
-                for path in schema.datatype_attributes(trees, datatype):
-                    if element_name in path:
-                        paths.append(path)
-
-        return paths
+try:
+    import networkx as nx
+    from networkx.drawing.nx_agraph import graphviz_layout
+    import matplotlib.pyplot as plt
+    _DRAW_GRAPHS = True
+except Exception:
+    _DRAW_GRAPHS = False
+
+from . import schema
+from .jsonutil import get_column
+from .search import Search
+
+
+class Inspector(object):
+    """ Database introspection interface.
+    """
+
+    def __init__(self, interface):
+        """
+            Parameters
+            ----------
+            interface:
+                :class:`Interface` Object
+        """
+        self._intf = interface
+        self._get_json = interface._get_json
+        self._auto = True
+        self._tick = 30
+
+        self.schemas = SchemasInspector(interface)
+
+    def __call__(self):
+        for name in ['experiment', 'assessor', 'scan', 'reconstruction']:
+            self._resource_struct(name)
+
+    def set_autolearn(self, auto=None, tick=None):
+        """ Once in a while queries will persist additional
+            information on the server. This information is available
+            through the following methods of this class:
+
+                - experiment_types
+                - assessor_types
+                - scan_types
+                - reconstruction_types
+
+            It is also transparently used in insert operations.
+
+            Parameters
+            ----------
+            auto: boolean
+                True to enable auto learn. False to disable.
+            tick: int
+                Every 'tick' seconds, if a query is issued, additional
+                information will be persisted.
+
+            See Also
+            --------
+            :func:`EObject.insert`
+        """
+        if auto is not None:
+            self._auto = auto
+        if tick is not None:
+            self._tick = tick
+
+    def datatypes(self, pattern='*', fields_pattern=None):
+        """ Discovers the datatypes and datafields of the database.
+
+            Parameters
+            ----------
+            pattern: string
+                Pattern for the datatype. May include wildcards.
+            fields_pattern: string
+                - Pattern for the datafields -- may include wildcards.
+                - If specified, datafields will be returned instead of
+                  datatypes.
+
+            Returns
+            -------
+            list : datatypes or datafields depending on the argument usage.
+        """
+        self._intf._get_entry_point()
+
+        search_els = self._get_json('%s/search/elements?format=json' %
+                                    self._intf._get_entry_point())
+
+        if not fields_pattern and ('*' in pattern or '?' in pattern):
+            return get_column(search_els, 'ELEMENT_NAME', pattern)
+
+        else:
+            fields = []
+            for datatype in get_column(search_els, 'ELEMENT_NAME', pattern):
+                df = self._datafields(datatype, fields_pattern or '*', True)
+                fields.extend(df)
+
+            return fields
+
+    def _datafields(self, datatype, pattern='*', prepend_type=True):
+        self._intf._get_entry_point()
+
+        search_fds = self._get_json('%s/search/elements/%s?format=json' %
+                                    (self._intf._get_entry_point(),
+                                        datatype))
+
+        fields = get_column(search_fds, 'FIELD_ID', pattern)
+
+        return ['%s/%s' % (datatype, field)
+                if prepend_type else field
+                for field in fields
+                if '=' not in field and 'SHARINGSHAREPROJECT' not in field
+                ]
+
+    def experiment_types(self):
+        """ Returns the datatypes used at the experiment level in this
+            database.
+
+            See Also
+            --------
+            :func:`Inspector.set_autolearn`
+        """
+        return self._resource_types('experiment')
+
+    def assessor_types(self):
+        """ Returns the datatypes used at the assessor level in this
+            database.
+
+            See Also
+            --------
+            :func:`Inspector.set_autolearn`
+        """
+        return self._resource_types('assessor')
+
+    def reconstruction_types(self):
+        """ Returns the datatypes used at the reconstruction level in this
+            database.
+
+            See Also
+            --------
+            :func:`Inspector.set_autolearn`
+        """
+        return self._resource_types('reconstruction')
+
+    def scan_types(self):
+        """ Returns the datatypes used at the scan level in this
+            database.
+
+            See Also
+            --------
+            :func:`Inspector.set_autolearn`
+        """
+        return self._resource_types('scan')
+
+    def field_values(self, field_name):
+        """ Look for the values a specific datafield takes in the database.
+        """
+        self._intf._get_entry_point()
+
+        search_tbl = Search(field_name.split('/')[0],
+                            [field_name], self._intf
+                            )
+
+        criteria = [('%s/ID' % field_name.split('/')[0], 'LIKE', '%'), 'AND']
+
+        return list(set([val
+                         for entry in search_tbl.where(criteria)
+                         for val in entry.values()
+                         ])
+                    )
+
+    def project_values(self):
+        """ Look for the values a the project level in the database.
+
+            .. note::
+                Is equivalent to interface.select.projects().get()
+        """
+        self._intf._get_entry_point()
+
+        return get_column(self._get_json(
+                '%s/projects' % self._intf._entry), 'ID')
+
+    def subject_values(self, project=None):
+        """ Look for the values a the subject level in the database.
+
+            .. note::
+                Is equivalent to interface.select('//subjects').get()
+        """
+        self._intf._get_entry_point()
+
+        uri = '%s/subjects?columns=ID' % self._intf._entry
+
+        if project is not None:
+            uri += '&project=%s' % project
+
+        return get_column(self._get_json(uri), 'ID')
+
+    def experiment_values(self, datatype, project=None):
+        """ Look for the values a the experiment level for a given datatype
+            in the database.
+
+            .. note::
+                The  datatype should be one of Inspector.experiment_types()
+
+            Parameters
+            ----------
+            datatype: string
+                An experiment type. eg: xnat:mrsessiondata
+            project: string
+                Optional. Restrict operation to a project.
+        """
+        self._intf._get_entry_point()
+
+        uri = '%s/experiments?columns=ID' % self._intf._entry
+        if datatype is not None:
+            uri += '&xsiType=%s' % datatype
+        if project is not None:
+            uri += '&project=%s' % project
+
+        return get_column(self._get_json(uri), 'ID')
+
+    def assessor_values(self, experiment_type, project=None):
+        """ Look for the values at the assessor level for a given experiment
+            type in the database.
+
+            .. note::
+               The experiment type should be one of
+               Inspector.experiment_types()
+
+            .. warning::
+                Depending on the number of elements the operation may
+                take a while.
+
+            Parameters
+            ----------
+            datatype: string
+                An experiment type. eg: xnat:mrsessiondata
+            project: string
+                Optional. Restrict operation to a project.
+        """
+        return self._sub_experiment_values('assessor',
+                                           project, experiment_type)
+
+    def scan_values(self, experiment_type, project=None):
+        """ Look for the values at the scan level for a given experiment
+            type in the database.
+
+            .. note::
+               The experiment type should be one of
+               Inspector.experiment_types()
+
+            .. warning::
+                Depending on the number of elements the operation may
+                take a while.
+
+            Parameters
+            ----------
+            datatype: string
+                An experiment type.
+            project: string
+                Optional. Restrict operation to a project.
+        """
+        return self._sub_experiment_values('scan', project, experiment_type)
+
+    def reconstruction_values(self, experiment_type, project=None):
+        """ Look for the values at the reconstruction level for a given
+            experiment type in the database.
+
+            .. note::
+               The experiment type should be one of
+               Inspector.experiment_types()
+
+            .. warning::
+                Depending on the number of elements the operation may
+                take a while.
+
+            Parameters
+            ----------
+            datatype: string
+                An experiment type.
+            project: string
+                Optional. Restrict operation to a project.
+        """
+        return self._sub_experiment_values('reconstruction',
+                                           project, experiment_type)
+
+    def structure(self):
+        """ Displays the keywords structure used in XNAT REST API.
+        """
+        def traverse(coll, lvl):
+            for key in schema.resources_tree[coll]:
+                print('%s+%s' % (' ' * lvl, key.upper()))
+
+                datatypes = set([
+                        self._intf._struct[uri]
+                        for uri in self._intf._struct.keys()
+                        if uri.split('/')[-2] == key
+                        ])
+
+                if datatypes != set():
+                    print('%s  %s' % (' ' * lvl, '-' * len(key)))
+
+                for datatype in datatypes:
+                    print('%s- %s' % (' ' * lvl, datatype))
+
+                if key in schema.resources_tree.keys():
+                    traverse(key, lvl + 4)
+
+        print('- %s' % 'PROJECTS')
+        traverse('projects', 4)
+
+    def _sub_experiment_values(self, sub_exp, project, experiment_type):
+        self._intf._get_entry_point()
+
+        values = []
+
+        column = '%s/%ss/%s/id' % \
+            (experiment_type.lower(), sub_exp, sub_exp)
+
+        sub_exps = '%s/experiments?columns=ID,%s' % (self._intf._entry,
+                                                     column
+                                                     )
+
+        if project is not None:
+            sub_exps += '&project=%s' % project
+
+        values = get_column(self._get_json(sub_exps), column)
+
+        return list(set(values))
+
+    def _resource_struct(self, name):
+
+        return self._intf._struct
+
+    def _resource_types(self, name):
+        return list(set(self._resource_struct(name).values()))
+
+
+class GraphData(object):
+    def __init__(self, interface):
+        self._intf = interface
+        self._struct = interface._struct
+
+    # def link(self, subjects, fields):
+
+    #     criteria = [('xnat:subjectData/SUBJECT_ID', '=', _id)
+    #                 for _id in subjects
+    #                 ]
+    #     criteria += ['OR']
+    #     # variables = ['xnat:subjectData/SUBJECT_ID'] + fields
+
+    #     subject_id = 'xnat:subjectData/SUBJECT_ID'
+
+    #     for field in fields:
+
+    #         field_tbl = self._intf.select('xnat:subjectData',
+    #                                       [subject_id, field]
+    #                                       ).where(criteria)
+    #         head = field_tbl.headers()
+    #         head.remove('subject_id')
+    #         head = head[0]
+    #         possible = set(field_tbl.get(head))
+
+    #         groups = {}
+
+    #         for val in possible:
+    #             groups[val] = field_tbl.where(**{head:val}
+    #                                             ).select('subject_id')
+
+    #     return groups
+
+    def datatypes(self, pattern='*'):
+        graph = nx.DiGraph()
+        graph.add_node('datatypes')
+        graph.labels = {'datatypes': 'datatypes'}
+        graph.weights = {'datatypes': 100.0}
+
+        datatypes = self._intf.inspect.datatypes(pattern)
+        namespaces = set([dat.split(':')[0] for dat in datatypes])
+
+        for ns in namespaces:
+            graph.add_edge('datatypes', ns)
+            graph.weights[ns] = 70.0
+
+            for dat in datatypes:
+                if dat.startswith(ns):
+                    graph.add_edge(ns, dat)
+                    graph.weights[dat] = 40.0
+
+        return graph
+
+    def rest_resource(self, name):
+        resource_types = self._intf.inspect._resource_types(name)
+
+        graph = nx.DiGraph()
+        graph.add_node(name)
+        graph.labels = {name: name}
+        graph.weights = {name: 100.0}
+
+        namespaces = set([exp.split(':')[0] for exp in resource_types])
+
+        for ns in namespaces:
+            graph.add_edge(name, ns)
+            graph.weights[ns] = 70.0
+
+            for exp in resource_types:
+                if exp.startswith(ns):
+                    graph.add_edge(ns, exp)
+                    graph.weights[exp] = 40.0
+
+        return graph
+
+    def field_values(self, field_name):
+
+        search_tbl = Search(field_name.split('/')[0],
+                            [field_name], self._intf
+                            )
+
+        criteria = [('%s/ID' % field_name.split('/')[0], 'LIKE', '%'), 'AND']
+
+        dist = {}
+
+        for entry in search_tbl.where(criteria):
+            for val in entry.values():
+                dist.setdefault(val, 1.0)
+                dist[val] += 1
+
+        graph = nx.Graph()
+        graph.add_node(field_name)
+        graph.weights = dist
+        graph.weights[field_name] = 100.0
+
+        for val in dist.keys():
+            graph.add_edge(field_name, val)
+
+        return graph
+
+    def architecture(self, with_datatypes=True):
+        graph = nx.DiGraph()
+        graph.add_node('projects')
+        graph.labels = {'projects': 'projects'}
+        graph.weights = {'projects': 100.0}
+
+        def traverse(lkw, as_lkw):
+
+            for key in schema.resources_tree[lkw]:
+                as_key = '%s_%s' % (as_lkw, key)
+                weight = (1 - len(as_key*2)/100.0) * 100
+                graph.add_edge(as_lkw, as_key)
+                graph.labels[as_key] = key
+                graph.weights[as_key] = weight
+
+                if with_datatypes:
+                    for uri in self._struct.keys():
+                        if uri.split('/')[-2] == key:
+                            datatype = self._struct[uri]
+                            graph.add_edge(as_key, datatype)
+                            graph.weights[datatype] = 10
+                            graph.labels[datatype] = datatype
+
+                traverse(key, as_key)
+
+        traverse('projects', 'projects')
+
+        return graph
+
+
+class PaintGraph(object):
+    def __init__(self, interface):
+        self._intf = interface
+        self.get_graph = interface._get_graph
+
+    def architecture(self, with_datatypes=True, save=None):
+        graph = self.get_graph.architecture(with_datatypes)
+
+        plt.figure(figsize=(8, 8))
+        pos = graphviz_layout(graph, prog='twopi', args='')
+
+        # node_size = [(float(graph.degree(v)) * 5)**3 for v in graph]
+        # node_size = [graph.weights[v] ** 2 for v in graph]
+        # node_color = [float(graph.degree(v)) for v in graph]
+        # node_color = [graph.weights[v] ** 2 for v in graph]
+
+        cost = lambda v: float(graph.degree(v)) ** 3 + \
+            graph.weights[v] ** 2
+
+        costs = norm_costs([cost(v) for v in graph], 10000)
+
+        nx.draw(graph, pos, labels=graph.labels,
+                node_size=costs, node_color=costs,
+                font_size=13, font_color='orange',
+                font_weight='bold', with_labels=True
+                )
+
+        plt.axis('off')
+
+        if save is not None:
+            plt.savefig(save)
+
+        plt.show()
+
+    def experiments(self, save=None):
+        graph = self.get_graph.rest_resource('experiments')
+        self._draw_rest_resource(graph, save=None)
+
+    def assessors(self, save=None):
+        graph = self.get_graph.rest_resource('assessors')
+        self._draw_rest_resource(graph, save=None)
+
+    def reconstructions(self, save=None):
+        graph = self.get_graph.rest_resource('reconstructions')
+        self._draw_rest_resource(graph, save=None)
+
+    def scans(self):
+        graph = self.get_graph.rest_resource('scans')
+        self._draw_rest_resource(graph)
+
+    def _draw_rest_resource(self, graph, save=None):
+        plt.figure(figsize=(8, 8))
+        pos = graphviz_layout(graph, prog='twopi', args='')
+
+        cost = lambda v: float(graph.degree(v)) ** 3 + \
+            graph.weights[v] ** 2
+
+        node_size = [cost(v) for v in graph]
+        # node_size = [graph.weights[v] ** 2 for v in graph]
+        # node_color = [float(graph.degree(v)) for v in graph]
+        node_color = [cost(v) for v in graph]
+
+        nx.draw(graph, pos,
+                node_size=node_size, node_color=node_color,
+                font_size=13, font_color='green', font_weight='bold'
+                )
+
+        plt.axis('off')
+
+        if save is not None:
+            plt.savefig(save)
+
+        plt.show()
+
+    def datatypes(self, pattern='*', save=None):
+        graph = self.get_graph.datatypes(pattern)
+
+        plt.figure(figsize=(8, 8))
+        pos = graphviz_layout(graph, prog='twopi', args='')
+
+        cost = lambda v: float(graph.degree(v)) ** 3 + \
+            graph.weights[v] ** 2
+
+        node_size = [cost(v) for v in graph]
+        # node_size = [graph.weights[v] ** 2 for v in graph]
+        # node_color = [float(graph.degree(v)) for v in graph]
+        node_color = [cost(v) for v in graph]
+
+        nx.draw(graph, pos,
+                node_size=node_size, node_color=node_color,
+                font_size=13, font_color='green', font_weight='bold',
+                with_labels=True
+                )
+
+        plt.axis('off')
+
+        if save is not None:
+            plt.savefig(save)
+
+        plt.show()
+
+    def field_values(self, field_name, save=None):
+        graph = self.get_graph.field_values(field_name)
+
+        plt.figure(figsize=(8, 8))
+        pos = graphviz_layout(graph, prog='twopi', args='')
+
+        cost = lambda v: graph.weights[v]
+
+        graph.weights[field_name] = max([cost(v) for v in graph]) / 2.0
+
+        costs = norm_costs([cost(v) for v in graph], 10000)
+
+        nx.draw(graph, pos,
+                node_size=costs, node_color=costs,
+                font_size=13, font_color='black',
+                font_weight='bold', with_labels=True
+                )
+
+        plt.axis('off')
+
+        if save is not None:
+            plt.savefig(save)
+
+        plt.show()
+
+
+def norm_costs(costs, norm=1000):
+    max_cost = max(costs)
+
+    return [(cost / max_cost) * norm for cost in costs]
+
+
+# class GraphDrawer(object):
+#     def __init__(self, interface):
+#         self._intf = interface
+
+#     def datatypes(self, project):
+#         self._intf.connection.set_strategy('offline')
+
+#         experiments_types = self._intf.inspect.datatypes.experiments(project)
+
+#         labels = {project:project, 'Experiments':'Experiments'}
+
+#         g = nx.Graph()
+
+#         g.add_edge(project, 'Experiments', {'weight':1})
+
+#         for exp_type in experiments_types:
+#             g.add_edge('Experiments', exp_type, {'weight':8})
+#             labels[exp_type] = exp_type
+
+#         pos = nx.graphviz_layout(g, prog='twopi', args='')
+
+#         nx.draw_networkx_nodes(g, pos,
+#                                nodelist=[project],
+#                                node_color='green', alpha=0.7,
+#                                node_size=2500, node_shape='s')
+
+#         nx.draw_networkx_nodes(g, pos,
+#                                nodelist=['Experiments'],
+#                                node_color='blue', alpha=0.7,
+#                                node_size=2000, node_shape='p')
+
+#         nx.draw_networkx_nodes(g, pos,
+#                                nodelist=experiments_types,
+#                                node_color='red', alpha=0.7,
+#                                node_size=1500, node_shape='o')
+
+#         nx.draw_networkx_edges(g, pos, width=2, alpha=0.5,
+#                                edge_color='black')
+
+#         nx.draw_networkx_labels(g, pos, labels,
+#                                 alpha=0.9, font_size=8,
+#                                 font_color='black', font_weight='bold')
+
+#         plt.axis('off')
+#         plt.show()
+
+#         self._intf.connection.revert_strategy()
+
+class SchemasInspector(object):
+    def __init__(self, interface):
+        self._intf = interface
+
+    def __call__(self):
+        self._intf.manage.schemas()
+
+        for xsd in self._intf.manage.schemas():
+            print('-'*40)
+            print(xsd.upper())
+            print('-'*40)
+            print()
+
+            trees = self._intf.manage.schemas._trees[xsd]
+            for datatype in schema.datatypes(trees):
+                print('[%s]' % datatype)
+                print()
+
+                for path in schema.datatype_attributes(trees, datatype):
+                    print(path)
+
+                print()
+
+    def look_for(self, element_name, datatype_name=None):
+        paths = []
+        self._intf.manage.schemas._init()
+
+        if ':' in element_name:
+            for root in self._intf.manage.schemas._trees.values():
+                paths.extend(schema.datatype_attributes(root, element_name))
+            return paths
+
+        for xsd in self._intf.manage.schemas():
+            # nsmap = self._intf.manage.schemas._trees[xsd].nsmap
+            trees = self._intf.manage.schemas._trees[xsd]
+            if datatype_name is not None:
+                datatypes = [datatype_name]
+            else:
+                datatypes = schema.datatypes(trees)
+
+            for datatype in datatypes:
+                for path in schema.datatype_attributes(trees, datatype):
+                    if element_name in path:
+                        paths.append(path)
+
+        return paths
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/httputil.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/httputil.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-
-_boundary = '----------ThIs_Is_tHe_bouNdaRY_$'
-_crlf = '\r\n'
-
-
-def file_message(content, content_type, path, name):
-    body = []
-    body.append('--' + _boundary)
-    body.append('Content-Disposition: form-data; '
-                'name="%s"; filename="%s"' % (path, name)
-                )
-    body.append('Content-Type: %s' % content_type)
-    body.append('')
-
-    body.append(content)
-    body.append('--' + _boundary + '--')
-    body.append('')
-    body = _crlf.join(body)
-    content_type = 'multipart/form-data; boundary=%s' % _boundary
-
-    return body, content_type
+
+_boundary = '----------ThIs_Is_tHe_bouNdaRY_$'
+_crlf = '\r\n'
+
+
+def file_message(content, content_type, path, name):
+    body = []
+    body.append('--' + _boundary)
+    body.append('Content-Disposition: form-data; '
+                'name="%s"; filename="%s"' % (path, name)
+                )
+    body.append('Content-Type: %s' % content_type)
+    body.append('')
+
+    body.append(content)
+    body.append('--' + _boundary + '--')
+    body.append('')
+    body = _crlf.join(body)
+    content_type = 'multipart/form-data; boundary=%s' % _boundary
+
+    return body, content_type
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/interfaces.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/jsonutil.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/jsonutil.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/manage.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/manage.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,308 +1,308 @@
-from lxml import etree
-import urllib
-from .search import SearchManager
-from .users import Users
-from .resources import Project
-from .tags import Tags
-from .jsonutil import JsonTable
-
-
-class GlobalManager(object):
-    """ Mainly a container class to provide a clean interface for all
-        management classes.
-    """
-
-    def __init__(self, interface):
-        self._intf = interface
-
-        self.search = SearchManager(self._intf)
-        self.users = Users(self._intf)
-        self.tags = Tags(self._intf)
-        self.schemas = SchemaManager(self._intf)
-        self.prearchive = PreArchive(self._intf)
-
-    def register_callback(self, func):
-        """ Defines a callback to execute when collections of resources are
-            accessed.
-
-            Parameters
-            ----------
-            func: callable
-                A callable that takes the current collection object as first
-                argument and the current element object as second argument.
-
-            Examples
-            --------
-            >>> def notify(cobj, eobj):
-            >>>    print eobj._uri
-            >>> interface.manage.register_callback(notify)
-        """
-        self._intf._callback = func
-
-    def unregister_callback(self):
-        """ Unregisters the callback.
-        """
-        self._intf._callback = None
-
-    def project(self, project_id):
-        """ Returns a project manager.
-        """
-        return ProjectManager(project_id, self._intf)
-
-
-class ProjectManager(object):
-    """ Management interface for projects.
-
-        This functionalities are also available through `Project` objects.
-    """
-
-    def __init__(self, project_id, interface):
-
-        self._intf = interface
-        self._intf._get_entry_point()
-
-        project = Project('%s/projects/%s' % (self._intf._entry,
-                                              project_id
-                                              ),
-                          self._intf
-                          )
-
-        self.prearchive_code = project.prearchive_code
-        self.set_prearchive_code = project.set_prearchive_code
-        self.quarantine_code = project.quarantine_code
-        self.set_quarantine_code = project.set_quarantine_code
-        self.current_arc = project.current_arc
-        self.set_subfolder_in_current_arc = \
-            project.set_subfolder_in_current_arc
-        self.accessibility = project.accessibility
-        self.users = project.users
-        self.owners = project.owners
-        self.members = project.members
-        self.collaborators = project.collaborators
-        self.user_role = project.user_role
-        self.add_user = project.add_user
-        self.remove_user = project.remove_user
-
-
-class SchemaManager(object):
-    """ Management interface for XNAT schemas.
-
-        The aim is to provide a minimal set of functionalities to parse
-        and look at XNAT schemas.
-    """
-
-    def __init__(self, interface):
-        self._intf = interface
-        self._trees = {}
-
-    def __call__(self):
-        return self._trees.keys()
-
-    def add(self, url):
-        """ Loads an additional schema.
-
-            Parameters
-            ----------
-            url: str
-                url of the schema relative to the server.
-                    e.g. for
-                    http://central.xnat.org/xapi/schemas/xnat give
-                    ``/xapi/schemas/xnat``
-
-        """
-
-        # if not re.match('/?schemas/.*/.*\.xsd', url):
-        #    if not 'schemas' in url and re.match('/?\w+/\w+[.]xsd', url):
-        #        url = join_uri('/schemas', url)
-        #
-        #    elif not re.match('^[^/].xsd', url):
-        #        url = '/schemas/%s/%s'%(url.split('.xsd')[0], url)
-        #    else:
-        #        raise NotImplementedError
-
-        self._trees[url.split('/')[-1]] = \
-            etree.fromstring(self._intf._exec(url))
-
-    def remove(self, name):
-        """ Removes a schema.
-        """
-        if name in self._trees.keys():
-            del self._trees[name]
-
-
-"""
-   Fields Of the Prearchive
-   ------------------------
-   Each session in the prearchive
-    has the following fields:
-       "project" - The name of the project. "Unassigned" if the session is
-            unassigned.
-       "timestamp" - The time (down to millisecond) that this session was
-            received by XNAT. "20110603_124835868" for example.
-       "lastmod" - The time this session as last modified. Moving, resetting
-            etc. updates this time
-       "uploaded" - The time this session was uploaded to XNAT. Usually the
-            same as "timestamp"
-       "scan_date" - The date this session was scanned.
-       "scan_time" - The time this session was scanned.
-       "subject" - The name of the subject
-       "folderName" - The id of this session. Corresponds to XNAT's session id,
-       "name" - The name of this session. Corresponds to XNAT's session label.
-       "tag" - This session's unique DICOM identifier. Usually the SOP
-            instance UID.
-       "status" - The current status of this session
-       "url" - The unique uri of this session.
-       "autoarchive" - Whether this session should be auto-archived.
-    For more in-depth information about the prearchive see:
-    http://docs.xnat.org/Using+the+Prearchive#XNAT%201.5:%20Managing%20Data%20with%20the%20Prearchive-Operations-Session%20Status
-
-    Uniquely identifying a session
-    ------------------------------
-    Every session in the prearchive uniquely is identified by "project",
-    "timestamp" and "folderName".
-    (13/7/2011) - Each session could have been uniquely identified by the "url"
-                  field or the "tag" field. These are arguably more elegant
-                  identifiers but for now the "project", "timestamp",
-                  "folderName" triple is used.
-
-"""
-
-
-class PreArchive(object):
-    def __init__(self, interface):
-        self._intf = interface
-
-    """
-    Retrieve the status of a session
-    Parameters
-    ----------
-       triple - A list containing the project, timestamp and session id, in
-       that order.
-    """
-    def status(self, triple):
-        return JsonTable(
-            self._intf._get_json('/data/prearchive/projects')
-            ).where(
-            project=triple[0], timestamp=triple[1], folderName=triple[2]
-            ).get('status')
-
-    """
-    Retrieve the contents of the prearchive.
-    """
-    def get(self):
-        return JsonTable(self._intf._get_json('/data/prearchive/projects'),
-                         ['project', 'timestamp', 'folderName']
-                         ).select(['project', 'timestamp', 'folderName']
-                                  ).as_list()[1:]
-
-    """
-    Retrieve the scans of a give session triple
-    Parameters
-    ----------
-       triple - A list containing the project, timestamp and session id, in
-       that order.
-    """
-    def get_scans(self, triple):
-        return JsonTable(self._intf._get_json(
-                '/data/prearchive/projects/%s/scans'
-                % '/'.join(triple))).get('ID')
-
-    """
-    Retrieve the resource of a session triple
-    Parameters
-    ----------
-       triple - A list containing the project, timestamp and session id, in
-       that order.
-       scan_id - id of the scan
-    """
-    def get_resources(self, triple, scan_id):
-        return JsonTable(self._intf._get_json(
-                '/data/prearchive/projects/%s'
-                '/scans/%s/resources' % ('/'.join(triple), scan_id)
-                )).get('label')
-
-    """
-    Retrieve a list of files in a given session triple
-    Parameters
-    ----------
-       triple - A list containing the project, timestamp and session id, in
-       that order.
-       scan_id - id of the scan
-       resource_id - id of the resource
-    """
-    def get_files(self, triple, scan_id, resource_id):
-        return JsonTable(self._intf._get_json(
-                '/data/prearchive/projects/%s'
-                '/scans/%s/resources/%s/files' % ('/'.join(triple),
-                                                  scan_id,
-                                                  resource_id)
-                )).get('Name')
-
-    """
-    Move multiple sessions to a project in the prearchive asynchronously.
-    If only one session is it is done now.
-
-    This does *not* archive a session.
-
-    Parameters
-    ----------
-       uris - a list of session uris
-       new_project - The name of the project to which to move the sessions.
-    """
-
-    def move(self, uris, new_project):
-        add_src = lambda u: urllib.urlencode({'src': u})
-
-        async_ = len(uris) > 1 and 'true' or 'false'
-        print(async_)
-
-        post_body = '&'.join((map(add_src, uris)) +
-                             [urllib.urlencode({'newProject': new_project})] +
-                             [urllib.urlencode({'async': async_})])
-
-        request_uri = '/data/services/prearchive/move?format=csv'
-        ct = {'content-type': 'application/x-www-form-urlencoded'}
-        return self._intf._exec(request_uri, 'POST', post_body, ct)
-
-    """
-    Reinspect the file on the filesystem on the XNAT server and recreate the
-    parameters of the file. Essentially a refresh of the file.
-
-    Be warned that if this session has been scheduled for an operation, that
-    operation is cancelled.
-    Parameters
-    ----------
-       uris - a list of session uris
-       new_project - The name of the project to which to move the sessions.
-    """
-
-    def reset(self, triple):
-        post_body = "action=build"
-        request_uri = '/data/prearchive/projects/%s?format=single' \
-                      % '/'.join(triple)
-        ct = {'content-type': 'application/x-www-form-urlencoded'}
-        return self._intf._exec(request_uri, 'POST', post_body, ct)
-
-    """
-    Delete  a session from the prearchive
-    Parameters
-    ----------
-       uri - The uri of the session to delete
-    """
-
-    def delete(self, uri):
-        post_body = "src=" + uri + "&" + "async=false"
-        request_uri = "/data/services/prearchive/delete?format=csv"
-        ct = {'content-type': 'application/x-www-form-urlencoded'}
-        return self._intf._exec(request_uri, 'POST', post_body, ct)
-    """
-    Get the uri of the given session.
-    Parameters
-    ----------
-       triple - A list containing the project, timestamp and session id, in
-       that order.
-    """
-    def get_uri(self, triple):
-        j = JsonTable(self._intf._get_json('/data/prearchive/projects'))
-        return j.where(project=triple[0], timestamp=triple[1],
-                       folderName=triple[2]).get('url')
+from lxml import etree
+import urllib
+from .search import SearchManager
+from .users import Users
+from .resources import Project
+from .tags import Tags
+from .jsonutil import JsonTable
+
+
+class GlobalManager(object):
+    """ Mainly a container class to provide a clean interface for all
+        management classes.
+    """
+
+    def __init__(self, interface):
+        self._intf = interface
+
+        self.search = SearchManager(self._intf)
+        self.users = Users(self._intf)
+        self.tags = Tags(self._intf)
+        self.schemas = SchemaManager(self._intf)
+        self.prearchive = PreArchive(self._intf)
+
+    def register_callback(self, func):
+        """ Defines a callback to execute when collections of resources are
+            accessed.
+
+            Parameters
+            ----------
+            func: callable
+                A callable that takes the current collection object as first
+                argument and the current element object as second argument.
+
+            Examples
+            --------
+            >>> def notify(cobj, eobj):
+            >>>    print eobj._uri
+            >>> interface.manage.register_callback(notify)
+        """
+        self._intf._callback = func
+
+    def unregister_callback(self):
+        """ Unregisters the callback.
+        """
+        self._intf._callback = None
+
+    def project(self, project_id):
+        """ Returns a project manager.
+        """
+        return ProjectManager(project_id, self._intf)
+
+
+class ProjectManager(object):
+    """ Management interface for projects.
+
+        This functionalities are also available through `Project` objects.
+    """
+
+    def __init__(self, project_id, interface):
+
+        self._intf = interface
+        self._intf._get_entry_point()
+
+        project = Project('%s/projects/%s' % (self._intf._entry,
+                                              project_id
+                                              ),
+                          self._intf
+                          )
+
+        self.prearchive_code = project.prearchive_code
+        self.set_prearchive_code = project.set_prearchive_code
+        self.quarantine_code = project.quarantine_code
+        self.set_quarantine_code = project.set_quarantine_code
+        self.current_arc = project.current_arc
+        self.set_subfolder_in_current_arc = \
+            project.set_subfolder_in_current_arc
+        self.accessibility = project.accessibility
+        self.users = project.users
+        self.owners = project.owners
+        self.members = project.members
+        self.collaborators = project.collaborators
+        self.user_role = project.user_role
+        self.add_user = project.add_user
+        self.remove_user = project.remove_user
+
+
+class SchemaManager(object):
+    """ Management interface for XNAT schemas.
+
+        The aim is to provide a minimal set of functionalities to parse
+        and look at XNAT schemas.
+    """
+
+    def __init__(self, interface):
+        self._intf = interface
+        self._trees = {}
+
+    def __call__(self):
+        return self._trees.keys()
+
+    def add(self, url):
+        """ Loads an additional schema.
+
+            Parameters
+            ----------
+            url: str
+                url of the schema relative to the server.
+                    e.g. for
+                    http://central.xnat.org/xapi/schemas/xnat give
+                    ``/xapi/schemas/xnat``
+
+        """
+
+        # if not re.match('/?schemas/.*/.*\.xsd', url):
+        #    if not 'schemas' in url and re.match('/?\w+/\w+[.]xsd', url):
+        #        url = join_uri('/schemas', url)
+        #
+        #    elif not re.match('^[^/].xsd', url):
+        #        url = '/schemas/%s/%s'%(url.split('.xsd')[0], url)
+        #    else:
+        #        raise NotImplementedError
+
+        self._trees[url.split('/')[-1]] = \
+            etree.fromstring(self._intf._exec(url))
+
+    def remove(self, name):
+        """ Removes a schema.
+        """
+        if name in self._trees.keys():
+            del self._trees[name]
+
+
+"""
+   Fields Of the Prearchive
+   ------------------------
+   Each session in the prearchive
+    has the following fields:
+       "project" - The name of the project. "Unassigned" if the session is
+            unassigned.
+       "timestamp" - The time (down to millisecond) that this session was
+            received by XNAT. "20110603_124835868" for example.
+       "lastmod" - The time this session as last modified. Moving, resetting
+            etc. updates this time
+       "uploaded" - The time this session was uploaded to XNAT. Usually the
+            same as "timestamp"
+       "scan_date" - The date this session was scanned.
+       "scan_time" - The time this session was scanned.
+       "subject" - The name of the subject
+       "folderName" - The id of this session. Corresponds to XNAT's session id,
+       "name" - The name of this session. Corresponds to XNAT's session label.
+       "tag" - This session's unique DICOM identifier. Usually the SOP
+            instance UID.
+       "status" - The current status of this session
+       "url" - The unique uri of this session.
+       "autoarchive" - Whether this session should be auto-archived.
+    For more in-depth information about the prearchive see:
+    http://docs.xnat.org/Using+the+Prearchive#XNAT%201.5:%20Managing%20Data%20with%20the%20Prearchive-Operations-Session%20Status
+
+    Uniquely identifying a session
+    ------------------------------
+    Every session in the prearchive uniquely is identified by "project",
+    "timestamp" and "folderName".
+    (13/7/2011) - Each session could have been uniquely identified by the "url"
+                  field or the "tag" field. These are arguably more elegant
+                  identifiers but for now the "project", "timestamp",
+                  "folderName" triple is used.
+
+"""
+
+
+class PreArchive(object):
+    def __init__(self, interface):
+        self._intf = interface
+
+    """
+    Retrieve the status of a session
+    Parameters
+    ----------
+       triple - A list containing the project, timestamp and session id, in
+       that order.
+    """
+    def status(self, triple):
+        return JsonTable(
+            self._intf._get_json('/data/prearchive/projects')
+            ).where(
+            project=triple[0], timestamp=triple[1], folderName=triple[2]
+            ).get('status')
+
+    """
+    Retrieve the contents of the prearchive.
+    """
+    def get(self):
+        return JsonTable(self._intf._get_json('/data/prearchive/projects'),
+                         ['project', 'timestamp', 'folderName']
+                         ).select(['project', 'timestamp', 'folderName']
+                                  ).as_list()[1:]
+
+    """
+    Retrieve the scans of a give session triple
+    Parameters
+    ----------
+       triple - A list containing the project, timestamp and session id, in
+       that order.
+    """
+    def get_scans(self, triple):
+        return JsonTable(self._intf._get_json(
+                '/data/prearchive/projects/%s/scans'
+                % '/'.join(triple))).get('ID')
+
+    """
+    Retrieve the resource of a session triple
+    Parameters
+    ----------
+       triple - A list containing the project, timestamp and session id, in
+       that order.
+       scan_id - id of the scan
+    """
+    def get_resources(self, triple, scan_id):
+        return JsonTable(self._intf._get_json(
+                '/data/prearchive/projects/%s'
+                '/scans/%s/resources' % ('/'.join(triple), scan_id)
+                )).get('label')
+
+    """
+    Retrieve a list of files in a given session triple
+    Parameters
+    ----------
+       triple - A list containing the project, timestamp and session id, in
+       that order.
+       scan_id - id of the scan
+       resource_id - id of the resource
+    """
+    def get_files(self, triple, scan_id, resource_id):
+        return JsonTable(self._intf._get_json(
+                '/data/prearchive/projects/%s'
+                '/scans/%s/resources/%s/files' % ('/'.join(triple),
+                                                  scan_id,
+                                                  resource_id)
+                )).get('Name')
+
+    """
+    Move multiple sessions to a project in the prearchive asynchronously.
+    If only one session is it is done now.
+
+    This does *not* archive a session.
+
+    Parameters
+    ----------
+       uris - a list of session uris
+       new_project - The name of the project to which to move the sessions.
+    """
+
+    def move(self, uris, new_project):
+        add_src = lambda u: urllib.urlencode({'src': u})
+
+        async_ = len(uris) > 1 and 'true' or 'false'
+        print(async_)
+
+        post_body = '&'.join((map(add_src, uris)) +
+                             [urllib.urlencode({'newProject': new_project})] +
+                             [urllib.urlencode({'async': async_})])
+
+        request_uri = '/data/services/prearchive/move?format=csv'
+        ct = {'content-type': 'application/x-www-form-urlencoded'}
+        return self._intf._exec(request_uri, 'POST', post_body, ct)
+
+    """
+    Reinspect the file on the filesystem on the XNAT server and recreate the
+    parameters of the file. Essentially a refresh of the file.
+
+    Be warned that if this session has been scheduled for an operation, that
+    operation is cancelled.
+    Parameters
+    ----------
+       uris - a list of session uris
+       new_project - The name of the project to which to move the sessions.
+    """
+
+    def reset(self, triple):
+        post_body = "action=build"
+        request_uri = '/data/prearchive/projects/%s?format=single' \
+                      % '/'.join(triple)
+        ct = {'content-type': 'application/x-www-form-urlencoded'}
+        return self._intf._exec(request_uri, 'POST', post_body, ct)
+
+    """
+    Delete  a session from the prearchive
+    Parameters
+    ----------
+       uri - The uri of the session to delete
+    """
+
+    def delete(self, uri):
+        post_body = "src=" + uri + "&" + "async=false"
+        request_uri = "/data/services/prearchive/delete?format=csv"
+        ct = {'content-type': 'application/x-www-form-urlencoded'}
+        return self._intf._exec(request_uri, 'POST', post_body, ct)
+    """
+    Get the uri of the given session.
+    Parameters
+    ----------
+       triple - A list containing the project, timestamp and session id, in
+       that order.
+    """
+    def get_uri(self, triple):
+        j = JsonTable(self._intf._get_json('/data/prearchive/projects'))
+        return j.where(project=triple[0], timestamp=triple[1],
+                       folderName=triple[2]).get('url')
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/pathutil.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/pathutil.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import os
-
-
-def find_files(src):
-    names = os.listdir(src)
-
-    errors = []
-    files = []
-
-    for name in names:
-        srcname = os.path.join(src, name)
-        try:
-            if os.path.islink(srcname):
-                linkto = os.readlink(srcname)
-                files.extend(find_files(linkto))
-                # os.symlink(linkto, dstname)
-            elif os.path.isdir(srcname):
-                files.extend(find_files(srcname))
-            else:
-                files.append(srcname)
-        except (IOError, os.error) as why:
-            errors.append((srcname, str(why)))
-
-    return files
-
-
-def ensure_dir_exists(dir_path):
-    if not os.path.exists(dir_path):
-        os.makedirs(dir_path)
-    return os.path.isdir(dir_path)
+import os
+
+
+def find_files(src):
+    names = os.listdir(src)
+
+    errors = []
+    files = []
+
+    for name in names:
+        srcname = os.path.join(src, name)
+        try:
+            if os.path.islink(srcname):
+                linkto = os.readlink(srcname)
+                files.extend(find_files(linkto))
+                # os.symlink(linkto, dstname)
+            elif os.path.isdir(srcname):
+                files.extend(find_files(srcname))
+            else:
+                files.append(srcname)
+        except (IOError, os.error) as why:
+            errors.append((srcname, str(why)))
+
+    return files
+
+
+def ensure_dir_exists(dir_path):
+    if not os.path.exists(dir_path):
+        os.makedirs(dir_path)
+    return os.path.isdir(dir_path)
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/pipelines.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/pipelines.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/provenance.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/provenance.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,309 +1,309 @@
-import time
-import platform
-import socket
-
-from lxml import etree
-from lxml.etree import Element, QName
-
-from .uriutil import uri_parent
-from .jsonutil import JsonTable
-from . import httputil
-
-_nsmap = {'xnat': 'http://nrg.wustl.edu/xnat',
-          'prov': 'http://www.nbirn.net/prov',
-          'xsi': 'http://www.w3.org/2001/XMLSchema-instance'}
-
-_required = ['program', 'timestamp', 'user', 'machine', 'platform']
-_optional = ['program_version', 'program_arguments',
-             'cvs',
-             'platform_version',
-             'compiler', 'compiler_version',
-             'library', 'library_version'
-             ]
-
-_all = ['program', 'program_version', 'program_arguments',
-        'timestamp',
-        'cvs',
-        'user',
-        'machine',
-        'platform', 'platform_version',
-        'compiler', 'compiler_version',
-        # 'library', 'library_version'
-        ]
-
-_platform_name, _hostname, \
-    _platform_version, _platform_version2,\
-    _machine, _machine2 = platform.uname()
-_machine = socket.gethostname()
-
-
-def provenance_document(eobj, process_steps, overwrite):
-    root_node = etree.fromstring(eobj.get())
-
-    existing_prov = None
-    for child in root_node.getchildren():
-        if str(child.tag).endswith('provenance'):
-            existing_prov = child
-            break
-
-    if existing_prov is not None and not overwrite:
-        prov_node = existing_prov
-    else:
-        if existing_prov is not None and overwrite:
-            root_node.remove(existing_prov)
-
-        prov_node = Element(QName(_nsmap['xnat'], 'provenance'),
-                            nsmap=_nsmap
-                            )
-        root_node.insert(0, prov_node)
-
-    prov_node.extend(provenance_parameters(process_steps))
-
-    return etree.tostring(root_node.getroottree())
-
-
-def provenance_parameters(process_steps):
-    prov = []
-
-    for step in process_steps:
-
-        if not set(_required).issubset(step.keys()):
-            missing = list(set(_required).difference(step.keys()))
-
-            raise Exception(('Following attributes are '
-                             'required to define provenance: %s' % missing
-                             )
-                            )
-
-        prov.append(process_step_xml(**step))
-
-    return prov
-
-
-def process_step_xml(**kwargs):
-
-    step_node = Element(QName(_nsmap['prov'], 'processStep'), nsmap=_nsmap)
-
-    program_node = Element(QName(_nsmap['prov'], 'program'), nsmap=_nsmap)
-    program_node.text = kwargs['program']
-
-    if 'program_version' in kwargs.keys():
-        program_node.set('version', kwargs['program_version'])
-
-    if 'program_arguments' in kwargs.keys():
-        program_node.set('arguments', kwargs['program_arguments'])
-
-    step_node.append(program_node)
-
-    timestamp_node = Element(QName(_nsmap['prov'], 'timestamp'),
-                             nsmap=_nsmap
-                             )
-    timestamp_node.text = kwargs['timestamp']
-
-    step_node.append(timestamp_node)
-
-    if 'cvs' in kwargs.keys():
-        cvs_node = Element(QName(_nsmap['prov'], 'cvs'), nsmap=_nsmap)
-        cvs_node.text = kwargs['cvs']
-
-        step_node.append(cvs_node)
-
-    user_node = Element(QName(_nsmap['prov'], 'user'), nsmap=_nsmap)
-    user_node.text = kwargs['user']
-
-    step_node.append(user_node)
-
-    machine_node = Element(QName(_nsmap['prov'], 'machine'), nsmap=_nsmap)
-    machine_node.text = kwargs['machine']
-
-    step_node.append(machine_node)
-
-    platform_node = Element(QName(_nsmap['prov'], 'platform'), nsmap=_nsmap)
-    platform_node.text = kwargs['platform']
-
-    if 'platform_version' in kwargs.keys():
-        platform_node.set('version', kwargs['platform_version'])
-
-    step_node.append(platform_node)
-
-    if 'compiler' in kwargs.keys():
-        compiler_node = Element(QName(_nsmap['prov'], 'compiler'),
-                                nsmap=_nsmap
-                                )
-        compiler_node.text = kwargs['compiler']
-
-        if 'compiler_version' in kwargs.keys():
-            compiler_node.set('version', kwargs['compiler_version'])
-
-        step_node.append(compiler_node)
-
-    if 'library' in kwargs.keys():
-        library_node = Element(QName(_nsmap['prov'], 'library'),
-                               nsmap=_nsmap)
-        library_node.text = kwargs['library']
-
-        if 'library_version' in kwargs.keys():
-            library_node.set('version', kwargs['library_version'])
-
-        step_node.append(library_node)
-
-    return step_node
-
-
-class Provenance(object):
-    """ Class to annotate processed data with provenance information.
-        The following parameters are available:
-
-            - program
-            - program_version
-            - program_arguments
-            - timestamp
-            - cvs
-            - user
-            - machine
-            - platform
-            - platform_version
-            - compiler
-            - compiler_version
-
-        Examples
-        --------
-            >>> prov = {'program':'young',
-                        'timestamp':'2011-03-01T12:01:01.897987',
-                        'user':'angus',
-                        'machine':'war',
-                        'platform':'linux',
-                        }
-            >>> element.provenance.set(prov)
-            >>> element.provenance.get()
-            >>> element.delete()
-    """
-
-    def __init__(self, eobject):
-        self._intf = eobject._intf
-        self._eobject = eobject
-
-    def set(self, process_steps, overwrite=False):
-        """ Set provenance information for the data within this element.
-
-            .. note::
-
-                If some required parameters are not provided, theses
-                parameters will be extracted from the current machine
-                and set automatically. Those parameters are:
-                    - machine
-                    - platform
-                    - timestamp
-                    - user
-
-            .. warning::
-                overwrite option doesn't work because of a bug with the
-                allowDataDeletion flag in XNAT
-
-            Parameters
-            ----------
-            process_steps: list or dict
-                dict or list of dicts to define the processing steps
-                of the data. The minimum set of information to give
-                is: program, timestamp, user, machine and platform. More
-                keywords in the class documentation.
-            overwrite: boolean
-                If False the process_steps are added to the existing ones.
-                Else the processing steps overwrite any existing provenance.
-        """
-        if isinstance(process_steps, dict):
-            process_steps = [process_steps]
-
-        for process_step in process_steps:
-            _timestamp = time.strftime('%Y-%m-%dT%H:%M:%S',
-                                       time.localtime()
-                                       )
-
-            if 'machine' not in process_step.keys():
-                process_step['machine'] = _machine
-            if 'platform' not in process_step.keys():
-                process_step['platform'] = _platform_name
-                process_step['platform_version'] = _platform_version
-            if 'timestamp' not in process_step.keys():
-                process_step['timestamp'] = _timestamp
-            if 'user' not in process_step.keys():
-                process_step['user'] = self._intf._user
-
-        doc = provenance_document(self._eobject, process_steps, overwrite)
-        doc = doc.decode('utf-8')
-
-        body, content_type = httputil.file_message(
-            doc, 'text/xml', 'prov.xml', 'prov.xml')
-
-        prov_uri = self._eobject._uri
-
-        if overwrite:
-            prov_uri += '?allowDataDeletion=true'
-
-        self._intf._exec(prov_uri,
-                         method='PUT',
-                         body=body,
-                         headers={'content-type': content_type})
-
-    def get(self):
-        """ Gets all the provenance information for that object.
-
-            Returns
-            -------
-            A list of dicts.
-        """
-        datatype = self._eobject.datatype()
-
-        columns = ['%s/ID' % datatype] + [
-            '%s/provenance/processStep/%s' % (datatype, field)
-            for field in _all
-            ]
-
-        prov_uri = uri_parent(self._eobject._uri)
-        prov_uri += '?columns='
-        prov_uri += ','.join(columns)
-
-        steps = []
-
-        table = JsonTable(self._intf._get_json(prov_uri))
-
-        id_header = 'ID' if table.has_header('ID') \
-            else '%s/id' % datatype.lower()
-
-        for step in table.where(**{id_header: self._eobject.id()}):
-            step_dict = {}
-            for key in step.keys():
-                if 'processstep' in key:
-                    step_dict[key.split('processstep/')[1]] = step[key]
-
-            steps.append(step_dict)
-
-        return steps
-
-    def delete(self):
-        """ Removes the provenance attached to this object.
-
-            .. warning::
-                doesn't work because of a bug with the allowDataDeletion
-                flag in XNAT
-        """
-
-        provenance_node = self._eobject.xpath('//xnat:provenance')
-
-        if provenance_node != []:
-            provenance_node = provenance_node[0]
-
-            parent_node = provenance_node.getparent()
-            parent_node.remove(provenance_node)
-
-            doc = etree.tostring(parent_node.getroottree())
-
-            body, content_type = httputil.file_message(
-                doc, 'text/xml', 'prov.xml', 'prov.xml')
-
-            self._intf._exec(
-                '%s?allowDataDeletion=true' % self._eobject._uri,
-                method='PUT',
-                body=body,
-                headers={'content-type': content_type}
-                )
+import time
+import platform
+import socket
+
+from lxml import etree
+from lxml.etree import Element, QName
+
+from .uriutil import uri_parent
+from .jsonutil import JsonTable
+from . import httputil
+
+_nsmap = {'xnat': 'http://nrg.wustl.edu/xnat',
+          'prov': 'http://www.nbirn.net/prov',
+          'xsi': 'http://www.w3.org/2001/XMLSchema-instance'}
+
+_required = ['program', 'timestamp', 'user', 'machine', 'platform']
+_optional = ['program_version', 'program_arguments',
+             'cvs',
+             'platform_version',
+             'compiler', 'compiler_version',
+             'library', 'library_version'
+             ]
+
+_all = ['program', 'program_version', 'program_arguments',
+        'timestamp',
+        'cvs',
+        'user',
+        'machine',
+        'platform', 'platform_version',
+        'compiler', 'compiler_version',
+        # 'library', 'library_version'
+        ]
+
+_platform_name, _hostname, \
+    _platform_version, _platform_version2,\
+    _machine, _machine2 = platform.uname()
+_machine = socket.gethostname()
+
+
+def provenance_document(eobj, process_steps, overwrite):
+    root_node = etree.fromstring(eobj.get())
+
+    existing_prov = None
+    for child in root_node.getchildren():
+        if str(child.tag).endswith('provenance'):
+            existing_prov = child
+            break
+
+    if existing_prov is not None and not overwrite:
+        prov_node = existing_prov
+    else:
+        if existing_prov is not None and overwrite:
+            root_node.remove(existing_prov)
+
+        prov_node = Element(QName(_nsmap['xnat'], 'provenance'),
+                            nsmap=_nsmap
+                            )
+        root_node.insert(0, prov_node)
+
+    prov_node.extend(provenance_parameters(process_steps))
+
+    return etree.tostring(root_node.getroottree())
+
+
+def provenance_parameters(process_steps):
+    prov = []
+
+    for step in process_steps:
+
+        if not set(_required).issubset(step.keys()):
+            missing = list(set(_required).difference(step.keys()))
+
+            raise Exception(('Following attributes are '
+                             'required to define provenance: %s' % missing
+                             )
+                            )
+
+        prov.append(process_step_xml(**step))
+
+    return prov
+
+
+def process_step_xml(**kwargs):
+
+    step_node = Element(QName(_nsmap['prov'], 'processStep'), nsmap=_nsmap)
+
+    program_node = Element(QName(_nsmap['prov'], 'program'), nsmap=_nsmap)
+    program_node.text = kwargs['program']
+
+    if 'program_version' in kwargs.keys():
+        program_node.set('version', kwargs['program_version'])
+
+    if 'program_arguments' in kwargs.keys():
+        program_node.set('arguments', kwargs['program_arguments'])
+
+    step_node.append(program_node)
+
+    timestamp_node = Element(QName(_nsmap['prov'], 'timestamp'),
+                             nsmap=_nsmap
+                             )
+    timestamp_node.text = kwargs['timestamp']
+
+    step_node.append(timestamp_node)
+
+    if 'cvs' in kwargs.keys():
+        cvs_node = Element(QName(_nsmap['prov'], 'cvs'), nsmap=_nsmap)
+        cvs_node.text = kwargs['cvs']
+
+        step_node.append(cvs_node)
+
+    user_node = Element(QName(_nsmap['prov'], 'user'), nsmap=_nsmap)
+    user_node.text = kwargs['user']
+
+    step_node.append(user_node)
+
+    machine_node = Element(QName(_nsmap['prov'], 'machine'), nsmap=_nsmap)
+    machine_node.text = kwargs['machine']
+
+    step_node.append(machine_node)
+
+    platform_node = Element(QName(_nsmap['prov'], 'platform'), nsmap=_nsmap)
+    platform_node.text = kwargs['platform']
+
+    if 'platform_version' in kwargs.keys():
+        platform_node.set('version', kwargs['platform_version'])
+
+    step_node.append(platform_node)
+
+    if 'compiler' in kwargs.keys():
+        compiler_node = Element(QName(_nsmap['prov'], 'compiler'),
+                                nsmap=_nsmap
+                                )
+        compiler_node.text = kwargs['compiler']
+
+        if 'compiler_version' in kwargs.keys():
+            compiler_node.set('version', kwargs['compiler_version'])
+
+        step_node.append(compiler_node)
+
+    if 'library' in kwargs.keys():
+        library_node = Element(QName(_nsmap['prov'], 'library'),
+                               nsmap=_nsmap)
+        library_node.text = kwargs['library']
+
+        if 'library_version' in kwargs.keys():
+            library_node.set('version', kwargs['library_version'])
+
+        step_node.append(library_node)
+
+    return step_node
+
+
+class Provenance(object):
+    """ Class to annotate processed data with provenance information.
+        The following parameters are available:
+
+            - program
+            - program_version
+            - program_arguments
+            - timestamp
+            - cvs
+            - user
+            - machine
+            - platform
+            - platform_version
+            - compiler
+            - compiler_version
+
+        Examples
+        --------
+            >>> prov = {'program':'young',
+                        'timestamp':'2011-03-01T12:01:01.897987',
+                        'user':'angus',
+                        'machine':'war',
+                        'platform':'linux',
+                        }
+            >>> element.provenance.set(prov)
+            >>> element.provenance.get()
+            >>> element.delete()
+    """
+
+    def __init__(self, eobject):
+        self._intf = eobject._intf
+        self._eobject = eobject
+
+    def set(self, process_steps, overwrite=False):
+        """ Set provenance information for the data within this element.
+
+            .. note::
+
+                If some required parameters are not provided, theses
+                parameters will be extracted from the current machine
+                and set automatically. Those parameters are:
+                    - machine
+                    - platform
+                    - timestamp
+                    - user
+
+            .. warning::
+                overwrite option doesn't work because of a bug with the
+                allowDataDeletion flag in XNAT
+
+            Parameters
+            ----------
+            process_steps: list or dict
+                dict or list of dicts to define the processing steps
+                of the data. The minimum set of information to give
+                is: program, timestamp, user, machine and platform. More
+                keywords in the class documentation.
+            overwrite: boolean
+                If False the process_steps are added to the existing ones.
+                Else the processing steps overwrite any existing provenance.
+        """
+        if isinstance(process_steps, dict):
+            process_steps = [process_steps]
+
+        for process_step in process_steps:
+            _timestamp = time.strftime('%Y-%m-%dT%H:%M:%S',
+                                       time.localtime()
+                                       )
+
+            if 'machine' not in process_step.keys():
+                process_step['machine'] = _machine
+            if 'platform' not in process_step.keys():
+                process_step['platform'] = _platform_name
+                process_step['platform_version'] = _platform_version
+            if 'timestamp' not in process_step.keys():
+                process_step['timestamp'] = _timestamp
+            if 'user' not in process_step.keys():
+                process_step['user'] = self._intf._user
+
+        doc = provenance_document(self._eobject, process_steps, overwrite)
+        doc = doc.decode('utf-8')
+
+        body, content_type = httputil.file_message(
+            doc, 'text/xml', 'prov.xml', 'prov.xml')
+
+        prov_uri = self._eobject._uri
+
+        if overwrite:
+            prov_uri += '?allowDataDeletion=true'
+
+        self._intf._exec(prov_uri,
+                         method='PUT',
+                         body=body,
+                         headers={'content-type': content_type})
+
+    def get(self):
+        """ Gets all the provenance information for that object.
+
+            Returns
+            -------
+            A list of dicts.
+        """
+        datatype = self._eobject.datatype()
+
+        columns = ['%s/ID' % datatype] + [
+            '%s/provenance/processStep/%s' % (datatype, field)
+            for field in _all
+            ]
+
+        prov_uri = uri_parent(self._eobject._uri)
+        prov_uri += '?columns='
+        prov_uri += ','.join(columns)
+
+        steps = []
+
+        table = JsonTable(self._intf._get_json(prov_uri))
+
+        id_header = 'ID' if table.has_header('ID') \
+            else '%s/id' % datatype.lower()
+
+        for step in table.where(**{id_header: self._eobject.id()}):
+            step_dict = {}
+            for key in step.keys():
+                if 'processstep' in key:
+                    step_dict[key.split('processstep/')[1]] = step[key]
+
+            steps.append(step_dict)
+
+        return steps
+
+    def delete(self):
+        """ Removes the provenance attached to this object.
+
+            .. warning::
+                doesn't work because of a bug with the allowDataDeletion
+                flag in XNAT
+        """
+
+        provenance_node = self._eobject.xpath('//xnat:provenance')
+
+        if provenance_node != []:
+            provenance_node = provenance_node[0]
+
+            parent_node = provenance_node.getparent()
+            parent_node.remove(provenance_node)
+
+            doc = etree.tostring(parent_node.getroottree())
+
+            body, content_type = httputil.file_message(
+                doc, 'text/xml', 'prov.xml', 'prov.xml')
+
+            self._intf._exec(
+                '%s?allowDataDeletion=true' % self._eobject._uri,
+                method='PUT',
+                body=body,
+                headers={'content-type': content_type}
+                )
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/resources.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/resources.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/schema.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/schema.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/search.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/search.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/select.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/select.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,382 +1,382 @@
-import re
-
-from . import schema
-from .search import Search
-from .resources import CObject, Project, Projects, Experiment, Experiments
-# imports used implicitly
-from .uriutil import inv_translate_uri
-# from .uriutil import uri_last
-from .errors import ProgrammingError
-
-DEBUG = False
-
-
-def is_type_level(element):
-    return element.strip('/') in schema.resources_types and \
-           not is_expand_level(element)
-
-
-def is_singular_type_level(element):
-    return element.strip('/') in schema.resources_singular and \
-           not is_expand_level(element)
-
-
-def is_expand_level(element):
-    return element.startswith('//') and \
-        element.strip('/') in schema.resources_types
-
-
-def is_id_level(element):
-    return element is not None and \
-        element.strip('/') not in schema.resources_types
-
-
-def is_wildid_level(element):
-    return element is not None and \
-        element.strip('/') not in schema.resources_types and \
-        ('?' in element or '*' in element)
-
-
-def expand_level(element, fullpath):
-
-    def find_paths(element, path=[]):
-        resources_dict = schema.resources_tree
-
-        element = element.strip('/')
-        paths = []
-
-        if path == []:
-            path = [element]
-
-        init_path = path[:]
-
-        for key in resources_dict.keys():
-
-            path = init_path[:]
-            if element in resources_dict[key]:
-                path.append(key)
-                look_again = find_paths(key, path)
-
-                if look_again != []:
-                    paths.extend(look_again)
-                else:
-                    path.reverse()
-                    paths.append('/' + '/'.join(path))
-
-        return paths
-
-    absolute_paths = find_paths(element)
-
-    els = re.findall('/{1,2}.*?(?=/{1,2}|$)', fullpath)
-
-    index = els.index(element)
-
-    if index == 0:
-        return absolute_paths
-    else:
-        for i in range(1, 4):
-            if is_type_level(els[index - i]) or\
-               is_expand_level(els[index - i]):
-                parent_level = els[index - i]
-                break
-
-    if parent_level.strip('/') in schema.resources_singular:
-        parent_level += 's'
-
-    return [abspath.split(parent_level)[1]
-            for abspath in absolute_paths
-            if parent_level in abspath]
-
-
-def mtransform(paths):
-    tpaths = []
-
-    for path in paths:
-        els = re.findall('/{1,2}.*?(?=/{1,2}|$)', path)
-        tels = []
-        ignore_path = False
-
-        for i, curr_el in enumerate(els):
-
-            if i + 1 < len(els):
-                next_el = els[i + 1]
-            else:
-                next_el = None
-
-            if is_type_level(curr_el):
-
-                if not is_id_level(next_el):
-                    if not is_singular_type_level(curr_el):
-                        tels.append(curr_el)
-                        tels.append('/*')
-                    else:
-                        tels.append(curr_el + 's')
-                        tels.append('/*')
-                else:
-                    if not is_singular_type_level(curr_el):
-                        if not is_wildid_level(next_el):
-                            tels.append(curr_el.rstrip('s'))
-                        else:
-                            tels.append(curr_el)
-                    else:
-                        if not is_wildid_level(next_el):
-                            tels.append(curr_el)
-                        else:
-                            tels.append(curr_el + 's')
-
-            elif is_expand_level(curr_el):
-
-                exp_paths = [''.join(els[:i] + [rel_path] + els[i + 1:])
-                             for rel_path in expand_level(curr_el, path)
-                             ]
-
-                tpaths.extend(mtransform(exp_paths))
-                ignore_path = True
-                break
-
-            elif is_id_level(curr_el):
-                tels.append(curr_el)
-
-            else:
-                raise ProgrammingError('in %s' % path)
-
-        if not ignore_path:
-            tpaths.append(''.join(tels))
-
-    return tpaths
-
-
-def group_paths(paths):
-    groups = {}
-
-    for path in paths:
-        resources = [el
-                     for el in re.findall('/{1,2}.*?(?=/{1,2}|$)', path)
-                     if el.strip('/') in schema.resources_types
-                     and el.strip('/') not in ['files', 'file']
-                     ]
-
-        if len(resources) == 1:
-            groups.setdefault(resources[0], set()).add(path)
-            continue
-
-        for alt_path in paths:
-            if alt_path.endswith(path):
-
-                alt_rsc = \
-                    [el for el in re.findall('/{1,2}.*?(?=/{1,2}|$)',
-                                             alt_path
-                                             )
-                     if el.strip('/') in schema.resources_types
-                        and el.strip('/') not in ['files', 'file']
-                     ]
-
-                if alt_rsc[-1].strip('/') in \
-                        ['files', 'file', 'resources', 'resource'] + \
-                        list(schema.rest_translation.keys()):
-
-                    groups.setdefault(alt_rsc[-2] + alt_rsc[-1], set()
-                                      ).add(alt_path)
-
-                else:
-                    groups.setdefault(alt_rsc[-1], set()).add(alt_path)
-
-    return groups
-
-
-def compute(path):
-    if not re.match('/project(s)?|//.+', path):
-        path = '/' + path
-
-    path = inv_translate_uri(path)
-
-    try:
-        groups = group_paths(mtransform([path]))
-    except Exception:
-        raise ProgrammingError('in %s' % path)
-
-    best = []
-
-    for name in groups:
-        lightest = (0, None)
-
-        for path in groups[name]:
-            score = len(path.split('/'))
-
-            if lightest == (0, None) or lightest[0] > score:
-                lightest = (score, path)
-
-        best.append(lightest[1])
-
-    return best
-
-
-class Select(object):
-    """ Data selection interface. Callable object that indicates the
-        data to be returned to the user.
-
-        Examples
-        --------
-            Select with a path:
-                >>> interface.select('/projects/myproj/subjects').get()
-
-            Select with a datatype:
-                >>> columns = ['xnat:subjectData/PROJECT',
-                               'xnat:subjectData/SUBJECT_ID'
-                               ]
-                >>> criteria = [('xnat:subjectData/SUBJECT_ID', 'LIKE', '*'),
-                                'AND'
-                                ]
-                >>> interface.select('xnat:subjectData', columns
-                            ).where(criteria)
-    """
-    def __init__(self, interface):
-        """
-            Parameters
-            ----------
-            interface: :class:`Interface`
-                Main interface reference.
-        """
-
-        self._intf = interface
-
-    def project(self, ID):
-        """ Access a particular project.
-
-            Parameters
-            ----------
-            ID: string
-                ID of the project.
-        """
-        self._intf._get_entry_point()
-
-        return globals()['Project'](
-            '%s/projects/%s' % (self._intf._entry, ID), self._intf)
-
-    def projects(self, id_filter='*'):
-        """ Returns the list of all visible projects for the server.
-
-            Parameters
-            ----------
-            id_filter: string
-                Name pattern to filter the returned projects.
-        """
-        self._intf._get_entry_point()
-
-        return globals()['Projects'](
-            '%s/projects' % self._intf._entry, self._intf, id_filter)
-
-    def experiment(self, ID):
-        """ Access a particular experiment.
-
-            Parameters
-            ----------
-            ID: string
-                XNAT ID of experiment (NOT LABEL).
-        """
-        self._intf._get_entry_point()
-
-        return globals()['Experiment'](
-            '%s/experiments/%s' % (self._intf._entry, ID), self._intf)
-
-    def experiments(self, id_filter='*'):
-        """ Returns the list of all visible experiments for the server.
-
-            Parameters
-            ----------
-            id_filter: string
-                Name pattern to filter the returned experiments
-                (MUST BE XNAT ID's not labels).
-        """
-        self._intf._get_entry_point()
-
-        return globals()['Experiments'](
-            '%s/experiments' % self._intf._entry, self._intf, id_filter)
-
-    def tag(self, name):
-        self._intf._get_entry_point()
-
-        return self._intf.manage.tags.get(name).references()
-
-    def tags(self):
-        self._intf._get_entry_point()
-
-        return self._intf.manage.tags()
-
-    def __repr__(self):
-        return '<Root Object>'
-
-    def __call__(self, datatype_or_path, columns=[]):
-        """ Select clause to specify what type of data is to be returned.
-
-            Parameters
-            ----------
-            datatype_or_path: string
-                Can either be a resource path or a datatype:
-                    - when a path, REST resources are returned, the
-                      `columns` argument is useless.
-                    - when a datatype, a search Object is returned,
-                      the `columns` argument has to be specified.
-            columns: list
-                List of fieldtypes e.g. xnat:subjectData/SUBJECT_ID
-                Datatype and columns are used to specify the search table
-                that has to be returned. Use the method `where` on the
-                `Search` object to trigger a search on the database.
-        """
-        self._intf._get_entry_point()
-
-        if datatype_or_path.startswith('/tag'):
-            if len(datatype_or_path.split('/')) == 3:
-                return self.tag(datatype_or_path.split('/')[-1])
-            else:
-                return self.tags()
-
-        if datatype_or_path in ['/', '//', self._intf._entry]:
-            return self
-
-        if datatype_or_path.startswith(self._intf._entry):
-            datatype_or_path = datatype_or_path.split(
-                self._intf._entry, 1)[1]
-
-        if datatype_or_path.startswith('/'):
-            return_list = []
-
-            try:
-                for path in compute(datatype_or_path):
-                    if DEBUG:
-                        print('path: %s' % path)
-
-                    pairs = zip(path.split('/')[1::2], path.split('/')[2::2])
-
-                    # # in case a level id has a / - allowed for files only
-                    # if len(path.split('/')[1:]) % 2 == 1 \
-                    #         and uri_last(path) not in schema.resources_types:
-
-                    #     pairs[-1] = (pairs[-1][0], uri_last(path))
-
-                    obj = self
-                    for resource, identifier in pairs:
-
-                        if isinstance(obj, list):
-                            obj = [getattr(sobj, resource)(identifier)
-                                   for sobj in obj]
-                        else:
-                            obj = getattr(obj, resource)(identifier)
-
-                    return_list.append(obj)
-
-                if len(return_list) == 1:
-                    return return_list[0]
-                else:
-                    return CObject(return_list, self._intf)
-
-            except Exception as e:
-                if DEBUG:
-                    print(e)
-                raise ProgrammingError('in %s' % datatype_or_path)
-
-        else:
-            if columns == []:
-                columns = self._intf.inspect.datatypes(datatype_or_path)
-
-            return Search(datatype_or_path, columns, self._intf)
+import re
+
+from . import schema
+from .search import Search
+from .resources import CObject, Project, Projects, Experiment, Experiments
+# imports used implicitly
+from .uriutil import inv_translate_uri
+# from .uriutil import uri_last
+from .errors import ProgrammingError
+
+DEBUG = False
+
+
+def is_type_level(element):
+    return element.strip('/') in schema.resources_types and \
+           not is_expand_level(element)
+
+
+def is_singular_type_level(element):
+    return element.strip('/') in schema.resources_singular and \
+           not is_expand_level(element)
+
+
+def is_expand_level(element):
+    return element.startswith('//') and \
+        element.strip('/') in schema.resources_types
+
+
+def is_id_level(element):
+    return element is not None and \
+        element.strip('/') not in schema.resources_types
+
+
+def is_wildid_level(element):
+    return element is not None and \
+        element.strip('/') not in schema.resources_types and \
+        ('?' in element or '*' in element)
+
+
+def expand_level(element, fullpath):
+
+    def find_paths(element, path=[]):
+        resources_dict = schema.resources_tree
+
+        element = element.strip('/')
+        paths = []
+
+        if path == []:
+            path = [element]
+
+        init_path = path[:]
+
+        for key in resources_dict.keys():
+
+            path = init_path[:]
+            if element in resources_dict[key]:
+                path.append(key)
+                look_again = find_paths(key, path)
+
+                if look_again != []:
+                    paths.extend(look_again)
+                else:
+                    path.reverse()
+                    paths.append('/' + '/'.join(path))
+
+        return paths
+
+    absolute_paths = find_paths(element)
+
+    els = re.findall('/{1,2}.*?(?=/{1,2}|$)', fullpath)
+
+    index = els.index(element)
+
+    if index == 0:
+        return absolute_paths
+    else:
+        for i in range(1, 4):
+            if is_type_level(els[index - i]) or\
+               is_expand_level(els[index - i]):
+                parent_level = els[index - i]
+                break
+
+    if parent_level.strip('/') in schema.resources_singular:
+        parent_level += 's'
+
+    return [abspath.split(parent_level)[1]
+            for abspath in absolute_paths
+            if parent_level in abspath]
+
+
+def mtransform(paths):
+    tpaths = []
+
+    for path in paths:
+        els = re.findall('/{1,2}.*?(?=/{1,2}|$)', path)
+        tels = []
+        ignore_path = False
+
+        for i, curr_el in enumerate(els):
+
+            if i + 1 < len(els):
+                next_el = els[i + 1]
+            else:
+                next_el = None
+
+            if is_type_level(curr_el):
+
+                if not is_id_level(next_el):
+                    if not is_singular_type_level(curr_el):
+                        tels.append(curr_el)
+                        tels.append('/*')
+                    else:
+                        tels.append(curr_el + 's')
+                        tels.append('/*')
+                else:
+                    if not is_singular_type_level(curr_el):
+                        if not is_wildid_level(next_el):
+                            tels.append(curr_el.rstrip('s'))
+                        else:
+                            tels.append(curr_el)
+                    else:
+                        if not is_wildid_level(next_el):
+                            tels.append(curr_el)
+                        else:
+                            tels.append(curr_el + 's')
+
+            elif is_expand_level(curr_el):
+
+                exp_paths = [''.join(els[:i] + [rel_path] + els[i + 1:])
+                             for rel_path in expand_level(curr_el, path)
+                             ]
+
+                tpaths.extend(mtransform(exp_paths))
+                ignore_path = True
+                break
+
+            elif is_id_level(curr_el):
+                tels.append(curr_el)
+
+            else:
+                raise ProgrammingError('in %s' % path)
+
+        if not ignore_path:
+            tpaths.append(''.join(tels))
+
+    return tpaths
+
+
+def group_paths(paths):
+    groups = {}
+
+    for path in paths:
+        resources = [el
+                     for el in re.findall('/{1,2}.*?(?=/{1,2}|$)', path)
+                     if el.strip('/') in schema.resources_types
+                     and el.strip('/') not in ['files', 'file']
+                     ]
+
+        if len(resources) == 1:
+            groups.setdefault(resources[0], set()).add(path)
+            continue
+
+        for alt_path in paths:
+            if alt_path.endswith(path):
+
+                alt_rsc = \
+                    [el for el in re.findall('/{1,2}.*?(?=/{1,2}|$)',
+                                             alt_path
+                                             )
+                     if el.strip('/') in schema.resources_types
+                        and el.strip('/') not in ['files', 'file']
+                     ]
+
+                if alt_rsc[-1].strip('/') in \
+                        ['files', 'file', 'resources', 'resource'] + \
+                        list(schema.rest_translation.keys()):
+
+                    groups.setdefault(alt_rsc[-2] + alt_rsc[-1], set()
+                                      ).add(alt_path)
+
+                else:
+                    groups.setdefault(alt_rsc[-1], set()).add(alt_path)
+
+    return groups
+
+
+def compute(path):
+    if not re.match('/project(s)?|//.+', path):
+        path = '/' + path
+
+    path = inv_translate_uri(path)
+
+    try:
+        groups = group_paths(mtransform([path]))
+    except Exception:
+        raise ProgrammingError('in %s' % path)
+
+    best = []
+
+    for name in groups:
+        lightest = (0, None)
+
+        for path in groups[name]:
+            score = len(path.split('/'))
+
+            if lightest == (0, None) or lightest[0] > score:
+                lightest = (score, path)
+
+        best.append(lightest[1])
+
+    return best
+
+
+class Select(object):
+    """ Data selection interface. Callable object that indicates the
+        data to be returned to the user.
+
+        Examples
+        --------
+            Select with a path:
+                >>> interface.select('/projects/myproj/subjects').get()
+
+            Select with a datatype:
+                >>> columns = ['xnat:subjectData/PROJECT',
+                               'xnat:subjectData/SUBJECT_ID'
+                               ]
+                >>> criteria = [('xnat:subjectData/SUBJECT_ID', 'LIKE', '*'),
+                                'AND'
+                                ]
+                >>> interface.select('xnat:subjectData', columns
+                            ).where(criteria)
+    """
+    def __init__(self, interface):
+        """
+            Parameters
+            ----------
+            interface: :class:`Interface`
+                Main interface reference.
+        """
+
+        self._intf = interface
+
+    def project(self, ID):
+        """ Access a particular project.
+
+            Parameters
+            ----------
+            ID: string
+                ID of the project.
+        """
+        self._intf._get_entry_point()
+
+        return globals()['Project'](
+            '%s/projects/%s' % (self._intf._entry, ID), self._intf)
+
+    def projects(self, id_filter='*'):
+        """ Returns the list of all visible projects for the server.
+
+            Parameters
+            ----------
+            id_filter: string
+                Name pattern to filter the returned projects.
+        """
+        self._intf._get_entry_point()
+
+        return globals()['Projects'](
+            '%s/projects' % self._intf._entry, self._intf, id_filter)
+
+    def experiment(self, ID):
+        """ Access a particular experiment.
+
+            Parameters
+            ----------
+            ID: string
+                XNAT ID of experiment (NOT LABEL).
+        """
+        self._intf._get_entry_point()
+
+        return globals()['Experiment'](
+            '%s/experiments/%s' % (self._intf._entry, ID), self._intf)
+
+    def experiments(self, id_filter='*'):
+        """ Returns the list of all visible experiments for the server.
+
+            Parameters
+            ----------
+            id_filter: string
+                Name pattern to filter the returned experiments
+                (MUST BE XNAT ID's not labels).
+        """
+        self._intf._get_entry_point()
+
+        return globals()['Experiments'](
+            '%s/experiments' % self._intf._entry, self._intf, id_filter)
+
+    def tag(self, name):
+        self._intf._get_entry_point()
+
+        return self._intf.manage.tags.get(name).references()
+
+    def tags(self):
+        self._intf._get_entry_point()
+
+        return self._intf.manage.tags()
+
+    def __repr__(self):
+        return '<Root Object>'
+
+    def __call__(self, datatype_or_path, columns=[]):
+        """ Select clause to specify what type of data is to be returned.
+
+            Parameters
+            ----------
+            datatype_or_path: string
+                Can either be a resource path or a datatype:
+                    - when a path, REST resources are returned, the
+                      `columns` argument is useless.
+                    - when a datatype, a search Object is returned,
+                      the `columns` argument has to be specified.
+            columns: list
+                List of fieldtypes e.g. xnat:subjectData/SUBJECT_ID
+                Datatype and columns are used to specify the search table
+                that has to be returned. Use the method `where` on the
+                `Search` object to trigger a search on the database.
+        """
+        self._intf._get_entry_point()
+
+        if datatype_or_path.startswith('/tag'):
+            if len(datatype_or_path.split('/')) == 3:
+                return self.tag(datatype_or_path.split('/')[-1])
+            else:
+                return self.tags()
+
+        if datatype_or_path in ['/', '//', self._intf._entry]:
+            return self
+
+        if datatype_or_path.startswith(self._intf._entry):
+            datatype_or_path = datatype_or_path.split(
+                self._intf._entry, 1)[1]
+
+        if datatype_or_path.startswith('/'):
+            return_list = []
+
+            try:
+                for path in compute(datatype_or_path):
+                    if DEBUG:
+                        print('path: %s' % path)
+
+                    pairs = zip(path.split('/')[1::2], path.split('/')[2::2])
+
+                    # # in case a level id has a / - allowed for files only
+                    # if len(path.split('/')[1:]) % 2 == 1 \
+                    #         and uri_last(path) not in schema.resources_types:
+
+                    #     pairs[-1] = (pairs[-1][0], uri_last(path))
+
+                    obj = self
+                    for resource, identifier in pairs:
+
+                        if isinstance(obj, list):
+                            obj = [getattr(sobj, resource)(identifier)
+                                   for sobj in obj]
+                        else:
+                            obj = getattr(obj, resource)(identifier)
+
+                    return_list.append(obj)
+
+                if len(return_list) == 1:
+                    return return_list[0]
+                else:
+                    return CObject(return_list, self._intf)
+
+            except Exception as e:
+                if DEBUG:
+                    print(e)
+                raise ProgrammingError('in %s' % datatype_or_path)
+
+        else:
+            if columns == []:
+                columns = self._intf.inspect.datatypes(datatype_or_path)
+
+            return Search(datatype_or_path, columns, self._intf)
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/uriutil.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/uriutil.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-from .schema import rest_translation
-# from .schema import resources_types
-
-
-def translate_uri(uri):
-    segs = uri.split('/')
-    for key in rest_translation.keys():
-        if key in segs[-2:]:
-            uri = uri.replace(key, rest_translation[key])
-
-    return uri
-
-
-def inv_translate_uri(uri):
-    inv_table = dict(zip(rest_translation.values(), rest_translation.keys()))
-
-    for key in inv_table.keys():
-        uri = uri.replace('/%s' % key, '/%s' % inv_table[key])
-
-    return uri
-
-
-def join_uri(uri, *segments):
-    part1 = [seg.lstrip('/') for seg in segments]
-    return '/'.join(uri.split('/') + part1).rstrip('/')
-
-
-def uri_last(uri):
-    # return uri.split(uri_parent(uri))[1].strip('/')
-    return uri.split('/')[-1]
-
-
-def uri_nextlast(uri):
-    # return uri_last(uri.split(uri_last(uri))[0].strip('/'))
-    # support files in a hierarchy
-    if '/files/' in uri:
-        return 'files'
-    return uri.split('/')[-2]
-
-
-def uri_parent(uri):
-    # parent = uri
-
-    # if not os.path.split(uri)[1] in resources_types:
-    #     while os.path.split(parent)[1] not in resources_types:
-    #         parent = os.path.split(parent)[0]
-
-    #     return parent
-
-    # support files in a hierarchy by stripping all but one level
-    files_index = uri.find('/files/')
-    if files_index >= 0:
-        uri = uri[:7+files_index]
-    return uri_split(uri)[0]
-
-
-def uri_grandparent(uri):
-    return uri_parent(uri_parent(uri))
-
-
-def uri_split(uri):
-    return uri.rsplit('/', 1)
-
-
-def uri_segment(uri, start=None, end=None):
-    if start is None and end is None:
-        return uri
-    elif start is None:
-        return '/'+'/'.join(uri.split('/')[:end])
-    elif end is None:
-        return '/'+'/'.join(uri.split('/')[start:])
-    else:
-        return '/'+'/'.join(uri.split('/')[start:end])
-
-
-def uri_shape(uri):
-    import re
-
-    kwid_map = dict(zip(uri.split('/')[1::2], uri.split('/')[2::2]))
-    shapes = {}
-
-    for kw in kwid_map:
-        seps = kwid_map[kw]
-
-        for char in re.findall('[a-zA-Z0-9]', seps):
-            seps = seps.replace(char, '')
-            chunks = []
-            p = '|'.join(seps)
-            s = re.split(p, kwid_map[kw]) if p != '' else kwid_map[kw]
-            for chunk in s:
-                try:
-                    float(chunk)
-                    chunk = '*'
-                except Exception:
-                    pass
-
-                chunks.append(chunk)
-
-            shapes[kw] = '?'.join(chunks)
-
-    return make_uri(shapes)
-
-
-def make_uri(_dict):
-    uri = ''
-
-    kws = ['projects', 'subjects', 'experiments', 'assessors',
-           'reconstructions', 'scans', 'resources', 'in_resources',
-           'out_resources', 'files', 'in_files', 'out_files']
-
-    for kw in kws:
-        if kw in _dict.keys():
-            uri += '/%s/%s' % (kw, _dict.get(kw))
-
-    return uri
-
-
-def check_entry(func):
-    def inner(*args, **kwargs):
-        args[0]._intf._get_entry_point()
-        return func(*args, **kwargs)
-
-    return inner
-
-
-def extract_uri(uri):
-    """
-    Destructure the given REST uri into project,subject and experiment.
-
-    Returns None if any one of project,subject or experiment is unspecified in
-    the URI and a (project,subject,experiment) triple otherwise.
-    """
-    # elements in URLs are always separated by /, regardless of client
-    split = uri.split('/')
-    # a well qualified uri has a project subject, and experiment name
-    # so when split the following items should be present:
-    # ['', 'data', 'projects', 'project-name', 'subjects', 'subject-name',
-    # 'experiments', 'experiment-name', 'scans']
-
-    # Based on the above comment if there aren't 9 items in the split list the
-    # uri isn't well qualified
-    if (len(split) != 9):
-        return None
-
-    project = split[3]
-    subject = split[5]
-    experiment = split[7]
-
-    return (project, subject, experiment)
-
-
-def file_path(uri):
-    """return the relative path of the file in the given URI
-
-    for uri = '/.../files/a/b/c', return 'a/b/c'
-
-    raises ValueError (through .index()) if '/files/' is not in the URI
-    """
-    return uri[7+uri.index('/files/'):]
+from .schema import rest_translation
+# from .schema import resources_types
+
+
+def translate_uri(uri):
+    segs = uri.split('/')
+    for key in rest_translation.keys():
+        if key in segs[-2:]:
+            uri = uri.replace(key, rest_translation[key])
+
+    return uri
+
+
+def inv_translate_uri(uri):
+    inv_table = dict(zip(rest_translation.values(), rest_translation.keys()))
+
+    for key in inv_table.keys():
+        uri = uri.replace('/%s' % key, '/%s' % inv_table[key])
+
+    return uri
+
+
+def join_uri(uri, *segments):
+    part1 = [seg.lstrip('/') for seg in segments]
+    return '/'.join(uri.split('/') + part1).rstrip('/')
+
+
+def uri_last(uri):
+    # return uri.split(uri_parent(uri))[1].strip('/')
+    return uri.split('/')[-1]
+
+
+def uri_nextlast(uri):
+    # return uri_last(uri.split(uri_last(uri))[0].strip('/'))
+    # support files in a hierarchy
+    if '/files/' in uri:
+        return 'files'
+    return uri.split('/')[-2]
+
+
+def uri_parent(uri):
+    # parent = uri
+
+    # if not os.path.split(uri)[1] in resources_types:
+    #     while os.path.split(parent)[1] not in resources_types:
+    #         parent = os.path.split(parent)[0]
+
+    #     return parent
+
+    # support files in a hierarchy by stripping all but one level
+    files_index = uri.find('/files/')
+    if files_index >= 0:
+        uri = uri[:7+files_index]
+    return uri_split(uri)[0]
+
+
+def uri_grandparent(uri):
+    return uri_parent(uri_parent(uri))
+
+
+def uri_split(uri):
+    return uri.rsplit('/', 1)
+
+
+def uri_segment(uri, start=None, end=None):
+    if start is None and end is None:
+        return uri
+    elif start is None:
+        return '/'+'/'.join(uri.split('/')[:end])
+    elif end is None:
+        return '/'+'/'.join(uri.split('/')[start:])
+    else:
+        return '/'+'/'.join(uri.split('/')[start:end])
+
+
+def uri_shape(uri):
+    import re
+
+    kwid_map = dict(zip(uri.split('/')[1::2], uri.split('/')[2::2]))
+    shapes = {}
+
+    for kw in kwid_map:
+        seps = kwid_map[kw]
+
+        for char in re.findall('[a-zA-Z0-9]', seps):
+            seps = seps.replace(char, '')
+            chunks = []
+            p = '|'.join(seps)
+            s = re.split(p, kwid_map[kw]) if p != '' else kwid_map[kw]
+            for chunk in s:
+                try:
+                    float(chunk)
+                    chunk = '*'
+                except Exception:
+                    pass
+
+                chunks.append(chunk)
+
+            shapes[kw] = '?'.join(chunks)
+
+    return make_uri(shapes)
+
+
+def make_uri(_dict):
+    uri = ''
+
+    kws = ['projects', 'subjects', 'experiments', 'assessors',
+           'reconstructions', 'scans', 'resources', 'in_resources',
+           'out_resources', 'files', 'in_files', 'out_files']
+
+    for kw in kws:
+        if kw in _dict.keys():
+            uri += '/%s/%s' % (kw, _dict.get(kw))
+
+    return uri
+
+
+def check_entry(func):
+    def inner(*args, **kwargs):
+        args[0]._intf._get_entry_point()
+        return func(*args, **kwargs)
+
+    return inner
+
+
+def extract_uri(uri):
+    """
+    Destructure the given REST uri into project,subject and experiment.
+
+    Returns None if any one of project,subject or experiment is unspecified in
+    the URI and a (project,subject,experiment) triple otherwise.
+    """
+    # elements in URLs are always separated by /, regardless of client
+    split = uri.split('/')
+    # a well qualified uri has a project subject, and experiment name
+    # so when split the following items should be present:
+    # ['', 'data', 'projects', 'project-name', 'subjects', 'subject-name',
+    # 'experiments', 'experiment-name', 'scans']
+
+    # Based on the above comment if there aren't 9 items in the split list the
+    # uri isn't well qualified
+    if (len(split) != 9):
+        return None
+
+    project = split[3]
+    subject = split[5]
+    experiment = split[7]
+
+    return (project, subject, experiment)
+
+
+def file_path(uri):
+    """return the relative path of the file in the given URI
+
+    for uri = '/.../files/a/b/c', return 'a/b/c'
+
+    raises ValueError (through .index()) if '/files/' is not in the URI
+    """
+    return uri[7+uri.index('/files/'):]
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/users.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/users.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from .jsonutil import JsonTable
-
-
-class Users(object):
-    """ Database user management interface. It is used to retrieve information
-        on users registered on a server.
-
-        .. note::
-
-            At the moment user creation and deletion is not supported through
-            the REST API but it will be at some point.
-
-        Examples
-        --------
-            >>> interface.manage.users()
-            ['list_of_users']
-            >>> interface.manage.users.firstname('nosetests')
-            'nose'
-
-        See Also
-        --------
-        :func:`Project.users`
-        :func:`Project.add_user`
-        :func:`Project.remove_user`
-    """
-
-    def __init__(self, interface):
-        """
-            Parameters
-            ----------
-            interface: :class:`Interface`
-                Main interface reference.
-        """
-        self._intf = interface
-
-    def __call__(self):
-        """ Returns the list of all registered users on the server.
-        """
-        self._intf._get_entry_point()
-
-        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
-                         ).get('login', always_list=True)
-
-    def firstname(self, login):
-        """ Returns the firstname of the user.
-        """
-        self._intf._get_entry_point()
-
-        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
-                         ).where(login=login)['firstname']
-
-    def lastname(self, login):
-        """ Returns the lastname of the user.
-        """
-        self._intf._get_entry_point()
-
-        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
-                         ).where(login=login)['lastname']
-
-    def id(self, login):
-        """ Returns the id of the user.
-        """
-        self._intf._get_entry_point()
-
-        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
-                         ).where(login=login)['xdat_user_id']
-
-    def email(self, login):
-        """ Returns the email of the user.
-        """
-        self._intf._get_entry_point()
-
-        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
-                         ).where(login=login)['email']
-
-    def resources(self):
-        """ Returns the resources of the user.
-        """
-        self._intf._get_entry_point()
-
-        print(self._intf._get_json(
-            '%s/user/cache/resources' % self._intf._entry))
+from .jsonutil import JsonTable
+
+
+class Users(object):
+    """ Database user management interface. It is used to retrieve information
+        on users registered on a server.
+
+        .. note::
+
+            At the moment user creation and deletion is not supported through
+            the REST API but it will be at some point.
+
+        Examples
+        --------
+            >>> interface.manage.users()
+            ['list_of_users']
+            >>> interface.manage.users.firstname('nosetests')
+            'nose'
+
+        See Also
+        --------
+        :func:`Project.users`
+        :func:`Project.add_user`
+        :func:`Project.remove_user`
+    """
+
+    def __init__(self, interface):
+        """
+            Parameters
+            ----------
+            interface: :class:`Interface`
+                Main interface reference.
+        """
+        self._intf = interface
+
+    def __call__(self):
+        """ Returns the list of all registered users on the server.
+        """
+        self._intf._get_entry_point()
+
+        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
+                         ).get('login', always_list=True)
+
+    def firstname(self, login):
+        """ Returns the firstname of the user.
+        """
+        self._intf._get_entry_point()
+
+        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
+                         ).where(login=login)['firstname']
+
+    def lastname(self, login):
+        """ Returns the lastname of the user.
+        """
+        self._intf._get_entry_point()
+
+        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
+                         ).where(login=login)['lastname']
+
+    def id(self, login):
+        """ Returns the id of the user.
+        """
+        self._intf._get_entry_point()
+
+        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
+                         ).where(login=login)['xdat_user_id']
+
+    def email(self, login):
+        """ Returns the email of the user.
+        """
+        self._intf._get_entry_point()
+
+        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
+                         ).where(login=login)['email']
+
+    def resources(self):
+        """ Returns the resources of the user.
+        """
+        self._intf._get_entry_point()
+
+        print(self._intf._get_json(
+            '%s/user/cache/resources' % self._intf._entry))
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/xpass.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/xpass.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/core/xpath_store.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/core/xpath_store.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-import re
-from lxml import etree
-
-from .jsonutil import JsonTable
-
-
-def get_subject_id(location):
-    f = open(location, 'rb')
-    content = f.read()
-    f.close()
-
-    subject = re.findall('<xnat:Subject\sID="(.*?)"\s', content)
-
-    if subject != []:
-        return subject[0]
-
-
-class XpathStore(object):
-
-    """ This utility class is used to query XML files describing XNAT
-        subjects but which are stored in the cache directory. Xpath is
-        used as the query lanaguage but a few helpers are provided
-        to make simple queries.
-    """
-
-    def __init__(self, interface):
-        self._intf = interface
-        self._nsmap = {}
-        self._tree = etree.Element('Store')
-
-    def __call__(self, xpath):
-        if self._tree is None:
-            self._load()
-
-        return self._tree.xpath(xpath, namespaces=self._nsmap)
-
-    def _load(self, content):
-        if not content:
-            return
-        new_subject = etree.fromstring(content)
-        self._nsmap = new_subject.nsmap
-        subject_id = new_subject.xpath('@ID')[0]
-        old_subject = self.subject(subject_id)
-        if old_subject:
-            self._tree.replace(old_subject, new_subject)
-        else:
-            self._tree.append(new_subject)
-
-    def _last_modified(self):
-        entry_point = self._intf._get_entry_point()
-        uri = '%s/subjects?columns=last_modified' % entry_point
-
-        return dict(JsonTable(self._intf._get_json(uri),
-                              order_by=['ID', 'last_modified']
-                              ).select(['ID', 'last_modified']
-                                       ).items())
-
-    def update(self):
-        """ Updates the xml files in the cachedir.
-        """
-
-        self.checkout(subjects=self.subjects())
-
-    def checkout(self, project=None, subjects=None):
-        """ Downloads all the subject XMLs for a project or a list
-            of subjects.
-
-            Parameters
-            ----------
-            project: str
-                The id of the project
-            subjects: list
-                List of subjects that have to be downloaded.
-        """
-        if project is not None and subjects is None:
-            for s in self._intf.select('/project/%s/subjects' % project):
-                self._load(s.get())
-        elif subjects is not None:
-            for sid in subjects:
-                self._load(self._intf._exec('%s/subjects/%s?format=xml' % (
-                          self._intf._get_entry_point(), sid))
-                          )
-
-    def subject(self, subject_id):
-        tmp = self.__call__('//xnat:Subject[@ID="%s"]' % (subject_id))
-
-        if len(tmp) > 0:
-            return tmp[1]
-        return None
-
-    def subjects(self):
-        """ Returns all the subject ids.
-        """
-        return self.__call__('//xnat:Subject/attribute::ID')
-
-    def keys(self):
-        """ Returns attribute keys at the subject level.
-        """
-        return self.element_keys('xnat:Subject')
-
-    def values(self, key):
-        """ Returns the values for all subjects for a specific attribute.
-        """
-        return self.element_values('xnat:Subject', key)
-
-    def attrs(self):
-        """ Returns the attributes of all subjects.
-        """
-        return self.element_attrs('xnat:Subject')
-
-    def elements(self):
-        """ Returns the element names for all subjects elements.
-
-            .. note:: in xpath terms, this function is returning all
-                the names of the subjects descendant nodes.
-        """
-        elements = set()
-
-        for element in self.__call__('//xnat:Subject/descendant::*'):
-            for ns in element.nsmap:
-                if element.nsmap[ns] in element.tag:
-                    n = element.tag.replace('{%s}' % element.nsmap[ns],
-                                            '%s:' % ns)
-                    elements.add(n)
-
-        return list(elements)
-
-    def element_attrs(self, name):
-        """ Returns the attributes of this specific element.
-        """
-        attrs = []
-
-        for element in self.__call__('//%s' % name):
-            attrs.append(element.attrib)
-
-        return attrs
-
-    def element_keys(self, name):
-        """ Returns the attribute keys of this specific element.
-        """
-        keys = set()
-
-        for element in self.__call__('//%s' % name):
-            for element_key in element.keys():
-                keys.add(element_key)
-
-        return list(keys)
-
-    def element_values(self, name, key):
-        """ Returns the attribute values of this specific element.
-        """
-        values = set()
-
-        for subject in self.__call__('//%s' % name):
-            values.add(subject.get(key))
-
-        return list(values)
-
-    def element_text(self, name):
-        """ Returns the text values of this specific element.
-        """
-        return list(set(self.__call__('//%s/child::text()' % name)))
+import re
+from lxml import etree
+
+from .jsonutil import JsonTable
+
+
+def get_subject_id(location):
+    f = open(location, 'rb')
+    content = f.read()
+    f.close()
+
+    subject = re.findall('<xnat:Subject\sID="(.*?)"\s', content)
+
+    if subject != []:
+        return subject[0]
+
+
+class XpathStore(object):
+
+    """ This utility class is used to query XML files describing XNAT
+        subjects but which are stored in the cache directory. Xpath is
+        used as the query lanaguage but a few helpers are provided
+        to make simple queries.
+    """
+
+    def __init__(self, interface):
+        self._intf = interface
+        self._nsmap = {}
+        self._tree = etree.Element('Store')
+
+    def __call__(self, xpath):
+        if self._tree is None:
+            self._load()
+
+        return self._tree.xpath(xpath, namespaces=self._nsmap)
+
+    def _load(self, content):
+        if not content:
+            return
+        new_subject = etree.fromstring(content)
+        self._nsmap = new_subject.nsmap
+        subject_id = new_subject.xpath('@ID')[0]
+        old_subject = self.subject(subject_id)
+        if old_subject:
+            self._tree.replace(old_subject, new_subject)
+        else:
+            self._tree.append(new_subject)
+
+    def _last_modified(self):
+        entry_point = self._intf._get_entry_point()
+        uri = '%s/subjects?columns=last_modified' % entry_point
+
+        return dict(JsonTable(self._intf._get_json(uri),
+                              order_by=['ID', 'last_modified']
+                              ).select(['ID', 'last_modified']
+                                       ).items())
+
+    def update(self):
+        """ Updates the xml files in the cachedir.
+        """
+
+        self.checkout(subjects=self.subjects())
+
+    def checkout(self, project=None, subjects=None):
+        """ Downloads all the subject XMLs for a project or a list
+            of subjects.
+
+            Parameters
+            ----------
+            project: str
+                The id of the project
+            subjects: list
+                List of subjects that have to be downloaded.
+        """
+        if project is not None and subjects is None:
+            for s in self._intf.select('/project/%s/subjects' % project):
+                self._load(s.get())
+        elif subjects is not None:
+            for sid in subjects:
+                self._load(self._intf._exec('%s/subjects/%s?format=xml' % (
+                          self._intf._get_entry_point(), sid))
+                          )
+
+    def subject(self, subject_id):
+        tmp = self.__call__('//xnat:Subject[@ID="%s"]' % (subject_id))
+
+        if len(tmp) > 0:
+            return tmp[1]
+        return None
+
+    def subjects(self):
+        """ Returns all the subject ids.
+        """
+        return self.__call__('//xnat:Subject/attribute::ID')
+
+    def keys(self):
+        """ Returns attribute keys at the subject level.
+        """
+        return self.element_keys('xnat:Subject')
+
+    def values(self, key):
+        """ Returns the values for all subjects for a specific attribute.
+        """
+        return self.element_values('xnat:Subject', key)
+
+    def attrs(self):
+        """ Returns the attributes of all subjects.
+        """
+        return self.element_attrs('xnat:Subject')
+
+    def elements(self):
+        """ Returns the element names for all subjects elements.
+
+            .. note:: in xpath terms, this function is returning all
+                the names of the subjects descendant nodes.
+        """
+        elements = set()
+
+        for element in self.__call__('//xnat:Subject/descendant::*'):
+            for ns in element.nsmap:
+                if element.nsmap[ns] in element.tag:
+                    n = element.tag.replace('{%s}' % element.nsmap[ns],
+                                            '%s:' % ns)
+                    elements.add(n)
+
+        return list(elements)
+
+    def element_attrs(self, name):
+        """ Returns the attributes of this specific element.
+        """
+        attrs = []
+
+        for element in self.__call__('//%s' % name):
+            attrs.append(element.attrib)
+
+        return attrs
+
+    def element_keys(self, name):
+        """ Returns the attribute keys of this specific element.
+        """
+        keys = set()
+
+        for element in self.__call__('//%s' % name):
+            for element_key in element.keys():
+                keys.add(element_key)
+
+        return list(keys)
+
+    def element_values(self, name, key):
+        """ Returns the attribute values of this specific element.
+        """
+        values = set()
+
+        for subject in self.__call__('//%s' % name):
+            values.add(subject.get(key))
+
+        return list(values)
+
+    def element_text(self, name):
+        """ Returns the text values of this specific element.
+        """
+        return list(set(self.__call__('//%s/child::text()' % name)))
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/__init__.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/array_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/array_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     @skip_if_no_network
     def test_array_scans(self):
         '''
         Get a list of scans from a given experiment which has multiple types
         of scans (i.e. PETScans and CTScans) and assert it gathers them all.
         '''
-        s = self._intf.array.scans(experiment_id='XNAT_E16718').data
+        s = self._intf.array.scans(experiment_id='xnat_E02685').data
         self.assertEqual(len(s), 1)
 
     @skip_if_no_network
     def test_array_mrscans(self):
         '''
         Get a list of MRI scans from a given experiment which has multiple
         scans mixed (i.e. MRScans and MRSpectroscopies, aka OtherDicomScans)
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/attributes_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/attributes_test.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/custom_variables_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/custom_variables_test.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/graphdata_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/graphdata_test.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/interfaces_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/interfaces_test.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/manage_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/manage_test.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/pipelines_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/pipelines_test.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/prearchive_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/prearchive_test.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/provenance_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/provenance_test.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/repr_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/repr_test.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/resources_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/resources_test.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/search_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/search_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,26 +47,26 @@
     assert isinstance(central.inspect.subject_values(), list)
 
 
 def test_search():
     results = central.select(
         'xnat:mrSessionData',
         central.inspect.datatypes('xnat:mrSessionData')
-        ).where([('xnat:mrSessionData/XNAT_COL_MRSESSIONDATAFIELDSTRENGTH',
-                  'LIKE', '*1.5*'), 'AND'])
+        ).where([('xnat:mrSessionData/tag',
+                  'LIKE', '*anonymized*'), 'AND'])
 
     assert isinstance(results, jsonutil.JsonTable)
 
 
 def test_save_search():
     central.manage.search.save(
         search_name, 'xnat:mrSessionData',
         central.inspect.datatypes('xnat:mrSessionData'),
-        [('xnat:mrSessionData/XNAT_COL_MRSESSIONDATAFIELDSTRENGTH',
-          'LIKE', '*1.5*'), 'AND'])
+        [('xnat:mrSessionData/tag',
+          'LIKE', '*anonymized*'), 'AND'])
 
     assert search_name in central.manage.search.saved()
 
 
 def test_get_search():
     results = central.manage.search.get(search_name)
     assert isinstance(results, jsonutil.JsonTable)
@@ -77,16 +77,16 @@
     assert search_name not in central.manage.search.saved()
 
 
 def test_save_search_template():
     central.manage.search.save_template(
         search_template_name, 'xnat:mrSessionData',
         central.inspect.datatypes('xnat:mrSessionData'),
-        [('xnat:mrSessionData/XNAT_COL_MRSESSIONDATAFIELDSTRENGTH',
-          'LIKE', '*1.5*'), 'AND']
+        [('xnat:mrSessionData/tag',
+          'LIKE', '*anonymized*'), 'AND']
         )
 
     assert search_template_name in central.manage.search.saved_templates()
 
 
 def test_delete_search_template():
     central.manage.search.delete_template(search_template_name)
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/select_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/select_test.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from pyxnat import select
-
-
-def test_switch_to_singular():
-    assert select.compute('/projects/nosetests') == ['/project/nosetests']
-
-
-def test_switch_to_plural():
-    assert select.compute('/project') == ['/projects/*']
-
-
-def test_complete_stars_plural():
-    assert select.compute('/projects/subjects/experiments') == \
-           ['/projects/*/subjects/*/experiments/*']
-
-
-def test_complete_stars_singular():
-    assert select.compute('/project/subject/experiment') == \
-           ['/projects/*/subjects/*/experiments/*']
-
-
-def test_simple_root_expand():
-    assert select.compute('//experiments') == \
-           ['/projects/*/subjects/*/experiments/*']
-
-
-def test_simple_level_expand():
-    assert select.compute('/projects/IMAGEN//experiments') == \
-           ['/project/IMAGEN/subjects/*/experiments/*']
-
-
-def test_leaf_level_expand():
-    assert set(select.compute('//files')) == \
-        set(['/projects/*/subjects/*/experiments/*/resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/reconstructions/*/in_resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/scans/*/resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/assessors/*/out_resources/*/files/*',
-             '/projects/*/subjects/*/resources/*/files/*',
-             '/projects/*/resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/reconstructions/*/out_resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/assessors/*/in_resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/assessors/*/resources/*/files/*'])
-
-
-def test_double_level_expand():
-    assert set(select.compute('//experiments//files')) == \
-        set(['/projects/*/subjects/*/experiments/*/resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/reconstructions/*/in_resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/scans/*/resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/assessors/*/out_resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/assessors/*/in_resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/reconstructions/*/out_resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/assessors/*/resources/*/files/*'])
-
-
-def test_compute_all():
-    assert set(select.compute('/projects/nosetests//experiments/*Session*//files/myfile.txt')) == \
-        set(['/project/nosetests/subjects/*/experiments/*Session*/resources/*/file/myfile.txt',
-             '/project/nosetests/subjects/*/experiments/*Session*/reconstructions/*/in_resources/*/file/myfile.txt',
-             '/project/nosetests/subjects/*/experiments/*Session*/scans/*/resources/*/file/myfile.txt',
-             '/project/nosetests/subjects/*/experiments/*Session*/assessors/*/out_resources/*/file/myfile.txt',
-             '/project/nosetests/subjects/*/experiments/*Session*/assessors/*/in_resources/*/file/myfile.txt',
-             '/project/nosetests/subjects/*/experiments/*Session*/reconstructions/*/out_resources/*/file/myfile.txt',
-             '/project/nosetests/subjects/*/experiments/*Session*/assessors/*/resources/*/file/myfile.txt'])
+from pyxnat import select
+
+
+def test_switch_to_singular():
+    assert select.compute('/projects/nosetests') == ['/project/nosetests']
+
+
+def test_switch_to_plural():
+    assert select.compute('/project') == ['/projects/*']
+
+
+def test_complete_stars_plural():
+    assert select.compute('/projects/subjects/experiments') == \
+           ['/projects/*/subjects/*/experiments/*']
+
+
+def test_complete_stars_singular():
+    assert select.compute('/project/subject/experiment') == \
+           ['/projects/*/subjects/*/experiments/*']
+
+
+def test_simple_root_expand():
+    assert select.compute('//experiments') == \
+           ['/projects/*/subjects/*/experiments/*']
+
+
+def test_simple_level_expand():
+    assert select.compute('/projects/IMAGEN//experiments') == \
+           ['/project/IMAGEN/subjects/*/experiments/*']
+
+
+def test_leaf_level_expand():
+    assert set(select.compute('//files')) == \
+        set(['/projects/*/subjects/*/experiments/*/resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/reconstructions/*/in_resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/scans/*/resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/assessors/*/out_resources/*/files/*',
+             '/projects/*/subjects/*/resources/*/files/*',
+             '/projects/*/resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/reconstructions/*/out_resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/assessors/*/in_resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/assessors/*/resources/*/files/*'])
+
+
+def test_double_level_expand():
+    assert set(select.compute('//experiments//files')) == \
+        set(['/projects/*/subjects/*/experiments/*/resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/reconstructions/*/in_resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/scans/*/resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/assessors/*/out_resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/assessors/*/in_resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/reconstructions/*/out_resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/assessors/*/resources/*/files/*'])
+
+
+def test_compute_all():
+    assert set(select.compute('/projects/nosetests//experiments/*Session*//files/myfile.txt')) == \
+        set(['/project/nosetests/subjects/*/experiments/*Session*/resources/*/file/myfile.txt',
+             '/project/nosetests/subjects/*/experiments/*Session*/reconstructions/*/in_resources/*/file/myfile.txt',
+             '/project/nosetests/subjects/*/experiments/*Session*/scans/*/resources/*/file/myfile.txt',
+             '/project/nosetests/subjects/*/experiments/*Session*/assessors/*/out_resources/*/file/myfile.txt',
+             '/project/nosetests/subjects/*/experiments/*Session*/assessors/*/in_resources/*/file/myfile.txt',
+             '/project/nosetests/subjects/*/experiments/*Session*/reconstructions/*/out_resources/*/file/myfile.txt',
+             '/project/nosetests/subjects/*/experiments/*Session*/assessors/*/resources/*/file/myfile.txt'])
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/sessionmirror_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/sessionmirror_test.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/test_resource_functions.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/test_resource_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -239,7 +239,25 @@
     assert ts.shape == (287, 109)
     assert df.shape[0] == ts.shape[1]
 
     df2 = df.dropna(axis=0, how='all').dropna(axis=1, how='all')
     ts2 = ts.dropna(axis=0, how='all').dropna(axis=1, how='all')
     assert ts2.shape == (287, 99)
     assert df2.shape[0] == ts2.shape[1]
+
+
+def test_3dasl_volumes():
+    r = e1.resource('3DASL_QUANTIFICATION')
+    v = r.volumes()
+    # assert GM > WM > CSF
+    assert(v['T1_fast_pve_1'] > v['T1_fast_pve_2'] > v['T1_fast_pve_0'])
+
+
+def test_3dasl_perfusion():
+    r = e1.resource('3DASL_QUANTIFICATION')
+    perf = r.perfusion()
+    assert(perf.shape == (124, 6))
+    q = 'atlas=="global" & region=="GM"'
+    gm_perf = perf.query(q)['mean'].item()
+    q = 'atlas=="global" & region=="WM"'
+    wm_perf = perf.query(q)['mean'].item()
+    assert(gm_perf > wm_perf)
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/uriutil_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/uriutil_test.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from pyxnat import uriutil
-
-
-def test_translate_uri():
-    assert uriutil.translate_uri('/assessors/out_resources/files') == \
-           '/assessors/out/resources/files'
-    assert uriutil.translate_uri('/assessors/out_resource/files') == \
-           '/assessors/out/resource/files'
-    assert uriutil.translate_uri('/assessors/in_resources/files') == \
-           '/assessors/in/resources/files'
-    assert uriutil.translate_uri('/assessors/in_resource/files') == \
-           '/assessors/in/resource/files'
-
-
-def test_inv_translate_uri():
-    assert uriutil.inv_translate_uri('/assessors/out/resources/files') == \
-           '/assessors/out_resources/files'
-    assert uriutil.inv_translate_uri('/assessors/out/resource/files') == \
-           '/assessors/out_resource/files'
-    assert uriutil.inv_translate_uri('/assessors/in/resources/files') == \
-           '/assessors/in_resources/files'
-    assert uriutil.inv_translate_uri('/assessors/in/resource/files') == \
-           '/assessors/in_resource/files'
-
-
-def test_join_uri():
-    uri = uriutil.join_uri('/projects', 'project_id', 'subjects', 'subject_id')
-    assert uri == '/projects/project_id/subjects/subject_id'
-
-
-def test_uri_last():
-    assert uriutil.uri_last('/projects/1/subjects/2') == '2'
-
-
-def test_uri_nextlast():
-    assert uriutil.uri_nextlast('/projects/1/subjects/2') == 'subjects'
-
-
-def test_uri_parent():
-    uri = uriutil.uri_parent('/projects/1/subjects/2')
-    assert uri == '/projects/1/subjects'
-
-
-def test_uri_grandparent():
-    uri = uriutil.uri_grandparent('/projects/1/subjects/2')
-    assert uri == '/projects/1'
-
-
-def test_uri_split():
-    uri = uriutil.uri_split('/projects/1/subjects/2')
-    assert uri == ['/projects/1/subjects', '2']
+from pyxnat import uriutil
+
+
+def test_translate_uri():
+    assert uriutil.translate_uri('/assessors/out_resources/files') == \
+           '/assessors/out/resources/files'
+    assert uriutil.translate_uri('/assessors/out_resource/files') == \
+           '/assessors/out/resource/files'
+    assert uriutil.translate_uri('/assessors/in_resources/files') == \
+           '/assessors/in/resources/files'
+    assert uriutil.translate_uri('/assessors/in_resource/files') == \
+           '/assessors/in/resource/files'
+
+
+def test_inv_translate_uri():
+    assert uriutil.inv_translate_uri('/assessors/out/resources/files') == \
+           '/assessors/out_resources/files'
+    assert uriutil.inv_translate_uri('/assessors/out/resource/files') == \
+           '/assessors/out_resource/files'
+    assert uriutil.inv_translate_uri('/assessors/in/resources/files') == \
+           '/assessors/in_resources/files'
+    assert uriutil.inv_translate_uri('/assessors/in/resource/files') == \
+           '/assessors/in_resource/files'
+
+
+def test_join_uri():
+    uri = uriutil.join_uri('/projects', 'project_id', 'subjects', 'subject_id')
+    assert uri == '/projects/project_id/subjects/subject_id'
+
+
+def test_uri_last():
+    assert uriutil.uri_last('/projects/1/subjects/2') == '2'
+
+
+def test_uri_nextlast():
+    assert uriutil.uri_nextlast('/projects/1/subjects/2') == 'subjects'
+
+
+def test_uri_parent():
+    uri = uriutil.uri_parent('/projects/1/subjects/2')
+    assert uri == '/projects/1/subjects'
+
+
+def test_uri_grandparent():
+    uri = uriutil.uri_grandparent('/projects/1/subjects/2')
+    assert uri == '/projects/1'
+
+
+def test_uri_split():
+    uri = uriutil.uri_split('/projects/1/subjects/2')
+    assert uri == ['/projects/1/subjects', '2']
```

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/user_and_project_management_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/user_and_project_management_test.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/xpass_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/xpass_test.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/pyxnat/tests/xpath_test.py` & `bbrc-pyxnat-1.6.3.dev1/pyxnat/tests/xpath_test.py`

 * *Files identical despite different names*

### Comparing `bbrc-pyxnat-1.6.2/setup.py` & `bbrc-pyxnat-1.6.3.dev1/setup.py`

 * *Files identical despite different names*

