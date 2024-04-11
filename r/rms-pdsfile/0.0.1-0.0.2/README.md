# Comparing `tmp/rms-pdsfile-0.0.1.tar.gz` & `tmp/rms-pdsfile-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-pdsfile-0.0.1.tar", last modified: Wed Feb  7 22:07:00 2024, max compression
+gzip compressed data, was "rms-pdsfile-0.0.2.tar", last modified: Thu Apr 11 22:19:12 2024, max compression
```

## Comparing `rms-pdsfile-0.0.1.tar` & `rms-pdsfile-0.0.2.tar`

### file list

```diff
@@ -1,91 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 22:07:00.731902 rms-pdsfile-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 22:07:00.711901 rms-pdsfile-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 22:07:00.715901 rms-pdsfile-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-02-07 22:07:00.731902 rms-pdsfile-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 22:07:00.719901 rms-pdsfile-0.0.1/pdsfile/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-07 22:07:00.000000 rms-pdsfile-0.0.1/pdsfile/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 22:07:00.719901 rms-pdsfile-0.0.1/pdsfile/pds3file/
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 22:07:00.723901 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/ASTROM_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    61669 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/COCIRS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46937 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/COISS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51957 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/CORSS_8xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2378 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/COSP_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25740 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/COUVIS_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22597 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/COUVIS_8xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    43611 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/COVIMS_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23350 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/COVIMS_8xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20525 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/EBROCC_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    77854 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/GO_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21788 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/HSTxx_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9721 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/JNOJIR_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7790 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/JNOJNC_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/JNOSP_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2380 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/NHSP_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    53813 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/NHxxxx_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1078 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/RES_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12928 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/RPX_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2523 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/VGIRIS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    64913 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/VGISS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/VG_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2483 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/VG_20xx.py
--rw-r--r--   0 runner    (1001) docker     (127)   129879 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/VG_28xx.py
--rw-r--r--   0 runner    (1001) docker     (127)    36617 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4823 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/rules/pytest_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 22:07:00.723901 rms-pdsfile-0.0.1/pdsfile/pds3file/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    89283 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/tests/test_pds3file_blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    30943 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py
--rw-r--r--   0 runner    (1001) docker     (127)    35772 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/tests/test_pds3file_whitebox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 22:07:00.723901 rms-pdsfile-0.0.1/pdsfile/pds4file/
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds4file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 22:07:00.727902 rms-pdsfile-0.0.1/pdsfile/pds4file/rules/
--rw-r--r--   0 runner    (1001) docker     (127)    36423 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds4file/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46920 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds4file/rules/cassini_iss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47069 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds4file/rules/cassini_vims.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4810 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds4file/rules/pytest_support.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47804 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds4file/rules/uranus_occs_earthbased.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 22:07:00.727902 rms-pdsfile-0.0.1/pdsfile/pds4file/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds4file/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds4file/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24667 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pds4file/tests/test_pds4file_blackbox.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34894 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pdscache.py
--rw-r--r--   0 runner    (1001) docker     (127)   230457 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pdsfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19658 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/pdsviewable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pdsfile/preload_and_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 22:07:00.731902 rms-pdsfile-0.0.1/rms_pdsfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-02-07 22:07:00.000000 rms-pdsfile-0.0.1/rms_pdsfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-02-07 22:07:00.000000 rms-pdsfile-0.0.1/rms_pdsfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 22:07:00.000000 rms-pdsfile-0.0.1/rms_pdsfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-07 22:07:00.000000 rms-pdsfile-0.0.1/rms_pdsfile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-07 22:07:00.000000 rms-pdsfile-0.0.1/rms_pdsfile.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      617 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/run_tests_coverage.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 22:07:00.715901 rms-pdsfile-0.0.1/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 22:07:00.727902 rms-pdsfile-0.0.1/scripts/automated_tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1763 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/scripts/automated_tests/pdsfile_main_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-07 22:07:00.731902 rms-pdsfile-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 22:07:00.727902 rms-pdsfile-0.0.1/validation/
--rwxr-xr-x   0 runner    (1001) docker     (127)    18175 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/validation/pdsarchives.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31377 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/validation/pdschecksums.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/validation/pdsdata-sync.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    34502 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/validation/pdsdependency.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17150 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/validation/pdsindexshelf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31801 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/validation/pdsinfoshelf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    73841 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/validation/pdslinkshelf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29426 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/validation/re-validate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-02-07 22:06:52.000000 rms-pdsfile-0.0.1/validation/shelf-consistency-check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.094759 rms-pdsfile-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.078759 rms-pdsfile-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.078759 rms-pdsfile-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/.github/workflows/run-tests-and-opus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-11 22:19:12.094759 rms-pdsfile-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.082759 rms-pdsfile-0.0.2/pdsfile/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 22:19:11.000000 rms-pdsfile-0.0.2/pdsfile/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.082759 rms-pdsfile-0.0.2/pdsfile/pds3file/
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.086759 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/ASTROM_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    61669 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COCIRS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46937 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COISS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51098 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/CORSS_8xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2378 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COSP_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25774 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COUVIS_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22138 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COUVIS_8xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43611 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COVIMS_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COVIMS_8xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20096 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/EBROCC_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    77854 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/GO_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21822 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/HSTxx_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9721 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/JNOJIR_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7790 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/JNOJNC_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/JNOSP_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2380 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/NHSP_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53813 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/NHxxxx_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1078 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/RES_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12928 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/RPX_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2523 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VGIRIS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    64913 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VGISS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VG_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2483 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VG_20xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129879 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VG_28xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36492 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4823 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/pytest_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.086759 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    89512 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pds3file_blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30950 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35786 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pds3file_whitebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.090759 rms-pdsfile-0.0.2/pdsfile/pds4file/
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.090759 rms-pdsfile-0.0.2/pdsfile/pds4file/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)    36279 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23585 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/rules/cassini_iss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24720 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/rules/cassini_vims.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4872 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/rules/pytest_support.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57915 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/rules/uranus_occs_earthbased.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101120 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.090759 rms-pdsfile-0.0.2/pdsfile/pds4file/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33847 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/tests/test_pds4file_blackbox.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34894 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pdscache.py
+-rw-r--r--   0 runner    (1001) docker     (127)   230846 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pdsfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19658 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pdsviewable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/preload_and_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.094759 rms-pdsfile-0.0.2/rms_pdsfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-11 22:19:12.000000 rms-pdsfile-0.0.2/rms_pdsfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-11 22:19:12.000000 rms-pdsfile-0.0.2/rms_pdsfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:19:12.000000 rms-pdsfile-0.0.2/rms_pdsfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 22:19:12.000000 rms-pdsfile-0.0.2/rms_pdsfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:19:12.000000 rms-pdsfile-0.0.2/rms_pdsfile.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/run_tests_coverage.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.078759 rms-pdsfile-0.0.2/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.090759 rms-pdsfile-0.0.2/scripts/automated_tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1714 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/scripts/automated_tests/pdsfile_main_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 22:19:12.094759 rms-pdsfile-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.094759 rms-pdsfile-0.0.2/validation/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18175 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/pdsarchives.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31377 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/pdschecksums.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/pdsdata-sync.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34502 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/pdsdependency.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17150 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/pdsindexshelf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31801 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/pdsinfoshelf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    73841 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/pdslinkshelf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29426 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/re-validate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/shelf-consistency-check.py
```

### Comparing `rms-pdsfile-0.0.1/.github/workflows/publish_to_test_pypi.yml` & `rms-pdsfile-0.0.2/.github/workflows/publish_to_test_pypi.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 name: Publish to Test PyPI
-run-name: Publish to Test PyPI triggered by ${{ github.ref_type }} ${{ github.ref_name }}
+run-name: "Publish to Test PyPI: ${{ github.ref_type }} ${{ github.ref_name }}"
 
 on:
   workflow_dispatch:
 
 jobs:
   upload_pypi:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python 3.12
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.12
 
       - name: Build
         run: |
-          python3 -m pip install --upgrade build && python3 -m build
+          python -m pip install --upgrade build
+          python -m build
 
       - name: Publish package
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.TEST_PYPI_API_TOKEN }}
           repository-url: https://test.pypi.org/legacy/
```

### Comparing `rms-pdsfile-0.0.1/.github/workflows/run-tests.yml` & `rms-pdsfile-0.0.2/.github/workflows/run-tests.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 name: Run Tests
-run-name: Run Tests triggered by ${{ github.ref_type }} ${{ github.ref_name }} or ${{ github.triggering_actor }}
+run-name: "Run Tests: ${{ github.ref_type }} ${{ github.ref_name }} by ${{ github.triggering_actor }}"
 
 on:
   workflow_dispatch:
-  pull_request:
-    branches: [ main ]
+  workflow_call:
   push:
     branches: [ main ]
   schedule:
     - cron: "00 08 * * *"   # 12am PST, 1am PDT
 
+defaults:
+  run:
+    shell: bash
+
 jobs:
   test:
     name: Test pdsfile
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         # Because we can run multiple tests at the same time
@@ -37,28 +40,48 @@
             python-version: "3.11"
           - os: self-hosted-macos
             python-version: "3.12"
           - os: self-hosted-windows
             python-version: "3.12"
       fail-fast: true
     steps:
-      - name: Checkout
+      - name: Checkout rms-pdsfile
         uses: actions/checkout@v4
         with:
           ref: ${{ github.event.pull_request.head.sha }}
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Test with coverage
+        # Because self-hosted runners keep a global Python environment that
+        # isn't wiped between runs, the various requirements.txt files will
+        # interfere with each other. As a result, we use a venv for cases
+        # where it matters.
         run: |
+          echo
+          env
+          echo
+          rm -rf venv
+          python -m venv venv
+          if [[ ${{ matrix.os }} == self-hosted-windows ]]; then
+            source venv/Scripts/activate
+          else
+            source venv/bin/activate
+          fi
+          python -m pip install --upgrade pip
+          python -m pip install wheel
+          python -m pip install -r requirements.txt
+          echo
+          python -m pip freeze
+          echo
           scripts/automated_tests/pdsfile_main_test.sh
-        shell: bash
 
       - name: Upload coverage report to codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
+        if: matrix.os == 'self-hosted-linux' && matrix.python-version == '3.12'
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           files: ./coverage.xml
           verbose: true
```

### Comparing `rms-pdsfile-0.0.1/.gitignore` & `rms-pdsfile-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/LICENSE` & `rms-pdsfile-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/conftest.py` & `rms-pdsfile-0.0.2/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # Configuration & setup before running tests on pds4file
 ##########################################################################################
 
 import os
 from pdsfile import (Pds3File,
                      Pds4File)
-from pdsfile.pds3file.tests.helper import PDS_HOLDINGS_DIR
+from pdsfile.pds3file.tests.helper import PDS3_HOLDINGS_DIR
 from pdsfile.pds4file.tests.helper import PDS4_HOLDINGS_DIR
 import pdslogger
 import pytest
 
 ##########################################################################################
 # Setup before all tests
 ##########################################################################################
@@ -33,9 +33,9 @@
         Pds3File.use_shelves_only(False)
         Pds4File.use_shelves_only(False)
     else: # pragma: no cover
         Pds3File.use_shelves_only(True)
         Pds4File.use_shelves_only(True)
 
     # turn_on_logger("test_log.txt")
-    Pds3File.preload(PDS_HOLDINGS_DIR)
+    Pds3File.preload(PDS3_HOLDINGS_DIR)
     Pds4File.preload(PDS4_HOLDINGS_DIR)
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/__init__.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/ASTROM_xxxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/ASTROM_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/COCIRS_xxxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COCIRS_xxxx.py`

 * *Files 0% similar despite different names*

```diff
@@ -590,15 +590,15 @@
     (r'diagrams/COCIRS_[56]xxx.*/TARGETS/.*_thumb\..*', 0, ('browse', 10, 'browse_thumb',  'Browse Image (thumbnail)', False)),
     (r'diagrams/COCIRS_[56]xxx.*/TARGETS/.*_small\..*', 0, ('browse', 20, 'browse_small',  'Browse Image (small)',     False)),
     (r'diagrams/COCIRS_[56]xxx.*/TARGETS/.*_med\..*',   0, ('browse', 30, 'browse_medium', 'Browse Image (medium)',    False)),
     (r'diagrams/COCIRS_[56]xxx.*/TARGETS/.*_full\..*',  0, ('browse', 40, 'browse_full',   'Browse Image (full)',      True)),
 
     # CUBE 0xxx/1xxx
     # Cube index
-    (r'metadata/COCIRS_[01]xxx.*/.*cube.*(?<!supplemental)_index\..*',      0, ('metadata',       8, 'cube_index',        'Cube Index',           False)),
+    (r'metadata/COCIRS_[01]xxx.*/.*cube.*(?<!supplemental)_index\..*',      0, ('metadata',       4, 'cube_index',        'Cube Index',           False)),
     # Data
     (r'volumes/COCIRS_[01]xxx.*/DATA/CUBE/.*',             0, ('Cassini CIRS', 10, 'cocirs_cube',  'Spectral Image Cube', True)),
     # Extra viewable image
     (r'volumes/COCIRS_[01]xxx.*/EXTRAS/CUBE_OVERVIEW/.*',  0, ('Cassini CIRS', 20, 'cocirs_extra', 'Extra Cube Preview Image', False)),
 
     # Documentation
     (r'documents/COCIRS_[05]xxx/.*',                       0, ('Cassini CIRS', 700, 'cocirs_documentation', 'Documentation', False)),
@@ -1015,21 +1015,21 @@
           False): ['previews/COCIRS_0xxx/COCIRS_0406/DATA/CUBE/POINT_PERSPECTIVE/000IA_PRESOI001____RI____699_F4_038P_small.jpg'],
          ('browse',
           10,
           'browse_thumb',
           'Browse Image (thumbnail)',
           False): ['previews/COCIRS_0xxx/COCIRS_0406/DATA/CUBE/POINT_PERSPECTIVE/000IA_PRESOI001____RI____699_F4_038P_thumb.jpg'],
          ('metadata',
-          8,
+          4,
           'cube_index',
           'Cube Index',
           False): ['metadata/COCIRS_0xxx/COCIRS_0406/COCIRS_0406_cube_point_index.tab',
                    'metadata/COCIRS_0xxx/COCIRS_0406/COCIRS_0406_cube_point_index.lbl'],
          ('metadata',
-          9,
+          8,
           'supplemental_index',
           'Supplemental Index',
           False): ['metadata/COCIRS_0xxx/COCIRS_0406/COCIRS_0406_cube_point_supplemental_index.tab',
                    'metadata/COCIRS_0xxx/COCIRS_0406/COCIRS_0406_cube_point_supplemental_index.lbl'],
          ('Cassini CIRS',
           700,
           'cocirs_documentation',
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/COISS_xxxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COISS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/CORSS_8xxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/CORSS_8xxx.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,21 +265,15 @@
 
 associations_to_metadata = translator.TranslatorByRegex([
     (r'volumes/CORSS_8xxx(|_v[0-9\.]+)/(CORSS_8...)/(data|EASYDATA)', 0,
             r'metadata/CORSS_8xxx/\2'),
     (r'volumes/CORSS_8xxx(|_v[0-9\.]+)/(CORSS_8...)/(data|EASYDATA).*/(\w+)\..*', 0,
             r'metadata/CORSS_8xxx/\2/\2_index.tab/\4'),
     (r'volumes/CORSS_8xxx(|_v[0-9\.]+)/(CORSS_8...)/(data|EASYDATA).*/(\w+)_TAU.*', 0,
-            [r'metadata/CORSS_8xxx/\2/\2_profile_index.tab/\4_TAU_01KM',
-             r'metadata/CORSS_8xxx/\2/\2_profile_index.tab/\4_TAU_1400M',
-             r'metadata/CORSS_8xxx/\2/\2_profile_index.tab/\4_TAU_1600M',
-             r'metadata/CORSS_8xxx/\2/\2_profile_index.tab/\4_TAU_2400M',
-             r'metadata/CORSS_8xxx/\2/\2_profile_index.tab/\4_TAU_3000M',
-             r'metadata/CORSS_8xxx/\2/\2_profile_index.tab/\4_TAU_4000M',
-             r'metadata/CORSS_8xxx/\2/\2_supplemental_index.tab/\4_TAU_01KM',
+            [r'metadata/CORSS_8xxx/\2/\2_supplemental_index.tab/\4_TAU_01KM',
              r'metadata/CORSS_8xxx/\2/\2_supplemental_index.tab/\4_TAU_1400M',
              r'metadata/CORSS_8xxx/\2/\2_supplemental_index.tab/\4_TAU_1600M',
              r'metadata/CORSS_8xxx/\2/\2_supplemental_index.tab/\4_TAU_2400M',
              r'metadata/CORSS_8xxx/\2/\2_supplemental_index.tab/\4_TAU_3000M',
              r'metadata/CORSS_8xxx/\2/\2_supplemental_index.tab/\4_TAU_4000M',
             ]),
 ])
@@ -412,16 +406,14 @@
              r'previews/CORSS_8xxx/\2/data/\3\4/\3\4_TimeLine_Table_thumb.jpg',
              r'previews/CORSS_8xxx/\2/browse/\3\4_OccTrack_Geometry_full.jpg',
              r'previews/CORSS_8xxx/\2/browse/\3\4_OccTrack_Geometry_med.jpg',
              r'previews/CORSS_8xxx/\2/browse/\3\4_OccTrack_Geometry_small.jpg',
              r'previews/CORSS_8xxx/\2/browse/\3\4_OccTrack_Geometry_thumb.jpg',
              r'metadata/CORSS_8xxx/\2/CORSS_8001_index.lbl',
              r'metadata/CORSS_8xxx/\2/CORSS_8001_index.tab',
-             r'metadata/CORSS_8xxx/\2/CORSS_8001_profile_index.lbl',
-             r'metadata/CORSS_8xxx/\2/CORSS_8001_profile_index.tab',
              r'metadata/CORSS_8xxx/\2/CORSS_8001_supplemental_index.lbl',
              r'metadata/CORSS_8xxx/\2/CORSS_8001_supplemental_index.tab',
             ]),
 ])
 
 ##########################################################################################
 # OPUS_ID
@@ -581,34 +573,34 @@
         (( 1, 0, 4, 0, 0), 'diagrams/CORSS_8xxx/CORSS_8001/data/Rev007/Rev007E_RSS_2005_123_K34_E_full.jpg'),
         (( 1, 0, 4, 0, 0), 'diagrams/CORSS_8xxx/CORSS_8001/data/Rev054/Rev054CE_RSS_2007_353_K55_E_full.jpg'),
         (( 1, 5, 0, 0, 1), 'volumes/CORSS_8xxx/CORSS_8001/browse/Rev007_OccTrack_Geometry.pdf'),
         (( 1, 5, 0, 0, 1), 'volumes/CORSS_8xxx/CORSS_8001/browse/Rev007_OccTrack_Geometry.LBL'),
         (( 2, 5, 1, 0, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev007'),
         (( 8, 5, 0, 0, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev007/Rev007E'),
         (( 8, 1, 4, 0, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev007/Rev007E/Rev007E_RSS_2005_123_K34_E'),
-        ((20, 1, 4, 3, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev007/Rev007E/Rev007E_RSS_2005_123_K34_E/RSS_2005_123_K34_E_TAU_01KM.TAB'),
-        ((20, 1, 4, 3, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev007/Rev007E/Rev007E_RSS_2005_123_K34_E/RSS_2005_123_K34_E_TAU_01KM.LBL'),
-        ((20, 1, 4, 3, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev007/Rev007E/Rev007E_RSS_2005_123_K34_E/RSS_2005_123_K34_E_TAU_10KM.TAB'),
+        ((20, 1, 4, 2, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev007/Rev007E/Rev007E_RSS_2005_123_K34_E/RSS_2005_123_K34_E_TAU_01KM.TAB'),
+        ((20, 1, 4, 2, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev007/Rev007E/Rev007E_RSS_2005_123_K34_E/RSS_2005_123_K34_E_TAU_01KM.LBL'),
+        ((20, 1, 4, 2, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev007/Rev007E/Rev007E_RSS_2005_123_K34_E/RSS_2005_123_K34_E_TAU_10KM.TAB'),
         ((20, 1, 4, 1, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev007/Rev007E/Rev007E_RSS_2005_123_K34_E/RSS_2005_123_K34_E_CAL.TAB'),
         ((20, 1, 4, 1, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev007/Rev007E/Rev007E_RSS_2005_123_K34_E/RSS_2005_123_K34_E_DLP_500M.TAB'),
         ((20, 1, 4, 1, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev007/Rev007E/Rev007E_RSS_2005_123_K34_E/RSS_2005_123_K34_E_GEO.TAB'),
         (( 8, 5, 0, 0, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev054/Rev054CE'),
         (( 8, 1, 4, 0, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev054/Rev054CE/Rev054CE_RSS_2007_353_K55_E'),
-        ((20, 1, 4, 3, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev054/Rev054CE/Rev054CE_RSS_2007_353_K55_E/RSS_2007_353_K55_E_TAU_01KM.TAB'),
-        ((20, 1, 4, 3, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev054/Rev054CE/Rev054CE_RSS_2007_353_K55_E/RSS_2007_353_K55_E_TAU_01KM.LBL'),
-        ((20, 1, 4, 3, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev054/Rev054CE/Rev054CE_RSS_2007_353_K55_E/RSS_2007_353_K55_E_TAU_10KM.TAB'),
+        ((20, 1, 4, 2, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev054/Rev054CE/Rev054CE_RSS_2007_353_K55_E/RSS_2007_353_K55_E_TAU_01KM.TAB'),
+        ((20, 1, 4, 2, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev054/Rev054CE/Rev054CE_RSS_2007_353_K55_E/RSS_2007_353_K55_E_TAU_01KM.LBL'),
+        ((20, 1, 4, 2, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev054/Rev054CE/Rev054CE_RSS_2007_353_K55_E/RSS_2007_353_K55_E_TAU_10KM.TAB'),
         ((20, 1, 4, 1, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev054/Rev054CE/Rev054CE_RSS_2007_353_K55_E/RSS_2007_353_K55_E_CAL.TAB'),
         ((20, 1, 4, 1, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev054/Rev054CE/Rev054CE_RSS_2007_353_K55_E/RSS_2007_353_K55_E_DLP_500M.TAB'),
         ((20, 1, 4, 1, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev054/Rev054CE/Rev054CE_RSS_2007_353_K55_E/RSS_2007_353_K55_E_GEO.TAB'),
         ((20, 1, 4, 1, 1), 'volumes/CORSS_8xxx/CORSS_8001/data/Rev054/Rev054CE/Rev054CE_RSS_2007_353_K55_E/Rev054CE_RSS_2007_353_K55_E_Summary.pdf'),
         (( 2, 2, 1, 1, 1), 'volumes/CORSS_8xxx_v1/CORSS_8001/EASYDATA'),
         (( 1, 1, 4, 0, 1), 'volumes/CORSS_8xxx_v1/CORSS_8001/EASYDATA/Rev07E_RSS_2005_123_K34_E'),
-        (( 1, 1, 4, 3, 1), 'volumes/CORSS_8xxx_v1/CORSS_8001/EASYDATA/Rev07E_RSS_2005_123_X43_E/RSS_2005_123_X43_E_TAU_01KM.TAB'),
-        (( 1, 1, 4, 3, 1), 'volumes/CORSS_8xxx_v1/CORSS_8001/EASYDATA/Rev07E_RSS_2005_123_X43_E/RSS_2005_123_X43_E_TAU_01KM.LBL'),
-        (( 1, 1, 4, 3, 1), 'volumes/CORSS_8xxx_v1/CORSS_8001/EASYDATA/Rev07E_RSS_2005_123_X43_E/RSS_2005_123_X43_E_TAU_10KM.TAB'),
+        (( 1, 1, 4, 2, 1), 'volumes/CORSS_8xxx_v1/CORSS_8001/EASYDATA/Rev07E_RSS_2005_123_X43_E/RSS_2005_123_X43_E_TAU_01KM.TAB'),
+        (( 1, 1, 4, 2, 1), 'volumes/CORSS_8xxx_v1/CORSS_8001/EASYDATA/Rev07E_RSS_2005_123_X43_E/RSS_2005_123_X43_E_TAU_01KM.LBL'),
+        (( 1, 1, 4, 2, 1), 'volumes/CORSS_8xxx_v1/CORSS_8001/EASYDATA/Rev07E_RSS_2005_123_X43_E/RSS_2005_123_X43_E_TAU_10KM.TAB'),
         (( 1, 1, 4, 1, 1), 'volumes/CORSS_8xxx_v1/CORSS_8001/EASYDATA/Rev07E_RSS_2005_123_X43_E/RSS_2005_123_X43_E_CAL.TAB'),
         (( 1, 1, 4, 1, 1), 'volumes/CORSS_8xxx_v1/CORSS_8001/EASYDATA/Rev07E_RSS_2005_123_X43_E/RSS_2005_123_X43_E_GEO.TAB'),
         (( 1, 1, 4, 0, 1), 'volumes/CORSS_8xxx_v1/CORSS_8001/EASYDATA/Rev07E_RSS_2005_123_X43_E/Rev07E_RSS_2005_123_X43_E_Summary.pdf'),
     ]
 
     for (counts, path) in TESTS:
         unmatched = unmatched_patterns(associations_to_volumes, path)
@@ -739,20 +731,14 @@
               5,
               'rms_index',
               'RMS Node Augmented Index',
               False): ['metadata/CORSS_8xxx/CORSS_8001/CORSS_8001_index.tab',
                        'metadata/CORSS_8xxx/CORSS_8001/CORSS_8001_index.lbl'],
              ('metadata',
               8,
-              'profile_index',
-              'Profile Index',
-              False): ['metadata/CORSS_8xxx/CORSS_8001/CORSS_8001_profile_index.tab',
-                       'metadata/CORSS_8xxx/CORSS_8001/CORSS_8001_profile_index.lbl'],
-             ('metadata',
-              9,
               'supplemental_index',
               'Supplemental Index',
               False): ['metadata/CORSS_8xxx/CORSS_8001/CORSS_8001_supplemental_index.tab',
                        'metadata/CORSS_8xxx/CORSS_8001/CORSS_8001_supplemental_index.lbl'],
              ('Cassini RSS',
               70,
               'corss_occ_documentation',
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/COSP_xxxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COSP_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/COUVIS_0xxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COUVIS_0xxx.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
           ('metadata',
            5,
            'rms_index',
            'RMS Node Augmented Index',
            False): ['metadata/COUVIS_0xxx/COUVIS_0001/COUVIS_0001_index.tab',
                     'metadata/COUVIS_0xxx/COUVIS_0001/COUVIS_0001_index.lbl'],
           ('metadata',
-           9,
+           8,
            'supplemental_index',
            'Supplemental Index',
            False): ['metadata/COUVIS_0xxx/COUVIS_0001/COUVIS_0001_supplemental_index.tab',
                     'metadata/COUVIS_0xxx/COUVIS_0001/COUVIS_0001_supplemental_index.lbl'],
           ('Cassini UVIS',
            30,
            'couvis_documentation',
@@ -440,14 +440,15 @@
 )
 def test_associated_abspaths(input_path, category, expected):
     target_pdsfile = instantiate_target_pdsfile(input_path)
     res = target_pdsfile.associated_abspaths(
         category=category)
     result_paths = []
     result_paths += pds3file.Pds3File.logicals_for_abspaths(res)
+    assert len(result_paths) != 0
     for path in result_paths:
         assert path in expected
 
 def test_opus_id_to_primary_logical_path():
     TESTS = [
         'volumes/COUVIS_0xxx/COUVIS_0001/DATA/D1999_007/FUV1999_007_16_57.DAT',
         'volumes/COUVIS_0xxx/COUVIS_0001/DATA/D1999_007/HDAC1999_007_16_33.DAT',
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/COUVIS_8xxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COUVIS_8xxx.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,14 @@
              r'diagrams/COUVIS_8xxx/\2/data/\3_thumb.jpg',
             ]),
 ])
 
 associations_to_metadata = translator.TranslatorByRegex([
     (r'volumes/COUVIS_8xxx(|_v[0-9\.]+)/(COUVIS_8...)/(data|DATA/EASYDATA)/(UVIS_HSP.*)_(TAU\w+KM)\..*', 0,
             [r'metadata/COUVIS_8xxx/\2/\2_index.tab/\4_\5',
-             r'metadata/COUVIS_8xxx/\2/\2_profile_index.tab/\4_TAU01',
              r'metadata/COUVIS_8xxx/\2/\2_supplemental_index.tab/\4_TAU01',
             ]),
 ])
 
 associations_to_documents = translator.TranslatorByRegex([
     (r'volumes/COUVIS_8xxx(|_[^/]+)/COUVIS_8\d\d\d',    0, r'documents/COUVIS_8xxx/*'),
     (r'volumes/COUVIS_8xxx(|_[^/]+)/COUVIS_8\d\d\d/.+', 0, r'documents/COUVIS_8xxx'),
@@ -176,16 +175,14 @@
              r'previews/COUVIS_8xxx/\2/data/\4_thumb.jpg',
              r'diagrams/COUVIS_8xxx/\2/data/\4_full.jpg',
              r'diagrams/COUVIS_8xxx/\2/data/\4_med.jpg',
              r'diagrams/COUVIS_8xxx/\2/data/\4_small.jpg',
              r'diagrams/COUVIS_8xxx/\2/data/\4_thumb.jpg',
              r'metadata/COUVIS_8xxx/\2/\2_index.lbl',
              r'metadata/COUVIS_8xxx/\2/\2_index.tab',
-             r'metadata/COUVIS_8xxx/\2/\2_profile_index.lbl',
-             r'metadata/COUVIS_8xxx/\2/\2_profile_index.tab',
              r'metadata/COUVIS_8xxx/\2/\2_supplemental_index.lbl',
              r'metadata/COUVIS_8xxx/\2/\2_supplemental_index.tab',
             ]),
 ])
 
 ##########################################################################################
 # OPUS_ID
@@ -324,20 +321,14 @@
             5,
             'rms_index',
             'RMS Node Augmented Index',
             False): ['metadata/COUVIS_8xxx/COUVIS_8001/COUVIS_8001_index.tab',
              'metadata/COUVIS_8xxx/COUVIS_8001/COUVIS_8001_index.lbl'],
            ('metadata',
             8,
-            'profile_index',
-            'Profile Index',
-            False): ['metadata/COUVIS_8xxx/COUVIS_8001/COUVIS_8001_profile_index.tab',
-             'metadata/COUVIS_8xxx/COUVIS_8001/COUVIS_8001_profile_index.lbl'],
-           ('metadata',
-            9,
             'supplemental_index',
             'Supplemental Index',
             False): ['metadata/COUVIS_8xxx/COUVIS_8001/COUVIS_8001_supplemental_index.tab',
                      'metadata/COUVIS_8xxx/COUVIS_8001/COUVIS_8001_supplemental_index.lbl'],
            ('Cassini UVIS',
             30,
             'couvis_occ_documentation',
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/COVIMS_0xxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COVIMS_0xxx.py`

 * *Files 0% similar despite different names*

```diff
@@ -466,15 +466,15 @@
          ('metadata',
           5,
           'rms_index',
           'RMS Node Augmented Index',
           False): ['metadata/COVIMS_0xxx/COVIMS_0006/COVIMS_0006_index.tab',
            'metadata/COVIMS_0xxx/COVIMS_0006/COVIMS_0006_index.lbl'],
          ('metadata',
-          9,
+          8,
           'supplemental_index',
           'Supplemental Index',
           False): ['metadata/COVIMS_0xxx/COVIMS_0006/COVIMS_0006_supplemental_index.tab',
            'metadata/COVIMS_0xxx/COVIMS_0006/COVIMS_0006_supplemental_index.lbl'],
          ('Cassini VIMS',
           140,
           'covims_documentation',
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/COVIMS_8xxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COVIMS_8xxx.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,14 @@
              r'diagrams/COVIMS_8xxx/\2/data/\3_thumb.jpg',
             ]),
 ])
 
 associations_to_metadata = translator.TranslatorByRegex([
     (r'volumes/COVIMS_8xxx(|_v[0-9\.]+)/(COVIMS_8...)/data/(VIMS_.*)_(TAU_\d+KM)\..*', 0,
             [r'metadata/COVIMS_8xxx/\2/\2_index.tab/\3_\4',
-             r'metadata/COVIMS_8xxx/\2/\2_profile_index.tab/\3_TAU01',
              r'metadata/COVIMS_8xxx/\2/\2_supplemental_index.tab/\3_TAU01',
             ]),
 ])
 
 associations_to_documents = translator.TranslatorByRegex([
     (r'volumes/COVIMS_8xxx/COVIMS_8\d\d\d', 0,
             r'documents/COVIMS_8xxx/*'),
@@ -220,16 +219,14 @@
              r'previews/COVIMS_8xxx/\2/browse/\4_TAU_STAR_thumb.jpg',
              r'diagrams/COVIMS_8xxx/\2/data/\4_full.jpg',
              r'diagrams/COVIMS_8xxx/\2/data/\4_med.jpg',
              r'diagrams/COVIMS_8xxx/\2/data/\4_small.jpg',
              r'diagrams/COVIMS_8xxx/\2/data/\4_thumb.jpg',
              r'metadata/COVIMS_8xxx/\2/\2_index.lbl',
              r'metadata/COVIMS_8xxx/\2/\2_index.tab',
-             r'metadata/COVIMS_8xxx/\2/\2_profile_index.lbl',
-             r'metadata/COVIMS_8xxx/\2/\2_profile_index.tab',
              r'metadata/COVIMS_8xxx/\2/\2_supplemental_index.lbl',
              r'metadata/COVIMS_8xxx/\2/\2_supplemental_index.tab',
             ]),
 ])
 
 ##########################################################################################
 # OPUS_ID
@@ -377,20 +374,14 @@
           5,
           'rms_index',
           'RMS Node Augmented Index',
           False): ['metadata/COVIMS_8xxx/COVIMS_8001/COVIMS_8001_index.tab',
                    'metadata/COVIMS_8xxx/COVIMS_8001/COVIMS_8001_index.lbl'],
          ('metadata',
           8,
-          'profile_index',
-          'Profile Index',
-          False): ['metadata/COVIMS_8xxx/COVIMS_8001/COVIMS_8001_profile_index.tab',
-                   'metadata/COVIMS_8xxx/COVIMS_8001/COVIMS_8001_profile_index.lbl'],
-         ('metadata',
-          9,
           'supplemental_index',
           'Supplemental Index',
           False): ['metadata/COVIMS_8xxx/COVIMS_8001/COVIMS_8001_supplemental_index.tab',
                    'metadata/COVIMS_8xxx/COVIMS_8001/COVIMS_8001_supplemental_index.lbl'],
          ('Cassini VIMS',
           30,
           'covims_occ_documentation',
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/EBROCC_xxxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/EBROCC_xxxx.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,17 +73,15 @@
            ]),
 ])
 
 associations_to_metadata = translator.TranslatorByRegex([
     (r'volumes/EBROCC_xxxx(|_v[0-9\.]+)/(EBROCC_....)/(DATA|BROWSE|SORCDATA|GEOMETRY)/\w+/(\w+)\.\w+', 0,
            r'metadata/EBROCC_xxxx/\2/\2_index.tab/\4'),
     (r'volumes/EBROCC_xxxx(|_v[0-9\.]+)/(EBROCC_....)/DATA/\w+/(\w+)\.\w+', 0,
-           [r'metadata/EBROCC_xxxx/\2/\2_profile_index.tab/\4',
-            r'metadata/EBROCC_xxxx/\2/\2_supplemental_index.tab/\4',
-           ]),
+           r'metadata/EBROCC_xxxx/\2/\2_supplemental_index.tab/\4'),
 ])
 
 ##########################################################################################
 # VIEW_OPTIONS (grid_view_allowed, multipage_view_allowed, continuous_view_allowed)
 ##########################################################################################
 
 view_options = translator.TranslatorByRegex([
@@ -91,20 +89,20 @@
 ])
 
 ##########################################################################################
 # OPUS_TYPE
 ##########################################################################################
 
 opus_type = translator.TranslatorByRegex([
-    (r'volumes/.*/DATA/\w+/\w+\.(TAB|LBL)',          0, ('Earth-based Occultations',  0, 'ebro_profile', 'Occultation Profile', True)),
-    (r'volumes/.*/GEOMETRY/\w+/\w+\.(TAB|LBL)',      0, ('Earth-based Occultations', 10, 'ebro_geom',    'Geometry Table',      True)),
-    (r'volumes/.*/BROWSE/\w+/\w+PB\.(PDF|PS|LBL)',   0, ('Earth-based Occultations', 20, 'ebro_preview', 'Preview Plot',        True)),
-    (r'volumes/.*/BROWSE/\w+/\w+GB\.(PDF|PS|LBL)',   0, ('Earth-based Occultations', 30, 'ebro_diagram', 'Geometry Diagram',    False)),
-    (r'volumes/.*/SORCDATA/\w+/\w+_GEOMETRY\..*',    0, ('Earth-based Occultations', 40, 'ebro_source',  'Source Data',         False)),
-    (r'volumes/.*/SORCDATA/\w+/\w+GRESS\.(OUT|LBL)', 0, ('Earth-based Occultations', 40, 'ebro_source',  'Source Data',         False)),
+    (r'volumes/.*/DATA/\w+/\w+\.(TAB|LBL)',          0, ('Earth-based Occultations',  0, 'ebro_occ_profile', 'Occultation Profile', True)),
+    (r'volumes/.*/GEOMETRY/\w+/\w+\.(TAB|LBL)',      0, ('Earth-based Occultations', 10, 'ebro_occ_geom',    'Geometry Table',      True)),
+    (r'volumes/.*/BROWSE/\w+/\w+PB\.(PDF|PS|LBL)',   0, ('Earth-based Occultations', 20, 'ebro_occ_preview', 'Preview Plot',        True)),
+    (r'volumes/.*/BROWSE/\w+/\w+GB\.(PDF|PS|LBL)',   0, ('Earth-based Occultations', 30, 'ebro_occ_diagram', 'Geometry Diagram',    False)),
+    (r'volumes/.*/SORCDATA/\w+/\w+_GEOMETRY\..*',    0, ('Earth-based Occultations', 40, 'ebro_occ_source',  'Source Data',         False)),
+    (r'volumes/.*/SORCDATA/\w+/\w+GRESS\.(OUT|LBL)', 0, ('Earth-based Occultations', 40, 'ebro_occ_source',  'Source Data',         False)),
 ])
 
 ##########################################################################################
 # OPUS_FORMAT
 ##########################################################################################
 
 opus_format = translator.TranslatorByRegex([
@@ -139,45 +137,43 @@
             r'previews/EBROCC_xxxx/\2/BROWSE/\4GB_thumb.jpg',
             r'previews/EBROCC_xxxx/\2/BROWSE/\4PB_full.jpg',
             r'previews/EBROCC_xxxx/\2/BROWSE/\4PB_med.jpg',
             r'previews/EBROCC_xxxx/\2/BROWSE/\4PB_small.jpg',
             r'previews/EBROCC_xxxx/\2/BROWSE/\4PB_thumb.jpg',
             r'metadata/EBROCC_xxxx/\2/\2_index.lbl',
             r'metadata/EBROCC_xxxx/\2/\2_index.tab',
-            r'metadata/EBROCC_xxxx/\2/\2_profile_index.lbl',
-            r'metadata/EBROCC_xxxx/\2/\2_profile_index.tab',
             r'metadata/EBROCC_xxxx/\2/\2_supplemental_index.lbl',
             r'metadata/EBROCC_xxxx/\2/\2_supplemental_index.tab',
            ]),
 ])
 
 ##########################################################################################
 # OPUS_ID
 ##########################################################################################
 
 opus_id = translator.TranslatorByRegex([
-    (r'.*/EBROCC_xxxx.*/\w+/ESO1M/ES1_(I|E).*',  0, r'eso1m-apph-occ-1989-184-28sgr-#LOWER#\1'),
-    (r'.*/EBROCC_xxxx.*/\w+/ESO22M/ES2_(I|E).*', 0, r'eso22m-apph-occ-1989-184-28sgr-#LOWER#\1'),
-    (r'.*/EBROCC_xxxx.*/\w+/IRTF/IRT_(I|E).*',   0, r'irtf-urac-occ-1989-184-28sgr-#LOWER#\1'),
+    (r'.*/EBROCC_xxxx.*/\w+/ESO1M/ES1_(I|E).*',  0, r'esosil1m04-apph-occ-1989-184-28sgr-#LOWER#\1'),
+    (r'.*/EBROCC_xxxx.*/\w+/ESO22M/ES2_(I|E).*', 0, r'esosil2m2-apph-occ-1989-184-28sgr-#LOWER#\1'),
+    (r'.*/EBROCC_xxxx.*/\w+/IRTF/IRT_(I|E).*',   0, r'irtf3m2-urac-occ-1989-184-28sgr-#LOWER#\1'),
     (r'.*/EBROCC_xxxx.*/\w+/LICK1M/LIC_(I|E).*', 0, r'lick1m-ccdc-occ-1989-184-28sgr-#LOWER#\1'),
-    (r'.*/EBROCC_xxxx.*/\w+/MCD27M/MCD_(I|E).*', 0, r'mcd27m-iirar-occ-1989-184-28sgr-#LOWER#\1'),
-    (r'.*/EBROCC_xxxx.*/\w+/PAL200/PAL_(I|E).*', 0, r'pal200-circ-occ-1989-184-28sgr-#LOWER#\1')
+    (r'.*/EBROCC_xxxx.*/\w+/MCD27M/MCD_(I|E).*', 0, r'mcd2m7-iirar-occ-1989-184-28sgr-#LOWER#\1'),
+    (r'.*/EBROCC_xxxx.*/\w+/PAL200/PAL_(I|E).*', 0, r'pal5m08-circ-occ-1989-184-28sgr-#LOWER#\1')
 ])
 
 ##########################################################################################
 # OPUS_ID_TO_PRIMARY_LOGICAL_PATH
 ##########################################################################################
 
 opus_id_to_primary_logical_path = translator.TranslatorByRegex([
-    (r'eso1m-apph-occ-1989-184-28sgr-(.*)',   0, r'volumes/EBROCC_xxxx/EBROCC_0001/DATA/ESO1M/ES1_#UPPER#\1PD.TAB'),
-    (r'eso22m-apph-occ-1989-184-28sgr-(.*)',  0, r'volumes/EBROCC_xxxx/EBROCC_0001/DATA/ESO22M/ES2_#UPPER#\1PD.TAB'),
-    (r'irtf-urac-occ-1989-184-28sgr-(.*)',    0, r'volumes/EBROCC_xxxx/EBROCC_0001/DATA/IRTF/IRT_#UPPER#\1PD.TAB'),
+    (r'esosil1m04-apph-occ-1989-184-28sgr-(.*)',   0, r'volumes/EBROCC_xxxx/EBROCC_0001/DATA/ESO1M/ES1_#UPPER#\1PD.TAB'),
+    (r'esosil2m2-apph-occ-1989-184-28sgr-(.*)',  0, r'volumes/EBROCC_xxxx/EBROCC_0001/DATA/ESO22M/ES2_#UPPER#\1PD.TAB'),
+    (r'irtf3m2-urac-occ-1989-184-28sgr-(.*)',    0, r'volumes/EBROCC_xxxx/EBROCC_0001/DATA/IRTF/IRT_#UPPER#\1PD.TAB'),
     (r'lick1m-ccdc-occ-1989-184-28sgr-(.*)',  0, r'volumes/EBROCC_xxxx/EBROCC_0001/DATA/LICK1M/LIC_#UPPER#\1PD.TAB'),
-    (r'mcd27m-iirar-occ-1989-184-28sgr-(.*)', 0, r'volumes/EBROCC_xxxx/EBROCC_0001/DATA/MCD27M/MCD_#UPPER#\1PD.TAB'),
-    (r'pal200-circ-occ-1989-184-28sgr-(.*)',  0, r'volumes/EBROCC_xxxx/EBROCC_0001/DATA/PAL200/PAL_#UPPER#\1PD.TAB'),
+    (r'mcd2m7-iirar-occ-1989-184-28sgr-(.*)', 0, r'volumes/EBROCC_xxxx/EBROCC_0001/DATA/MCD27M/MCD_#UPPER#\1PD.TAB'),
+    (r'pal5m08-circ-occ-1989-184-28sgr-(.*)',  0, r'volumes/EBROCC_xxxx/EBROCC_0001/DATA/PAL200/PAL_#UPPER#\1PD.TAB'),
 ])
 
 ##########################################################################################
 # DATA_SET_ID
 ##########################################################################################
 
 data_set_id = translator.TranslatorByRegex([
@@ -248,16 +244,15 @@
     TESTS = [
         (2, 'volumes.*/DATA/.*'),
         (6, 'volumes.*/BROWSE/.*'),
         (2, 'volumes.*/GEOMETRY/.*'),
         (4, 'volumes.*/SORCDATA/.*'),
         (4, 'previews.*/DATA/.*'),
         (8, 'previews/.*/BROWSE/.*'),
-        (6, 'metadata.*index.*'),
-        (2, 'metadata.*profile.*'),
+        (4, 'metadata.*index.*'),
         (2, 'metadata.*supplemental.*'),
     ]
 
     PATH = 'volumes/EBROCC_xxxx/EBROCC_0001/DATA/ESO1M/ES1_EPD.LBL'
     abspaths = translate_all(opus_products, PATH)
     trimmed = [p.rpartition('holdings/')[-1] for p in abspaths]
     for (count, pattern) in TESTS:
@@ -269,43 +264,43 @@
 # and '/volumes/EBROCC_xxxx/EBROCC_0001/BROWSE/ESO1M/ES1_EPB.LBL' here. OPUS
 # will ignore the duplicated items
     'input_path,expected',
     [
         ('volumes/EBROCC_xxxx/EBROCC_0001/DATA/ESO1M/ES1_EPD.TAB',
         {('Earth-based Occultations',
           0,
-          'ebro_profile',
+          'ebro_occ_profile',
           'Occultation Profile',
           True): ['volumes/EBROCC_xxxx/EBROCC_0001/DATA/ESO1M/ES1_EPD.TAB',
                   'volumes/EBROCC_xxxx/EBROCC_0001/DATA/ESO1M/ES1_EPD.LBL'],
          ('Earth-based Occultations',
           30,
-          'ebro_diagram',
+          'ebro_occ_diagram',
           'Geometry Diagram',
           False): ['volumes/EBROCC_xxxx/EBROCC_0001/BROWSE/ESO1M/ES1_EGB.PS',
                    'volumes/EBROCC_xxxx/EBROCC_0001/BROWSE/ESO1M/ES1_EGB.PDF',
                    'volumes/EBROCC_xxxx/EBROCC_0001/BROWSE/ESO1M/ES1_EGB.LBL',
                    'volumes/EBROCC_xxxx/EBROCC_0001/BROWSE/ESO1M/ES1_EGB.LBL'],
          ('Earth-based Occultations',
           20,
-          'ebro_preview',
+          'ebro_occ_preview',
           'Preview Plot',
           True): ['volumes/EBROCC_xxxx/EBROCC_0001/BROWSE/ESO1M/ES1_EPB.PS',
                   'volumes/EBROCC_xxxx/EBROCC_0001/BROWSE/ESO1M/ES1_EPB.PDF',
                   'volumes/EBROCC_xxxx/EBROCC_0001/BROWSE/ESO1M/ES1_EPB.LBL',
                   'volumes/EBROCC_xxxx/EBROCC_0001/BROWSE/ESO1M/ES1_EPB.LBL'],
          ('Earth-based Occultations',
           10,
-          'ebro_geom',
+          'ebro_occ_geom',
           'Geometry Table',
           True): ['volumes/EBROCC_xxxx/EBROCC_0001/GEOMETRY/ESO1M/ES1_EGD.TAB',
                   'volumes/EBROCC_xxxx/EBROCC_0001/GEOMETRY/ESO1M/ES1_EGD.LBL'],
          ('Earth-based Occultations',
           40,
-          'ebro_source',
+          'ebro_occ_source',
           'Source Data',
           False): ['volumes/EBROCC_xxxx/EBROCC_0001/SORCDATA/ESO1M/ES1_EGRESS_GEOMETRY.DAT',
                    'volumes/EBROCC_xxxx/EBROCC_0001/SORCDATA/ESO1M/ES1_EGRESS_GEOMETRY.LBL',
                    'volumes/EBROCC_xxxx/EBROCC_0001/SORCDATA/ESO1M/ES1_EGRESS.OUT',
                    'volumes/EBROCC_xxxx/EBROCC_0001/SORCDATA/ESO1M/ES1_EGRESS.LBL'],
          ('browse',
           40,
@@ -339,20 +334,14 @@
           5,
           'rms_index',
           'RMS Node Augmented Index',
           False): ['metadata/EBROCC_xxxx/EBROCC_0001/EBROCC_0001_index.tab',
                    'metadata/EBROCC_xxxx/EBROCC_0001/EBROCC_0001_index.lbl'],
          ('metadata',
           8,
-          'profile_index',
-          'Profile Index',
-          False): ['metadata/EBROCC_xxxx/EBROCC_0001/EBROCC_0001_profile_index.tab',
-                   'metadata/EBROCC_xxxx/EBROCC_0001/EBROCC_0001_profile_index.lbl'],
-         ('metadata',
-          9,
           'supplemental_index',
           'Supplemental Index',
           False): ['metadata/EBROCC_xxxx/EBROCC_0001/EBROCC_0001_supplemental_index.tab',
                    'metadata/EBROCC_xxxx/EBROCC_0001/EBROCC_0001_supplemental_index.lbl']}
         )
     ]
 )
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/GO_0xxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/GO_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/HSTxx_xxxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/HSTxx_xxxx.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,14 +341,15 @@
 def test_associated_abspaths(input_path, category, selection, flag, expected):
     target_pdsfile = instantiate_target_pdsfile(input_path)
     index_row = target_pdsfile.child_of_index(selection, flag)
     res = index_row.associated_abspaths(
         category=category)
     result_paths = []
     result_paths += pds3file.Pds3File.logicals_for_abspaths(res)
+    assert len(result_paths) != 0
     for path in result_paths:
         assert path in expected
     for path in expected:
         assert path in result_paths
 
 
 def test_opus_id_to_primary_logical_path():
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/JNOJIR_xxxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/JNOJIR_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/JNOJNC_xxxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/JNOJNC_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/JNOSP_xxxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/JNOSP_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/NHSP_xxxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/NHSP_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/NHxxxx_xxxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/NHxxxx_xxxx.py`

 * *Files 0% similar despite different names*

```diff
@@ -673,15 +673,15 @@
           ('metadata',
            5,
            'rms_index',
            'RMS Node Augmented Index',
            False): ['metadata/NHxxLO_xxxx/NHLALO_1001/NHLALO_1001_index.tab',
                     'metadata/NHxxLO_xxxx/NHLALO_1001/NHLALO_1001_index.lbl'],
           ('metadata',
-           9,
+           8,
            'supplemental_index',
            'Supplemental Index',
            False): ['metadata/NHxxLO_xxxx/NHLALO_1001/NHLALO_1001_supplemental_index.tab',
                     'metadata/NHxxLO_xxxx/NHLALO_1001/NHLALO_1001_supplemental_index.lbl'],
           ('New Horizons LORRI',
            50,
            'nh_lorri_raw_alternate',
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/RES_xxxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/RES_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/RPX_xxxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/RPX_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/VGIRIS_xxxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VGIRIS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/VGISS_xxxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VGISS_xxxx.py`

 * *Files 0% similar despite different names*

```diff
@@ -719,15 +719,15 @@
          ('metadata',
           7,
           'raw_image_index',
           'Raw Image Index',
           False): ['metadata/VGISS_5xxx/VGISS_5101/VGISS_5101_raw_image_index.tab',
                    'metadata/VGISS_5xxx/VGISS_5101/VGISS_5101_raw_image_index.lbl'],
          ('metadata',
-          9,
+          8,
           'supplemental_index',
           'Supplemental Index',
           False): ['metadata/VGISS_5xxx/VGISS_5101/VGISS_5101_supplemental_index.tab',
                    'metadata/VGISS_5xxx/VGISS_5101/VGISS_5101_supplemental_index.lbl'],
          ('Voyager ISS',
           100,
           'vgiss_documentation',
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/VG_0xxx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VG_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/VG_20xx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VG_20xx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/VG_28xx.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VG_28xx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1047,15 +1047,15 @@
              ('metadata',
               5,
               'rms_index',
               'RMS Node Augmented Index',
               False): ['metadata/VG_28xx/VG_2801/VG_2801_index.tab',
                        'metadata/VG_28xx/VG_2801/VG_2801_index.lbl'],
              ('metadata',
-              9,
+              8,
               'supplemental_index',
               'Supplemental Index',
               False): ['metadata/VG_28xx/VG_2801/VG_2801_supplemental_index.tab',
                        'metadata/VG_28xx/VG_2801/VG_2801_supplemental_index.lbl']}
         ),
         ('volumes/VG_28xx/VG_2801/EASYDATA/KM000_1/PU1P01DE.TAB',
             {('Voyager PPS',
@@ -1157,15 +1157,15 @@
              ('metadata',
               5,
               'rms_index',
               'RMS Node Augmented Index',
               False): ['metadata/VG_28xx/VG_2801/VG_2801_index.tab',
                        'metadata/VG_28xx/VG_2801/VG_2801_index.lbl'],
              ('metadata',
-              9,
+              8,
               'supplemental_index',
               'Supplemental Index',
               False): ['metadata/VG_28xx/VG_2801/VG_2801_supplemental_index.tab',
                        'metadata/VG_28xx/VG_2801/VG_2801_supplemental_index.lbl']}
         ),
         # VG_2802
         ('volumes/VG_28xx/VG_2802/EASYDATA/FILTER01/US1F01.TAB',
@@ -1270,15 +1270,15 @@
              ('metadata',
               5,
               'rms_index',
               'RMS Node Augmented Index',
               False): ['metadata/VG_28xx/VG_2802/VG_2802_index.tab',
                        'metadata/VG_28xx/VG_2802/VG_2802_index.lbl'],
              ('metadata',
-              9,
+              8,
               'supplemental_index',
               'Supplemental Index',
               False): ['metadata/VG_28xx/VG_2802/VG_2802_supplemental_index.tab',
                        'metadata/VG_28xx/VG_2802/VG_2802_supplemental_index.lbl']}
         ),
         ('volumes/VG_28xx/VG_2802/EASYDATA/FILTER01/UU1F01EE.TAB',
             {('Voyager UVS',
@@ -1382,15 +1382,15 @@
              ('metadata',
               5,
               'rms_index',
               'RMS Node Augmented Index',
               False): ['metadata/VG_28xx/VG_2802/VG_2802_index.tab',
                        'metadata/VG_28xx/VG_2802/VG_2802_index.lbl'],
              ('metadata',
-              9,
+              8,
               'supplemental_index',
               'Supplemental Index',
               False): ['metadata/VG_28xx/VG_2802/VG_2802_supplemental_index.tab',
                        'metadata/VG_28xx/VG_2802/VG_2802_supplemental_index.lbl']}
         ),
         ('volumes/VG_28xx/VG_2802/EASYDATA/FILTER01/UN1F01.TAB',
             {('Voyager UVS',
@@ -1600,15 +1600,15 @@
              ('metadata',
               5,
               'rms_index',
               'RMS Node Augmented Index',
               False): ['metadata/VG_28xx/VG_2802/VG_2802_index.tab',
                        'metadata/VG_28xx/VG_2802/VG_2802_index.lbl'],
              ('metadata',
-              9,
+              8,
               'supplemental_index',
               'Supplemental Index',
               False): ['metadata/VG_28xx/VG_2802/VG_2802_supplemental_index.tab',
                        'metadata/VG_28xx/VG_2802/VG_2802_supplemental_index.lbl']}
         ),
         # VG_2803
         ('volumes/VG_28xx/VG_2803/S_RINGS/EASYDATA/KM000_2/RS1P2X07.LBL',
@@ -1825,15 +1825,15 @@
              ('metadata',
               5,
               'rms_index',
               'RMS Node Augmented Index',
               False): ['metadata/VG_28xx/VG_2803/VG_2803_index.tab',
                        'metadata/VG_28xx/VG_2803/VG_2803_index.lbl'],
              ('metadata',
-              9,
+              8,
               'supplemental_index',
               'Supplemental Index',
               False): ['metadata/VG_28xx/VG_2803/VG_2803_supplemental_index.tab',
                        'metadata/VG_28xx/VG_2803/VG_2803_supplemental_index.lbl']}
         ),
         ('volumes/VG_28xx/VG_2803/U_RINGS/EASYDATA/KM00_2/RU1P2X4I.TAB',
             {('Voyager RSS',
@@ -1891,15 +1891,15 @@
              ('metadata',
               5,
               'rms_index',
               'RMS Node Augmented Index',
               False): ['metadata/VG_28xx/VG_2803/VG_2803_index.tab',
                        'metadata/VG_28xx/VG_2803/VG_2803_index.lbl'],
              ('metadata',
-              9,
+              8,
               'supplemental_index',
               'Supplemental Index',
               False): ['metadata/VG_28xx/VG_2803/VG_2803_supplemental_index.tab',
                        'metadata/VG_28xx/VG_2803/VG_2803_supplemental_index.lbl']}
         ),
         # VG_2810
         ('volumes/VG_28xx/VG_2810/DATA/IS2_P0001_V01_KM002.TAB',
@@ -2142,15 +2142,15 @@
              ('metadata',
               5,
               'rms_index',
               'RMS Node Augmented Index',
               False): ['metadata/VG_28xx/VG_2810/VG_2810_index.tab',
                        'metadata/VG_28xx/VG_2810/VG_2810_index.lbl'],
              ('metadata',
-              9,
+              8,
               'supplemental_index',
               'Supplemental Index',
               False): ['metadata/VG_28xx/VG_2810/VG_2810_supplemental_index.tab',
                        'metadata/VG_28xx/VG_2810/VG_2810_supplemental_index.lbl']}
         ),
     ]
 )
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/__init__.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -516,16 +516,15 @@
     (r'metadata/.*_(moon|charon)_summary\..*', 0, ('metadata', 30, 'moon_geometry',   'Moon Geometry Index',   False)),
     (r'metadata/.*_ring_summary\..*',          0, ('metadata', 40, 'ring_geometry',   'Ring Geometry Index',   False)),
 
     # Metadata index
     (r'metadata/.*_\d+_index\..*',         0, ('metadata', 5, 'rms_index',          'RMS Node Augmented Index',     False)),
     (r'metadata/.*_hstfiles\..*',          0, ('metadata', 6, 'hstfiles_index',     'HST Files Associations Index', False)),
     (r'metadata/.*raw_image_index\..*',    0, ('metadata', 7, 'raw_image_index',    'Raw Image Index',              False)),
-    (r'metadata/.*profile_index\..*',      0, ('metadata', 8, 'profile_index',      'Profile Index',                False)),
-    (r'metadata/.*supplemental_index\..*', 0, ('metadata', 9, 'supplemental_index', 'Supplemental Index',           False)),
+    (r'metadata/.*supplemental_index\..*', 0, ('metadata', 8, 'supplemental_index', 'Supplemental Index',           False)),
 ])
 
 ##########################################################################################
 # OPUS_FORMAT
 #
 # Returns a tuple (interchange format, file format) where the first is 'Binary', 'ASCII' or 'UTF-8' and the latter is the format
 # of the file, e.g., 'Vicar', 'FITS', 'Table', 'PDS3 Label', etc.
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/rules/pytest_support.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/pytest_support.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/tests/helper.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/tests/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 # Helper functions for tests on pds3file
 ##########################################################################################
 
 import os
 import pdsfile.pds3file as pds3file
 
 try:
-    PDS_HOLDINGS_DIR = os.environ['PDS_HOLDINGS_DIR']
+    PDS3_HOLDINGS_DIR = os.environ['PDS3_HOLDINGS_DIR']
 except KeyError: # pragma: no cover
-    raise KeyError("'PDS_HOLDINGS_DIR' environment variable not set")
+    raise KeyError("'PDS3_HOLDINGS_DIR' environment variable not set")
 
 def instantiate_target_pdsfile(path, is_abspath=True):
     if is_abspath:
-        TESTFILE_PATH = PDS_HOLDINGS_DIR + '/' + path
+        TESTFILE_PATH = PDS3_HOLDINGS_DIR + '/' + path
         target_pdsfile = pds3file.Pds3File.from_abspath(TESTFILE_PATH)
     else:
         TESTFILE_PATH = path
         target_pdsfile = pds3file.Pds3File.from_logical_path(TESTFILE_PATH)
     return target_pdsfile
 
 def get_pdsfiles(paths, is_abspath=True):
     pdsfiles_arr = []
     if is_abspath:
         for path in paths:
-            TESTFILE_PATH = PDS_HOLDINGS_DIR + '/' +  path
+            TESTFILE_PATH = PDS3_HOLDINGS_DIR + '/' +  path
             target_pdsfile = pds3file.Pds3File.from_abspath(TESTFILE_PATH)
             pdsfiles_arr.append(target_pdsfile)
     else:
         for path in paths:
             TESTFILE_PATH = path
             target_pdsfile = pds3file.Pds3File.from_logical_path(TESTFILE_PATH)
             pdsfiles_arr.append(target_pdsfile)
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/tests/test_pds3file_blackbox.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pds3file_blackbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from pdsfile.pdsfile import (logical_path_from_abspath,
                              repair_case,
                              selected_path_from_path)
 
 import pytest
 import re
 
-from .helper import (PDS_HOLDINGS_DIR,
+from .helper import (PDS3_HOLDINGS_DIR,
                      instantiate_target_pdsfile)
 
-PDS_PDSDATA_PATH = PDS_HOLDINGS_DIR[:PDS_HOLDINGS_DIR.index('holdings')]
+PDS_PDSDATA_PATH = PDS3_HOLDINGS_DIR[:PDS3_HOLDINGS_DIR.index('holdings')]
 
 ##########################################################################################
 # Blackbox test for functions & properties in Pds3File class
 ##########################################################################################
 class TestPds3FileBlackBox:
     ############################################################################
     # Test on SUBCLASS, make sure rules all exist in the dictionary
@@ -67,15 +67,15 @@
 
     ############################################################################
     # Local implementations of basic filesystem operations
     ############################################################################
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-            (PDS_HOLDINGS_DIR + '/volumes/COISS_2xxx',
+            (PDS3_HOLDINGS_DIR + '/volumes/COISS_2xxx',
              [
                 'COISS_2090', 'COISS_2025', 'COISS_2055', 'COISS_2058',
                 'COISS_2086', 'COISS_2105', 'COISS_2067', 'COISS_2017',
                 'COISS_2049', 'COISS_2011', 'COISS_2026', 'COISS_2039',
                 'COISS_2073', 'COISS_2044', 'COISS_2062', 'COISS_2037',
                 'COISS_2114', 'COISS_2110', 'COISS_2072', 'COISS_2002',
                 'COISS_2108', 'COISS_2093', 'COISS_2030', 'COISS_2081',
@@ -215,23 +215,23 @@
         target_pdsfile = instantiate_target_pdsfile(input_path)
         assert target_pdsfile.islabel == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('diagrams/COCIRS_5xxx/COCIRS_5401/BROWSE/TARGETS/IMG0401130240_FP1_thumb.jpg',
-             PDS_HOLDINGS_DIR + '/diagrams/COCIRS_5xxx/COCIRS_5401/BROWSE/TARGETS/IMG0401130240_FP1_thumb.jpg'),
-            ('volumes', PDS_HOLDINGS_DIR + '/volumes')
+             PDS3_HOLDINGS_DIR + '/diagrams/COCIRS_5xxx/COCIRS_5401/BROWSE/TARGETS/IMG0401130240_FP1_thumb.jpg'),
+            ('volumes', PDS3_HOLDINGS_DIR + '/volumes')
         ]
     )
     def test_absolute_or_logical_path(self, input_path, expected):
         """absolute_or_logical_path: get abspath."""
         target_pdsfile = instantiate_target_pdsfile(input_path)
         if expected is None: # pragma: no cover
-            expected = PDS_HOLDINGS_DIR + '/' + input_path
+            expected = PDS3_HOLDINGS_DIR + '/' + input_path
         assert target_pdsfile.absolute_or_logical_path == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('diagrams/COCIRS_6xxx/COCIRS_6004/BROWSE/SATURN/POI1004010000_FP1_small.jpg',
              '/holdings/diagrams/COCIRS_6xxx/COCIRS_6004/BROWSE/SATURN/POI1004010000_FP1_small.jpg'),
@@ -344,18 +344,18 @@
         target_pdsfile = instantiate_target_pdsfile(input_path)
         assert target_pdsfile.label_basename == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('volumes/GO_0xxx/GO_0017/J0/OPNAV/C0346405900R.IMG',
-             PDS_HOLDINGS_DIR + '/volumes/GO_0xxx/GO_0017/J0/OPNAV/C0346405900R.LBL'),
+             PDS3_HOLDINGS_DIR + '/volumes/GO_0xxx/GO_0017/J0/OPNAV/C0346405900R.LBL'),
             ('volumes/GO_0xxx/GO_0017/J0/OPNAV', ''),
             ('metadata/GO_0xxx/GO_0017/GO_0017_index.tab',
-             PDS_HOLDINGS_DIR + '/metadata/GO_0xxx/GO_0017/GO_0017_index.lbl'),
+             PDS3_HOLDINGS_DIR + '/metadata/GO_0xxx/GO_0017/GO_0017_index.lbl'),
             ('previews/GO_0xxx/GO_0017/J0/OPNAV/C0346405900R_med.jpg', '')
         ]
     )
     def test_label_abspath(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         assert target_pdsfile.label_abspath == expected
 
@@ -521,15 +521,15 @@
         assert target_pdsfile.childnames == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('volumes/COCIRS_6xxx/COCIRS_6004/DATA/GEODATA/GEO1004021018_699.LBL',
              [
-                PDS_HOLDINGS_DIR + '/volumes/COCIRS_6xxx/COCIRS_6004/DATA/GEODATA/GEO1004021018_699.TAB'
+                PDS3_HOLDINGS_DIR + '/volumes/COCIRS_6xxx/COCIRS_6004/DATA/GEODATA/GEO1004021018_699.TAB'
              ])
         ]
     )
     def test_data_abspaths(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.data_abspaths
 
@@ -827,15 +827,15 @@
         res = pds3file.Pds3File.version_info(suffix=input_suffix)
         assert res == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('previews/VGISS_5xxx/VGISS_5101/DATA/C13854XX/C1385455_small.jpg',
-             'Pds3File.VGISS_xxxx("' + PDS_HOLDINGS_DIR + '/previews/VGISS_5xxx/VGISS_5101/DATA/C13854XX/C1385455_small.jpg")'),
+             'Pds3File.VGISS_xxxx("' + PDS3_HOLDINGS_DIR + '/previews/VGISS_5xxx/VGISS_5101/DATA/C13854XX/C1385455_small.jpg")'),
         ]
     )
     def test___repr__1(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.__repr__()
         assert res == expected
 
@@ -848,34 +848,34 @@
     # Test for alternative constructors
     ############################################################################
     @pytest.mark.parametrize(
         'input_path,basename,expected',
         [
             ('volumes/COCIRS_6xxx/COCIRS_6004/DATA/GEODATA/',
              'GEO1004021018_699.LBL',
-             PDS_HOLDINGS_DIR + '/volumes/COCIRS_6xxx/COCIRS_6004/DATA/GEODATA/GEO1004021018_699.LBL'),
+             PDS3_HOLDINGS_DIR + '/volumes/COCIRS_6xxx/COCIRS_6004/DATA/GEODATA/GEO1004021018_699.LBL'),
             ('metadata/COISS_1xxx/COISS_1001',
              'COISS_1001_inventory.tab',
-             PDS_HOLDINGS_DIR + '/metadata/COISS_1xxx/COISS_1001/COISS_1001_inventory.tab'),
+             PDS3_HOLDINGS_DIR + '/metadata/COISS_1xxx/COISS_1001/COISS_1001_inventory.tab'),
         ]
     )
     def test_child(self, input_path, basename, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         print(target_pdsfile.category_)
         res = target_pdsfile.child(basename=basename)
         assert isinstance(res, pds3file.Pds3File)
         assert res.abspath == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('volumes/COCIRS_0xxx_v3/COCIRS_0401/DATA/TSDR/NAV_DATA/TAR04012400.LBL',
-             PDS_HOLDINGS_DIR + '/volumes/COCIRS_0xxx_v3/COCIRS_0401/DATA/TSDR/NAV_DATA'),
+             PDS3_HOLDINGS_DIR + '/volumes/COCIRS_0xxx_v3/COCIRS_0401/DATA/TSDR/NAV_DATA'),
             ('volumes/COCIRS_1xxx/COCIRS_1001/DATA/TSDR/NAV_DATA/TAR10013100.DAT',
-             PDS_HOLDINGS_DIR + '/volumes/COCIRS_1xxx/COCIRS_1001/DATA/TSDR/NAV_DATA'),
+             PDS3_HOLDINGS_DIR + '/volumes/COCIRS_1xxx/COCIRS_1001/DATA/TSDR/NAV_DATA'),
         ]
     )
     def test_parent(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.parent()
         assert isinstance(res, pds3file.Pds3File)
         assert res.abspath == expected
@@ -893,16 +893,16 @@
         assert res.logical_path == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('volumes/COISS_0xxx/COISS_0001/data/wacfm/bit_wght/13302/133020.lbl',
              True),
-            (PDS_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
-             PDS_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL'),
+            (PDS3_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
+             PDS3_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL'),
         ]
     )
     def test_from_abspath(self, input_path, expected):
         try:
             res = pds3file.Pds3File.from_abspath(abspath=input_path)
             assert isinstance(res, pds3file.Pds3File)
             assert res.abspath == expected
@@ -989,40 +989,40 @@
         assert isinstance(res, pds3file.Pds3File)
         assert res.logical_path == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('volumes/CORSS_8xxx/CORSS_8001/data/Rev007/Rev007E/Rev007E_RSS_2005_123_K34_E/RSS_2005_123_K34_E_CAL.LBL',
-             PDS_HOLDINGS_DIR + '/volumes/CORSS_8xxx/CORSS_8001/data/Rev007/Rev007E/Rev007E_RSS_2005_123_K34_E/RSS_2005_123_K34_E_CAL.LBL'),
-            (PDS_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
-             PDS_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL'),
+             PDS3_HOLDINGS_DIR + '/volumes/CORSS_8xxx/CORSS_8001/data/Rev007/Rev007E/Rev007E_RSS_2005_123_K34_E/RSS_2005_123_K34_E_CAL.LBL'),
+            (PDS3_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
+             PDS3_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL'),
         ]
     )
     def test__from_absolute_or_logical_path(self, input_path, expected):
         res = pds3file.Pds3File._from_absolute_or_logical_path(path=input_path)
         assert isinstance(res, pds3file.Pds3File)
         assert res.abspath == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('holdings/volumes/COUVIS_0xxx_v1/COUVIS_0009/DATA/D2004_274/EUV2004_274_01_39.DAT',
-             PDS_HOLDINGS_DIR + '/volumes/COUVIS_0xxx_v1/COUVIS_0009/DATA/D2004_274/EUV2004_274_01_39.DAT'),
+             PDS3_HOLDINGS_DIR + '/volumes/COUVIS_0xxx_v1/COUVIS_0009/DATA/D2004_274/EUV2004_274_01_39.DAT'),
             ('volumes/COCIRS_0xxx/COCIRS_0012/DATA/NAV_DATA/GEO00120100.DAT',
-             PDS_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/COCIRS_0012/DATA/NAV_DATA/GEO00120100.DAT'),
+             PDS3_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/COCIRS_0012/DATA/NAV_DATA/GEO00120100.DAT'),
             ('COVIMS_0xxx/COVIMS_0001/data/1999010T054026_1999010T060958',
-             PDS_HOLDINGS_DIR + '/volumes/COVIMS_0xxx/COVIMS_0001/data/1999010T054026_1999010T060958'),
+             PDS3_HOLDINGS_DIR + '/volumes/COVIMS_0xxx/COVIMS_0001/data/1999010T054026_1999010T060958'),
             ('metadata/HSTOx_xxxx/HSTO0_7308',
-             PDS_HOLDINGS_DIR + '/metadata/HSTOx_xxxx/HSTO0_7308'),
-            ('HSTOx_xxxx', PDS_HOLDINGS_DIR + '/volumes/HSTOx_xxxx'),
+             PDS3_HOLDINGS_DIR + '/metadata/HSTOx_xxxx/HSTO0_7308'),
+            ('HSTOx_xxxx', PDS3_HOLDINGS_DIR + '/volumes/HSTOx_xxxx'),
             ('volumes/VGIRIS_xxxx_peer_review/VGIRIS_0001/DATA/JUPITER_VG1/C1547XXX.LBL',
-             PDS_HOLDINGS_DIR + '/volumes/VGIRIS_xxxx_peer_review/VGIRIS_0001/DATA/JUPITER_VG1/C1547XXX.LBL'),
+             PDS3_HOLDINGS_DIR + '/volumes/VGIRIS_xxxx_peer_review/VGIRIS_0001/DATA/JUPITER_VG1/C1547XXX.LBL'),
             ('COCIRS_1001/DATA/CUBE/EQUIRECTANGULAR/123RI_EQLBS002_____CI____699_F1_039E.tar.gz',
-             PDS_HOLDINGS_DIR + '/volumes/COCIRS_1xxx/COCIRS_1001/DATA/CUBE/EQUIRECTANGULAR/123RI_EQLBS002_____CI____699_F1_039E.tar.gz'),
+             PDS3_HOLDINGS_DIR + '/volumes/COCIRS_1xxx/COCIRS_1001/DATA/CUBE/EQUIRECTANGULAR/123RI_EQLBS002_____CI____699_F1_039E.tar.gz'),
         ]
     )
     def test_from_path(self, input_path, expected):
         res = pds3file.Pds3File.from_path(path=input_path)
         assert isinstance(res, pds3file.Pds3File)
         assert res.abspath == expected
 
@@ -1043,17 +1043,19 @@
     ############################################################################
     # Test for OPUS support methods
     ############################################################################
     # from_filespec will only work with files under /volumes
     @pytest.mark.parametrize(
         'filespec,expected',
         [
-            ('COISS_0001', PDS_HOLDINGS_DIR + '/volumes/COISS_0xxx/COISS_0001'),
+            ('COISS_0001', PDS3_HOLDINGS_DIR + '/volumes/COISS_0xxx/COISS_0001'),
             ('COISS_1001/data/1294561143_1295221348/W1294561202_1.IMG',
-             PDS_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.IMG'),
+             PDS3_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.IMG'),
+            ('HSTI1_3667/DATA/VISIT_01/ICOK01H9Q.LBL',
+             PDS3_HOLDINGS_DIR + '/volumes/HSTIx_xxxx/HSTI1_3667/DATA/VISIT_01/ICOK01H9Q.LBL'),
         ]
     )
     def test_from_filespec(self, filespec, expected):
         res = pds3file.Pds3File.from_filespec(filespec=filespec)
         assert isinstance(res, pds3file.Pds3File)
         assert res.abspath == expected
 
@@ -1080,25 +1082,25 @@
              'volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL'),
             ('hst-07308-stis-o43b05c1q',
              'volumes/HSTOx_xxxx/HSTO0_7308/DATA/VISIT_05/O43B05C1Q.LBL'),
             ('hst-05167-wfpc2-u2no0404t',
              'volumes/HSTUx_xxxx/HSTU0_5167/DATA/VISIT_04/U2NO0404T.LBL'),
             ('nh-lorri-lor_0003103486',
              'volumes/NHxxLO_xxxx/NHLALO_1001/data/20060224_000310/lor_0003103486_0x630_eng.fit'),
-            ('eso1m-apph-occ-1989-184-28sgr-e',
+            ('esosil1m04-apph-occ-1989-184-28sgr-e',
              'volumes/EBROCC_xxxx/EBROCC_0001/DATA/ESO1M/ES1_EPD.TAB'),
-            ('eso22m-apph-occ-1989-184-28sgr-i',
+            ('esosil2m2-apph-occ-1989-184-28sgr-i',
              'volumes/EBROCC_xxxx/EBROCC_0001/DATA/ESO22M/ES2_IPD.TAB'),
             ('lick1m-ccdc-occ-1989-184-28sgr-e',
              'volumes/EBROCC_xxxx/EBROCC_0001/DATA/LICK1M/LIC_EPD.TAB'),
-            ('irtf-urac-occ-1989-184-28sgr-i',
+            ('irtf3m2-urac-occ-1989-184-28sgr-i',
              'volumes/EBROCC_xxxx/EBROCC_0001/DATA/IRTF/IRT_IPD.TAB'),
-            ('pal200-circ-occ-1989-184-28sgr-i',
+            ('pal5m08-circ-occ-1989-184-28sgr-i',
              'volumes/EBROCC_xxxx/EBROCC_0001/DATA/PAL200/PAL_IPD.TAB'),
-            ('mcd27m-iirar-occ-1989-184-28sgr-i',
+            ('mcd2m7-iirar-occ-1989-184-28sgr-i',
              'volumes/EBROCC_xxxx/EBROCC_0001/DATA/MCD27M/MCD_IPD.TAB'),
             ('co-rss-occ-2005-159-rev009-k55-e',
              'volumes/CORSS_8xxx/CORSS_8001/data/Rev009/Rev009E/Rev009E_RSS_2005_159_K55_E/RSS_2005_159_K55_E_TAU_01KM.TAB'),
 
             # ('nh-mvic-mc0_0032528036',
             # 'volumes/NHxxMV_xxxx/NHJUMV_1001/data/20070131_003252/mc0_0032528036_0x536_eng_1.fit'),
             # ('nh-mvic-mc0_0005261846',
@@ -1115,15 +1117,15 @@
         assert target_pdsfile1.opus_id == input_id
         assert target_pdsfile2.opus_id == input_id
 
     @pytest.mark.parametrize(
         'opus_id,expected',
         [
             ('hst-07176-nicmos-n4bi01l4q',
-             PDS_HOLDINGS_DIR + '/volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL')
+             PDS3_HOLDINGS_DIR + '/volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL')
         ]
     )
     def test_from_opus_id2(self, opus_id, expected):
         res = pds3file.Pds3File.from_opus_id(opus_id=opus_id)
         assert isinstance(res, pds3file.Pds3File)
         assert res.abspath == expected
 
@@ -1157,32 +1159,32 @@
         assert isinstance(res, pds3file.Pds3File)
         assert res.logical_path == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('metadata/VGISS_8xxx/VGISS_8201/VGISS_8201_inventory.tab',
-             PDS_HOLDINGS_DIR + '/metadata/VGISS_8xxx/VGISS_8201'),
+             PDS3_HOLDINGS_DIR + '/metadata/VGISS_8xxx/VGISS_8201'),
             ('metadata/VGISS_6xxx/VGISS_6101',
-             PDS_HOLDINGS_DIR + '/metadata/VGISS_6xxx/VGISS_6101'),
+             PDS3_HOLDINGS_DIR + '/metadata/VGISS_6xxx/VGISS_6101'),
             ('volumes/VGISS_7xxx/VGISS_7201/DATA/C24476XX/C2447654_RAW.lbl',
-             PDS_HOLDINGS_DIR + '/volumes/VGISS_7xxx/VGISS_7201')
+             PDS3_HOLDINGS_DIR + '/volumes/VGISS_7xxx/VGISS_7201')
         ]
     )
     def test_volume_abspath(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         assert target_pdsfile.volume_abspath() == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('volumes/HSTOx_xxxx/HSTO0_7308/DATA/VISIT_05/O43B05C1Q.ASC',
-             PDS_HOLDINGS_DIR + '/volumes/HSTOx_xxxx'),
+             PDS3_HOLDINGS_DIR + '/volumes/HSTOx_xxxx'),
             ('previews/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q_thumb.jpg',
-             PDS_HOLDINGS_DIR + '/previews/HSTNx_xxxx')
+             PDS3_HOLDINGS_DIR + '/previews/HSTNx_xxxx')
         ]
     )
     def test_volset_abspath(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         assert target_pdsfile.volset_abspath() == expected
 
     ############################################################################
@@ -1254,15 +1256,15 @@
         assert res.logical_path == expected
 
     @pytest.mark.parametrize(
         'input_path,selection,flag,expected',
         [
             ('metadata/HSTUx_xxxx/HSTU0_5167/HSTU0_5167_index.tab',
              'U2NO0404T', '',
-             PDS_HOLDINGS_DIR + '/volumes/HSTUx_xxxx/HSTU0_5167/DATA/VISIT_04/U2NO0404T.LBL'),
+             PDS3_HOLDINGS_DIR + '/volumes/HSTUx_xxxx/HSTU0_5167/DATA/VISIT_04/U2NO0404T.LBL'),
         ]
     )
     def test_data_abspath_associated_with_index_row(self, input_path,
                                                     selection, flag,
                                                     expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         index_row = target_pdsfile.child_of_index(selection, flag)
@@ -1272,17 +1274,17 @@
     ############################################################################
     # Test for checksum path associations
     ############################################################################
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('volumes/COUVIS_0xxx_v1/COUVIS_0009/DATA/D2004_274/EUV2004_274_01_39.lbl',
-             PDS_HOLDINGS_DIR + '/checksums-volumes/COUVIS_0xxx_v1/COUVIS_0009_md5.txt'),
+             PDS3_HOLDINGS_DIR + '/checksums-volumes/COUVIS_0xxx_v1/COUVIS_0009_md5.txt'),
             ('metadata/VGISS_5xxx/VGISS_5101/VGISS_5101_supplemental_index.tab',
-             PDS_HOLDINGS_DIR + '/checksums-metadata/VGISS_5xxx/VGISS_5101_metadata_md5.txt')
+             PDS3_HOLDINGS_DIR + '/checksums-metadata/VGISS_5xxx/VGISS_5101_metadata_md5.txt')
         ]
     )
     def test_checksum_path_and_lskip(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         if target_pdsfile.archives_:
             lskip = (len(target_pdsfile.root_) + len('checksums_')
                      + len(target_pdsfile.category_))
@@ -1293,81 +1295,81 @@
         expected = (expected, lskip)
         assert target_pdsfile.checksum_path_and_lskip() == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('archives-volumes/COCIRS_0xxx',
-             PDS_HOLDINGS_DIR + '/checksums-archives-volumes/COCIRS_0xxx_md5.txt'),
+             PDS3_HOLDINGS_DIR + '/checksums-archives-volumes/COCIRS_0xxx_md5.txt'),
             ('volumes/COCIRS_0xxx/COCIRS_0010',
-             PDS_HOLDINGS_DIR + '/checksums-volumes/COCIRS_0xxx/COCIRS_0010_md5.txt'),
+             PDS3_HOLDINGS_DIR + '/checksums-volumes/COCIRS_0xxx/COCIRS_0010_md5.txt'),
             ('checksums-volumes/COCIRS_0xxx/COCIRS_0010_md5.txt', '')
         ]
     )
     def test_checksum_path_if_exact(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.checksum_path_if_exact()
         assert res == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             # ('archives-volumes/COCIRS_0xxx/COCIRS_0010.tar.gz',
             #  (
-            #     PDS_HOLDINGS_DIR + '/archives-volumes/COCIRS_0xxx',
-            #     PDS_HOLDINGS_DIR + '/archives-volumes/COCIRS_0xxx/')),
+            #     PDS3_HOLDINGS_DIR + '/archives-volumes/COCIRS_0xxx',
+            #     PDS3_HOLDINGS_DIR + '/archives-volumes/COCIRS_0xxx/')),
             ('checksums-volumes/COCIRS_0xxx/COCIRS_0010_md5.txt',
              (
-                PDS_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/COCIRS_0010',
-                PDS_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/')),
+                PDS3_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/COCIRS_0010',
+                PDS3_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/')),
         ]
     )
     def test_dirpath_and_prefix_for_checksum(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.dirpath_and_prefix_for_checksum()
         assert res == expected
 
     ############################################################################
     # Test for archive path associations
     ############################################################################
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('metadata/HSTUx_xxxx/HSTU0_5167/HSTU0_5167_index.tab',
-             PDS_HOLDINGS_DIR + '/archives-metadata/HSTUx_xxxx/HSTU0_5167_metadata.tar.gz'),
+             PDS3_HOLDINGS_DIR + '/archives-metadata/HSTUx_xxxx/HSTU0_5167_metadata.tar.gz'),
             ('volumes/EBROCC_xxxx/EBROCC_0001/DATA/ESO1M/ES1_EPD.LBL',
-             PDS_HOLDINGS_DIR + '/archives-volumes/EBROCC_xxxx/EBROCC_0001.tar.gz')
+             PDS3_HOLDINGS_DIR + '/archives-volumes/EBROCC_xxxx/EBROCC_0001.tar.gz')
         ]
     )
     def test_archive_path_and_lskip(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         lskip = (len(target_pdsfile.root_) + len(target_pdsfile.category_)
                  + len(target_pdsfile.bundleset_))
         expected = (expected, lskip)
         assert target_pdsfile.archive_path_and_lskip() == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('archives-volumes/COCIRS_0xxx/COCIRS_0010.tar.gz', ''),
             ('volumes/COCIRS_0xxx/COCIRS_0010',
-             PDS_HOLDINGS_DIR + '/archives-volumes/COCIRS_0xxx/COCIRS_0010.tar.gz'),
+             PDS3_HOLDINGS_DIR + '/archives-volumes/COCIRS_0xxx/COCIRS_0010.tar.gz'),
         ]
     )
     def test_archive_path_if_exact(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.archive_path_if_exact()
         assert res == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('archives-volumes/COCIRS_0xxx/COCIRS_0010.tar.gz',
-             (PDS_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/COCIRS_0010',
-              PDS_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/')),
+             (PDS3_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/COCIRS_0010',
+              PDS3_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/')),
         ]
     )
     def test_dirpath_and_prefix_for_archive(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.dirpath_and_prefix_for_archive()
         assert res == expected
 
@@ -1661,16 +1663,16 @@
         'input_path,expected',
         [
             ([
                 'volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
                 'volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL'
              ],
              [
-                 PDS_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
-                 PDS_HOLDINGS_DIR + '/volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL'
+                 PDS3_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
+                 PDS3_HOLDINGS_DIR + '/volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL'
              ])
         ]
     )
     def test_abspaths_for_pdsfiles(self, input_path, expected):
         pdsfiles = []
         for path in input_path:
             pdsfiles.append(instantiate_target_pdsfile(path))
@@ -1724,16 +1726,16 @@
         for basename in res:
             assert basename in expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ([
-                PDS_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
-                PDS_HOLDINGS_DIR + '/volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL'
+                PDS3_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
+                PDS3_HOLDINGS_DIR + '/volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL'
              ],
              [
                 'volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
                 'volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL',
              ])
         ]
     )
@@ -1744,16 +1746,16 @@
         for path in res:
             assert path in expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ([
-                PDS_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
-                PDS_HOLDINGS_DIR + '/volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL'
+                PDS3_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
+                PDS3_HOLDINGS_DIR + '/volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL'
              ],
              ['W1294561202_1.LBL', 'N4BI01L4Q.LBL'])
         ]
     )
     def test_basenames_for_abspaths(self, input_path, expected):
         res = pds3file.Pds3File.basenames_for_abspaths(abspaths=input_path)
 
@@ -1784,16 +1786,16 @@
         'input_path,expected',
         [
             ([
                 'volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
                 'volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL'
              ],
              [
-                PDS_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
-                PDS_HOLDINGS_DIR + '/volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL',
+                PDS3_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
+                PDS3_HOLDINGS_DIR + '/volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL',
              ])
         ]
     )
     def test_abspaths_for_logicals(self, input_path, expected):
         res = pds3file.Pds3File.abspaths_for_logicals(logical_paths=input_path,
                                                     must_exist=True)
 
@@ -1817,15 +1819,15 @@
             assert basename in expected
 
     @pytest.mark.parametrize(
         'input_path,basenames,expected',
         [
             ('volumes/COISS_0xxx/COISS_0001/data/wacfm/bit_wght/13302',
              ['133020.lbl'],
-             [PDS_HOLDINGS_DIR + '/volumes/COISS_0xxx/COISS_0001/data/wacfm/bit_wght/13302/133020.lbl'])
+             [PDS3_HOLDINGS_DIR + '/volumes/COISS_0xxx/COISS_0001/data/wacfm/bit_wght/13302/133020.lbl'])
         ]
     )
     def test_abspaths_for_basenames(self, input_path, basenames, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.abspaths_for_basenames(basenames=basenames)
 
         for path in res:
@@ -1865,15 +1867,15 @@
         print(target_associated_parallel.logical_path)
         assert target_associated_parallel.logical_path == expected
 
     @pytest.mark.parametrize(
         'input_path,expected_path',
         [
             ('volumes/COCIRS_0xxx/COCIRS_0012/DATA/NAV_DATA/GEO00120100.DAT',
-             [PDS_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/COCIRS_0012/DATA/NAV_DATA/GEO00120100.DAT']),
+             [PDS3_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/COCIRS_0012/DATA/NAV_DATA/GEO00120100.DAT']),
 
         ]
     )
     def test_copy(self, input_path, expected_path):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         pdsf_copy = target_pdsfile.copy()
         assert pdsf_copy.abspath in expected_path
@@ -1897,26 +1899,26 @@
 ##########################################################################################
 class TestPds3FileHelperBlackBox:
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('volumes/COVIMS_8xxx/COVIMS_8001/data/VIMS_2017_251_GAMCRU_I_TAU_10KM.tab',
              True),
-            (PDS_HOLDINGS_DIR + '/metadata/COVIMS_0xxx/COVIMS_0001',
+            (PDS3_HOLDINGS_DIR + '/metadata/COVIMS_0xxx/COVIMS_0001',
              False),
         ]
     )
     def test_is_logical_path(self, input_path, expected):
         res = pds3file.Pds3File.is_logical_path(path=input_path)
         assert res == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-            (PDS_HOLDINGS_DIR + '/volumes/COUVIS_0xxx/COUVIS_0058/DATA/D2017_001/EUV2017_001_03_49.dat',
+            (PDS3_HOLDINGS_DIR + '/volumes/COUVIS_0xxx/COUVIS_0058/DATA/D2017_001/EUV2017_001_03_49.dat',
              'volumes/COUVIS_0xxx/COUVIS_0058/DATA/D2017_001/EUV2017_001_03_49.dat'),
             ('volumes/COUVIS_0xxx/COUVIS_0058/DATA/D2017_001/EUV2017_001_03_49.dat',
              'volumes/COUVIS_0xxx/COUVIS_0058/DATA/D2017_001/EUV2017_001_03_49.dat'),
         ]
     )
     def test_logical_path_from_abspath(self, input_path, expected):
         try:
@@ -1924,27 +1926,27 @@
             assert res == expected
         except ValueError as err:
             assert True # Not an absolute path
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-            (PDS_HOLDINGS_DIR + '/volumes/COUVIS_0xxx/COUVIS_0058/DATA/D2017_001/EUV2017_001_03_49.DAT',
-             PDS_HOLDINGS_DIR + '/volumes/COUVIS_0xxx/COUVIS_0058/DATA/D2017_001/EUV2017_001_03_49.DAT')
+            (PDS3_HOLDINGS_DIR + '/volumes/COUVIS_0xxx/COUVIS_0058/DATA/D2017_001/EUV2017_001_03_49.DAT',
+             PDS3_HOLDINGS_DIR + '/volumes/COUVIS_0xxx/COUVIS_0058/DATA/D2017_001/EUV2017_001_03_49.DAT')
         ]
     )
     def test_repair_case(self, input_path, expected):
         res = repair_case(input_path, pds3file.Pds3File)
         assert res.lower() == expected.lower()
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-            (PDS_HOLDINGS_DIR + '/volumes/COUVIS_0xxx/COUVIS_0058/DATA/D2017_001/EUV2017_001_03_49.dat',
-             PDS_HOLDINGS_DIR + '/volumes/COUVIS_0xxx/COUVIS_0058/DATA/D2017_001/EUV2017_001_03_49.dat'),
+            (PDS3_HOLDINGS_DIR + '/volumes/COUVIS_0xxx/COUVIS_0058/DATA/D2017_001/EUV2017_001_03_49.dat',
+             PDS3_HOLDINGS_DIR + '/volumes/COUVIS_0xxx/COUVIS_0058/DATA/D2017_001/EUV2017_001_03_49.dat'),
             ('volumes/COISS_0xxx/COISS_0001/data/wacfm/bit_wght/13302/133020.lbl',
-             PDS_HOLDINGS_DIR + '/volumes/COISS_0xxx/COISS_0001/data/wacfm/bit_wght/13302/133020.lbl'),
+             PDS3_HOLDINGS_DIR + '/volumes/COISS_0xxx/COISS_0001/data/wacfm/bit_wght/13302/133020.lbl'),
         ]
     )
     def test_selected_path_from_path(self, input_path, expected):
         res = selected_path_from_path(input_path, pds3file.Pds3File)
         assert res == expected
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 import datetime
 import os
 import pdsfile.pds3file as pds3file
 from pdsfile import pdsviewable
 import pytest
 
-from .helper import (PDS_HOLDINGS_DIR,
+from .helper import (PDS3_HOLDINGS_DIR,
                      instantiate_target_pdsfile)
 
 try:
-    PDS_TESTING_ROOT = PDS_HOLDINGS_DIR[:PDS_HOLDINGS_DIR.rindex('pdsdata')]
+    PDS_TESTING_ROOT = PDS3_HOLDINGS_DIR[:PDS3_HOLDINGS_DIR.rindex('pdsdata')]
 except ValueError: # pragma: no cover
     PDS_TESTING_ROOT = '/Library/WebServer/Documents/'
 
 ##########################################################################################
 # Blackbox test for internal cached in PdsFile class
 ##########################################################################################
 class TestPdsFileBlackBox:
@@ -318,23 +318,23 @@
         assert res1 == res2
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('volumes/COUVIS_0xxx_v1/COUVIS_0009/DATA/D2004_274/EUV2004_274_01_39.LBL',
              [
-                (58, 'EUV2004_274_01_39.DAT', PDS_HOLDINGS_DIR + '/volumes/COUVIS_0xxx_v1/COUVIS_0009/DATA/D2004_274/EUV2004_274_01_39.DAT'),
+                (58, 'EUV2004_274_01_39.DAT', PDS3_HOLDINGS_DIR + '/volumes/COUVIS_0xxx_v1/COUVIS_0009/DATA/D2004_274/EUV2004_274_01_39.DAT'),
              ]),
             ('volumes/COCIRS_0xxx/COCIRS_0012/DATA', []),
             ('previews/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561261_1_thumb.jpg', []),
             ('volumes/COCIRS_0xxx/COCIRS_0012/DATA/NAV_DATA/GEO00120100.LBL',
              [
-                (24, 'GEO00120100.DAT', PDS_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/COCIRS_0012/DATA/NAV_DATA/GEO00120100.DAT'),
-                (25, 'GEO00120100.DAT', PDS_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/COCIRS_0012/DATA/NAV_DATA/GEO00120100.DAT'),
-                (32, 'GEO.FMT', PDS_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/COCIRS_0012/DATA/NAV_DATA/GEO.FMT')
+                (24, 'GEO00120100.DAT', PDS3_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/COCIRS_0012/DATA/NAV_DATA/GEO00120100.DAT'),
+                (25, 'GEO00120100.DAT', PDS3_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/COCIRS_0012/DATA/NAV_DATA/GEO00120100.DAT'),
+                (32, 'GEO.FMT', PDS3_HOLDINGS_DIR + '/volumes/COCIRS_0xxx/COCIRS_0012/DATA/NAV_DATA/GEO.FMT')
              ])
         ]
     )
     def test_internal_link_info(self, input_path, expected):
         """internal_link_info: return self._internal_links_filled"""
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res1 = target_pdsfile.internal_link_info
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/tests/test_pds3file_whitebox.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pds3file_whitebox.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 import os
 import pdsfile.pds3file as pds3file
 from pdsfile import pdsviewable
 import pytest
 import re
 
-from .helper import (PDS_HOLDINGS_DIR,
+from .helper import (PDS3_HOLDINGS_DIR,
                      instantiate_target_pdsfile)
 
-PDS_PDSDATA_PATH = PDS_HOLDINGS_DIR[:PDS_HOLDINGS_DIR.index('holdings')]
+PDS_PDSDATA_PATH = PDS3_HOLDINGS_DIR[:PDS3_HOLDINGS_DIR.index('holdings')]
 
 ##########################################################################################
 # Whitebox test for functions & properties in PdsFile class
 ##########################################################################################
 class TestPdsFileWhiteBox:
     ############################################################################
     # Test for properties
@@ -310,17 +310,17 @@
     ############################################################################
     # Test for functions
     ############################################################################
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('volumes',
-             'Pds3File.COCIRS_xxxx("' + PDS_HOLDINGS_DIR + '/volumes/COCIRS_0xxx")'),
+             'Pds3File.COCIRS_xxxx("' + PDS3_HOLDINGS_DIR + '/volumes/COCIRS_0xxx")'),
             # ('volumes/ASTROM_xxxx/ASTROM_0001',
-            #  'Pds3File.ASTROM_xxxx("' + PDS_HOLDINGS_DIR + '/volumes/ASTROM_xxxx/ASTROM_0001/VOLDESC.CAT")'),
+            #  'Pds3File.ASTROM_xxxx("' + PDS3_HOLDINGS_DIR + '/volumes/ASTROM_xxxx/ASTROM_0001/VOLDESC.CAT")'),
         ]
     )
     def test__repr__(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(
             input_path, is_abspath=False)
         child = target_pdsfile.child(basename='COCIRS_0xxx')
         res = child.__repr__()
@@ -421,27 +421,27 @@
     ############################################################################
     # Test for associated volumes and volsets
     ############################################################################
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('archives-volumes/COUVIS_0xxx/COUVIS_0001.tar.gz',
-             PDS_HOLDINGS_DIR + '/archives-volumes/COUVIS_0xxx/COUVIS_0001.tar.gz'),
+             PDS3_HOLDINGS_DIR + '/archives-volumes/COUVIS_0xxx/COUVIS_0001.tar.gz'),
 
         ]
     )
     def test_volume_abspath(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         assert target_pdsfile.volume_abspath() == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('checksums-archives-volumes/ASTROM_xxxx_md5.txt',
-             PDS_HOLDINGS_DIR + '/checksums-archives-volumes/ASTROM_xxxx_md5.txt'),
+             PDS3_HOLDINGS_DIR + '/checksums-archives-volumes/ASTROM_xxxx_md5.txt'),
         ]
     )
     def test_volset_abspath(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         assert target_pdsfile.volset_abspath() == expected
 
     ############################################################################
@@ -560,16 +560,16 @@
         'input_path,expected',
         [
             ([
                 'volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
                 'volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL'
              ],
              [
-                 PDS_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
-                 PDS_HOLDINGS_DIR + '/volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL'
+                 PDS3_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
+                 PDS3_HOLDINGS_DIR + '/volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL'
              ])
         ]
     )
     def test_abspaths_for_pdsfiles(self, input_path, expected):
         pdsfiles = []
         for path in input_path:
             pdsfiles.append(instantiate_target_pdsfile(path))
@@ -626,16 +626,16 @@
         for basename in res:
             assert basename in expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ([
-                PDS_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
-                PDS_HOLDINGS_DIR + '/volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL'
+                PDS3_HOLDINGS_DIR + '/volumes/COISS_1xxx/COISS_1001/data/1294561143_1295221348/W1294561202_1.LBL',
+                PDS3_HOLDINGS_DIR + '/volumes/HSTNx_xxxx/HSTN0_7176/DATA/VISIT_01/N4BI01L4Q.LBL'
              ],
              ['W1294561202_1.LBL', 'N4BI01L4Q.LBL'])
         ]
     )
     def test_basenames_for_abspaths(self, input_path, expected):
         res = pds3file.Pds3File.basenames_for_abspaths(abspaths=input_path,
                                                      must_exist=True)
@@ -681,15 +681,15 @@
             assert basename in expected
 
     @pytest.mark.parametrize(
         'input_path,basenames,expected',
         [
             ('volumes/COISS_0xxx/COISS_0001/data/wacfm/bit_wght/13302',
              ['133020.lbl'],
-             [PDS_HOLDINGS_DIR + '/volumes/COISS_0xxx/COISS_0001/data/wacfm/bit_wght/13302/133020.lbl'])
+             [PDS3_HOLDINGS_DIR + '/volumes/COISS_0xxx/COISS_0001/data/wacfm/bit_wght/13302/133020.lbl'])
         ]
     )
     def test_abspaths_for_basenames(self, input_path, basenames, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.abspaths_for_basenames(basenames=basenames,
                                                     must_exist=True)
 
@@ -867,16 +867,16 @@
             if error_msg in str(e.value):
                 res = True
         assert res
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-            (PDS_HOLDINGS_DIR + '/volumes/COISS_0xxx/COISS_0001',
-             PDS_HOLDINGS_DIR + '/volumes/COISS_0xxx/COISS_0001'),
+            (PDS3_HOLDINGS_DIR + '/volumes/COISS_0xxx/COISS_0001',
+             PDS3_HOLDINGS_DIR + '/volumes/COISS_0xxx/COISS_0001'),
         ]
     )
     def test_from_abspath(self, input_path, expected):
         if input_path in pds3file.Pds3File.CACHE:
             del pds3file.Pds3File.CACHE[input_path]
         res = pds3file.Pds3File.from_abspath(abspath=input_path,
                                            fix_case=True)
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py` & `rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds4file/__init__.py` & `rms-pdsfile-0.0.2/pdsfile/pds4file/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds4file/rules/__init__.py` & `rms-pdsfile-0.0.2/pdsfile/pds4file/rules/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,16 +259,16 @@
 # Defines files associated with a given file. A dictionary of Translators keyed by 'volumes', 'calibrated', 'browse', 'diagrams',
 # or 'metadata'.
 #
 # These Translators take a logical path and return logical paths of associated files based on the key.
 ##########################################################################################
 
 ASSOCIATIONS = {
-    'volumes'   : translator.TranslatorByRegex([
-                        (r'documents/([A-Z][A-Z0-9x]{1,5}_....).*', 0, r'volumes/\1'),
+    'bundles'   : translator.TranslatorByRegex([
+                        (r'documents/(\w.*)/.*', 0, r'bundles/\1'),
                     ]),
     'previews'  : translator.NullTranslator(),
     'calibrated': translator.NullTranslator(),
     'diagrams'  : translator.NullTranslator(),
     'metadata'  : translator.TranslatorByRegex([
                         (r'metadata/([\w\.]+)/.*', 0, r'metadata/\1/AAREADME.txt'),
                         (r'volumes/([A-Z][A-Z0-9x]{1,5}_....)(|_[\w\.]+)/([\w]+)/index', re.I,
@@ -497,16 +497,15 @@
     (r'metadata/.*_(moon|charon)_summary\..*', 0, ('metadata', 30, 'moon_geometry',   'Moon Geometry Index',   False)),
     (r'metadata/.*_ring_summary\..*',          0, ('metadata', 40, 'ring_geometry',   'Ring Geometry Index',   False)),
 
     # Metadata index
     (r'metadata/.*_\d+_index\..*',         0, ('metadata', 5, 'rms_index',          'RMS Node Augmented Index',     False)),
     (r'metadata/.*_hstfiles\..*',          0, ('metadata', 6, 'hstfiles_index',     'HST Files Associations Index', False)),
     (r'metadata/.*raw_image_index\..*',    0, ('metadata', 7, 'raw_image_index',    'Raw Image Index',              False)),
-    (r'metadata/.*profile_index\..*',      0, ('metadata', 8, 'profile_index',      'Profile Index',                False)),
-    (r'metadata/.*supplemental_index\..*', 0, ('metadata', 9, 'supplemental_index', 'Supplemental Index',           False)),
+    (r'metadata/.*supplemental_index\..*', 0, ('metadata', 8, 'supplemental_index', 'Supplemental Index',           False)),
 ])
 
 ##########################################################################################
 # OPUS_FORMAT
 #
 # Returns a tuple (interchange format, file format) where the first is 'Binary', 'ASCII' or 'UTF-8' and the latter is the format
 # of the file, e.g., 'Vicar', 'FITS', 'Table', 'PDS3 Label', etc.
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds4file/rules/pytest_support.py` & `rms-pdsfile-0.0.2/pdsfile/pds4file/rules/pytest_support.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     return unmatched
 
 ##########################################################################################
 # Dave's test suite helpers
 ##########################################################################################
 
 def instantiate_target_pdsfile(path, is_abspath=True):
+    path = 'bundles/'+path
     if is_abspath:
         TESTFILE_PATH = abspath_for_logical_path(path, pds4file.Pds4File)
         target_pdsfile = pds4file.Pds4File.from_abspath(TESTFILE_PATH)
     else:
         TESTFILE_PATH = path
         target_pdsfile = pds4file.Pds4File.from_logical_path(TESTFILE_PATH)
     return target_pdsfile
@@ -109,17 +110,17 @@
 ):
     target_pdsfile = instantiate_target_pdsfile(input_path, is_abspath)
     results = target_pdsfile.opus_products()
     # Note that messages are more useful if extra values are identified before
     # missing values. That's because extra items are generally more diagnostic
     # of the issue at hand.
     for key in results:
-        assert key in expected, f'Extra key: {key}'
+        assert key in expected, f'Extra key: {key} = {results[key]}'
     for key in expected:
-        assert key in results, f'Missing key: {key}'
+        assert key in results, f'Missing key: {key} = {expected[key]}'
     for key in results:
         result_paths = []       # flattened list of logical paths
         for pdsfiles in results[key]:
             result_paths += pds4file.Pds4File.logicals_for_pdsfiles(pdsfiles)
         for path in result_paths:
             assert path in expected[key], f'Extra file under key {key}: {path}'
         for path in expected[key]:
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pds4file/tests/helper.py` & `rms-pdsfile-0.0.2/pdsfile/pds4file/tests/helper.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pdscache.py` & `rms-pdsfile-0.0.2/pdsfile/pdscache.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/pdsfile.py` & `rms-pdsfile-0.0.2/pdsfile/pdsfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         with open(abspath, 'rb') as f:
             pass
 
     return abspath
 
 def formatted_file_size(size):
     order = int(math.log10(size) // 3) if size else 0
-    return '{:.3g} {}'.format(size / 1000.**order, FILE_BYTE_UNITS[order])
+    return f'{size / 1000.**order:.3g} {FILE_BYTE_UNITS[order]}'
 
 def abspath_for_logical_path(path, cls):
     """Return the absolute path derived from the given logical path.
 
     The logical path starts at the category, below the holdings/ directory. To
     get the absolute path, we need to figure out where the holdings directory is
     located. Note that there can be multiple drives hosting multiple holdings
@@ -189,16 +189,16 @@
     # Use the list of preloaded holdings directories if it is not empty
     if cls.LOCAL_PRELOADED:
         holdings_list = cls.LOCAL_PRELOADED
 
     elif cls.LOCAL_HOLDINGS_DIRS:
         holdings_list = cls.LOCAL_HOLDINGS_DIRS
 
-    elif 'PDS_HOLDINGS_DIR' in os.environ:
-        holdings_list = [os.environ['PDS_HOLDINGS_DIR']]
+    elif 'PDS3_HOLDINGS_DIR' in os.environ:
+        holdings_list = [os.environ['PDS3_HOLDINGS_DIR']]
         cls.LOCAL_HOLDINGS_DIRS = holdings_list
 
     # Without a preload or an environment variable, check the
     # /Library/WebSever/Documents directory for a symlink. This only works for
     # MacOS with the website installed, but that's OK.
     else:
         holdings_dirs = glob.glob('/Library/WebServer/Documents/holdings*')
@@ -646,15 +646,14 @@
                 _ = cls.CACHE['$VOLS-'  + category + '/']
                 pdsf0 = cls.CACHE[category]
 
                 # Also get the bundleset-level PdsFile inside each category
                 for bundleset in pdsf0.childnames:
                     if bundleset.endswith('.txt') or bundleset.endswith('.tar.gz'):
                         continue
-
                     # Get the entry keyed by the logical path
                     pdsf1 = cls.CACHE[category + '/' + bundleset.lower()]
 
                     # Also get its bundle-level children
                     for bundlename in pdsf1.childnames:
                         if bundlename.endswith('.txt') or bundlename.endswith('.tar.gz'):
                             continue
@@ -1217,15 +1216,15 @@
         absolute path does not point to a checksum file, it returns None.
 
         Keyword arguments:
             abspath -- the absolute path of the checksum file.
         """
 
         # Checksum files need special handling
-        if '/holdings/checksums-' in abspath:
+        if f'/{cls.PDS_HOLDINGS}/checksums-' in abspath:
             testpath = abspath.replace('/checksums-', '/')
 
             for voltype in cls.VOLTYPES:
                 testpath = testpath.replace('_' + voltype + '_md5.txt', '')
 
             return testpath
 
@@ -1247,29 +1246,29 @@
 
         Keyword arguments:
             abspath              -- the absolute path of the file.
             force_case_sensitive -- a flag to determine if the basename will be case
                                     sensitive (default False)
         """
 
-        if 'holdings/_infoshelf' in abspath:
+        if f'{cls.PDS_HOLDINGS}/_infoshelf' in abspath:
             return os.path.exists(abspath)
 
         # Handle index rows
         if '.tab/' in abspath:
             parts = abspath.partition('.tab/')
             if not cls.os_path_exists(parts[0] + '.tab'):
                 return False
             pdsf = cls.from_abspath(parts[0] + '.tab')
             return (pdsf.exists and
                     pdsf.child_of_index(parts[2], flag='').exists)
 
         # If it's for documentation, we don't create shelf files, we will just use the
         # os.path.exists
-        if cls.SHELVES_ONLY and 'holdings/documents' not in abspath:
+        if cls.SHELVES_ONLY and f'{cls.PDS_HOLDINGS}/documents' not in abspath:
             try:
                 (shelf_abspath,
                  key) = cls.shelf_path_and_key_for_abspath(abspath, 'info')
 
                 if key:
                     shelf = cls._get_shelf(shelf_abspath,
                                                log_missing_file=False)
@@ -1280,27 +1279,27 @@
                                     # open of the file.
                 else:
                     return False
             except (ValueError, IndexError, IOError, OSError):
                 pass
 
             # Maybe it's associated with something else in the infoshelf tree
-            if '/holdings/' in abspath:
+            if f'/{cls.PDS_HOLDINGS}/' in abspath:
 
                 # Maybe there's an associated directory in the infoshelf tree
-                shelf_abspath = abspath.replace('/holdings/',
-                                                '/holdings/_infoshelf-')
+                shelf_abspath = abspath.replace(f'/{cls.PDS_HOLDINGS}/',
+                                                f'/{cls.PDS_HOLDINGS}/_infoshelf-')
                 if cls.os_path_exists(shelf_abspath):
                     return True
 
                 # Maybe there's an associated shelf file in the infoshelf tree
                 if cls.os_path_exists(shelf_abspath + '_info.pickle'):
                     return True
 
-                # Checksum files need special handling
+                # Checksum files need special handling, before doing special handling,
                 testpath = cls._non_checksum_abspath(abspath)
                 if testpath and cls.os_path_exists(testpath):
                     return True
 
         if force_case_sensitive and cls.FS_IS_CASE_INSENSITIVE:
             test = os.path.exists(abspath)
             if not test:
@@ -1338,19 +1337,19 @@
                                     # open of the file.
                 else:
                     return False
             except (ValueError, IndexError, IOError, OSError):
                 pass
 
             # Maybe it's associated with something else in the infoshelf tree
-            if '/holdings/' in abspath:
+            if f'/{cls.PDS_HOLDINGS}/' in abspath:
 
                 # Maybe there's an associated directory in the infoshelf tree
-                shelf_abspath = abspath.replace('/holdings/',
-                                                '/holdings/_infoshelf-')
+                shelf_abspath = abspath.replace(f'/{cls.PDS_HOLDINGS}/',
+                                                f'/{cls.PDS_HOLDINGS}/_infoshelf-')
                 if os.path.exists(shelf_abspath):
                     return True
 
                 # Maybe there's an associated shelf file in the infoshelf tree
                 if os.path.exists(shelf_abspath + '_info.pickle'):
                     return True
 
@@ -1397,88 +1396,88 @@
                     basename = key[lprefix:]
                     if '/' not in basename:
                         basenames.append(basename)
 
                 return basenames
 
             # Deal with checksums-archives directories
-            if '/holdings/checksums-archives-' in abspath:
+            if f'/{cls.PDS_HOLDINGS}/checksums-archives-' in abspath:
                 if abspath.endswith('.txt'):
                     return []
 
                 testpath = abspath.replace('/checksums-','/')
                 results = cls.os_listdir(testpath)
 
                 for voltype in cls.VOLTYPES:
-                  if '-' + voltype in abspath:
-                    if voltype == 'volumes':
-                        return [r + '_md5.txt' for r in results]
-                    else:
-                        return [r + '_' + voltype + '_md5.txt' for r in results]
+                    if '-' + voltype in abspath:
+                        if voltype == 'volumes':
+                            return [r + '_md5.txt' for r in results]
+                        else:
+                            return [r + '_' + voltype + '_md5.txt' for r in results]
 
                 raise ValueError('Invalid abspath for os_listdir: ' + abspath)
 
             # Deal with checksums directories
-            if '/holdings/checksums-' in abspath:
+            if f'/{cls.PDS_HOLDINGS}/checksums-' in abspath:
                 if abspath.endswith('_md5.txt'):
                     return []
 
                 testpath = abspath.replace('/checksums-','/')
                 results = cls.os_listdir(testpath)
 
-                after = abspath.rpartition('/holdings/checksums-')[-1]
+                after = abspath.rpartition(f'/{cls.PDS_HOLDINGS}/checksums-')[-1]
                 parts = after.split('/')
                 if len(parts) == 1:         # category-level call
                     return results
 
                 voltype = parts[0]
-                if voltype == 'volumes':
+                if voltype == 'volumes' or voltype == 'bundles':
                     return [r + '_md5.txt' for r in results]
                 else:
                     return [r + '_' + voltype + '_md5.txt' for r in results]
 
             # Deal with archive directories
-            if '/holdings/archives-' in abspath:
+            if f'/{cls.PDS_HOLDINGS}/archives-' in abspath:
                 if abspath.endswith('.tar.gz'):
                     return []
 
                 testpath = abspath.replace('/archives-','/')
                 results = cls.os_listdir(testpath)
 
-                after = abspath.rpartition('/holdings/archives-')[-1]
+                after = abspath.rpartition(f'/{cls.PDS_HOLDINGS}/archives-')[-1]
                 parts = after.split('/')
                 if len(parts) == 1:         # category-level call
                     return results
 
                 voltype = parts[0]
                 if voltype == 'volumes':
                     return [r + '.tar.gz' for r in results]
                 else:
                     return [r + '_' + voltype + '.tar.gz' for r in results]
 
             # Deal with other holdings directories, e.g., holdings/volumes
-            if '/holdings/' in abspath:
+            if f'/{cls.PDS_HOLDINGS}/' in abspath:
 
                 # Maybe there's an associated directory in the infoshelf tree
-                shelf_abspath = abspath.replace('/holdings/',
-                                                '/holdings/_infoshelf-')
+                shelf_abspath = abspath.replace(f'/{cls.PDS_HOLDINGS}/',
+                                                f'/{cls.PDS_HOLDINGS}/_infoshelf-')
                 try:
                     results = os.listdir(shelf_abspath)
                 except FileNotFoundError:
                     # If the shelf file is missing, try the actual file system
                     # For documentation, we have all files available but not the shelf
                     # files, therefore we will check the actual file system for documents.
                     childnames = os.listdir(abspath)
                     return [c for c in childnames
                             if c != '.DS_Store' and not c.startswith('._')]
 
                 if not results:
                     return []
 
-                after = abspath.rpartition('/holdings/')[-1]
+                after = abspath.rpartition(f'/{cls.PDS_HOLDINGS}/')[-1]
                 parts = after.split('/')
                 if len(parts) == 1:         # category-level call
                     return results
 
                 # Isolate unique bundle names from shelf files
                 # This prevent duplicated results for _info.py and _info.pickle
                 filtered = []
@@ -1531,17 +1530,17 @@
 
         # Find the shelf file(s) if any
         abspath = abspath.rstrip('/')
         try:
             (pattern, key) = cls.shelf_path_and_key_for_abspath(abspath, 'info')
         except ValueError:
             # For a category-level holdings dir, this might still work
-            if '/holdings/' in abspath:
-                pattern = abspath.replace('/holdings/',
-                                          '/holdings/_infoshelf-')
+            if f'/{cls.PDS_HOLDINGS}/' in abspath:
+                pattern = abspath.replace(f'/{cls.PDS_HOLDINGS}/',
+                                          f'/{cls.PDS_HOLDINGS}/_infoshelf-')
                 key = None  # Below, None indicates that we handled this error
             else:
                 pattern = ''
 
         if not pattern:
             shelf_paths = []
         elif _needs_glob(pattern):
@@ -1554,25 +1553,25 @@
         # If there are no exact infoshelf files, revert to the file system
         if not shelf_paths:
             return _clean_glob(cls, abspath, force_case_sensitive)
 
         # If the check for an exact shelf file failed, just convert the list
         # of shelf/info directories back to holdings directories
         if key is None:
-            return [p.replace('/holdings/_infoshelf-', '/holdings/')
+            return [p.replace(f'/{cls.PDS_HOLDINGS}/_infoshelf-', f'/{cls.PDS_HOLDINGS}/')
                     for p in shelf_paths]
 
         # Gather the matching entries in each shelf
         abspaths = []
         for shelf_path in shelf_paths:
             shelf = cls._get_shelf(shelf_path)
-            parts = shelf_path.split('/holdings/_infoshelf-')
+            parts = shelf_path.split(f'/{cls.PDS_HOLDINGS}/_infoshelf-')
             assert len(parts) == 2
 
-            root_ = parts[0] + '/holdings/' + parts[1].split('_info.')[0] + '/'
+            root_ = parts[0] + f'/{cls.PDS_HOLDINGS}/' + parts[1].split('_info.')[0] + '/'
 
             if _needs_glob(key):
                 # Since shelf files are always in alphabetical order, we can
                 # use a binary search to figure out where to start comparing
                 # strings. This is useful because there can be a lot of
                 # paths to search through, and fnmatchcase is slow.
                 w1 = key.find('?')
@@ -1794,21 +1793,22 @@
 
     @property
     def indexshelf_abspath(self):
         """Return the absolute path to the indexshelf file if this is an index file;
         blank otherwise.
         """
 
+        cls = type(self)
         if self._indexshelf_abspath is None:
             if self.extension not in ('.tab', '.TAB'):
                 self._indexshelf_abspath = ''
             else:
                 abspath = self.abspath
-                abspath = abspath.replace('/holdings/',
-                                          '/holdings/_indexshelf-')
+                abspath = abspath.replace(f'/{cls.PDS_HOLDINGS}/',
+                                          f'/{cls.PDS_HOLDINGS}/_indexshelf-')
                 abspath = abspath.replace('.tab', '.pickle')
                 abspath = abspath.replace('.TAB', '.pickle')
                 self._indexshelf_abspath = abspath
 
             self._recache()
 
         return self._indexshelf_abspath
@@ -3781,17 +3781,18 @@
 
         if parts[0] != '':
             raise ValueError('Not an absolute path: ' + abspath)
 
         # Search for "holdings"
         parts_lc = [p.lower() for p in parts]
         try:
-            PDS_HOLDINGS_index = parts_lc.index(cls.PDS_HOLDINGS) # Change variable name to distinguish from PDS3
+            # Change variable name to distinguish from PDS3
+            PDS_HOLDINGS_index = parts_lc.index(cls.PDS_HOLDINGS)
         except ValueError:
-            raise ValueError('"{}" directory not found in: '.format(cls.PDS_HOLDINGS) + abspath)
+            raise ValueError(f'"{cls.PDS_HOLDINGS}" directory not found in: {abspath}')
         ### Pause the cache
         cls.CACHE.pause()
         try:
             # Fill in this.disk_, the absolute path to the directory containing
             # subdirectory "holdings"
             # this = PdsFile()
             this = cls()
@@ -3882,15 +3883,15 @@
         return this
 
     @classmethod
     def _from_absolute_or_logical_path(cls, path, fix_case=False, must_exist=False,
                                        caching='default', lifetime=None):
         """Return a PdsFile based on either an absolute or a logical path."""
 
-        if '/holdings/' in path:
+        if f'/{cls.PDS_HOLDINGS}/' in path:
             return cls.from_abspath(path,
                                     fix_case=False, must_exist=False,
                                     caching='default', lifetime=None)
         else:
             return cls.from_logical_path(path,
                                          fix_case=False, must_exist=False,
                                          caching='default', lifetime=None)
@@ -3927,15 +3928,15 @@
         path_lc = path.lower()
         try:
             return cls.CACHE[path_lc]
         except KeyError:
             pass
 
         # Strip off a "holdings" directory if found
-        k = path_lc.find('holdings')
+        k = path_lc.find(cls.PDS_HOLDINGS)
         if k >= 0:
             path = path[k:]
             path = path.partition('/')[2]   # remove up to the next slash
 
         # Interpret leading parts
         # this = PdsFile()
         this = cls()
@@ -5043,40 +5044,40 @@
 
         Keyword arguments:
             abspath    -- the absolute path of the file
             shelf_type -- shelf type, e.g., 'info' or 'link' (default 'info')
         """
 
         # No checksum shelf files allowed
-        (root, _, logical_path) = abspath.partition('/holdings/')
+        (root, _, logical_path) = abspath.partition(f'/{cls.PDS_HOLDINGS}/')
         if logical_path.startswith('checksums'):
             raise ValueError('No shelf files for checksums: ' + logical_path)
 
         (dir_prefix, file_suffix) = cls.SHELF_PATH_INFO[shelf_type]
 
         # For archive files, the shelf is associated with the bundleset
         if logical_path.startswith('archives'):
             parts = logical_path.split('/')
             if len(parts) < 2:
                 raise ValueError('Archive shelves require bundle sets: ' +
                                  logical_path)
 
-            shelf_abspath = ''.join([root, '/holdings/', dir_prefix,
+            shelf_abspath = ''.join([root, f'/{cls.PDS_HOLDINGS}/', dir_prefix,
                                      parts[0], '/', parts[1],
                                      file_suffix, '.pickle'])
             key = '/'.join(parts[2:])
 
         # Otherwise, the shelf is associated with the bundle
         else:
             parts = logical_path.split('/')
             if len(parts) < 3:
                 raise ValueError('Non-archive shelves require bundle names: ' +
                                  logical_path)
 
-            shelf_abspath = ''.join([root, '/holdings/', dir_prefix,
+            shelf_abspath = ''.join([root, f'/{cls.PDS_HOLDINGS}/', dir_prefix,
                                      parts[0], '/', parts[1], '/', parts[2],
                                      file_suffix, '.pickle'])
             key = '/'.join(parts[3:])
 
         return (shelf_abspath, key)
 
     @property
@@ -5827,17 +5828,15 @@
             else:
                 suffix = ''
 
             # Find the file(s) that match the pattern
             if not must_exist and not _needs_glob(pattern):
                 test_abspaths = [pattern]
             else:
-                test_abspaths = cls.glob_glob(pattern,
-                                                  force_case_sensitive=True)
-
+                test_abspaths = cls.glob_glob(pattern, force_case_sensitive=True)
             # With a suffix, make sure it matches a row of the index
             if suffix:
                 filtered_abspaths = []
                 for abspath in test_abspaths:
                     try:
                         parent = cls.from_abspath(abspath)
                         pdsf = parent.child_of_index(suffix)
```

### Comparing `rms-pdsfile-0.0.1/pdsfile/pdsviewable.py` & `rms-pdsfile-0.0.2/pdsfile/pdsviewable.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pdsfile/preload_and_cache.py` & `rms-pdsfile-0.0.2/pdsfile/preload_and_cache.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/pyproject.toml` & `rms-pdsfile-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/rms_pdsfile.egg-info/SOURCES.txt` & `rms-pdsfile-0.0.2/rms_pdsfile.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 .coveragerc
 .gitignore
+CODE_OF_CONDUCT.md
+CONTRIBUTING.md
 LICENSE
 README.md
 conftest.py
 pyproject.toml
 requirements.txt
 run_tests_coverage.sh
 setup.cfg
 .github/workflows/publish_to_pypi.yml
 .github/workflows/publish_to_test_pypi.yml
+.github/workflows/run-tests-and-opus.yml
 .github/workflows/run-tests.yml
 pdsfile/__init__.py
 pdsfile/_version.py
 pdsfile/pdscache.py
 pdsfile/pdsfile.py
 pdsfile/pdsviewable.py
 pdsfile/preload_and_cache.py
@@ -52,14 +55,15 @@
 pdsfile/pds3file/tests/test_pdsviewable_blackbox.py
 pdsfile/pds4file/__init__.py
 pdsfile/pds4file/rules/__init__.py
 pdsfile/pds4file/rules/cassini_iss.py
 pdsfile/pds4file/rules/cassini_vims.py
 pdsfile/pds4file/rules/pytest_support.py
 pdsfile/pds4file/rules/uranus_occs_earthbased.py
+pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py
 pdsfile/pds4file/tests/__init__.py
 pdsfile/pds4file/tests/helper.py
 pdsfile/pds4file/tests/test_pds4file_blackbox.py
 rms_pdsfile.egg-info/PKG-INFO
 rms_pdsfile.egg-info/SOURCES.txt
 rms_pdsfile.egg-info/dependency_links.txt
 rms_pdsfile.egg-info/requires.txt
```

### Comparing `rms-pdsfile-0.0.1/scripts/automated_tests/pdsfile_main_test.sh` & `rms-pdsfile-0.0.2/scripts/automated_tests/pdsfile_main_test.sh`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/bin/bash
 
 source ~/pdsfile_runner_secrets
 if [ $? -ne 0 ]; then exit -1; fi
 
-if [[ -z ${PDS_HOLDINGS_DIR+x} ]]; then
-    echo "PDS_HOLDINGS_DIR is not set"
+if [[ -z ${PDS3_HOLDINGS_DIR+x} ]]; then
+    echo "PDS3_HOLDINGS_DIR is not set"
     exit -1
 fi
 if [[ -z ${PDS4_HOLDINGS_DIR+x} ]]; then
-    echo "PDS_HOLDINGS_DIR is not set"
+    echo "PDS4_HOLDINGS_DIR is not set"
     exit -1
 fi
 
 pip3 install --upgrade pip
 pip3 install -r requirements.txt
 echo
 
@@ -37,15 +37,15 @@
 
 echo "================================================================"
 echo "PDSFILE SHELVES-ONLY TESTS"
 echo "================================================================"
 echo
 echo "Test start:" `date`
 echo
-python -m coverage run -a -m pytest pdsfile/pds3file/tests/ pdsfile/pds3file/rules/*.py pdsfile/pds4file/tests/ pdsfile/pds4file/rules/*.py --mode s
+python -m coverage run -a -m pytest pdsfile/pds3file/tests/ pdsfile/pds3file/rules/*.py --mode s
 if [ $? -ne 0 ]; then
     echo "********************************************"
     echo "*** PDSFILE SHELVES-ONLY FAILED UNIT TESTS ***"
     echo "********************************************"
     echo
     echo "Test end:" `date`
     exit -1
```

### Comparing `rms-pdsfile-0.0.1/validation/pdsarchives.py` & `rms-pdsfile-0.0.2/validation/pdsarchives.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/validation/pdschecksums.py` & `rms-pdsfile-0.0.2/validation/pdschecksums.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/validation/pdsdata-sync.sh` & `rms-pdsfile-0.0.2/validation/pdsdata-sync.sh`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/validation/pdsdependency.py` & `rms-pdsfile-0.0.2/validation/pdsdependency.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/validation/pdsindexshelf.py` & `rms-pdsfile-0.0.2/validation/pdsindexshelf.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/validation/pdsinfoshelf.py` & `rms-pdsfile-0.0.2/validation/pdsinfoshelf.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/validation/pdslinkshelf.py` & `rms-pdsfile-0.0.2/validation/pdslinkshelf.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/validation/re-validate.py` & `rms-pdsfile-0.0.2/validation/re-validate.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.1/validation/shelf-consistency-check.py` & `rms-pdsfile-0.0.2/validation/shelf-consistency-check.py`

 * *Files identical despite different names*

