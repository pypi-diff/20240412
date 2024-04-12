# Comparing `tmp/tad_dftd4-0.0.4.tar.gz` & `tmp/tad_dftd4-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tad_dftd4-0.0.4.tar", last modified: Wed May 17 06:56:31 2023, max compression
+gzip compressed data, was "tad_dftd4-0.1.0.tar", last modified: Fri Apr 12 09:24:40 2024, max compression
```

## Comparing `tad_dftd4-0.0.4.tar` & `tad_dftd4-0.1.0.tar`

### file list

```diff
@@ -1,132 +1,39 @@
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.154568 tad_dftd4-0.0.4/
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.142567 tad_dftd4-0.0.4/.github/
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/.github/workflows/
--rw-rw-r--   0 friede    (1000) friede    (1000)     1941 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/.github/workflows/python.yml
--rw-rw-r--   0 friede    (1000) friede    (1000)     1489 2023-05-17 06:54:22.000000 tad_dftd4-0.0.4/.github/workflows/release.yml
--rw-rw-r--   0 friede    (1000) friede    (1000)     3826 2023-03-13 12:39:50.000000 tad_dftd4-0.0.4/.gitignore
--rw-rw-r--   0 friede    (1000) friede    (1000)     1677 2023-05-16 16:49:12.000000 tad_dftd4-0.0.4/.pre-commit-config.yaml
--rw-rw-r--   0 friede    (1000) friede    (1000)    14449 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/.pylintrc
--rw-rw-r--   0 friede    (1000) friede    (1000)       23 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/.readthedocs.yaml
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/.vscode/
--rw-rw-r--   0 friede    (1000) friede    (1000)      688 2023-05-16 16:22:03.000000 tad_dftd4-0.0.4/.vscode/settings.json
--rw-rw-r--   0 friede    (1000) friede    (1000)     4919 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/CONTRIBUTING.md
--rw-rw-r--   0 friede    (1000) friede    (1000)    35149 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/COPYING
--rw-rw-r--   0 friede    (1000) friede    (1000)     7652 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/COPYING.LESSER
--rw-rw-r--   0 friede    (1000) friede    (1000)    10083 2023-05-17 06:56:31.154568 tad_dftd4-0.0.4/PKG-INFO
--rw-rw-r--   0 friede    (1000) friede    (1000)     9203 2023-05-16 16:22:03.000000 tad_dftd4-0.0.4/README.rst
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/doc/
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/doc/_static/
--rw-rw-r--   0 friede    (1000) friede    (1000)     3273 2023-05-16 16:22:03.000000 tad_dftd4-0.0.4/doc/_static/tad-dftd4-favicon.svg
--rw-rw-r--   0 friede    (1000) friede    (1000)     4282 2023-05-16 16:22:03.000000 tad_dftd4-0.0.4/doc/_static/tad-dftd4.svg
--rw-rw-r--   0 friede    (1000) friede    (1000)     1966 2023-03-13 12:40:20.000000 tad_dftd4-0.0.4/doc/conf.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     6408 2023-05-16 16:22:03.000000 tad_dftd4-0.0.4/doc/index.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)     1434 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/installation.rst
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/doc/modules/
--rw-rw-r--   0 friede    (1000) friede    (1000)       47 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/modules/_typing.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       47 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/charges.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       49 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/constants.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       46 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/cutoff.rst
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/doc/modules/damping/
--rw-rw-r--   0 friede    (1000) friede    (1000)       51 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/damping/atm.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       82 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/damping/index.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       56 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/damping/rational.rst
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/doc/modules/data/
--rw-rw-r--   0 friede    (1000) friede    (1000)       47 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/modules/data/en.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       53 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/modules/data/hardness.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)      100 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/data/index.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       49 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/modules/data/r4r2.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       50 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/modules/data/radii.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       49 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/modules/data/zeff.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       48 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/defaults.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       44 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/disp.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)      257 2023-03-13 12:13:06.000000 tad_dftd4-0.0.4/doc/modules/index.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       45 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/model.rst
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.146567 tad_dftd4-0.0.4/doc/modules/ncoord/
--rw-rw-r--   0 friede    (1000) friede    (1000)       52 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/ncoord/count.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       49 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/ncoord/d4.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       50 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/ncoord/eeq.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       83 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/ncoord/index.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       46 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/params.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       45 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/modules/utils.rst
--rw-rw-r--   0 friede    (1000) friede    (1000)       80 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/doc/requirements.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)      846 2023-03-13 12:39:51.000000 tad_dftd4-0.0.4/environment.yaml
--rw-rw-r--   0 friede    (1000) friede    (1000)     1439 2023-03-13 12:39:50.000000 tad_dftd4-0.0.4/pyproject.toml
--rw-rw-r--   0 friede    (1000) friede    (1000)     1108 2023-05-17 06:56:31.154568 tad_dftd4-0.0.4/setup.cfg
--rw-rw-r--   0 friede    (1000) friede    (1000)      816 2023-03-13 12:39:58.000000 tad_dftd4-0.0.4/setup.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.142567 tad_dftd4-0.0.4/src/
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/src/tad_dftd4/
--rw-rw-r--   0 friede    (1000) friede    (1000)     3721 2023-03-13 14:07:11.000000 tad_dftd4-0.0.4/src/tad_dftd4/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)      816 2023-05-17 06:54:22.000000 tad_dftd4-0.0.4/src/tad_dftd4/__version__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     7716 2023-03-13 12:40:23.000000 tad_dftd4-0.0.4/src/tad_dftd4/_typing.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    14333 2023-05-16 16:49:12.000000 tad_dftd4-0.0.4/src/tad_dftd4/charges.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2960 2023-03-13 12:40:22.000000 tad_dftd4-0.0.4/src/tad_dftd4/constants.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2393 2023-03-13 12:40:12.000000 tad_dftd4-0.0.4/src/tad_dftd4/cutoff.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/src/tad_dftd4/damping/
--rw-rw-r--   0 friede    (1000) friede    (1000)      932 2023-03-13 12:40:22.000000 tad_dftd4-0.0.4/src/tad_dftd4/damping/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4384 2023-05-16 16:49:12.000000 tad_dftd4-0.0.4/src/tad_dftd4/damping/atm.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2099 2023-05-16 16:49:12.000000 tad_dftd4-0.0.4/src/tad_dftd4/damping/rational.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/src/tad_dftd4/data/
--rw-rw-r--   0 friede    (1000) friede    (1000)     1045 2023-03-13 12:40:22.000000 tad_dftd4-0.0.4/src/tad_dftd4/data/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2002 2023-03-13 12:40:18.000000 tad_dftd4-0.0.4/src/tad_dftd4/data/en.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3442 2023-03-13 12:40:20.000000 tad_dftd4-0.0.4/src/tad_dftd4/data/hardness.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2611 2023-03-13 12:40:22.000000 tad_dftd4-0.0.4/src/tad_dftd4/data/r4r2.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2132 2023-05-16 16:22:03.000000 tad_dftd4-0.0.4/src/tad_dftd4/data/radii.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1702 2023-03-13 12:40:27.000000 tad_dftd4-0.0.4/src/tad_dftd4/data/zeff.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1594 2023-03-13 11:31:45.000000 tad_dftd4-0.0.4/src/tad_dftd4/defaults.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     9479 2023-05-16 16:49:12.000000 tad_dftd4-0.0.4/src/tad_dftd4/disp.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    11893 2023-05-17 06:54:22.000000 tad_dftd4-0.0.4/src/tad_dftd4/model.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/src/tad_dftd4/ncoord/
--rw-rw-r--   0 friede    (1000) friede    (1000)     3060 2023-03-13 12:40:25.000000 tad_dftd4-0.0.4/src/tad_dftd4/ncoord/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3697 2023-03-13 12:40:22.000000 tad_dftd4-0.0.4/src/tad_dftd4/ncoord/count.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3794 2023-05-16 16:49:12.000000 tad_dftd4-0.0.4/src/tad_dftd4/ncoord/d4.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4019 2023-05-16 16:49:12.000000 tad_dftd4-0.0.4/src/tad_dftd4/ncoord/eeq.py
--rw-rw-r--   0 friede    (1000) friede    (1000)   661085 2023-03-13 12:40:59.000000 tad_dftd4-0.0.4/src/tad_dftd4/params.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4713 2023-03-13 12:40:18.000000 tad_dftd4-0.0.4/src/tad_dftd4/utils.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/src/tad_dftd4.egg-info/
--rw-rw-r--   0 friede    (1000) friede    (1000)    10083 2023-05-17 06:56:31.000000 tad_dftd4-0.0.4/src/tad_dftd4.egg-info/PKG-INFO
--rw-rw-r--   0 friede    (1000) friede    (1000)     2771 2023-05-17 06:56:31.000000 tad_dftd4-0.0.4/src/tad_dftd4.egg-info/SOURCES.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)        1 2023-05-17 06:56:31.000000 tad_dftd4-0.0.4/src/tad_dftd4.egg-info/dependency_links.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)       75 2023-05-17 06:56:31.000000 tad_dftd4-0.0.4/src/tad_dftd4.egg-info/requires.txt
--rw-rw-r--   0 friede    (1000) friede    (1000)       10 2023-05-17 06:56:31.000000 tad_dftd4-0.0.4/src/tad_dftd4.egg-info/top_level.txt
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/test/
--rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:23.000000 tad_dftd4-0.0.4/test/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1812 2023-03-13 12:40:15.000000 tad_dftd4-0.0.4/test/conftest.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    58424 2023-03-13 12:40:37.000000 tad_dftd4-0.0.4/test/molecules.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/test/test_charge/
--rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:26.000000 tad_dftd4-0.0.4/test/test_charge/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4372 2023-03-13 12:40:23.000000 tad_dftd4-0.0.4/test/test_charge/samples.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     5882 2023-03-13 12:40:20.000000 tad_dftd4-0.0.4/test/test_charge/test_charges.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     3169 2023-03-13 12:40:24.000000 tad_dftd4-0.0.4/test/test_charge/test_general.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2097 2023-03-13 12:40:25.000000 tad_dftd4-0.0.4/test/test_charge/test_grad.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.150567 tad_dftd4-0.0.4/test/test_cutoff/
--rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:23.000000 tad_dftd4-0.0.4/test/test_cutoff/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2135 2023-03-13 14:07:11.000000 tad_dftd4-0.0.4/test/test_cutoff/test_general.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2171 2023-03-13 12:40:26.000000 tad_dftd4-0.0.4/test/test_cutoff/test_types.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.154568 tad_dftd4-0.0.4/test/test_disp/
--rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:29.000000 tad_dftd4-0.0.4/test/test_disp/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    29533 2023-03-13 12:40:31.000000 tad_dftd4-0.0.4/test/test_disp/samples.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4347 2023-03-13 12:40:26.000000 tad_dftd4-0.0.4/test/test_disp/test_atm.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4353 2023-03-13 12:40:29.000000 tad_dftd4-0.0.4/test/test_disp/test_full.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1802 2023-03-13 12:40:22.000000 tad_dftd4-0.0.4/test/test_disp/test_general.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2775 2023-03-13 12:40:24.000000 tad_dftd4-0.0.4/test/test_disp/test_grad.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     6524 2023-03-13 12:40:18.000000 tad_dftd4-0.0.4/test/test_disp/test_twobody.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.154568 tad_dftd4-0.0.4/test/test_model/
--rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:26.000000 tad_dftd4-0.0.4/test/test_model/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)    47409 2023-03-13 12:40:32.000000 tad_dftd4-0.0.4/test/test_model/samples.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2716 2023-03-13 12:40:29.000000 tad_dftd4-0.0.4/test/test_model/test_c6.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2023 2023-03-13 12:40:29.000000 tad_dftd4-0.0.4/test/test_model/test_general.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2666 2023-03-13 12:40:24.000000 tad_dftd4-0.0.4/test/test_model/test_model.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     4163 2023-03-13 12:40:24.000000 tad_dftd4-0.0.4/test/test_model/test_weights.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.154568 tad_dftd4-0.0.4/test/test_ncoord/
--rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:23.000000 tad_dftd4-0.0.4/test/test_ncoord/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     5232 2023-03-13 12:40:27.000000 tad_dftd4-0.0.4/test/test_ncoord/samples.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2365 2023-03-13 12:40:26.000000 tad_dftd4-0.0.4/test/test_ncoord/test_cn_d4.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2891 2023-03-13 12:40:25.000000 tad_dftd4-0.0.4/test/test_ncoord/test_cn_eeq.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     2153 2023-03-13 12:40:26.000000 tad_dftd4-0.0.4/test/test_ncoord/test_general.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1770 2023-03-13 12:40:27.000000 tad_dftd4-0.0.4/test/test_ncoord/test_grad.py
-drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2023-05-17 06:56:31.154568 tad_dftd4-0.0.4/test/test_utils/
--rw-rw-r--   0 friede    (1000) friede    (1000)      747 2023-03-13 12:40:30.000000 tad_dftd4-0.0.4/test/test_utils/__init__.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1750 2023-03-13 12:40:30.000000 tad_dftd4-0.0.4/test/test_utils/test_pack.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     5446 2023-03-13 12:40:24.000000 tad_dftd4-0.0.4/test/test_utils/test_real.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1748 2023-03-13 12:40:21.000000 tad_dftd4-0.0.4/test/utils.py
--rw-rw-r--   0 friede    (1000) friede    (1000)     1626 2023-03-13 12:39:50.000000 tad_dftd4-0.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.183323 tad_dftd4-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-12 09:24:40.179323 tad_dftd4-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-12 09:24:40.183323 tad_dftd4-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.171323 tad_dftd4-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.175323 tad_dftd4-0.1.0/src/tad_dftd4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/cutoff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.179323 tad_dftd4-0.1.0/src/tad_dftd4/damping/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/damping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/damping/atm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/damping/rational.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.179323 tad_dftd4-0.1.0/src/tad_dftd4/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/data/hardness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/data/r4r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/data/radii.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/data/zeff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/disp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12836 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.179323 tad_dftd4-0.1.0/src/tad_dftd4/ncoord/
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/ncoord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   795054 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.179323 tad_dftd4-0.1.0/src/tad_dftd4/typing/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/typing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-12 09:24:35.000000 tad_dftd4-0.1.0/src/tad_dftd4/typing/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:24:40.179323 tad_dftd4-0.1.0/src/tad_dftd4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-12 09:24:40.000000 tad_dftd4-0.1.0/src/tad_dftd4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-12 09:24:40.000000 tad_dftd4-0.1.0/src/tad_dftd4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:24:40.000000 tad_dftd4-0.1.0/src/tad_dftd4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-12 09:24:40.000000 tad_dftd4-0.1.0/src/tad_dftd4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 09:24:40.000000 tad_dftd4-0.1.0/src/tad_dftd4.egg-info/top_level.txt
```

### Comparing `tad_dftd4-0.0.4/PKG-INFO` & `tad_dftd4-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,631 +1,689 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7461 645f  : 2.1.Name: tad_
 00000020: 6466 7464 340a 5665 7273 696f 6e3a 2030  dftd4.Version: 0
-00000030: 2e30 2e34 0a53 756d 6d61 7279 3a20 546f  .0.4.Summary: To
+00000030: 2e31 2e30 0a53 756d 6d61 7279 3a20 546f  .1.0.Summary: To
 00000040: 7263 6820 6175 746f 6469 6666 2044 4654  rch autodiff DFT
 00000050: 2d44 3420 696d 706c 656d 656e 7461 7469  -D4 implementati
 00000060: 6f6e 0a41 7574 686f 723a 2022 4d61 7276  on.Author: "Marv
 00000070: 696e 2046 7269 6564 6522 0a4c 6963 656e  in Friede".Licen
-00000080: 7365 3a20 4c47 504c 2d33 2e30 0a43 6c61  se: LGPL-3.0.Cla
-00000090: 7373 6966 6965 723a 2046 7261 6d65 776f  ssifier: Framewo
-000000a0: 726b 203a 3a20 5079 7465 7374 0a43 6c61  rk :: Pytest.Cla
-000000b0: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
-000000c0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000000d0: 203a 3a20 474e 5520 4c65 7373 6572 2047   :: GNU Lesser G
-000000e0: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
-000000f0: 6365 6e73 6520 7633 2028 4c47 504c 7633  cense v3 (LGPLv3
-00000100: 290a 436c 6173 7369 6669 6572 3a20 4e61  ).Classifier: Na
-00000110: 7475 7261 6c20 4c61 6e67 7561 6765 203a  tural Language :
-00000120: 3a20 456e 676c 6973 680a 436c 6173 7369  : English.Classi
-00000130: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000140: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000150: 7468 6f6e 203a 3a20 330a 436c 6173 7369  thon :: 3.Classi
-00000160: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000170: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000180: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
-00000190: 790a 436c 6173 7369 6669 6572 3a20 5072  y.Classifier: Pr
-000001a0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001b0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001c0: 332e 380a 436c 6173 7369 6669 6572 3a20  3.8.Classifier: 
-000001d0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001e0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001f0: 3a20 332e 390a 436c 6173 7369 6669 6572  : 3.9.Classifier
-00000200: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000210: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000220: 203a 3a20 332e 3130 0a43 6c61 7373 6966   :: 3.10.Classif
-00000230: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000240: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000250: 686f 6e20 3a3a 2033 2e31 310a 436c 6173  hon :: 3.11.Clas
-00000260: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000270: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000280: 5079 7468 6f6e 203a 3a20 496d 706c 656d  Python :: Implem
-00000290: 656e 7461 7469 6f6e 203a 3a20 4350 7974  entation :: CPyt
-000002a0: 686f 6e0a 436c 6173 7369 6669 6572 3a20  hon.Classifier: 
-000002b0: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
-000002c0: 6669 632f 456e 6769 6e65 6572 696e 670a  fic/Engineering.
-000002d0: 436c 6173 7369 6669 6572 3a20 5479 7069  Classifier: Typi
-000002e0: 6e67 203a 3a20 5479 7065 640a 5265 7175  ng :: Typed.Requ
-000002f0: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
-00000300: 2e38 0a44 6573 6372 6970 7469 6f6e 2d43  .8.Description-C
-00000310: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-00000320: 742f 782d 7273 740a 5072 6f76 6964 6573  t/x-rst.Provides
-00000330: 2d45 7874 7261 3a20 6465 760a 4c69 6365  -Extra: dev.Lice
-00000340: 6e73 652d 4669 6c65 3a20 434f 5059 494e  nse-File: COPYIN
-00000350: 470a 4c69 6365 6e73 652d 4669 6c65 3a20  G.License-File: 
-00000360: 434f 5059 494e 472e 4c45 5353 4552 0a0a  COPYING.LESSER..
-00000370: 546f 7263 6820 6175 746f 6469 6666 2066  Torch autodiff f
-00000380: 6f72 2044 4654 2d44 340a 3d3d 3d3d 3d3d  or DFT-D4.======
-00000390: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000003a0: 3d3d 3d0a 0a2e 2e20 696d 6167 653a 3a20  ===.... image:: 
-000003b0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000003c0: 6c64 732e 696f 2f62 6164 6765 2f70 7974  lds.io/badge/pyt
-000003d0: 686f 6e2d 2533 453d 332e 382d 626c 7565  hon-%3E=3.8-blue
-000003e0: 2e73 7667 0a20 2020 203a 7461 7267 6574  .svg.    :target
-000003f0: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00000400: 6965 6c64 732e 696f 2f62 6164 6765 2f70  ields.io/badge/p
-00000410: 7974 686f 6e2d 332e 3825 3230 7c25 3230  ython-3.8%20|%20
-00000420: 332e 3925 3230 7c25 3230 332e 3130 2532  3.9%20|%203.10%2
-00000430: 307c 2532 3033 2e31 312d 626c 7565 2e73  0|%203.11-blue.s
-00000440: 7667 0a20 2020 203a 616c 743a 2050 7974  vg.    :alt: Pyt
-00000450: 686f 6e20 5665 7273 696f 6e73 0a0a 2e2e  hon Versions....
-00000460: 2069 6d61 6765 3a3a 2068 7474 7073 3a2f   image:: https:/
-00000470: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000480: 6769 7468 7562 2f76 2f72 656c 6561 7365  github/v/release
-00000490: 2f64 6674 6434 2f74 6164 2d64 6674 6434  /dftd4/tad-dftd4
-000004a0: 0a20 2020 203a 7461 7267 6574 3a20 6874  .    :target: ht
-000004b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000004c0: 2f64 6674 6434 2f74 6164 2d64 6674 6434  /dftd4/tad-dftd4
-000004d0: 2f72 656c 6561 7365 732f 6c61 7465 7374  /releases/latest
-000004e0: 0a20 2020 203a 616c 743a 2052 656c 6561  .    :alt: Relea
-000004f0: 7365 0a0a 2e2e 2069 6d61 6765 3a3a 2068  se.... image:: h
-00000500: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000510: 6473 2e69 6f2f 7079 7069 2f76 2f74 6164  ds.io/pypi/v/tad
-00000520: 2d64 6674 6434 0a20 2020 203a 7461 7267  -dftd4.    :targ
-00000530: 6574 3a20 6874 7470 733a 2f2f 7079 7069  et: https://pypi
-00000540: 2e6f 7267 2f70 726f 6a65 6374 2f74 6164  .org/project/tad
-00000550: 2d64 6674 6434 2f0a 2020 2020 3a61 6c74  -dftd4/.    :alt
-00000560: 3a20 5079 5049 0a0a 2e2e 2069 6d61 6765  : PyPI.... image
-00000570: 3a3a 2068 7474 7073 3a2f 2f69 6d67 2e73  :: https://img.s
-00000580: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000590: 4c69 6365 6e73 652d 4c47 504c 5f76 332d  License-LGPL_v3-
-000005a0: 626c 7565 2e73 7667 0a20 2020 203a 7461  blue.svg.    :ta
-000005b0: 7267 6574 3a20 6874 7470 733a 2f2f 7777  rget: https://ww
-000005c0: 772e 676e 752e 6f72 672f 6c69 6365 6e73  w.gnu.org/licens
-000005d0: 6573 2f6c 6770 6c2d 332e 300a 2020 2020  es/lgpl-3.0.    
-000005e0: 3a61 6c74 3a20 4c47 504c 2d33 2e30 0a0a  :alt: LGPL-3.0..
-000005f0: 2e2e 2069 6d61 6765 3a3a 2068 7474 7073  .. image:: https
-00000600: 3a2f 2f67 6974 6875 622e 636f 6d2f 6466  ://github.com/df
-00000610: 7464 342f 6466 7464 342f 776f 726b 666c  td4/dftd4/workfl
-00000620: 6f77 732f 4349 2f62 6164 6765 2e73 7667  ows/CI/badge.svg
-00000630: 0a20 2020 203a 7461 7267 6574 3a20 6874  .    :target: ht
-00000640: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000650: 2f64 6674 6434 2f64 6674 6434 2f61 6374  /dftd4/dftd4/act
-00000660: 696f 6e73 0a20 2020 203a 616c 743a 2043  ions.    :alt: C
-00000670: 490a 0a2e 2e20 696d 6167 653a 3a20 6874  I.... image:: ht
-00000680: 7470 733a 2f2f 7265 6164 7468 6564 6f63  tps://readthedoc
-00000690: 732e 6f72 672f 7072 6f6a 6563 7473 2f74  s.org/projects/t
-000006a0: 6164 2d64 6674 6434 2f62 6164 6765 2f3f  ad-dftd4/badge/?
-000006b0: 7665 7273 696f 6e3d 6c61 7465 7374 0a20  version=latest. 
-000006c0: 2020 203a 7461 7267 6574 3a20 6874 7470     :target: http
-000006d0: 733a 2f2f 7461 642d 6466 7464 342e 7265  s://tad-dftd4.re
-000006e0: 6164 7468 6564 6f63 732e 696f 0a20 2020  adthedocs.io.   
-000006f0: 203a 616c 743a 2044 6f63 756d 656e 7461   :alt: Documenta
-00000700: 7469 6f6e 2053 7461 7475 730a 0a2e 2e20  tion Status.... 
-00000710: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
-00000720: 636f 6465 636f 762e 696f 2f67 682f 6466  codecov.io/gh/df
-00000730: 7464 342f 7461 642d 6466 7464 342f 6272  td4/tad-dftd4/br
-00000740: 616e 6368 2f6d 6169 6e2f 6772 6170 682f  anch/main/graph/
-00000750: 6261 6467 652e 7376 673f 746f 6b65 6e3d  badge.svg?token=
-00000760: 4f47 4a4a 6e5a 3674 3447 0a20 2020 203a  OGJJnZ6t4G.    :
-00000770: 7461 7267 6574 3a20 6874 7470 733a 2f2f  target: https://
-00000780: 636f 6465 636f 762e 696f 2f67 682f 6466  codecov.io/gh/df
-00000790: 7464 342f 7461 642d 6466 7464 340a 2020  td4/tad-dftd4.  
-000007a0: 2020 3a61 6c74 3a20 436f 7665 7261 6765    :alt: Coverage
-000007b0: 0a0a 2e2e 2069 6d61 6765 3a3a 2068 7474  .... image:: htt
-000007c0: 7073 3a2f 2f72 6573 756c 7473 2e70 7265  ps://results.pre
-000007d0: 2d63 6f6d 6d69 742e 6369 2f62 6164 6765  -commit.ci/badge
-000007e0: 2f67 6974 6875 622f 6466 7464 342f 7461  /github/dftd4/ta
-000007f0: 642d 6466 7464 342f 6d61 696e 2e73 7667  d-dftd4/main.svg
-00000800: 0a20 2020 203a 7461 7267 6574 3a20 6874  .    :target: ht
-00000810: 7470 733a 2f2f 7265 7375 6c74 732e 7072  tps://results.pr
-00000820: 652d 636f 6d6d 6974 2e63 692f 6c61 7465  e-commit.ci/late
-00000830: 7374 2f67 6974 6875 622f 6466 7464 342f  st/github/dftd4/
-00000840: 7461 642d 6466 7464 342f 6d61 696e 0a20  tad-dftd4/main. 
-00000850: 2020 203a 616c 743a 2070 7265 2d63 6f6d     :alt: pre-com
-00000860: 6d69 742e 6369 2073 7461 7475 730a 0a49  mit.ci status..I
-00000870: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
-00000880: 2074 6865 2044 4654 2d44 3420 6469 7370   the DFT-D4 disp
-00000890: 6572 7369 6f6e 206d 6f64 656c 2069 6e20  ersion model in 
-000008a0: 5079 546f 7263 682e 0a54 6869 7320 6d6f  PyTorch..This mo
-000008b0: 6475 6c65 2061 6c6c 6f77 7320 746f 2070  dule allows to p
-000008c0: 726f 6365 7373 2061 2073 696e 676c 6520  rocess a single 
-000008d0: 7374 7275 6374 7572 6520 6f72 2061 2062  structure or a b
-000008e0: 6174 6368 206f 6620 7374 7275 6374 7572  atch of structur
-000008f0: 6573 2066 6f72 2074 6865 2063 616c 6375  es for the calcu
-00000900: 6c61 7469 6f6e 206f 6620 6174 6f6d 2d72  lation of atom-r
-00000910: 6573 6f6c 7665 6420 6469 7370 6572 7369  esolved dispersi
-00000920: 6f6e 2065 6e65 7267 6965 732e 0a0a 466f  on energies...Fo
-00000930: 7220 6465 7461 696c 7320 6f6e 2074 6865  r details on the
-00000940: 2044 3420 6469 7370 6572 7369 6f6e 206d   D4 dispersion m
-00000950: 6f64 656c 2c20 7365 650a 0a2d 205c 452e  odel, see..- \E.
-00000960: 2043 616c 6465 7765 7968 6572 2c20 432e   Caldeweyher, C.
-00000970: 2042 616e 6e77 6172 7468 2061 6e64 2053   Bannwarth and S
-00000980: 2e20 4772 696d 6d65 2c20 2a4a 2e20 4368  . Grimme, *J. Ch
-00000990: 656d 2e20 5068 7973 2e2a 2c20 2a2a 3230  em. Phys.*, **20
-000009a0: 3137 2a2a 2c20 2a31 3437 2a2c 2030 3334  17**, *147*, 034
-000009b0: 3131 322e 2044 4f49 3a20 6031 302e 3130  112. DOI: `10.10
-000009c0: 3633 2f31 2e34 3939 3332 3135 203c 6874  63/1.4993215 <ht
-000009d0: 7470 733a 2f2f 6478 2e64 6f69 2e6f 7267  tps://dx.doi.org
-000009e0: 2f31 302e 3130 3633 2f31 2e34 3939 3332  /10.1063/1.49932
-000009f0: 3135 3e60 5f5f 0a0a 2d20 5c45 2e20 4361  15>`__..- \E. Ca
-00000a00: 6c64 6577 6579 6865 722c 2053 2e20 4568  ldeweyher, S. Eh
-00000a10: 6c65 7274 2c20 412e 2048 616e 7365 6e2c  lert, A. Hansen,
-00000a20: 2048 2e20 4e65 7567 6562 6175 6572 2c20   H. Neugebauer, 
-00000a30: 532e 2053 7069 6368 6572 2c20 432e 2042  S. Spicher, C. B
-00000a40: 616e 6e77 6172 7468 2061 6e64 2053 2e20  annwarth and S. 
-00000a50: 4772 696d 6d65 2c20 2a4a 2e20 4368 656d  Grimme, *J. Chem
-00000a60: 2e20 5068 7973 2e2a 2c20 2a2a 3230 3139  . Phys.*, **2019
-00000a70: 2a2a 2c20 2a31 3530 2a2c 2031 3534 3132  **, *150*, 15412
-00000a80: 322e 2044 4f49 3a20 6031 302e 3130 3633  2. DOI: `10.1063
-00000a90: 2f31 2e35 3039 3032 3232 203c 6874 7470  /1.5090222 <http
-00000aa0: 733a 2f2f 6478 2e64 6f69 2e6f 7267 2f31  s://dx.doi.org/1
-00000ab0: 302e 3130 3633 2f31 2e35 3039 3032 3232  0.1063/1.5090222
-00000ac0: 3e60 5f5f 0a0a 2d20 5c45 2e20 4361 6c64  >`__..- \E. Cald
-00000ad0: 6577 6579 6865 722c 204a 2e2d 4d2e 204d  eweyher, J.-M. M
-00000ae0: 6577 6573 2c20 532e 2045 686c 6572 7420  ewes, S. Ehlert 
-00000af0: 616e 6420 532e 2047 7269 6d6d 652c 202a  and S. Grimme, *
-00000b00: 5068 7973 2e20 4368 656d 2e20 4368 656d  Phys. Chem. Chem
-00000b10: 2e20 5068 7973 2e2a 2c20 2a2a 3230 3230  . Phys.*, **2020
-00000b20: 2a2a 2c20 2a32 322a 2c20 3834 3939 2d38  **, *22*, 8499-8
-00000b30: 3531 322e 2044 4f49 3a20 6031 302e 3130  512. DOI: `10.10
-00000b40: 3339 2f44 3043 5030 3035 3032 4120 3c68  39/D0CP00502A <h
-00000b50: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-00000b60: 302e 3130 3339 2f44 3043 5030 3035 3032  0.1039/D0CP00502
-00000b70: 413e 605f 5f0a 0a46 6f72 2061 6c74 6572  A>`__..For alter
-00000b80: 6e61 7469 7665 2069 6d70 6c65 6d65 6e74  native implement
-00000b90: 6174 696f 6e73 2c20 616c 736f 2063 6865  ations, also che
-00000ba0: 636b 206f 7574 0a0a 6064 6674 6434 203c  ck out..`dftd4 <
-00000bb0: 6874 7470 733a 2f2f 6466 7464 342e 7265  https://dftd4.re
-00000bc0: 6164 7468 6564 6f63 732e 696f 3e60 5f5f  adthedocs.io>`__
-00000bd0: 3a0a 2020 496d 706c 656d 656e 7461 7469  :.  Implementati
-00000be0: 6f6e 206f 6620 7468 6520 4446 542d 4434  on of the DFT-D4
-00000bf0: 2064 6973 7065 7273 696f 6e20 6d6f 6465   dispersion mode
-00000c00: 6c20 696e 2046 6f72 7472 616e 2077 6974  l in Fortran wit
-00000c10: 6820 5079 7468 6f6e 2062 696e 6469 6e67  h Python binding
-00000c20: 732e 0a0a 6063 7070 2d64 3420 3c68 7474  s...`cpp-d4 <htt
-00000c30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000c40: 6466 7464 342f 6370 702d 6434 3e60 5f5f  dftd4/cpp-d4>`__
-00000c50: 3a0a 2020 496d 706c 656d 656e 7461 7469  :.  Implementati
-00000c60: 6f6e 206f 6620 7468 6520 4446 542d 4434  on of the DFT-D4
-00000c70: 2064 6973 7065 7273 696f 6e20 6d6f 6465   dispersion mode
-00000c80: 6c20 696e 2043 2b2b 2e0a 0a49 6e73 7461  l in C++...Insta
-00000c90: 6c6c 6174 696f 6e0a 2d2d 2d2d 2d2d 2d2d  llation.--------
-00000ca0: 2d2d 2d2d 0a0a 7069 700a 7e7e 7e0a 0a2a  ----..pip.~~~..*
-00000cb0: 7461 642d 6466 7464 342a 2063 616e 2065  tad-dftd4* can e
-00000cc0: 6173 696c 7920 6265 2069 6e73 7461 6c6c  asily be install
-00000cd0: 6564 2077 6974 6820 6060 7069 7060 602e  ed with ``pip``.
-00000ce0: 0a0a 2e2e 2063 6f64 653a 3a0a 0a20 2020  .... code::..   
-00000cf0: 2070 6970 2069 6e73 7461 6c6c 2074 6164   pip install tad
-00000d00: 2d64 6674 6434 0a0a 0a46 726f 6d20 736f  -dftd4...From so
-00000d10: 7572 6365 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  urce.~~~~~~~~~~~
-00000d20: 0a0a 5468 6973 2070 726f 6a65 6374 2069  ..This project i
-00000d30: 7320 686f 7374 6564 206f 6e20 4769 7448  s hosted on GitH
-00000d40: 7562 2061 7420 6064 6674 6434 2f74 6164  ub at `dftd4/tad
-00000d50: 2d64 6674 6434 203c 6874 7470 733a 2f2f  -dftd4 <https://
-00000d60: 6769 7468 7562 2e63 6f6d 2f64 6674 6434  github.com/dftd4
-00000d70: 2f74 6164 2d64 6674 6434 3e60 5f5f 2e0a  /tad-dftd4>`__..
-00000d80: 4f62 7461 696e 2074 6865 2073 6f75 7263  Obtain the sourc
-00000d90: 6520 6279 2063 6c6f 6e69 6e67 2074 6865  e by cloning the
-00000da0: 2072 6570 6f73 6974 6f72 7920 7769 7468   repository with
-00000db0: 0a0a 2e2e 2063 6f64 653a 3a0a 0a20 2020  .... code::..   
-00000dc0: 2067 6974 2063 6c6f 6e65 2068 7474 7073   git clone https
-00000dd0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6466  ://github.com/df
-00000de0: 7464 342f 7461 642d 6466 7464 340a 2020  td4/tad-dftd4.  
-00000df0: 2020 6364 2074 6164 2d64 6674 6434 0a0a    cd tad-dftd4..
-00000e00: 5765 2072 6563 6f6d 6d65 6e64 2075 7369  We recommend usi
-00000e10: 6e67 2061 2060 636f 6e64 6120 3c68 7474  ng a `conda <htt
-00000e20: 7073 3a2f 2f63 6f6e 6461 2e69 6f2f 3e60  ps://conda.io/>`
-00000e30: 5f5f 2065 6e76 6972 6f6e 6d65 6e74 2074  __ environment t
-00000e40: 6f20 696e 7374 616c 6c20 7468 6520 7061  o install the pa
-00000e50: 636b 6167 652e 0a59 6f75 2063 616e 2073  ckage..You can s
-00000e60: 6574 7570 2074 6865 2065 6e76 6972 6f6e  etup the environ
-00000e70: 6d65 6e74 206d 616e 6167 6572 2075 7369  ment manager usi
-00000e80: 6e67 2061 2060 6d61 6d62 6166 6f72 6765  ng a `mambaforge
-00000e90: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-00000ea0: 2e63 6f6d 2f63 6f6e 6461 2d66 6f72 6765  .com/conda-forge
-00000eb0: 2f6d 696e 6966 6f72 6765 3e60 5f5f 2069  /miniforge>`__ i
-00000ec0: 6e73 7461 6c6c 6572 2e0a 496e 7374 616c  nstaller..Instal
-00000ed0: 6c20 7468 6520 7265 7175 6972 6564 2064  l the required d
-00000ee0: 6570 656e 6465 6e63 6965 7320 6672 6f6d  ependencies from
-00000ef0: 2074 6865 2063 6f6e 6461 2d66 6f72 6765   the conda-forge
-00000f00: 2063 6861 6e6e 656c 2e0a 0a2e 2e20 636f   channel..... co
-00000f10: 6465 3a3a 0a0a 2020 2020 6d61 6d62 6120  de::..    mamba 
-00000f20: 656e 7620 6372 6561 7465 202d 6e20 746f  env create -n to
-00000f30: 7263 6820 2d66 2065 6e76 6972 6f6e 6d65  rch -f environme
-00000f40: 6e74 2e79 616d 6c0a 2020 2020 6d61 6d62  nt.yaml.    mamb
-00000f50: 6120 6163 7469 7661 7465 2074 6f72 6368  a activate torch
-00000f60: 0a0a 496e 7374 616c 6c20 7468 6973 2070  ..Install this p
-00000f70: 726f 6a65 6374 2077 6974 6820 6060 7069  roject with ``pi
-00000f80: 7060 6020 696e 2074 6865 2065 6e76 6972  p`` in the envir
-00000f90: 6f6e 6d65 6e74 0a0a 2e2e 2063 6f64 653a  onment.... code:
-00000fa0: 3a0a 0a20 2020 2070 6970 2069 6e73 7461  :..    pip insta
-00000fb0: 6c6c 202e 0a0a 5468 6520 666f 6c6c 6f77  ll ...The follow
-00000fc0: 696e 6720 6465 7065 6e64 656e 6369 6573  ing dependencies
-00000fd0: 2061 7265 2072 6571 7569 7265 640a 0a2d   are required..-
-00000fe0: 2060 6e75 6d70 7920 3c68 7474 7073 3a2f   `numpy <https:/
-00000ff0: 2f6e 756d 7079 2e6f 7267 2f3e 605f 5f0a  /numpy.org/>`__.
-00001000: 2d20 6074 6f72 6368 203c 6874 7470 733a  - `torch <https:
-00001010: 2f2f 7079 746f 7263 682e 6f72 672f 3e60  //pytorch.org/>`
-00001020: 5f5f 0a2d 2060 7079 7465 7374 203c 6874  __.- `pytest <ht
-00001030: 7470 733a 2f2f 646f 6373 2e70 7974 6573  tps://docs.pytes
-00001040: 742e 6f72 672f 3e60 5f5f 2028 7465 7374  t.org/>`__ (test
-00001050: 7320 6f6e 6c79 290a 0a44 6576 656c 6f70  s only)..Develop
-00001060: 6d65 6e74 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ment.-----------
-00001070: 0a0a 466f 7220 6465 7665 6c6f 706d 656e  ..For developmen
-00001080: 742c 2061 6464 6974 696f 6e61 6c6c 7920  t, additionally 
-00001090: 696e 7374 616c 6c20 7468 6520 666f 6c6c  install the foll
-000010a0: 6f77 696e 6720 746f 6f6c 7320 696e 2079  owing tools in y
-000010b0: 6f75 7220 656e 7669 726f 6e6d 656e 742e  our environment.
-000010c0: 0a0a 2e2e 2063 6f64 653a 3a0a 0a20 2020  .... code::..   
-000010d0: 206d 616d 6261 2069 6e73 7461 6c6c 2062   mamba install b
-000010e0: 6c61 636b 2063 6f76 6465 6661 756c 7473  lack covdefaults
-000010f0: 2063 6f76 6572 6167 6520 6d79 7079 2070   coverage mypy p
-00001100: 7265 2d63 6f6d 6d69 7420 7079 6c69 6e74  re-commit pylint
-00001110: 2074 6f78 0a0a 5769 7468 2070 6970 2c20   tox..With pip, 
-00001120: 6164 6420 7468 6520 6f70 7469 6f6e 2060  add the option `
-00001130: 602d 6560 6020 666f 7220 696e 7374 616c  `-e`` for instal
-00001140: 6c69 6e67 2069 6e20 6465 7665 6c6f 706d  ling in developm
-00001150: 656e 7420 6d6f 6465 2c20 616e 6420 6164  ent mode, and ad
-00001160: 6420 6060 5b64 6576 5d60 6020 666f 7220  d ``[dev]`` for 
-00001170: 7468 6520 6465 7665 6c6f 706d 656e 7420  the development 
-00001180: 6465 7065 6e64 656e 6369 6573 0a0a 2e2e  dependencies....
-00001190: 2063 6f64 653a 3a0a 0a20 2020 2070 6970   code::..    pip
-000011a0: 2069 6e73 7461 6c6c 202d 6520 2e5b 6465   install -e .[de
-000011b0: 765d 0a0a 5468 6520 7072 652d 636f 6d6d  v]..The pre-comm
-000011c0: 6974 2068 6f6f 6b73 2061 7265 2069 6e69  it hooks are ini
-000011d0: 7469 616c 697a 6564 2062 7920 7275 6e6e  tialized by runn
-000011e0: 696e 6720 7468 6520 666f 6c6c 6f77 696e  ing the followin
-000011f0: 6720 636f 6d6d 616e 6420 696e 2074 6865  g command in the
-00001200: 2072 6f6f 7420 6f66 2074 6865 2072 6570   root of the rep
-00001210: 6f73 6974 6f72 792e 0a0a 2e2e 2063 6f64  ository..... cod
-00001220: 653a 3a0a 0a20 2020 2070 7265 2d63 6f6d  e::..    pre-com
-00001230: 6d69 7420 696e 7374 616c 6c0a 0a46 6f72  mit install..For
-00001240: 2074 6573 7469 6e67 2061 6c6c 2050 7974   testing all Pyt
-00001250: 686f 6e20 656e 7669 726f 6e6d 656e 7473  hon environments
-00001260: 2c20 7369 6d70 6c79 2072 756e 2060 746f  , simply run `to
-00001270: 7860 2e0a 0a2e 2e20 636f 6465 3a3a 0a0a  x`..... code::..
-00001280: 2020 2020 746f 780a 0a4e 6f74 6520 7468      tox..Note th
-00001290: 6174 2074 6869 7320 7261 6e64 6f6d 697a  at this randomiz
-000012a0: 6573 2074 6865 206f 7264 6572 206f 6620  es the order of 
-000012b0: 7465 7374 7320 6275 7420 736b 6970 7320  tests but skips 
-000012c0: 226c 6172 6765 2220 7465 7374 732e 2054  "large" tests. T
-000012d0: 6f20 6d6f 6469 6679 2074 6869 7320 6265  o modify this be
-000012e0: 6861 7669 6f72 2c20 6074 6f78 6020 6861  havior, `tox` ha
-000012f0: 7320 746f 2073 6b69 7020 7468 6520 6f70  s to skip the op
-00001300: 7469 6f6e 616c 202a 706f 7361 7267 732a  tional *posargs*
-00001310: 2e0a 0a2e 2e20 636f 6465 3a3a 0a0a 2020  ..... code::..  
-00001320: 2020 746f 7820 2d2d 2074 6573 740a 0a45    tox -- test..E
-00001330: 7861 6d70 6c65 730a 2d2d 2d2d 2d2d 2d2d  xamples.--------
-00001340: 0a0a 5468 6520 666f 6c6c 6f77 696e 6720  ..The following 
-00001350: 6578 616d 706c 6520 7368 6f77 7320 686f  example shows ho
-00001360: 7720 746f 2063 616c 6375 6c61 7465 2074  w to calculate t
-00001370: 6865 2044 4654 2d44 3420 6469 7370 6572  he DFT-D4 disper
-00001380: 7369 6f6e 2065 6e65 7267 7920 666f 7220  sion energy for 
-00001390: 6120 7369 6e67 6c65 2073 7472 7563 7475  a single structu
-000013a0: 7265 2e0a 0a2e 2e20 636f 6465 3a3a 2070  re..... code:: p
-000013b0: 7974 686f 6e0a 0a20 2020 2069 6d70 6f72  ython..    impor
-000013c0: 7420 746f 7263 680a 2020 2020 696d 706f  t torch.    impo
-000013d0: 7274 2074 6164 5f64 6674 6434 2061 7320  rt tad_dftd4 as 
-000013e0: 6434 0a0a 2020 2020 6e75 6d62 6572 7320  d4..    numbers 
-000013f0: 3d20 6434 2e75 7469 6c73 2e74 6f5f 6e75  = d4.utils.to_nu
-00001400: 6d62 6572 2873 796d 626f 6c73 3d22 4320  mber(symbols="C 
-00001410: 4320 4320 4320 4e20 4320 5320 4820 4820  C C C N C S H H 
-00001420: 4820 4820 4822 2e73 706c 6974 2829 290a  H H H".split()).
-00001430: 0a20 2020 2023 2063 6f6f 7264 696e 6174  .    # coordinat
-00001440: 6573 2069 6e20 426f 6872 0a20 2020 2070  es in Bohr.    p
-00001450: 6f73 6974 696f 6e73 203d 2074 6f72 6368  ositions = torch
-00001460: 2e74 656e 736f 7228 0a20 2020 2020 2020  .tensor(.       
-00001470: 205b 0a20 2020 2020 2020 2020 2020 205b   [.            [
-00001480: 2d32 2e35 3637 3435 3638 3535 3634 3637  -2.5674568556467
-00001490: 312c 202d 302e 3032 3530 3939 3835 3937  1, -0.0250998597
-000014a0: 3939 3130 2c20 302e 3030 3030 3030 3030  9910, 0.00000000
-000014b0: 3030 3030 3030 5d2c 0a20 2020 2020 2020  000000],.       
-000014c0: 2020 2020 205b 2d31 2e33 3931 3737 3538       [-1.3917758
-000014d0: 3234 3535 3739 372c 202b 322e 3237 3639  2455797, +2.2769
-000014e0: 3631 3838 3838 3030 3134 2c20 302e 3030  6188880014, 0.00
-000014f0: 3030 3030 3030 3030 3030 3030 5d2c 0a20  000000000000],. 
-00001500: 2020 2020 2020 2020 2020 205b 2b31 2e32             [+1.2
-00001510: 3737 3834 3939 3536 3234 3839 342c 202b  7784995624894, +
-00001520: 322e 3435 3130 3734 3739 3735 3933 3836  2.45107479759386
-00001530: 2c20 302e 3030 3030 3030 3030 3030 3030  , 0.000000000000
-00001540: 3030 5d2c 0a20 2020 2020 2020 2020 2020  00],.           
-00001550: 205b 2b32 2e36 3238 3031 3933 3736 3135   [+2.62801937615
-00001560: 3739 332c 202b 302e 3235 3932 3737 3237  793, +0.25927727
-00001570: 3032 3831 3230 2c20 302e 3030 3030 3030  028120, 0.000000
-00001580: 3030 3030 3030 3030 5d2c 0a20 2020 2020  00000000],.     
-00001590: 2020 2020 2020 205b 2b31 2e34 3130 3937         [+1.41097
-000015a0: 3033 3336 3631 3132 332c 202d 312e 3939  033661123, -1.99
-000015b0: 3839 3039 3936 3037 3734 3132 2c20 302e  890996077412, 0.
-000015c0: 3030 3030 3030 3030 3030 3030 3030 5d2c  00000000000000],
-000015d0: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
-000015e0: 2e31 3731 3836 3130 3232 3938 3834 392c  .17186102298849,
-000015f0: 202d 322e 3334 3232 3035 3736 3238 3431   -2.342205762841
-00001600: 3830 2c20 302e 3030 3030 3030 3030 3030  80, 0.0000000000
-00001610: 3030 3030 5d2c 0a20 2020 2020 2020 2020  0000],.         
-00001620: 2020 205b 2d32 2e33 3935 3035 3939 3033     [-2.395059903
-00001630: 3638 3337 382c 202d 352e 3232 3633 3538  68378, -5.226358
-00001640: 3338 3333 3233 3632 2c20 302e 3030 3030  38332362, 0.0000
-00001650: 3030 3030 3030 3030 3030 5d2c 0a20 2020  0000000000],.   
-00001660: 2020 2020 2020 2020 205b 2b32 2e34 3139           [+2.419
-00001670: 3631 3938 3034 3535 3435 372c 202d 332e  61980455457, -3.
-00001680: 3632 3135 3830 3139 3235 3330 3435 2c20  62158019253045, 
-00001690: 302e 3030 3030 3030 3030 3030 3030 3030  0.00000000000000
-000016a0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-000016b0: 2d32 2e35 3137 3434 3337 3438 3436 3036  -2.5174437484606
-000016c0: 352c 202b 332e 3938 3138 3137 3133 3638  5, +3.9818171368
-000016d0: 3637 3436 2c20 302e 3030 3030 3030 3030  6746, 0.00000000
-000016e0: 3030 3030 3030 5d2c 0a20 2020 2020 2020  000000],.       
-000016f0: 2020 2020 205b 2b32 2e32 3432 3639 3034       [+2.2426904
-00001700: 3833 3834 3737 352c 202b 342e 3234 3338  8384775, +4.2438
-00001710: 3934 3733 3230 3336 3437 2c20 302e 3030  9473203647, 0.00
-00001720: 3030 3030 3030 3030 3030 3030 5d2c 0a20  000000000000],. 
-00001730: 2020 2020 2020 2020 2020 205b 2b34 2e36             [+4.6
-00001740: 3634 3838 3938 3435 3733 3935 362c 202b  6488984573956, +
-00001750: 302e 3137 3930 3735 3638 3030 3634 3039  0.17907568006409
-00001760: 2c20 302e 3030 3030 3030 3030 3030 3030  , 0.000000000000
-00001770: 3030 5d2c 0a20 2020 2020 2020 2020 2020  00],.           
-00001780: 205b 2d34 2e36 3030 3434 3234 3437 3832   [-4.60044244782
-00001790: 3233 372c 202d 302e 3137 3739 3437 3334  237, -0.17794734
-000017a0: 3633 3734 3133 2c20 302e 3030 3030 3030  637413, 0.000000
-000017b0: 3030 3030 3030 3030 5d2c 0a20 2020 2020  00000000],.     
-000017c0: 2020 205d 0a20 2020 2029 0a0a 2020 2020     ].    )..    
-000017d0: 2320 746f 7461 6c20 6368 6172 6765 206f  # total charge o
-000017e0: 6620 7468 6520 7379 7374 656d 0a20 2020  f the system.   
-000017f0: 2063 6861 7267 6520 3d20 746f 7263 682e   charge = torch.
-00001800: 7465 6e73 6f72 2830 2e30 290a 0a20 2020  tensor(0.0)..   
-00001810: 2023 2054 5053 5330 2d44 342d 4154 4d20   # TPSS0-D4-ATM 
-00001820: 7061 7261 6d65 7465 7273 0a20 2020 2070  parameters.    p
-00001830: 6172 616d 203d 207b 0a20 2020 2020 2020  aram = {.       
-00001840: 2022 7336 223a 2070 6f73 6974 696f 6e73   "s6": positions
-00001850: 2e6e 6577 5f74 656e 736f 7228 312e 3029  .new_tensor(1.0)
-00001860: 2c0a 2020 2020 2020 2020 2273 3822 3a20  ,.        "s8": 
-00001870: 706f 7369 7469 6f6e 732e 6e65 775f 7465  positions.new_te
-00001880: 6e73 6f72 2831 2e38 3538 3937 3735 3029  nsor(1.85897750)
-00001890: 2c0a 2020 2020 2020 2020 2273 3922 3a20  ,.        "s9": 
-000018a0: 706f 7369 7469 6f6e 732e 6e65 775f 7465  positions.new_te
-000018b0: 6e73 6f72 2831 2e30 292c 0a20 2020 2020  nsor(1.0),.     
-000018c0: 2020 2022 6131 223a 2070 6f73 6974 696f     "a1": positio
-000018d0: 6e73 2e6e 6577 5f74 656e 736f 7228 302e  ns.new_tensor(0.
-000018e0: 3434 3238 3639 3636 292c 0a20 2020 2020  44286966),.     
-000018f0: 2020 2022 6132 223a 2070 6f73 6974 696f     "a2": positio
-00001900: 6e73 2e6e 6577 5f74 656e 736f 7228 342e  ns.new_tensor(4.
-00001910: 3630 3233 3035 3334 292c 0a20 2020 207d  60230534),.    }
-00001920: 0a0a 2020 2020 656e 6572 6779 203d 2064  ..    energy = d
-00001930: 342e 6466 7464 3428 6e75 6d62 6572 732c  4.dftd4(numbers,
-00001940: 2070 6f73 6974 696f 6e73 2c20 6368 6172   positions, char
-00001950: 6765 2c20 7061 7261 6d29 0a20 2020 2074  ge, param).    t
-00001960: 6f72 6368 2e73 6574 5f70 7269 6e74 6f70  orch.set_printop
-00001970: 7469 6f6e 7328 7072 6563 6973 696f 6e3d  tions(precision=
-00001980: 3130 290a 2020 2020 7072 696e 7428 656e  10).    print(en
-00001990: 6572 6779 290a 2020 2020 2320 7465 6e73  ergy).    # tens
-000019a0: 6f72 285b 2d30 2e30 3032 3038 3431 3334  or([-0.002084134
-000019b0: 342c 202d 302e 3030 3138 3937 3131 3935  4, -0.0018971195
-000019c0: 2c20 2d30 2e30 3031 3831 3037 3531 332c  , -0.0018107513,
-000019d0: 202d 302e 3030 3138 3330 3536 3935 2c0a   -0.0018305695,.
-000019e0: 2020 2020 2320 2020 2020 2020 2020 2d30      #         -0
-000019f0: 2e30 3032 3137 3337 3639 332c 202d 302e  .0021737693, -0.
-00001a00: 3030 3139 3438 3432 3336 2c20 2d30 2e30  0019484236, -0.0
-00001a10: 3032 3237 3838 3235 332c 202d 302e 3030  022788253, -0.00
-00001a20: 3034 3038 3036 3538 2c0a 2020 2020 2320  04080658,.    # 
-00001a30: 2020 2020 2020 2020 2d30 2e30 3030 3432          -0.00042
-00001a40: 3631 3836 362c 202d 302e 3030 3034 3139  61866, -0.000419
-00001a50: 3938 3339 2c20 2d30 2e30 3030 3432 3830  9839, -0.0004280
-00001a60: 3736 382c 202d 302e 3030 3035 3130 3839  768, -0.00051089
-00001a70: 3335 5d29 0a0a 5468 6520 6e65 7874 2065  35])..The next e
-00001a80: 7861 6d70 6c65 2073 686f 7773 2074 6865  xample shows the
-00001a90: 2063 616c 6375 6c61 7469 6f6e 206f 6620   calculation of 
-00001aa0: 6469 7370 6572 7369 6f6e 2065 6e65 7267  dispersion energ
-00001ab0: 6965 7320 666f 7220 6120 6261 7463 6820  ies for a batch 
-00001ac0: 6f66 2073 7472 7563 7475 7265 732e 0a0a  of structures...
-00001ad0: 2e2e 2063 6f64 653a 3a20 7079 7468 6f6e  .. code:: python
-00001ae0: 0a0a 2020 2020 696d 706f 7274 2074 6f72  ..    import tor
-00001af0: 6368 0a20 2020 2069 6d70 6f72 7420 7461  ch.    import ta
-00001b00: 645f 6466 7464 3420 6173 2064 340a 0a20  d_dftd4 as d4.. 
-00001b10: 2020 2023 2053 3232 2073 7973 7465 6d20     # S22 system 
-00001b20: 343a 2066 6f72 6d61 6d69 6465 2064 696d  4: formamide dim
-00001b30: 6572 0a20 2020 206e 756d 6265 7273 203d  er.    numbers =
-00001b40: 2064 342e 7574 696c 732e 7061 636b 2828   d4.utils.pack((
-00001b50: 0a20 2020 2020 2020 2064 342e 7574 696c  .        d4.util
-00001b60: 732e 746f 5f6e 756d 6265 7228 2243 2043  s.to_number("C C
-00001b70: 204e 204e 2048 2048 2048 2048 2048 2048   N N H H H H H H
-00001b80: 204f 204f 222e 7370 6c69 7428 2929 2c0a   O O".split()),.
-00001b90: 2020 2020 2020 2020 6434 2e75 7469 6c73          d4.utils
-00001ba0: 2e74 6f5f 6e75 6d62 6572 2822 4320 4f20  .to_number("C O 
-00001bb0: 4e20 4820 4820 4822 2e73 706c 6974 2829  N H H H".split()
-00001bc0: 292c 0a20 2020 2029 290a 0a20 2020 2023  ),.    ))..    #
-00001bd0: 2063 6f6f 7264 696e 6174 6573 2069 6e20   coordinates in 
-00001be0: 426f 6872 0a20 2020 2070 6f73 6974 696f  Bohr.    positio
-00001bf0: 6e73 203d 2064 342e 7574 696c 732e 7061  ns = d4.utils.pa
-00001c00: 636b 2828 0a20 2020 2020 2020 2074 6f72  ck((.        tor
-00001c10: 6368 2e74 656e 736f 7228 5b0a 2020 2020  ch.tensor([.    
-00001c20: 2020 2020 2020 2020 5b2d 332e 3831 3436          [-3.8146
-00001c30: 3934 3838 3134 3339 3231 2c20 2b30 2e30  9488143921, +0.0
-00001c40: 3939 3933 3434 3134 3032 3931 322c 2030  9993441402912, 0
-00001c50: 2e30 3030 3030 3030 3030 3030 3030 305d  .00000000000000]
-00001c60: 2c0a 2020 2020 2020 2020 2020 2020 5b2b  ,.            [+
-00001c70: 332e 3831 3436 3934 3838 3134 3339 3231  3.81469488143921
-00001c80: 2c20 2d30 2e30 3939 3933 3434 3134 3032  , -0.09993441402
-00001c90: 3931 322c 2030 2e30 3030 3030 3030 3030  912, 0.000000000
-00001ca0: 3030 3030 305d 2c0a 2020 2020 2020 2020  00000],.        
-00001cb0: 2020 2020 5b2d 322e 3636 3033 3030 3439      [-2.66030049
-00001cc0: 3332 3430 3336 2c20 2d32 2e31 3538 3938  324036, -2.15898
-00001cd0: 3235 3135 3333 3530 382c 2030 2e30 3030  251533508, 0.000
-00001ce0: 3030 3030 3030 3030 3030 305d 2c0a 2020  00000000000],.  
-00001cf0: 2020 2020 2020 2020 2020 5b2b 322e 3636            [+2.66
-00001d00: 3033 3030 3439 3332 3430 3336 2c20 2b32  030049324036, +2
-00001d10: 2e31 3538 3938 3235 3135 3333 3530 382c  .15898251533508,
-00001d20: 2030 2e30 3030 3030 3030 3030 3030 3030   0.0000000000000
-00001d30: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
-00001d40: 5b2d 302e 3733 3137 3835 3239 3733 3933  [-0.731785297393
-00001d50: 3830 2c20 2d32 2e32 3832 3337 3739 3538  80, -2.282377958
-00001d60: 3239 3737 332c 2030 2e30 3030 3030 3030  29773, 0.0000000
-00001d70: 3030 3030 3030 305d 2c0a 2020 2020 2020  0000000],.      
-00001d80: 2020 2020 2020 5b2d 352e 3839 3033 3933        [-5.890393
-00001d90: 3235 3731 3431 3131 2c20 2d30 2e30 3235  25714111, -0.025
-00001da0: 3839 3131 3435 3639 3132 382c 2030 2e30  89114569128, 0.0
-00001db0: 3030 3030 3030 3030 3030 3030 305d 2c0a  0000000000000],.
-00001dc0: 2020 2020 2020 2020 2020 2020 5b2d 332e              [-3.
-00001dd0: 3731 3235 3439 3434 3830 3133 3331 2c20  71254944801331, 
-00001de0: 2d33 2e37 3336 3035 3737 3538 3333 3133  -3.7360577583313
-00001df0: 302c 2030 2e30 3030 3030 3030 3030 3030  0, 0.00000000000
-00001e00: 3030 305d 2c0a 2020 2020 2020 2020 2020  000],.          
-00001e10: 2020 5b2b 332e 3731 3235 3439 3434 3830    [+3.7125494480
-00001e20: 3133 3331 2c20 2b33 2e37 3336 3035 3737  1331, +3.7360577
-00001e30: 3538 3333 3133 302c 2030 2e30 3030 3030  5833130, 0.00000
-00001e40: 3030 3030 3030 3030 305d 2c0a 2020 2020  000000000],.    
-00001e50: 2020 2020 2020 2020 5b2b 302e 3733 3137          [+0.7317
-00001e60: 3835 3239 3733 3933 3830 2c20 2b32 2e32  8529739380, +2.2
-00001e70: 3832 3337 3739 3538 3239 3737 332c 2030  8237795829773, 0
-00001e80: 2e30 3030 3030 3030 3030 3030 3030 305d  .00000000000000]
-00001e90: 2c0a 2020 2020 2020 2020 2020 2020 5b2b  ,.            [+
-00001ea0: 352e 3839 3033 3933 3235 3731 3431 3131  5.89039325714111
-00001eb0: 2c20 2b30 2e30 3235 3839 3131 3435 3639  , +0.02589114569
-00001ec0: 3132 382c 2030 2e30 3030 3030 3030 3030  128, 0.000000000
-00001ed0: 3030 3030 305d 2c0a 2020 2020 2020 2020  00000],.        
-00001ee0: 2020 2020 5b2d 322e 3734 3432 3631 3032      [-2.74426102
-00001ef0: 3633 3832 3435 2c20 2b32 2e31 3631 3135  638245, +2.16115
-00001f00: 3537 3030 3638 3335 392c 2030 2e30 3030  570068359, 0.000
-00001f10: 3030 3030 3030 3030 3030 305d 2c0a 2020  00000000000],.  
-00001f20: 2020 2020 2020 2020 2020 5b2b 322e 3734            [+2.74
-00001f30: 3432 3631 3032 3633 3832 3435 2c20 2d32  426102638245, -2
-00001f40: 2e31 3631 3135 3537 3030 3638 3335 392c  .16115570068359,
-00001f50: 2030 2e30 3030 3030 3030 3030 3030 3030   0.0000000000000
-00001f60: 305d 2c0a 2020 2020 2020 2020 5d29 2c0a  0],.        ]),.
-00001f70: 2020 2020 2020 2020 746f 7263 682e 7465          torch.te
-00001f80: 6e73 6f72 285b 0a20 2020 2020 2020 2020  nsor([.         
-00001f90: 2020 205b 2d30 2e35 3535 3639 3734 3332     [-0.555697432
-00001fa0: 3033 3430 362c 202b 312e 3039 3033 3034  03406, +1.090304
-00001fb0: 3235 3436 3835 3537 2c20 302e 3030 3030  25468557, 0.0000
-00001fc0: 3030 3030 3030 3030 3030 5d2c 0a20 2020  0000000000],.   
-00001fd0: 2020 2020 2020 2020 205b 2b30 2e35 3134           [+0.514
-00001fe0: 3733 3633 3436 3738 3436 392c 202b 332e  73634678469, +3.
-00001ff0: 3135 3135 3235 3530 3236 3336 3131 2c20  15152550263611, 
-00002000: 302e 3030 3030 3030 3030 3030 3030 3030  0.00000000000000
-00002010: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-00002020: 2b30 2e35 3938 3639 3639 3032 3434 3434  +0.5986969024444
-00002030: 362c 202d 312e 3136 3836 3132 3633 3738  6, -1.1686126378
-00002040: 3934 3737 2c20 302e 3030 3030 3030 3030  9477, 0.00000000
-00002050: 3030 3030 3030 5d2c 0a20 2020 2020 2020  000000],.       
-00002060: 2020 2020 205b 2d30 2e34 3533 3535 3230       [-0.4535520
-00002070: 3336 3639 3133 342c 202d 322e 3734 3536  3669134, -2.7456
-00002080: 3837 3830 3433 3830 3634 2c20 302e 3030  8780438064, 0.00
-00002090: 3030 3030 3030 3030 3030 3030 5d2c 0a20  000000000000],. 
-000020a0: 2020 2020 2020 2020 2020 205b 2b32 2e35             [+2.5
-000020b0: 3237 3231 3230 3935 3434 3939 392c 202d  2721209544999, -
-000020c0: 312e 3239 3230 3038 3030 3935 3638 3637  1.29200800956867
-000020d0: 2c20 302e 3030 3030 3030 3030 3030 3030  , 0.000000000000
-000020e0: 3030 5d2c 0a20 2020 2020 2020 2020 2020  00],.           
-000020f0: 205b 2d32 2e36 3331 3339 3538 3735 3935   [-2.63139587595
-00002100: 3337 362c 202b 302e 3936 3434 3738 3639  376, +0.96447869
-00002110: 3435 3232 3430 2c20 302e 3030 3030 3030  452240, 0.000000
-00002120: 3030 3030 3030 3030 5d2c 0a20 2020 2020  00000000],.     
-00002130: 2020 205d 292c 0a20 2020 2029 290a 0a20     ]),.    )).. 
-00002140: 2020 2023 2074 6f74 616c 2063 6861 7267     # total charg
-00002150: 6520 6f66 2062 6f74 6820 7379 7374 656d  e of both system
-00002160: 0a20 2020 2063 6861 7267 6520 3d20 746f  .    charge = to
-00002170: 7263 682e 7465 6e73 6f72 285b 302e 302c  rch.tensor([0.0,
-00002180: 2030 2e30 5d29 0a0a 2020 2020 2320 5450   0.0])..    # TP
-00002190: 5353 302d 4434 2d41 544d 2070 6172 616d  SS0-D4-ATM param
-000021a0: 6574 6572 730a 2020 2020 7061 7261 6d20  eters.    param 
-000021b0: 3d20 7b0a 2020 2020 2020 2020 2273 3622  = {.        "s6"
-000021c0: 3a20 706f 7369 7469 6f6e 732e 6e65 775f  : positions.new_
-000021d0: 7465 6e73 6f72 2831 2e30 292c 0a20 2020  tensor(1.0),.   
-000021e0: 2020 2020 2022 7338 223a 2070 6f73 6974       "s8": posit
-000021f0: 696f 6e73 2e6e 6577 5f74 656e 736f 7228  ions.new_tensor(
-00002200: 312e 3835 3839 3737 3530 292c 0a20 2020  1.85897750),.   
-00002210: 2020 2020 2022 7339 223a 2070 6f73 6974       "s9": posit
-00002220: 696f 6e73 2e6e 6577 5f74 656e 736f 7228  ions.new_tensor(
-00002230: 312e 3029 2c0a 2020 2020 2020 2020 2261  1.0),.        "a
-00002240: 3122 3a20 706f 7369 7469 6f6e 732e 6e65  1": positions.ne
-00002250: 775f 7465 6e73 6f72 2830 2e34 3432 3836  w_tensor(0.44286
-00002260: 3936 3629 2c0a 2020 2020 2020 2020 2261  966),.        "a
-00002270: 3222 3a20 706f 7369 7469 6f6e 732e 6e65  2": positions.ne
-00002280: 775f 7465 6e73 6f72 2834 2e36 3032 3330  w_tensor(4.60230
-00002290: 3533 3429 2c0a 2020 2020 7d0a 0a20 2020  534),.    }..   
-000022a0: 2023 2063 616c 6375 6c61 7465 2064 6973   # calculate dis
-000022b0: 7065 7273 696f 6e20 656e 6572 6779 2069  persion energy i
-000022c0: 6e20 4861 7274 7265 650a 2020 2020 656e  n Hartree.    en
-000022d0: 6572 6779 203d 2074 6f72 6368 2e73 756d  ergy = torch.sum
-000022e0: 2864 342e 6466 7464 3428 6e75 6d62 6572  (d4.dftd4(number
-000022f0: 732c 2070 6f73 6974 696f 6e73 2c20 6368  s, positions, ch
-00002300: 6172 6765 2c20 7061 7261 6d29 2c20 2d31  arge, param), -1
-00002310: 290a 2020 2020 746f 7263 682e 7365 745f  ).    torch.set_
-00002320: 7072 696e 746f 7074 696f 6e73 2870 7265  printoptions(pre
-00002330: 6369 7369 6f6e 3d31 3029 0a20 2020 2070  cision=10).    p
-00002340: 7269 6e74 2865 6e65 7267 7929 0a20 2020  rint(energy).   
-00002350: 2023 2074 656e 736f 7228 5b2d 302e 3030   # tensor([-0.00
-00002360: 3838 3334 3134 3332 2c20 2d30 2e30 3032  88341432, -0.002
-00002370: 3730 3133 3630 375d 290a 2020 2020 7072  7013607]).    pr
-00002380: 696e 7428 656e 6572 6779 5b30 5d20 2d20  int(energy[0] - 
-00002390: 322a 656e 6572 6779 5b31 5d29 0a20 2020  2*energy[1]).   
-000023a0: 2023 2074 656e 736f 7228 2d30 2e30 3033   # tensor(-0.003
-000023b0: 3433 3134 3231 3729 0a0a 436f 6e74 7269  4314217)..Contri
-000023c0: 6275 7469 6e67 0a2d 2d2d 2d2d 2d2d 2d2d  buting.---------
-000023d0: 2d2d 2d0a 0a54 6869 7320 6973 2061 2076  ---..This is a v
-000023e0: 6f6c 756e 7465 6572 206f 7065 6e20 736f  olunteer open so
-000023f0: 7572 6365 2070 726f 6a65 6374 7320 616e  urce projects an
-00002400: 6420 636f 6e74 7269 6275 7469 6f6e 7320  d contributions 
-00002410: 6172 6520 616c 7761 7973 2077 656c 636f  are always welco
-00002420: 6d65 2e0a 506c 6561 7365 2c20 7461 6b65  me..Please, take
-00002430: 2061 206d 6f6d 656e 7420 746f 2072 6561   a moment to rea
-00002440: 6420 7468 6520 6063 6f6e 7472 6962 7574  d the `contribut
-00002450: 696e 6720 6775 6964 656c 696e 6573 203c  ing guidelines <
-00002460: 434f 4e54 5249 4255 5449 4e47 2e6d 643e  CONTRIBUTING.md>
-00002470: 605f 5f2e 0a0a 4c69 6365 6e73 650a 2d2d  `__...License.--
-00002480: 2d2d 2d2d 2d0a 0a54 6869 7320 7072 6f6a  -----..This proj
-00002490: 6563 7420 6973 2066 7265 6520 736f 6674  ect is free soft
-000024a0: 7761 7265 3a20 796f 7520 6361 6e20 7265  ware: you can re
-000024b0: 6469 7374 7269 6275 7465 2069 7420 616e  distribute it an
-000024c0: 642f 6f72 206d 6f64 6966 7920 6974 2075  d/or modify it u
-000024d0: 6e64 6572 2074 6865 2074 6572 6d73 206f  nder the terms o
-000024e0: 6620 7468 6520 4c65 7373 6572 2047 4e55  f the Lesser GNU
-000024f0: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
-00002500: 4c69 6365 6e73 6520 6173 2070 7562 6c69  License as publi
-00002510: 7368 6564 2062 7920 7468 6520 4672 6565  shed by the Free
-00002520: 2053 6f66 7477 6172 6520 466f 756e 6461   Software Founda
-00002530: 7469 6f6e 2c20 6569 7468 6572 2076 6572  tion, either ver
-00002540: 7369 6f6e 2033 206f 6620 7468 6520 4c69  sion 3 of the Li
-00002550: 6365 6e73 652c 206f 7220 2861 7420 796f  cense, or (at yo
-00002560: 7572 206f 7074 696f 6e29 2061 6e79 206c  ur option) any l
-00002570: 6174 6572 2076 6572 7369 6f6e 2e0a 0a54  ater version...T
-00002580: 6869 7320 7072 6f6a 6563 7420 6973 2064  his project is d
-00002590: 6973 7472 6962 7574 6564 2069 6e20 7468  istributed in th
-000025a0: 6520 686f 7065 2074 6861 7420 6974 2077  e hope that it w
-000025b0: 696c 6c20 6265 2075 7365 6675 6c2c 2062  ill be useful, b
-000025c0: 7574 2077 6974 686f 7574 2061 6e79 2077  ut without any w
-000025d0: 6172 7261 6e74 793b 2077 6974 686f 7574  arranty; without
-000025e0: 2065 7665 6e20 7468 6520 696d 706c 6965   even the implie
-000025f0: 6420 7761 7272 616e 7479 206f 6620 6d65  d warranty of me
-00002600: 7263 6861 6e74 6162 696c 6974 7920 6f72  rchantability or
-00002610: 2066 6974 6e65 7373 2066 6f72 2061 2070   fitness for a p
-00002620: 6172 7469 6375 6c61 7220 7075 7270 6f73  articular purpos
-00002630: 652e 2053 6565 2074 6865 204c 6573 7365  e. See the Lesse
-00002640: 7220 474e 5520 4765 6e65 7261 6c20 5075  r GNU General Pu
-00002650: 626c 6963 204c 6963 656e 7365 2066 6f72  blic License for
-00002660: 206d 6f72 6520 6465 7461 696c 732e 0a0a   more details...
-00002670: 556e 6c65 7373 2079 6f75 2065 7870 6c69  Unless you expli
-00002680: 6369 746c 7920 7374 6174 6520 6f74 6865  citly state othe
-00002690: 7277 6973 652c 2061 6e79 2063 6f6e 7472  rwise, any contr
-000026a0: 6962 7574 696f 6e20 696e 7465 6e74 696f  ibution intentio
-000026b0: 6e61 6c6c 7920 7375 626d 6974 7465 6420  nally submitted 
-000026c0: 666f 7220 696e 636c 7573 696f 6e20 696e  for inclusion in
-000026d0: 2074 6869 7320 7072 6f6a 6563 7420 6279   this project by
-000026e0: 2079 6f75 2c20 6173 2064 6566 696e 6564   you, as defined
-000026f0: 2069 6e20 7468 6520 4c65 7373 6572 2047   in the Lesser G
-00002700: 4e55 2047 656e 6572 616c 2050 7562 6c69  NU General Publi
-00002710: 6320 6c69 6365 6e73 652c 2073 6861 6c6c  c license, shall
-00002720: 2062 6520 6c69 6365 6e73 6564 2061 7320   be licensed as 
-00002730: 6162 6f76 652c 2077 6974 686f 7574 2061  above, without a
-00002740: 6e79 2061 6464 6974 696f 6e61 6c20 7465  ny additional te
-00002750: 726d 7320 6f72 2063 6f6e 6469 7469 6f6e  rms or condition
-00002760: 732e 0a                                  s..
+00000080: 7365 3a20 4170 6163 6865 2d32 2e30 0a43  se: Apache-2.0.C
+00000090: 6c61 7373 6966 6965 723a 2046 7261 6d65  lassifier: Frame
+000000a0: 776f 726b 203a 3a20 5079 7465 7374 0a43  work :: Pytest.C
+000000b0: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
+000000c0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+000000d0: 6564 203a 3a20 4170 6163 6865 2053 6f66  ed :: Apache Sof
+000000e0: 7477 6172 6520 4c69 6365 6e73 650a 436c  tware License.Cl
+000000f0: 6173 7369 6669 6572 3a20 4e61 7475 7261  assifier: Natura
+00000100: 6c20 4c61 6e67 7561 6765 203a 3a20 456e  l Language :: En
+00000110: 676c 6973 680a 436c 6173 7369 6669 6572  glish.Classifier
+00000120: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000130: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000140: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
+00000150: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000160: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000170: 203a 3a20 3320 3a3a 204f 6e6c 790a 436c   :: 3 :: Only.Cl
+00000180: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000190: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000001a0: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
+000001b0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000001c0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001d0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000001e0: 390a 436c 6173 7369 6669 6572 3a20 5072  9.Classifier: Pr
+000001f0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000200: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000210: 332e 3130 0a43 6c61 7373 6966 6965 723a  3.10.Classifier:
+00000220: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000230: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000240: 3a3a 2033 2e31 310a 436c 6173 7369 6669  :: 3.11.Classifi
+00000250: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000260: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000270: 6f6e 203a 3a20 496d 706c 656d 656e 7461  on :: Implementa
+00000280: 7469 6f6e 203a 3a20 4350 7974 686f 6e0a  tion :: CPython.
+00000290: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+000002a0: 6320 3a3a 2053 6369 656e 7469 6669 632f  c :: Scientific/
+000002b0: 456e 6769 6e65 6572 696e 670a 436c 6173  Engineering.Clas
+000002c0: 7369 6669 6572 3a20 5479 7069 6e67 203a  sifier: Typing :
+000002d0: 3a20 5479 7065 640a 5265 7175 6972 6573  : Typed.Requires
+000002e0: 2d50 7974 686f 6e3a 203e 3d33 2e38 0a44  -Python: >=3.8.D
+000002f0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+00000300: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+00000310: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
+00000320: 696c 653a 204c 4943 454e 5345 0a52 6571  ile: LICENSE.Req
+00000330: 7569 7265 732d 4469 7374 3a20 6e75 6d70  uires-Dist: nump
+00000340: 790a 5265 7175 6972 6573 2d44 6973 743a  y.Requires-Dist:
+00000350: 2074 6164 2d6d 6374 630a 5265 7175 6972   tad-mctc.Requir
+00000360: 6573 2d44 6973 743a 2074 6164 2d6d 756c  es-Dist: tad-mul
+00000370: 7469 6368 6172 6765 0a52 6571 7569 7265  ticharge.Require
+00000380: 732d 4469 7374 3a20 746f 7263 683e 3d31  s-Dist: torch>=1
+00000390: 2e31 310a 5072 6f76 6964 6573 2d45 7874  .11.Provides-Ext
+000003a0: 7261 3a20 6465 760a 5265 7175 6972 6573  ra: dev.Requires
+000003b0: 2d44 6973 743a 2062 6c61 636b 3b20 6578  -Dist: black; ex
+000003c0: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+000003d0: 7569 7265 732d 4469 7374 3a20 636f 7664  uires-Dist: covd
+000003e0: 6566 6175 6c74 733b 2065 7874 7261 203d  efaults; extra =
+000003f0: 3d20 2264 6576 220a 5265 7175 6972 6573  = "dev".Requires
+00000400: 2d44 6973 743a 206d 7970 793b 2065 7874  -Dist: mypy; ext
+00000410: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+00000420: 6972 6573 2d44 6973 743a 2070 7265 2d63  ires-Dist: pre-c
+00000430: 6f6d 6d69 743b 2065 7874 7261 203d 3d20  ommit; extra == 
+00000440: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
+00000450: 6973 743a 2070 796c 696e 743b 2065 7874  ist: pylint; ext
+00000460: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+00000470: 6972 6573 2d44 6973 743a 2070 7974 6573  ires-Dist: pytes
+00000480: 743b 2065 7874 7261 203d 3d20 2264 6576  t; extra == "dev
+00000490: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+000004a0: 2070 7974 6573 742d 636f 763b 2065 7874   pytest-cov; ext
+000004b0: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+000004c0: 6972 6573 2d44 6973 743a 2070 7974 6573  ires-Dist: pytes
+000004d0: 742d 7261 6e64 6f6d 2d6f 7264 6572 3b20  t-random-order; 
+000004e0: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
+000004f0: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
+00000500: 7465 7374 2d78 6469 7374 3b20 6578 7472  test-xdist; extr
+00000510: 6120 3d3d 2022 6465 7622 0a52 6571 7569  a == "dev".Requi
+00000520: 7265 732d 4469 7374 3a20 746f 783b 2065  res-Dist: tox; e
+00000530: 7874 7261 203d 3d20 2264 6576 220a 5072  xtra == "dev".Pr
+00000540: 6f76 6964 6573 2d45 7874 7261 3a20 746f  ovides-Extra: to
+00000550: 780a 5265 7175 6972 6573 2d44 6973 743a  x.Requires-Dist:
+00000560: 2063 6f76 6465 6661 756c 7473 3b20 6578   covdefaults; ex
+00000570: 7472 6120 3d3d 2022 746f 7822 0a52 6571  tra == "tox".Req
+00000580: 7569 7265 732d 4469 7374 3a20 7079 7465  uires-Dist: pyte
+00000590: 7374 3b20 6578 7472 6120 3d3d 2022 746f  st; extra == "to
+000005a0: 7822 0a52 6571 7569 7265 732d 4469 7374  x".Requires-Dist
+000005b0: 3a20 7079 7465 7374 2d63 6f76 3b20 6578  : pytest-cov; ex
+000005c0: 7472 6120 3d3d 2022 746f 7822 0a52 6571  tra == "tox".Req
+000005d0: 7569 7265 732d 4469 7374 3a20 7079 7465  uires-Dist: pyte
+000005e0: 7374 2d72 616e 646f 6d2d 6f72 6465 723b  st-random-order;
+000005f0: 2065 7874 7261 203d 3d20 2274 6f78 220a   extra == "tox".
+00000600: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
+00000610: 7974 6573 742d 7864 6973 743b 2065 7874  ytest-xdist; ext
+00000620: 7261 203d 3d20 2274 6f78 220a 0a23 2054  ra == "tox"..# T
+00000630: 6f72 6368 2041 7574 6f64 6966 6620 666f  orch Autodiff fo
+00000640: 7220 4446 542d 4434 0a0a 3c74 6162 6c65  r DFT-D4..<table
+00000650: 3e0a 2020 3c74 723e 0a20 2020 203c 7464  >.  <tr>.    <td
+00000660: 3e43 6f6d 7061 7469 6269 6c69 7479 3a3c  >Compatibility:<
+00000670: 2f74 643e 0a20 2020 203c 7464 3e0a 2020  /td>.    <td>.  
+00000680: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000690: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000006a0: 732e 696f 2f62 6164 6765 2f50 7974 686f  s.io/badge/Pytho
+000006b0: 6e2d 332e 3825 3230 7c25 3230 332e 3925  n-3.8%20|%203.9%
+000006c0: 3230 7c25 3230 332e 3130 2532 307c 2532  20|%203.10%20|%2
+000006d0: 3033 2e31 312d 626c 7565 2e73 7667 2220  03.11-blue.svg" 
+000006e0: 616c 743d 2250 7974 686f 6e20 5665 7273  alt="Python Vers
+000006f0: 696f 6e73 222f 3e0a 2020 2020 2020 3c69  ions"/>.      <i
+00000700: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000710: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000720: 6164 6765 2f50 7954 6f72 6368 2d25 3345  adge/PyTorch-%3E
+00000730: 3d31 2e31 312e 302d 626c 7565 2e73 7667  =1.11.0-blue.svg
+00000740: 2220 616c 743d 2250 7954 6f72 6368 2056  " alt="PyTorch V
+00000750: 6572 7369 6f6e 7322 2f3e 0a20 2020 203c  ersions"/>.    <
+00000760: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
+00000770: 7472 3e0a 2020 2020 3c74 643e 4176 6169  tr>.    <td>Avai
+00000780: 6c61 6269 6c69 7479 3a3c 2f74 643e 0a20  lability:</td>. 
+00000790: 2020 203c 7464 3e0a 2020 2020 2020 3c61     <td>.      <a
+000007a0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000007b0: 6974 6875 622e 636f 6d2f 6466 7464 342f  ithub.com/dftd4/
+000007c0: 7461 642d 6466 7464 342f 7265 6c65 6173  tad-dftd4/releas
+000007d0: 6573 2f6c 6174 6573 7422 3e0a 2020 2020  es/latest">.    
+000007e0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+000007f0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000800: 732e 696f 2f67 6974 6875 622f 762f 7265  s.io/github/v/re
+00000810: 6c65 6173 652f 6466 7464 342f 7461 642d  lease/dftd4/tad-
+00000820: 6466 7464 343f 636f 6c6f 723d 6f72 616e  dftd4?color=oran
+00000830: 6765 2220 616c 743d 2252 656c 6561 7365  ge" alt="Release
+00000840: 222f 3e0a 2020 2020 2020 3c2f 613e 0a20  "/>.      </a>. 
+00000850: 2020 2020 203c 6120 6872 6566 3d22 6874       <a href="ht
+00000860: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000870: 726f 6a65 6374 2f74 6164 2d64 6674 6434  roject/tad-dftd4
+00000880: 2f22 3e0a 2020 2020 2020 2020 3c69 6d67  /">.        <img
+00000890: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+000008a0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+000008b0: 692f 762f 7461 642d 6466 7464 343f 636f  i/v/tad-dftd4?co
+000008c0: 6c6f 723d 6f72 616e 6765 2220 616c 743d  lor=orange" alt=
+000008d0: 2250 7950 4922 2f3e 0a20 2020 2020 203c  "PyPI"/>.      <
+000008e0: 2f61 3e0a 2020 2020 2020 3c61 2068 7265  /a>.      <a hre
+000008f0: 663d 2268 7474 703a 2f2f 7777 772e 6170  f="http://www.ap
+00000900: 6163 6865 2e6f 7267 2f6c 6963 656e 7365  ache.org/license
+00000910: 732f 4c49 4345 4e53 452d 322e 3022 3e0a  s/LICENSE-2.0">.
+00000920: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000930: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000940: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
+00000950: 6963 656e 7365 2d41 7061 6368 6525 3230  icense-Apache%20
+00000960: 322e 302d 6f72 616e 6765 2e73 7667 2220  2.0-orange.svg" 
+00000970: 616c 743d 2241 7061 6368 652d 322e 3022  alt="Apache-2.0"
+00000980: 2f3e 0a20 2020 2020 203c 2f61 3e0a 2020  />.      </a>.  
+00000990: 2020 3c2f 7464 3e0a 2020 3c2f 7472 3e0a    </td>.  </tr>.
+000009a0: 2020 3c74 723e 0a20 2020 203c 7464 3e53    <tr>.    <td>S
+000009b0: 7461 7475 733a 3c2f 7464 3e0a 2020 2020  tatus:</td>.    
+000009c0: 3c74 643e 0a20 2020 2020 203c 6120 6872  <td>.      <a hr
+000009d0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000009e0: 7562 2e63 6f6d 2f64 6674 6434 2f74 6164  ub.com/dftd4/tad
+000009f0: 2d64 6674 6434 2f61 6374 696f 6e73 2f77  -dftd4/actions/w
+00000a00: 6f72 6b66 6c6f 7773 2f70 7974 686f 6e2e  orkflows/python.
+00000a10: 7961 6d6c 223e 0a20 2020 2020 2020 203c  yaml">.        <
+00000a20: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000a30: 2f67 6974 6875 622e 636f 6d2f 6466 7464  /github.com/dftd
+00000a40: 342f 7461 642d 6466 7464 342f 6163 7469  4/tad-dftd4/acti
+00000a50: 6f6e 732f 776f 726b 666c 6f77 732f 7079  ons/workflows/py
+00000a60: 7468 6f6e 2e79 616d 6c2f 6261 6467 652e  thon.yaml/badge.
+00000a70: 7376 6722 2061 6c74 3d22 5465 7374 2053  svg" alt="Test S
+00000a80: 7461 7475 7322 2f3e 0a20 2020 2020 203c  tatus"/>.      <
+00000a90: 2f61 3e0a 2020 2020 2020 3c61 2068 7265  /a>.      <a hre
+00000aa0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00000ab0: 622e 636f 6d2f 6466 7464 342f 7461 642d  b.com/dftd4/tad-
+00000ac0: 6466 7464 342f 6163 7469 6f6e 732f 776f  dftd4/actions/wo
+00000ad0: 726b 666c 6f77 732f 7265 6c65 6173 652e  rkflows/release.
+00000ae0: 7961 6d6c 223e 0a20 2020 2020 2020 203c  yaml">.        <
+00000af0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000b00: 2f67 6974 6875 622e 636f 6d2f 6466 7464  /github.com/dftd
+00000b10: 342f 7461 642d 6466 7464 342f 6163 7469  4/tad-dftd4/acti
+00000b20: 6f6e 732f 776f 726b 666c 6f77 732f 7265  ons/workflows/re
+00000b30: 6c65 6173 652e 7961 6d6c 2f62 6164 6765  lease.yaml/badge
+00000b40: 2e73 7667 2220 616c 743d 2242 7569 6c64  .svg" alt="Build
+00000b50: 2053 7461 7475 7322 2f3e 0a20 2020 2020   Status"/>.     
+00000b60: 203c 2f61 3e0a 2020 2020 2020 3c61 2068   </a>.      <a h
+00000b70: 7265 663d 2268 7474 7073 3a2f 2f74 6164  ref="https://tad
+00000b80: 2d64 6674 6434 2e72 6561 6474 6865 646f  -dftd4.readthedo
+00000b90: 6373 2e69 6f22 3e0a 2020 2020 2020 2020  cs.io">.        
+00000ba0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000bb0: 2f2f 7265 6164 7468 6564 6f63 732e 6f72  //readthedocs.or
+00000bc0: 672f 7072 6f6a 6563 7473 2f74 6164 2d64  g/projects/tad-d
+00000bd0: 6674 6434 2f62 6164 6765 2f3f 7665 7273  ftd4/badge/?vers
+00000be0: 696f 6e3d 6c61 7465 7374 2220 616c 743d  ion=latest" alt=
+00000bf0: 2244 6f63 756d 656e 7461 7469 6f6e 2053  "Documentation S
+00000c00: 7461 7475 7322 2f3e 0a20 2020 2020 203c  tatus"/>.      <
+00000c10: 2f61 3e0a 2020 2020 2020 3c61 2068 7265  /a>.      <a hre
+00000c20: 663d 2268 7474 7073 3a2f 2f72 6573 756c  f="https://resul
+00000c30: 7473 2e70 7265 2d63 6f6d 6d69 742e 6369  ts.pre-commit.ci
+00000c40: 2f6c 6174 6573 742f 6769 7468 7562 2f64  /latest/github/d
+00000c50: 6674 6434 2f74 6164 2d64 6674 6434 2f6d  ftd4/tad-dftd4/m
+00000c60: 6169 6e22 3e0a 2020 2020 2020 2020 3c69  ain">.        <i
+00000c70: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000c80: 7265 7375 6c74 732e 7072 652d 636f 6d6d  results.pre-comm
+00000c90: 6974 2e63 692f 6261 6467 652f 6769 7468  it.ci/badge/gith
+00000ca0: 7562 2f64 6674 6434 2f74 6164 2d64 6674  ub/dftd4/tad-dft
+00000cb0: 6434 2f6d 6169 6e2e 7376 6722 2061 6c74  d4/main.svg" alt
+00000cc0: 3d22 7072 652d 636f 6d6d 6974 2e63 6920  ="pre-commit.ci 
+00000cd0: 5374 6174 7573 222f 3e0a 2020 2020 2020  Status"/>.      
+00000ce0: 3c2f 613e 0a20 2020 2020 203c 6120 6872  </a>.      <a hr
+00000cf0: 6566 3d22 6874 7470 733a 2f2f 636f 6465  ef="https://code
+00000d00: 636f 762e 696f 2f67 682f 6466 7464 342f  cov.io/gh/dftd4/
+00000d10: 7461 642d 6466 7464 3422 3e0a 2020 2020  tad-dftd4">.    
+00000d20: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000d30: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00000d40: 2f67 682f 6466 7464 342f 7461 642d 6466  /gh/dftd4/tad-df
+00000d50: 7464 342f 6272 616e 6368 2f6d 6169 6e2f  td4/branch/main/
+00000d60: 6772 6170 682f 6261 6467 652e 7376 673f  graph/badge.svg?
+00000d70: 746f 6b65 6e3d 4f47 4a4a 6e5a 3674 3447  token=OGJJnZ6t4G
+00000d80: 2220 616c 743d 2243 6f76 6572 6167 6522  " alt="Coverage"
+00000d90: 2f3e 0a20 2020 2020 203c 2f61 3e0a 2020  />.      </a>.  
+00000da0: 2020 3c2f 7464 3e0a 2020 3c2f 7472 3e0a    </td>.  </tr>.
+00000db0: 3c2f 7461 626c 653e 0a0a 3c62 723e 0a0a  </table>..<br>..
+00000dc0: 496d 706c 656d 656e 7461 7469 6f6e 206f  Implementation o
+00000dd0: 6620 7468 6520 4446 542d 4434 2064 6973  f the DFT-D4 dis
+00000de0: 7065 7273 696f 6e20 6d6f 6465 6c20 696e  persion model in
+00000df0: 2050 7954 6f72 6368 2e20 5468 6973 206d   PyTorch. This m
+00000e00: 6f64 756c 6520 616c 6c6f 7773 2074 6f20  odule allows to 
+00000e10: 7072 6f63 6573 7320 6120 7369 6e67 6c65  process a single
+00000e20: 2073 7472 7563 7475 7265 206f 7220 6120   structure or a 
+00000e30: 6261 7463 6820 6f66 2073 7472 7563 7475  batch of structu
+00000e40: 7265 7320 666f 7220 7468 6520 6361 6c63  res for the calc
+00000e50: 756c 6174 696f 6e20 6f66 2061 746f 6d2d  ulation of atom-
+00000e60: 7265 736f 6c76 6564 2064 6973 7065 7273  resolved dispers
+00000e70: 696f 6e20 656e 6572 6769 6573 2e0a 0a46  ion energies...F
+00000e80: 6f72 2064 6574 6169 6c73 206f 6e20 7468  or details on th
+00000e90: 6520 4434 2064 6973 7065 7273 696f 6e20  e D4 dispersion 
+00000ea0: 6d6f 6465 6c2c 2073 6565 3a0a 0a2d 2045  model, see:..- E
+00000eb0: 2e20 4361 6c64 6577 6579 6865 722c 2043  . Caldeweyher, C
+00000ec0: 2e20 4261 6e6e 7761 7274 6820 616e 6420  . Bannwarth and 
+00000ed0: 532e 2047 7269 6d6d 652c 202a 4a2e 2043  S. Grimme, *J. C
+00000ee0: 6865 6d2e 2050 6879 732e 2a2c 2032 3031  hem. Phys.*, 201
+00000ef0: 372c 2031 3437 2c20 3033 3431 3132 2e20  7, 147, 034112. 
+00000f00: 5b44 4f49 3a20 3130 2e31 3036 332f 312e  [DOI: 10.1063/1.
+00000f10: 3439 3933 3231 355d 2868 7474 7073 3a2f  4993215](https:/
+00000f20: 2f64 782e 646f 692e 6f72 672f 3130 2e31  /dx.doi.org/10.1
+00000f30: 3036 332f 312e 3439 3933 3231 3529 0a2d  063/1.4993215).-
+00000f40: 2045 2e20 4361 6c64 6577 6579 6865 722c   E. Caldeweyher,
+00000f50: 2053 2e20 4568 6c65 7274 2c20 412e 2048   S. Ehlert, A. H
+00000f60: 616e 7365 6e2c 2048 2e20 4e65 7567 6562  ansen, H. Neugeb
+00000f70: 6175 6572 2c20 532e 2053 7069 6368 6572  auer, S. Spicher
+00000f80: 2c20 432e 2042 616e 6e77 6172 7468 2061  , C. Bannwarth a
+00000f90: 6e64 2053 2e20 4772 696d 6d65 2c20 2a4a  nd S. Grimme, *J
+00000fa0: 2e20 4368 656d 2e20 5068 7973 2e2a 2c20  . Chem. Phys.*, 
+00000fb0: 3230 3139 2c20 3135 302c 2031 3534 3132  2019, 150, 15412
+00000fc0: 322e 205b 444f 493a 2031 302e 3130 3633  2. [DOI: 10.1063
+00000fd0: 2f31 2e35 3039 3032 3232 5d28 6874 7470  /1.5090222](http
+00000fe0: 733a 2f2f 6478 2e64 6f69 2e6f 7267 2f31  s://dx.doi.org/1
+00000ff0: 302e 3130 3633 2f31 2e35 3039 3032 3232  0.1063/1.5090222
+00001000: 290a 2d20 452e 2043 616c 6465 7765 7968  ).- E. Caldeweyh
+00001010: 6572 2c20 4a2e 2d4d 2e20 4d65 7765 732c  er, J.-M. Mewes,
+00001020: 2053 2e20 4568 6c65 7274 2061 6e64 2053   S. Ehlert and S
+00001030: 2e20 4772 696d 6d65 2c20 2a50 6879 732e  . Grimme, *Phys.
+00001040: 2043 6865 6d2e 2043 6865 6d2e 2050 6879   Chem. Chem. Phy
+00001050: 732e 2a2c 2032 3032 302c 2032 322c 2038  s.*, 2020, 22, 8
+00001060: 3439 392d 3835 3132 2e20 5b44 4f49 3a20  499-8512. [DOI: 
+00001070: 3130 2e31 3033 392f 4430 4350 3030 3530  10.1039/D0CP0050
+00001080: 3241 5d28 6874 7470 733a 2f2f 646f 692e  2A](https://doi.
+00001090: 6f72 672f 3130 2e31 3033 392f 4430 4350  org/10.1039/D0CP
+000010a0: 3030 3530 3241 290a 0a46 6f72 2061 6c74  00502A)..For alt
+000010b0: 6572 6e61 7469 7665 2069 6d70 6c65 6d65  ernative impleme
+000010c0: 6e74 6174 696f 6e73 2c20 616c 736f 2063  ntations, also c
+000010d0: 6865 636b 206f 7574 3a0a 0a2d 205b 6466  heck out:..- [df
+000010e0: 7464 345d 2868 7474 7073 3a2f 2f64 6674  td4](https://dft
+000010f0: 6434 2e72 6561 6474 6865 646f 6373 2e69  d4.readthedocs.i
+00001100: 6f29 3a20 496d 706c 656d 656e 7461 7469  o): Implementati
+00001110: 6f6e 206f 6620 7468 6520 4446 542d 4434  on of the DFT-D4
+00001120: 2064 6973 7065 7273 696f 6e20 6d6f 6465   dispersion mode
+00001130: 6c20 696e 2046 6f72 7472 616e 2077 6974  l in Fortran wit
+00001140: 6820 5079 7468 6f6e 2062 696e 6469 6e67  h Python binding
+00001150: 732e 0a2d 205b 6370 702d 6434 5d28 6874  s..- [cpp-d4](ht
+00001160: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001170: 2f64 6674 6434 2f63 7070 2d64 3429 3a20  /dftd4/cpp-d4): 
+00001180: 496d 706c 656d 656e 7461 7469 6f6e 206f  Implementation o
+00001190: 6620 7468 6520 4446 542d 4434 2064 6973  f the DFT-D4 dis
+000011a0: 7065 7273 696f 6e20 6d6f 6465 6c20 696e  persion model in
+000011b0: 2043 2b2b 2e0a 0a23 2320 496e 7374 616c   C++...## Instal
+000011c0: 6c61 7469 6f6e 0a0a 2323 2320 7069 700a  lation..### pip.
+000011d0: 0a2a 7461 642d 6466 7464 342a 2063 616e  .*tad-dftd4* can
+000011e0: 2065 6173 696c 7920 6265 2069 6e73 7461   easily be insta
+000011f0: 6c6c 6564 2077 6974 6820 6060 7069 7060  lled with ``pip`
+00001200: 602e 0a0a 6060 6073 680a 7069 7020 696e  `...```sh.pip in
+00001210: 7374 616c 6c20 7461 642d 6466 7464 340a  stall tad-dftd4.
+00001220: 6060 600a 0a23 2323 2046 726f 6d20 736f  ```..### From so
+00001230: 7572 6365 0a0a 5468 6973 2070 726f 6a65  urce..This proje
+00001240: 6374 2069 7320 686f 7374 6564 206f 6e20  ct is hosted on 
+00001250: 4769 7448 7562 2061 7420 5b64 6674 6434  GitHub at [dftd4
+00001260: 2f74 6164 2d64 6674 6434 5d28 6874 7470  /tad-dftd4](http
+00001270: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00001280: 6674 6434 2f74 6164 2d64 6674 6434 292e  ftd4/tad-dftd4).
+00001290: 0a4f 6274 6169 6e20 7468 6520 736f 7572  .Obtain the sour
+000012a0: 6365 2062 7920 636c 6f6e 696e 6720 7468  ce by cloning th
+000012b0: 6520 7265 706f 7369 746f 7279 2077 6974  e repository wit
+000012c0: 680a 0a60 6060 7368 0a67 6974 2063 6c6f  h..```sh.git clo
+000012d0: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
+000012e0: 622e 636f 6d2f 6466 7464 342f 7461 642d  b.com/dftd4/tad-
+000012f0: 6466 7464 340a 6364 2074 6164 2d64 6674  dftd4.cd tad-dft
+00001300: 6434 0a60 6060 0a0a 5765 2072 6563 6f6d  d4.```..We recom
+00001310: 6d65 6e64 2075 7369 6e67 2061 205b 636f  mend using a [co
+00001320: 6e64 615d 2868 7474 7073 3a2f 2f63 6f6e  nda](https://con
+00001330: 6461 2e69 6f2f 2920 656e 7669 726f 6e6d  da.io/) environm
+00001340: 656e 7420 746f 2069 6e73 7461 6c6c 2074  ent to install t
+00001350: 6865 2070 6163 6b61 6765 2e0a 596f 7520  he package..You 
+00001360: 6361 6e20 7365 7475 7020 7468 6520 656e  can setup the en
+00001370: 7669 726f 6e6d 656e 7420 6d61 6e61 6765  vironment manage
+00001380: 7220 7573 696e 6720 6120 5b6d 616d 6261  r using a [mamba
+00001390: 666f 7267 655d 2868 7474 7073 3a2f 2f67  forge](https://g
+000013a0: 6974 6875 622e 636f 6d2f 636f 6e64 612d  ithub.com/conda-
+000013b0: 666f 7267 652f 6d69 6e69 666f 7267 6529  forge/miniforge)
+000013c0: 2069 6e73 7461 6c6c 6572 2e0a 496e 7374   installer..Inst
+000013d0: 616c 6c20 7468 6520 7265 7175 6972 6564  all the required
+000013e0: 2064 6570 656e 6465 6e63 6965 7320 6672   dependencies fr
+000013f0: 6f6d 2074 6865 2063 6f6e 6461 2d66 6f72  om the conda-for
+00001400: 6765 2063 6861 6e6e 656c 2e0a 0a60 6060  ge channel...```
+00001410: 7368 0a6d 616d 6261 2065 6e76 2063 7265  sh.mamba env cre
+00001420: 6174 6520 2d6e 2074 6f72 6368 202d 6620  ate -n torch -f 
+00001430: 656e 7669 726f 6e6d 656e 742e 7961 6d6c  environment.yaml
+00001440: 0a6d 616d 6261 2061 6374 6976 6174 6520  .mamba activate 
+00001450: 746f 7263 680a 6060 600a 0a49 6e73 7461  torch.```..Insta
+00001460: 6c6c 2074 6869 7320 7072 6f6a 6563 7420  ll this project 
+00001470: 7769 7468 2060 6070 6970 6060 2069 6e20  with ``pip`` in 
+00001480: 7468 6520 656e 7669 726f 6e6d 656e 740a  the environment.
+00001490: 0a60 6060 7368 0a70 6970 2069 6e73 7461  .```sh.pip insta
+000014a0: 6c6c 202e 0a60 6060 0a0a 5468 6520 666f  ll ..```..The fo
+000014b0: 6c6c 6f77 696e 6720 6465 7065 6e64 656e  llowing dependen
+000014c0: 6369 6573 2061 7265 2072 6571 7569 7265  cies are require
+000014d0: 640a 0a2d 205b 6e75 6d70 795d 2868 7474  d..- [numpy](htt
+000014e0: 7073 3a2f 2f6e 756d 7079 2e6f 7267 2f29  ps://numpy.org/)
+000014f0: 0a2d 205b 7461 642d 6d63 7463 5d28 6874  .- [tad-mctc](ht
+00001500: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001510: 2f74 6164 2d6d 6374 632f 7461 642d 6d63  /tad-mctc/tad-mc
+00001520: 7463 2f29 0a2d 205b 7461 642d 6d75 6c74  tc/).- [tad-mult
+00001530: 6963 6861 7267 655d 2868 7474 7073 3a2f  icharge](https:/
+00001540: 2f67 6974 6875 622e 636f 6d2f 7461 642d  /github.com/tad-
+00001550: 6d63 7463 2f74 6164 2d6d 756c 7469 6368  mctc/tad-multich
+00001560: 6172 6765 2f29 0a2d 205b 746f 7263 685d  arge/).- [torch]
+00001570: 2868 7474 7073 3a2f 2f70 7974 6f72 6368  (https://pytorch
+00001580: 2e6f 7267 2f29 0a2d 205b 7079 7465 7374  .org/).- [pytest
+00001590: 5d28 6874 7470 733a 2f2f 646f 6373 2e70  ](https://docs.p
+000015a0: 7974 6573 742e 6f72 672f 2920 2874 6573  ytest.org/) (tes
+000015b0: 7473 206f 6e6c 7929 0a0a 2323 2044 6576  ts only)..## Dev
+000015c0: 656c 6f70 6d65 6e74 0a0a 466f 7220 6465  elopment..For de
+000015d0: 7665 6c6f 706d 656e 742c 2061 6464 6974  velopment, addit
+000015e0: 696f 6e61 6c6c 7920 696e 7374 616c 6c20  ionally install 
+000015f0: 7468 6520 666f 6c6c 6f77 696e 6720 746f  the following to
+00001600: 6f6c 7320 696e 2079 6f75 7220 656e 7669  ols in your envi
+00001610: 726f 6e6d 656e 742e 0a0a 6060 6073 680a  ronment...```sh.
+00001620: 6d61 6d62 6120 696e 7374 616c 6c20 626c  mamba install bl
+00001630: 6163 6b20 636f 7664 6566 6175 6c74 7320  ack covdefaults 
+00001640: 6d79 7079 2070 7265 2d63 6f6d 6d69 7420  mypy pre-commit 
+00001650: 7079 6c69 6e74 2070 7974 6573 7420 7079  pylint pytest py
+00001660: 7465 7374 2d63 6f76 2070 7974 6573 742d  test-cov pytest-
+00001670: 7864 6973 7420 746f 780a 7069 7020 696e  xdist tox.pip in
+00001680: 7374 616c 6c20 7079 7465 7374 2d72 616e  stall pytest-ran
+00001690: 646f 6d2d 6f72 6465 720a 6060 600a 0a57  dom-order.```..W
+000016a0: 6974 6820 7069 702c 2061 6464 2074 6865  ith pip, add the
+000016b0: 206f 7074 696f 6e20 6060 2d65 6060 2066   option ``-e`` f
+000016c0: 6f72 2069 6e73 7461 6c6c 696e 6720 696e  or installing in
+000016d0: 2064 6576 656c 6f70 6d65 6e74 206d 6f64   development mod
+000016e0: 652c 2061 6e64 2061 6464 2060 605b 6465  e, and add ``[de
+000016f0: 765d 6060 2066 6f72 2074 6865 2064 6576  v]`` for the dev
+00001700: 656c 6f70 6d65 6e74 2064 6570 656e 6465  elopment depende
+00001710: 6e63 6965 730a 0a60 6060 7368 0a70 6970  ncies..```sh.pip
+00001720: 2069 6e73 7461 6c6c 202d 6520 2e5b 6465   install -e .[de
+00001730: 765d 0a60 6060 0a0a 5468 6520 7072 652d  v].```..The pre-
+00001740: 636f 6d6d 6974 2068 6f6f 6b73 2061 7265  commit hooks are
+00001750: 2069 6e69 7469 616c 697a 6564 2062 7920   initialized by 
+00001760: 7275 6e6e 696e 6720 7468 6520 666f 6c6c  running the foll
+00001770: 6f77 696e 6720 636f 6d6d 616e 6420 696e  owing command in
+00001780: 2074 6865 2072 6f6f 7420 6f66 2074 6865   the root of the
+00001790: 2072 6570 6f73 6974 6f72 792e 0a0a 6060   repository...``
+000017a0: 6073 680a 7072 652d 636f 6d6d 6974 2069  `sh.pre-commit i
+000017b0: 6e73 7461 6c6c 0a60 6060 0a0a 466f 7220  nstall.```..For 
+000017c0: 7465 7374 696e 6720 616c 6c20 5079 7468  testing all Pyth
+000017d0: 6f6e 2065 6e76 6972 6f6e 6d65 6e74 732c  on environments,
+000017e0: 2073 696d 706c 7920 7275 6e20 6074 6f78   simply run `tox
+000017f0: 602e 0a0a 6060 6073 680a 746f 780a 6060  `...```sh.tox.``
+00001800: 600a 0a4e 6f74 6520 7468 6174 2074 6869  `..Note that thi
+00001810: 7320 7261 6e64 6f6d 697a 6573 2074 6865  s randomizes the
+00001820: 206f 7264 6572 206f 6620 7465 7374 7320   order of tests 
+00001830: 6275 7420 736b 6970 7320 226c 6172 6765  but skips "large
+00001840: 2220 7465 7374 732e 2054 6f20 6d6f 6469  " tests. To modi
+00001850: 6679 2074 6869 7320 6265 6861 7669 6f72  fy this behavior
+00001860: 2c20 6074 6f78 6020 6861 7320 746f 2073  , `tox` has to s
+00001870: 6b69 7020 7468 6520 6f70 7469 6f6e 616c  kip the optional
+00001880: 202a 706f 7361 7267 732a 2e0a 0a60 6060   *posargs*...```
+00001890: 7368 0a74 6f78 202d 2d20 7465 7374 0a60  sh.tox -- test.`
+000018a0: 6060 0a0a 2323 2045 7861 6d70 6c65 730a  ``..## Examples.
+000018b0: 0a54 6865 2066 6f6c 6c6f 7769 6e67 2065  .The following e
+000018c0: 7861 6d70 6c65 2073 686f 7773 2068 6f77  xample shows how
+000018d0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+000018e0: 6520 4446 542d 4434 2064 6973 7065 7273  e DFT-D4 dispers
+000018f0: 696f 6e20 656e 6572 6779 2066 6f72 2061  ion energy for a
+00001900: 2073 696e 676c 6520 7374 7275 6374 7572   single structur
+00001910: 652e 0a0a 6060 6070 7974 686f 6e0a 696d  e...```python.im
+00001920: 706f 7274 2074 6f72 6368 0a69 6d70 6f72  port torch.impor
+00001930: 7420 7461 645f 6466 7464 3420 6173 2064  t tad_dftd4 as d
+00001940: 340a 696d 706f 7274 2074 6164 5f6d 6374  4.import tad_mct
+00001950: 6320 6173 206d 6374 630a 0a6e 756d 6265  c as mctc..numbe
+00001960: 7273 203d 206d 6374 632e 636f 6e76 6572  rs = mctc.conver
+00001970: 742e 7379 6d62 6f6c 5f74 6f5f 6e75 6d62  t.symbol_to_numb
+00001980: 6572 2873 796d 626f 6c73 3d22 4320 4320  er(symbols="C C 
+00001990: 4320 4320 4e20 4320 5320 4820 4820 4820  C C N C S H H H 
+000019a0: 4820 4822 2e73 706c 6974 2829 290a 0a23  H H".split())..#
+000019b0: 2063 6f6f 7264 696e 6174 6573 2069 6e20   coordinates in 
+000019c0: 426f 6872 0a70 6f73 6974 696f 6e73 203d  Bohr.positions =
+000019d0: 2074 6f72 6368 2e74 656e 736f 7228 0a20   torch.tensor(. 
+000019e0: 2020 205b 0a20 2020 2020 2020 205b 2d32     [.        [-2
+000019f0: 2e35 3637 3435 3638 3535 3634 3637 312c  .56745685564671,
+00001a00: 202d 302e 3032 3530 3939 3835 3937 3939   -0.025099859799
+00001a10: 3130 2c20 302e 3030 3030 3030 3030 3030  10, 0.0000000000
+00001a20: 3030 3030 5d2c 0a20 2020 2020 2020 205b  0000],.        [
+00001a30: 2d31 2e33 3931 3737 3538 3234 3535 3739  -1.3917758245579
+00001a40: 372c 202b 322e 3237 3639 3631 3838 3838  7, +2.2769618888
+00001a50: 3030 3134 2c20 302e 3030 3030 3030 3030  0014, 0.00000000
+00001a60: 3030 3030 3030 5d2c 0a20 2020 2020 2020  000000],.       
+00001a70: 205b 2b31 2e32 3737 3834 3939 3536 3234   [+1.27784995624
+00001a80: 3839 342c 202b 322e 3435 3130 3734 3739  894, +2.45107479
+00001a90: 3735 3933 3836 2c20 302e 3030 3030 3030  759386, 0.000000
+00001aa0: 3030 3030 3030 3030 5d2c 0a20 2020 2020  00000000],.     
+00001ab0: 2020 205b 2b32 2e36 3238 3031 3933 3736     [+2.628019376
+00001ac0: 3135 3739 332c 202b 302e 3235 3932 3737  15793, +0.259277
+00001ad0: 3237 3032 3831 3230 2c20 302e 3030 3030  27028120, 0.0000
+00001ae0: 3030 3030 3030 3030 3030 5d2c 0a20 2020  0000000000],.   
+00001af0: 2020 2020 205b 2b31 2e34 3130 3937 3033       [+1.4109703
+00001b00: 3336 3631 3132 332c 202d 312e 3939 3839  3661123, -1.9989
+00001b10: 3039 3936 3037 3734 3132 2c20 302e 3030  0996077412, 0.00
+00001b20: 3030 3030 3030 3030 3030 3030 5d2c 0a20  000000000000],. 
+00001b30: 2020 2020 2020 205b 2d31 2e31 3731 3836         [-1.17186
+00001b40: 3130 3232 3938 3834 392c 202d 322e 3334  102298849, -2.34
+00001b50: 3232 3035 3736 3238 3431 3830 2c20 302e  220576284180, 0.
+00001b60: 3030 3030 3030 3030 3030 3030 3030 5d2c  00000000000000],
+00001b70: 0a20 2020 2020 2020 205b 2d32 2e33 3935  .        [-2.395
+00001b80: 3035 3939 3033 3638 3337 382c 202d 352e  05990368378, -5.
+00001b90: 3232 3633 3538 3338 3333 3233 3632 2c20  22635838332362, 
+00001ba0: 302e 3030 3030 3030 3030 3030 3030 3030  0.00000000000000
+00001bb0: 5d2c 0a20 2020 2020 2020 205b 2b32 2e34  ],.        [+2.4
+00001bc0: 3139 3631 3938 3034 3535 3435 372c 202d  1961980455457, -
+00001bd0: 332e 3632 3135 3830 3139 3235 3330 3435  3.62158019253045
+00001be0: 2c20 302e 3030 3030 3030 3030 3030 3030  , 0.000000000000
+00001bf0: 3030 5d2c 0a20 2020 2020 2020 205b 2d32  00],.        [-2
+00001c00: 2e35 3137 3434 3337 3438 3436 3036 352c  .51744374846065,
+00001c10: 202b 332e 3938 3138 3137 3133 3638 3637   +3.981817136867
+00001c20: 3436 2c20 302e 3030 3030 3030 3030 3030  46, 0.0000000000
+00001c30: 3030 3030 5d2c 0a20 2020 2020 2020 205b  0000],.        [
+00001c40: 2b32 2e32 3432 3639 3034 3833 3834 3737  +2.2426904838477
+00001c50: 352c 202b 342e 3234 3338 3934 3733 3230  5, +4.2438947320
+00001c60: 3336 3437 2c20 302e 3030 3030 3030 3030  3647, 0.00000000
+00001c70: 3030 3030 3030 5d2c 0a20 2020 2020 2020  000000],.       
+00001c80: 205b 2b34 2e36 3634 3838 3938 3435 3733   [+4.66488984573
+00001c90: 3935 362c 202b 302e 3137 3930 3735 3638  956, +0.17907568
+00001ca0: 3030 3634 3039 2c20 302e 3030 3030 3030  006409, 0.000000
+00001cb0: 3030 3030 3030 3030 5d2c 0a20 2020 2020  00000000],.     
+00001cc0: 2020 205b 2d34 2e36 3030 3434 3234 3437     [-4.600442447
+00001cd0: 3832 3233 372c 202d 302e 3137 3739 3437  82237, -0.177947
+00001ce0: 3334 3633 3734 3133 2c20 302e 3030 3030  34637413, 0.0000
+00001cf0: 3030 3030 3030 3030 3030 5d2c 0a20 2020  0000000000],.   
+00001d00: 205d 0a29 0a0a 2320 746f 7461 6c20 6368   ].)..# total ch
+00001d10: 6172 6765 206f 6620 7468 6520 7379 7374  arge of the syst
+00001d20: 656d 0a63 6861 7267 6520 3d20 746f 7263  em.charge = torc
+00001d30: 682e 7465 6e73 6f72 2830 2e30 290a 0a23  h.tensor(0.0)..#
+00001d40: 2054 5053 5368 2d44 342d 4154 4d20 7061   TPSSh-D4-ATM pa
+00001d50: 7261 6d65 7465 7273 0a70 6172 616d 203d  rameters.param =
+00001d60: 207b 0a20 2020 2022 7336 223a 2070 6f73   {.    "s6": pos
+00001d70: 6974 696f 6e73 2e6e 6577 5f74 656e 736f  itions.new_tenso
+00001d80: 7228 312e 3029 2c0a 2020 2020 2273 3822  r(1.0),.    "s8"
+00001d90: 3a20 706f 7369 7469 6f6e 732e 6e65 775f  : positions.new_
+00001da0: 7465 6e73 6f72 2831 2e38 3538 3937 3735  tensor(1.8589775
+00001db0: 3029 2c0a 2020 2020 2273 3922 3a20 706f  0),.    "s9": po
+00001dc0: 7369 7469 6f6e 732e 6e65 775f 7465 6e73  sitions.new_tens
+00001dd0: 6f72 2831 2e30 292c 0a20 2020 2022 6131  or(1.0),.    "a1
+00001de0: 223a 2070 6f73 6974 696f 6e73 2e6e 6577  ": positions.new
+00001df0: 5f74 656e 736f 7228 302e 3434 3238 3639  _tensor(0.442869
+00001e00: 3636 292c 0a20 2020 2022 6132 223a 2070  66),.    "a2": p
+00001e10: 6f73 6974 696f 6e73 2e6e 6577 5f74 656e  ositions.new_ten
+00001e20: 736f 7228 342e 3630 3233 3035 3334 292c  sor(4.60230534),
+00001e30: 0a7d 0a0a 656e 6572 6779 203d 2064 342e  .}..energy = d4.
+00001e40: 6466 7464 3428 6e75 6d62 6572 732c 2070  dftd4(numbers, p
+00001e50: 6f73 6974 696f 6e73 2c20 6368 6172 6765  ositions, charge
+00001e60: 2c20 7061 7261 6d29 0a74 6f72 6368 2e73  , param).torch.s
+00001e70: 6574 5f70 7269 6e74 6f70 7469 6f6e 7328  et_printoptions(
+00001e80: 7072 6563 6973 696f 6e3d 3130 290a 7072  precision=10).pr
+00001e90: 696e 7428 656e 6572 6779 290a 2320 7465  int(energy).# te
+00001ea0: 6e73 6f72 285b 2d30 2e30 3032 3038 3431  nsor([-0.0020841
+00001eb0: 3334 342c 202d 302e 3030 3138 3937 3131  344, -0.00189711
+00001ec0: 3935 2c20 2d30 2e30 3031 3831 3037 3531  95, -0.001810751
+00001ed0: 332c 202d 302e 3030 3138 3330 3536 3935  3, -0.0018305695
+00001ee0: 2c0a 2320 2020 2020 2020 2020 2d30 2e30  ,.#         -0.0
+00001ef0: 3032 3137 3337 3639 332c 202d 302e 3030  021737693, -0.00
+00001f00: 3139 3438 3432 3336 2c20 2d30 2e30 3032  19484236, -0.002
+00001f10: 3237 3838 3235 332c 202d 302e 3030 3034  2788253, -0.0004
+00001f20: 3038 3036 3538 2c0a 2320 2020 2020 2020  080658,.#       
+00001f30: 2020 2d30 2e30 3030 3432 3631 3836 362c    -0.0004261866,
+00001f40: 202d 302e 3030 3034 3139 3938 3339 2c20   -0.0004199839, 
+00001f50: 2d30 2e30 3030 3432 3830 3736 382c 202d  -0.0004280768, -
+00001f60: 302e 3030 3035 3130 3839 3335 5d29 0a60  0.0005108935]).`
+00001f70: 6060 0a0a 5468 6520 6e65 7874 2065 7861  ``..The next exa
+00001f80: 6d70 6c65 2073 686f 7773 2074 6865 2063  mple shows the c
+00001f90: 616c 6375 6c61 7469 6f6e 206f 6620 6469  alculation of di
+00001fa0: 7370 6572 7369 6f6e 2065 6e65 7267 6965  spersion energie
+00001fb0: 7320 666f 7220 6120 6261 7463 6820 6f66  s for a batch of
+00001fc0: 2073 7472 7563 7475 7265 732e 0a0a 6060   structures...``
+00001fd0: 6070 7974 686f 6e0a 0a69 6d70 6f72 7420  `python..import 
+00001fe0: 746f 7263 680a 696d 706f 7274 2074 6164  torch.import tad
+00001ff0: 5f64 6674 6434 2061 7320 6434 0a69 6d70  _dftd4 as d4.imp
+00002000: 6f72 7420 7461 645f 6d63 7463 2061 7320  ort tad_mctc as 
+00002010: 6d63 7463 0a0a 2320 5332 3220 7379 7374  mctc..# S22 syst
+00002020: 656d 2034 3a20 666f 726d 616d 6964 6520  em 4: formamide 
+00002030: 6469 6d65 720a 6e75 6d62 6572 7320 3d20  dimer.numbers = 
+00002040: 6d63 7463 2e62 6174 6368 2e70 6163 6b28  mctc.batch.pack(
+00002050: 280a 2020 2020 6d63 7463 2e63 6f6e 7665  (.    mctc.conve
+00002060: 7274 2e73 796d 626f 6c5f 746f 5f6e 756d  rt.symbol_to_num
+00002070: 6265 7228 2243 2043 204e 204e 2048 2048  ber("C C N N H H
+00002080: 2048 2048 2048 2048 204f 204f 222e 7370   H H H H O O".sp
+00002090: 6c69 7428 2929 2c0a 2020 2020 6d63 7463  lit()),.    mctc
+000020a0: 2e63 6f6e 7665 7274 2e73 796d 626f 6c5f  .convert.symbol_
+000020b0: 746f 5f6e 756d 6265 7228 2243 204f 204e  to_number("C O N
+000020c0: 2048 2048 2048 222e 7370 6c69 7428 2929   H H H".split())
+000020d0: 2c0a 2929 0a0a 2320 636f 6f72 6469 6e61  ,.))..# coordina
+000020e0: 7465 7320 696e 2042 6f68 720a 706f 7369  tes in Bohr.posi
+000020f0: 7469 6f6e 7320 3d20 6d63 7463 2e62 6174  tions = mctc.bat
+00002100: 6368 2e70 6163 6b28 280a 2020 2020 746f  ch.pack((.    to
+00002110: 7263 682e 7465 6e73 6f72 285b 0a20 2020  rch.tensor([.   
+00002120: 2020 2020 205b 2d33 2e38 3134 3639 3438       [-3.8146948
+00002130: 3831 3433 3932 312c 202b 302e 3039 3939  8143921, +0.0999
+00002140: 3334 3431 3430 3239 3132 2c20 302e 3030  3441402912, 0.00
+00002150: 3030 3030 3030 3030 3030 3030 5d2c 0a20  000000000000],. 
+00002160: 2020 2020 2020 205b 2b33 2e38 3134 3639         [+3.81469
+00002170: 3438 3831 3433 3932 312c 202d 302e 3039  488143921, -0.09
+00002180: 3939 3334 3431 3430 3239 3132 2c20 302e  993441402912, 0.
+00002190: 3030 3030 3030 3030 3030 3030 3030 5d2c  00000000000000],
+000021a0: 0a20 2020 2020 2020 205b 2d32 2e36 3630  .        [-2.660
+000021b0: 3330 3034 3933 3234 3033 362c 202d 322e  30049324036, -2.
+000021c0: 3135 3839 3832 3531 3533 3335 3038 2c20  15898251533508, 
+000021d0: 302e 3030 3030 3030 3030 3030 3030 3030  0.00000000000000
+000021e0: 5d2c 0a20 2020 2020 2020 205b 2b32 2e36  ],.        [+2.6
+000021f0: 3630 3330 3034 3933 3234 3033 362c 202b  6030049324036, +
+00002200: 322e 3135 3839 3832 3531 3533 3335 3038  2.15898251533508
+00002210: 2c20 302e 3030 3030 3030 3030 3030 3030  , 0.000000000000
+00002220: 3030 5d2c 0a20 2020 2020 2020 205b 2d30  00],.        [-0
+00002230: 2e37 3331 3738 3532 3937 3339 3338 302c  .73178529739380,
+00002240: 202d 322e 3238 3233 3737 3935 3832 3937   -2.282377958297
+00002250: 3733 2c20 302e 3030 3030 3030 3030 3030  73, 0.0000000000
+00002260: 3030 3030 5d2c 0a20 2020 2020 2020 205b  0000],.        [
+00002270: 2d35 2e38 3930 3339 3332 3537 3134 3131  -5.8903932571411
+00002280: 312c 202d 302e 3032 3538 3931 3134 3536  1, -0.0258911456
+00002290: 3931 3238 2c20 302e 3030 3030 3030 3030  9128, 0.00000000
+000022a0: 3030 3030 3030 5d2c 0a20 2020 2020 2020  000000],.       
+000022b0: 205b 2d33 2e37 3132 3534 3934 3438 3031   [-3.71254944801
+000022c0: 3333 312c 202d 332e 3733 3630 3537 3735  331, -3.73605775
+000022d0: 3833 3331 3330 2c20 302e 3030 3030 3030  833130, 0.000000
+000022e0: 3030 3030 3030 3030 5d2c 0a20 2020 2020  00000000],.     
+000022f0: 2020 205b 2b33 2e37 3132 3534 3934 3438     [+3.712549448
+00002300: 3031 3333 312c 202b 332e 3733 3630 3537  01331, +3.736057
+00002310: 3735 3833 3331 3330 2c20 302e 3030 3030  75833130, 0.0000
+00002320: 3030 3030 3030 3030 3030 5d2c 0a20 2020  0000000000],.   
+00002330: 2020 2020 205b 2b30 2e37 3331 3738 3532       [+0.7317852
+00002340: 3937 3339 3338 302c 202b 322e 3238 3233  9739380, +2.2823
+00002350: 3737 3935 3832 3937 3733 2c20 302e 3030  7795829773, 0.00
+00002360: 3030 3030 3030 3030 3030 3030 5d2c 0a20  000000000000],. 
+00002370: 2020 2020 2020 205b 2b35 2e38 3930 3339         [+5.89039
+00002380: 3332 3537 3134 3131 312c 202b 302e 3032  325714111, +0.02
+00002390: 3538 3931 3134 3536 3931 3238 2c20 302e  589114569128, 0.
+000023a0: 3030 3030 3030 3030 3030 3030 3030 5d2c  00000000000000],
+000023b0: 0a20 2020 2020 2020 205b 2d32 2e37 3434  .        [-2.744
+000023c0: 3236 3130 3236 3338 3234 352c 202b 322e  26102638245, +2.
+000023d0: 3136 3131 3535 3730 3036 3833 3539 2c20  16115570068359, 
+000023e0: 302e 3030 3030 3030 3030 3030 3030 3030  0.00000000000000
+000023f0: 5d2c 0a20 2020 2020 2020 205b 2b32 2e37  ],.        [+2.7
+00002400: 3434 3236 3130 3236 3338 3234 352c 202d  4426102638245, -
+00002410: 322e 3136 3131 3535 3730 3036 3833 3539  2.16115570068359
+00002420: 2c20 302e 3030 3030 3030 3030 3030 3030  , 0.000000000000
+00002430: 3030 5d2c 0a20 2020 205d 292c 0a20 2020  00],.    ]),.   
+00002440: 2074 6f72 6368 2e74 656e 736f 7228 5b0a   torch.tensor([.
+00002450: 2020 2020 2020 2020 5b2d 302e 3535 3536          [-0.5556
+00002460: 3937 3433 3230 3334 3036 2c20 2b31 2e30  9743203406, +1.0
+00002470: 3930 3330 3432 3534 3638 3535 372c 2030  9030425468557, 0
+00002480: 2e30 3030 3030 3030 3030 3030 3030 305d  .00000000000000]
+00002490: 2c0a 2020 2020 2020 2020 5b2b 302e 3531  ,.        [+0.51
+000024a0: 3437 3336 3334 3637 3834 3639 2c20 2b33  473634678469, +3
+000024b0: 2e31 3531 3532 3535 3032 3633 3631 312c  .15152550263611,
+000024c0: 2030 2e30 3030 3030 3030 3030 3030 3030   0.0000000000000
+000024d0: 305d 2c0a 2020 2020 2020 2020 5b2b 302e  0],.        [+0.
+000024e0: 3539 3836 3936 3930 3234 3434 3436 2c20  59869690244446, 
+000024f0: 2d31 2e31 3638 3631 3236 3337 3839 3437  -1.1686126378947
+00002500: 372c 2030 2e30 3030 3030 3030 3030 3030  7, 0.00000000000
+00002510: 3030 305d 2c0a 2020 2020 2020 2020 5b2d  000],.        [-
+00002520: 302e 3435 3335 3532 3033 3636 3931 3334  0.45355203669134
+00002530: 2c20 2d32 2e37 3435 3638 3738 3034 3338  , -2.74568780438
+00002540: 3036 342c 2030 2e30 3030 3030 3030 3030  064, 0.000000000
+00002550: 3030 3030 305d 2c0a 2020 2020 2020 2020  00000],.        
+00002560: 5b2b 322e 3532 3732 3132 3039 3534 3439  [+2.527212095449
+00002570: 3939 2c20 2d31 2e32 3932 3030 3830 3039  99, -1.292008009
+00002580: 3536 3836 372c 2030 2e30 3030 3030 3030  56867, 0.0000000
+00002590: 3030 3030 3030 305d 2c0a 2020 2020 2020  0000000],.      
+000025a0: 2020 5b2d 322e 3633 3133 3935 3837 3539    [-2.6313958759
+000025b0: 3533 3736 2c20 2b30 2e39 3634 3437 3836  5376, +0.9644786
+000025c0: 3934 3532 3234 302c 2030 2e30 3030 3030  9452240, 0.00000
+000025d0: 3030 3030 3030 3030 305d 2c0a 2020 2020  000000000],.    
+000025e0: 5d29 2c0a 2929 0a0a 2320 746f 7461 6c20  ]),.))..# total 
+000025f0: 6368 6172 6765 206f 6620 626f 7468 2073  charge of both s
+00002600: 7973 7465 6d0a 6368 6172 6765 203d 2074  ystem.charge = t
+00002610: 6f72 6368 2e74 656e 736f 7228 5b30 2e30  orch.tensor([0.0
+00002620: 2c20 302e 305d 290a 0a23 2054 5053 5368  , 0.0])..# TPSSh
+00002630: 2d44 342d 4154 4d20 7061 7261 6d65 7465  -D4-ATM paramete
+00002640: 7273 0a70 6172 616d 203d 207b 0a20 2020  rs.param = {.   
+00002650: 2022 7336 223a 2070 6f73 6974 696f 6e73   "s6": positions
+00002660: 2e6e 6577 5f74 656e 736f 7228 312e 3029  .new_tensor(1.0)
+00002670: 2c0a 2020 2020 2273 3822 3a20 706f 7369  ,.    "s8": posi
+00002680: 7469 6f6e 732e 6e65 775f 7465 6e73 6f72  tions.new_tensor
+00002690: 2831 2e38 3538 3937 3735 3029 2c0a 2020  (1.85897750),.  
+000026a0: 2020 2273 3922 3a20 706f 7369 7469 6f6e    "s9": position
+000026b0: 732e 6e65 775f 7465 6e73 6f72 2831 2e30  s.new_tensor(1.0
+000026c0: 292c 0a20 2020 2022 6131 223a 2070 6f73  ),.    "a1": pos
+000026d0: 6974 696f 6e73 2e6e 6577 5f74 656e 736f  itions.new_tenso
+000026e0: 7228 302e 3434 3238 3639 3636 292c 0a20  r(0.44286966),. 
+000026f0: 2020 2022 6132 223a 2070 6f73 6974 696f     "a2": positio
+00002700: 6e73 2e6e 6577 5f74 656e 736f 7228 342e  ns.new_tensor(4.
+00002710: 3630 3233 3035 3334 292c 0a7d 0a0a 2320  60230534),.}..# 
+00002720: 6361 6c63 756c 6174 6520 6469 7370 6572  calculate disper
+00002730: 7369 6f6e 2065 6e65 7267 7920 696e 2048  sion energy in H
+00002740: 6172 7472 6565 0a65 6e65 7267 7920 3d20  artree.energy = 
+00002750: 746f 7263 682e 7375 6d28 6434 2e64 6674  torch.sum(d4.dft
+00002760: 6434 286e 756d 6265 7273 2c20 706f 7369  d4(numbers, posi
+00002770: 7469 6f6e 732c 2063 6861 7267 652c 2070  tions, charge, p
+00002780: 6172 616d 292c 202d 3129 0a74 6f72 6368  aram), -1).torch
+00002790: 2e73 6574 5f70 7269 6e74 6f70 7469 6f6e  .set_printoption
+000027a0: 7328 7072 6563 6973 696f 6e3d 3130 290a  s(precision=10).
+000027b0: 7072 696e 7428 656e 6572 6779 290a 2320  print(energy).# 
+000027c0: 7465 6e73 6f72 285b 2d30 2e30 3038 3833  tensor([-0.00883
+000027d0: 3431 3433 322c 202d 302e 3030 3237 3031  41432, -0.002701
+000027e0: 3336 3037 5d29 0a70 7269 6e74 2865 6e65  3607]).print(ene
+000027f0: 7267 795b 305d 202d 2032 2a65 6e65 7267  rgy[0] - 2*energ
+00002800: 795b 315d 290a 2320 7465 6e73 6f72 282d  y[1]).# tensor(-
+00002810: 302e 3030 3334 3331 3432 3137 290a 6060  0.0034314217).``
+00002820: 600a 0a23 2320 436f 6e74 7269 6275 7469  `..## Contributi
+00002830: 6e67 0a0a 5468 6973 2069 7320 6120 766f  ng..This is a vo
+00002840: 6c75 6e74 6565 7220 6f70 656e 2073 6f75  lunteer open sou
+00002850: 7263 6520 7072 6f6a 6563 7473 2061 6e64  rce projects and
+00002860: 2063 6f6e 7472 6962 7574 696f 6e73 2061   contributions a
+00002870: 7265 2061 6c77 6179 7320 7765 6c63 6f6d  re always welcom
+00002880: 652e 0a50 6c65 6173 652c 2074 616b 6520  e..Please, take 
+00002890: 6120 6d6f 6d65 6e74 2074 6f20 7265 6164  a moment to read
+000028a0: 2074 6865 205b 636f 6e74 7269 6275 7469   the [contributi
+000028b0: 6e67 2067 7569 6465 6c69 6e65 735d 2843  ng guidelines](C
+000028c0: 4f4e 5452 4942 5554 494e 472e 6d64 292e  ONTRIBUTING.md).
+000028d0: 0a0a 2323 204c 6963 656e 7365 0a0a 5468  ..## License..Th
+000028e0: 6973 2070 726f 6a65 6374 2069 7320 6c69  is project is li
+000028f0: 6365 6e73 6564 2075 6e64 6572 2074 6865  censed under the
+00002900: 2041 7061 6368 6520 4c69 6365 6e73 652c   Apache License,
+00002910: 2056 6572 7369 6f6e 2032 2e30 2028 7468   Version 2.0 (th
+00002920: 6520 224c 6963 656e 7365 2229 3b20 796f  e "License"); yo
+00002930: 7520 6d61 7920 6e6f 7420 7573 6520 7468  u may not use th
+00002940: 6973 2070 726f 6a65 6374 2773 2066 696c  is project's fil
+00002950: 6573 2065 7863 6570 7420 696e 2063 6f6d  es except in com
+00002960: 706c 6961 6e63 6520 7769 7468 2074 6865  pliance with the
+00002970: 204c 6963 656e 7365 2e20 596f 7520 6d61   License. You ma
+00002980: 7920 6f62 7461 696e 2061 2063 6f70 7920  y obtain a copy 
+00002990: 6f66 2074 6865 204c 6963 656e 7365 2061  of the License a
+000029a0: 740a 0a68 7474 703a 2f2f 7777 772e 6170  t..http://www.ap
+000029b0: 6163 6865 2e6f 7267 2f6c 6963 656e 7365  ache.org/license
+000029c0: 732f 4c49 4345 4e53 452d 322e 300a 0a55  s/LICENSE-2.0..U
+000029d0: 6e6c 6573 7320 7265 7175 6972 6564 2062  nless required b
+000029e0: 7920 6170 706c 6963 6162 6c65 206c 6177  y applicable law
+000029f0: 206f 7220 6167 7265 6564 2074 6f20 696e   or agreed to in
+00002a00: 2077 7269 7469 6e67 2c20 736f 6674 7761   writing, softwa
+00002a10: 7265 2064 6973 7472 6962 7574 6564 2075  re distributed u
+00002a20: 6e64 6572 2074 6865 204c 6963 656e 7365  nder the License
+00002a30: 2069 7320 6469 7374 7269 6275 7465 6420   is distributed 
+00002a40: 6f6e 2061 6e20 2241 5320 4953 2220 4241  on an "AS IS" BA
+00002a50: 5349 532c 2057 4954 484f 5554 2057 4152  SIS, WITHOUT WAR
+00002a60: 5241 4e54 4945 5320 4f52 2043 4f4e 4449  RANTIES OR CONDI
+00002a70: 5449 4f4e 5320 4f46 2041 4e59 204b 494e  TIONS OF ANY KIN
+00002a80: 442c 2065 6974 6865 7220 6578 7072 6573  D, either expres
+00002a90: 7320 6f72 2069 6d70 6c69 6564 2e20 5365  s or implied. Se
+00002aa0: 6520 7468 6520 4c69 6365 6e73 6520 666f  e the License fo
+00002ab0: 7220 7468 6520 7370 6563 6966 6963 206c  r the specific l
+00002ac0: 616e 6775 6167 6520 676f 7665 726e 696e  anguage governin
+00002ad0: 6720 7065 726d 6973 7369 6f6e 7320 616e  g permissions an
+00002ae0: 6420 6c69 6d69 7461 7469 6f6e 7320 756e  d limitations un
+00002af0: 6465 7220 7468 6520 4c69 6365 6e73 652e  der the License.
+00002b00: 0a                                       .
```

### Comparing `tad_dftd4-0.0.4/setup.cfg` & `tad_dftd4-0.1.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 [metadata]
 name = tad_dftd4
 version = attr: tad_dftd4.__version__.__version__
 description = Torch autodiff DFT-D4 implementation
-long_description = file: README.rst
-long_description_content_type = text/x-rst
+long_description = file: README.md
+long_description_content_type = text/markdown
 author = "Marvin Friede"
-license = LGPL-3.0
-license_files = 
-	COPYING
-	COPYING.LESSER
+license = Apache-2.0
+license_files = LICENSE
 classifiers = 
 	Framework :: Pytest
-	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
@@ -23,33 +21,46 @@
 	Topic :: Scientific/Engineering
 	Typing :: Typed
 
 [options]
 packages = find:
 install_requires = 
 	numpy
-	torch
+	tad-mctc
+	tad-multicharge
+	torch>=1.11
 python_requires = >=3.8
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 dev = 
 	black
 	covdefaults
-	coverage
+	mypy
 	pre-commit
 	pylint
 	pytest
+	pytest-cov
+	pytest-random-order
+	pytest-xdist
 	tox
+tox = 
+	covdefaults
+	pytest
+	pytest-cov
+	pytest-random-order
+	pytest-xdist
 
 [options.package_data]
-squarer = 
+tad_dftd4 = 
 	py.typed
+	**/*.npy
+	**/*.npz
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `tad_dftd4-0.0.4/src/tad_dftd4/__init__.py` & `tad_dftd4-0.1.0/src/tad_dftd4/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # This file is part of tad-dftd4.
 #
-# SPDX-Identifier: LGPL-3.0
-# Copyright (C) 2022 Marvin Friede
+# SPDX-Identifier: Apache-2.0
+# Copyright (C) 2024 Grimme Group
 #
-# tad-dftd4 is free software: you can redistribute it and/or modify it under
-# the terms of the GNU Lesser General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# tad-dftd4 is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Lesser General Public License for more details.
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with tad-dftd4. If not, see <https://www.gnu.org/licenses/>.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 """
 Torch autodiff DFT-D4
 =====================
 
 Implementation of the DFT-D4 dispersion model in PyTorch.
 This module allows to process a single structure or a batch of structures for
 the calculation of atom-resolved dispersion energies.
@@ -29,23 +28,24 @@
    Contributions are welcome, please checkout our
    `contributing guidelines <https://github.com/dftd4/tad-dftd4/blob/main/CONTRIBUTING.md>`_.
 
 Example
 -------
 >>> import torch
 >>> import tad_dftd4 as d4
+>>> import tad_mctc as mctc
 >>>
 >>> # S22 system 4: formamide dimer
->>> numbers = d4.utils.pack((
-...     d4.utils.to_number("C C N N H H H H H H O O".split()),
-...     d4.utils.to_number("C O N H H H".split()),
+>>> numbers = mctc.batch.pack((
+...     mctc.convert.symbol_to_number("C C N N H H H H H H O O".split()),
+...     mctc.convert.symbol_to_number("C O N H H H".split()),
 ... ))
 >>>
 >>> # coordinates in Bohr
->>> positions = d4.utils.pack((
+>>> positions = mctc.batch.pack((
 ...     torch.tensor([
 ...         [-3.81469488143921, +0.09993441402912, 0.00000000000000],
 ...         [+3.81469488143921, -0.09993441402912, 0.00000000000000],
 ...         [-2.66030049324036, -2.15898251533508, 0.00000000000000],
 ...         [+2.66030049324036, +2.15898251533508, 0.00000000000000],
 ...         [-0.73178529739380, -2.28237795829773, 0.00000000000000],
 ...         [-5.89039325714111, -0.02589114569128, 0.00000000000000],
@@ -65,15 +65,15 @@
 ...         [-2.63139587595376, +0.96447869452240, 0.00000000000000],
 ...     ]),
 ... ))
 >>>
 >>> # total charge of both systems
 >>> charge = torch.tensor([0.0, 0.0])
 >>>
->>> # TPSS0-D4-ATM parameters
+>>> # TPSSh-D4-ATM parameters
 >>> param = {
 ...     "s6": positions.new_tensor(1.0),
 ...     "s8": positions.new_tensor(1.85897750),
 ...     "s9": positions.new_tensor(1.0),
 ...     "a1": positions.new_tensor(0.44286966),
 ...     "a2": positions.new_tensor(4.60230534),
 ... }
@@ -84,11 +84,22 @@
 >>> print(energy)
 tensor([-0.0088341432, -0.0027013607])
 >>> print(energy[0] - 2*energy[1])
 tensor(-0.0034314217)
 """
 import torch
 
-from . import charges, cutoff, damping, data, disp, model, ncoord, utils
+from . import cutoff, damping, data, disp, model, ncoord, typing
 from .__version__ import __version__
-from ._typing import CountingFunction, DampingFunction, Tensor
 from .disp import dftd4
+
+__all__ = [
+    "__version__",
+    "cutoff",
+    "damping",
+    "data",
+    "dftd4",
+    "disp",
+    "model",
+    "ncoord",
+    "typing",
+]
```

### Comparing `tad_dftd4-0.0.4/src/tad_dftd4/cutoff.py` & `tad_dftd4-0.1.0/src/tad_dftd4/cutoff.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # This file is part of tad-dftd4.
 #
-# SPDX-Identifier: LGPL-3.0
-# Copyright (C) 2022 Marvin Friede
+# SPDX-Identifier: Apache-2.0
+# Copyright (C) 2024 Grimme Group
 #
-# tad-dftd4 is free software: you can redistribute it and/or modify it under
-# the terms of the GNU Lesser General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# tad-dftd4 is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Lesser General Public License for more details.
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with tad-dftd4. If not, see <https://www.gnu.org/licenses/>.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 """
 Cutoff
 ======
 
 Real-space cutoffs for the two-body and three-body dispersion energy
 as well as the coordination number within D4 and the EEQ Model.
 """
 from __future__ import annotations
 
 import torch
 
 from . import defaults
-from ._typing import Tensor, TensorLike
+from .typing import Tensor, TensorLike
+
+__all__ = ["Cutoff"]
 
 
 class Cutoff(TensorLike):
     """
     Collection of real-space cutoffs.
     """
```

### Comparing `tad_dftd4-0.0.4/src/tad_dftd4/damping/atm.py` & `tad_dftd4-0.1.0/src/tad_dftd4/damping/atm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # This file is part of tad-dftd4.
 #
-# SPDX-Identifier: LGPL-3.0
-# Copyright (C) 2022 Marvin Friede
+# SPDX-Identifier: Apache-2.0
+# Copyright (C) 2024 Grimme Group
 #
-# tad-dftd4 is free software: you can redistribute it and/or modify it under
-# the terms of the GNU Lesser General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# tad-dftd4 is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Lesser General Public License for more details.
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with tad-dftd4. If not, see <https://www.gnu.org/licenses/>.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 r"""
 Axilrod-Teller-Muto (ATM) dispersion term
 =========================================
 
 This module provides the dispersion energy evaluation for the three-body
 Axilrod-Teller-Muto dispersion term.
 
@@ -32,19 +31,21 @@
     {\left(r_\text{AB} r_\text{BC} r_\text{AC} \right)^3} \\
     f_\text{damp} &=
     \dfrac{1}{1+ 6 \left(\overline{R}_\text{ABC}\right)^{-16}}
 """
 from __future__ import annotations
 
 import torch
+from tad_mctc import storch
+from tad_mctc.batch import real_pairs, real_triples
 
-from .. import defaults
-from .._typing import Tensor
-from ..data import r4r2
-from ..utils import real_pairs, real_triples
+from .. import data, defaults
+from ..typing import DD, Tensor
+
+__all__ = ["get_atm_dispersion"]
 
 
 def get_atm_dispersion(
     numbers: Tensor,
     positions: Tensor,
     cutoff: Tensor,
     c6: Tensor,
@@ -78,63 +79,82 @@
         Exponent of zero damping function. Defaults to `14.0`.
 
     Returns
     -------
     Tensor
         Atom-resolved ATM dispersion energy.
     """
-    dd = {"device": positions.device, "dtype": positions.dtype}
+    dd: DD = {"device": positions.device, "dtype": positions.dtype}
 
-    s9 = s9.type(positions.dtype).to(positions.device)
-    alp = alp.type(positions.dtype).to(positions.device)
+    s9 = s9.to(**dd)
+    alp = alp.to(**dd)
 
     cutoff2 = cutoff * cutoff
 
+    mask_pairs = real_pairs(numbers, mask_diagonal=True)
+    mask_triples = real_triples(numbers, mask_diagonal=True, mask_self=True)
+
+    # filler values for masks
+    eps = torch.tensor(torch.finfo(positions.dtype).eps, **dd)
+    zero = torch.tensor(0.0, **dd)
+    one = torch.tensor(1.0, **dd)
+
     # C9_ABC = s9 * sqrt(|C6_AB * C6_AC * C6_BC|)
-    c9 = s9 * torch.sqrt(
-        torch.abs(c6.unsqueeze(-1) * c6.unsqueeze(-2) * c6.unsqueeze(-3))
+    c9 = s9 * storch.sqrt(
+        torch.abs(c6.unsqueeze(-1) * c6.unsqueeze(-2) * c6.unsqueeze(-3)),
     )
 
-    temp = (
-        a1 * torch.sqrt(3.0 * r4r2[numbers].unsqueeze(-1) * r4r2[numbers].unsqueeze(-2))
-        + a2
-    )
+    rad = data.R4R2[numbers]
+    radii = rad.unsqueeze(-1) * rad.unsqueeze(-2)
+    temp = a1 * storch.sqrt(3.0 * radii) + a2
+
     r0ij = temp.unsqueeze(-1)
     r0ik = temp.unsqueeze(-2)
     r0jk = temp.unsqueeze(-3)
     r0 = r0ij * r0ik * r0jk
 
     # actually faster than other alternatives
     # very slow: (pos.unsqueeze(-2) - pos.unsqueeze(-3)).pow(2).sum(-1)
     distances = torch.pow(
         torch.where(
-            real_pairs(numbers, diagonal=False),
-            torch.cdist(
-                positions, positions, p=2, compute_mode="use_mm_for_euclid_dist"
-            ),
-            torch.tensor(torch.finfo(positions.dtype).eps, **dd),
+            mask_pairs,
+            storch.cdist(positions, positions, p=2),
+            eps,
         ),
         2.0,
     )
 
     r2ij = distances.unsqueeze(-1)
     r2ik = distances.unsqueeze(-2)
     r2jk = distances.unsqueeze(-3)
     r2 = r2ij * r2ik * r2jk
     r1 = torch.sqrt(r2)
-    r3 = r1 * r2
-    r5 = r2 * r3
+    # add epsilon to avoid zero division later
+    r3 = torch.where(mask_triples, r1 * r2, eps)
+    r5 = torch.where(mask_triples, r2 * r3, eps)
+
+    # dividing by tiny numbers leads to huge numbers, which result in NaN's
+    # upon exponentiation in the subsequent step
+    base = r0 / torch.where(mask_triples, r1, one)
+
+    # to fix the previous mask, we mask again (not strictly necessary because
+    # `ang` is also masked and we later multiply with `ang`)
+    fdamp = torch.where(
+        mask_triples,
+        1.0 / (1.0 + 6.0 * base ** (alp / 3.0)),
+        zero,
+    )
 
-    fdamp = 1.0 / (1.0 + 6.0 * (r0 / r1) ** (alp / 3.0))
+    s = torch.where(
+        mask_triples,
+        (r2ij + r2jk - r2ik) * (r2ij - r2jk + r2ik) * (-r2ij + r2jk + r2ik),
+        zero,
+    )
 
-    s = (r2ij + r2jk - r2ik) * (r2ij - r2jk + r2ik) * (-r2ij + r2jk + r2ik)
     ang = torch.where(
-        real_triples(numbers, diagonal=False)
-        * (r2ij <= cutoff2)
-        * (r2jk <= cutoff2)
-        * (r2jk <= cutoff2),
+        mask_triples * (r2ij <= cutoff2) * (r2jk <= cutoff2) * (r2jk <= cutoff2),
         0.375 * s / r5 + 1.0 / r3,
         torch.tensor(0.0, **dd),
     )
 
     energy = ang * fdamp * c9
     return torch.sum(energy, dim=(-2, -1)) / 6.0
```

### Comparing `tad_dftd4-0.0.4/src/tad_dftd4/damping/rational.py` & `tad_dftd4-0.1.0/src/tad_dftd4/damping/rational.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # This file is part of tad-dftd4.
 #
-# SPDX-Identifier: LGPL-3.0
-# Copyright (C) 2022 Marvin Friede
+# SPDX-Identifier: Apache-2.0
+# Copyright (C) 2024 Grimme Group
 #
-# tad-dftd4 is free software: you can redistribute it and/or modify it under
-# the terms of the GNU Lesser General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# tad-dftd4 is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Lesser General Public License for more details.
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with tad-dftd4. If not, see <https://www.gnu.org/licenses/>.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 r"""
 Rational (Becke-Johnson) damping function
 =========================================
 
 This module defines the rational damping function, also known as Becke-Johnson
 damping.
 
@@ -29,15 +28,17 @@
     \left( a_1 R_0^{\text{AB}} + a_2 \right)^n}
 """
 from __future__ import annotations
 
 import torch
 
 from .. import defaults
-from .._typing import Tensor
+from ..typing import DD, Tensor
+
+__all__ = ["rational_damping"]
 
 
 def rational_damping(
     order: int,
     distances: Tensor,
     qq: Tensor,
     param: dict[str, Tensor],
@@ -58,12 +59,12 @@
         DFT-D4 damping parameters.
 
     Returns
     -------
     Tensor
         Values of the damping function.
     """
-    dd = {"device": distances.device, "dtype": distances.dtype}
+    dd: DD = {"device": distances.device, "dtype": distances.dtype}
 
     a1 = param.get("a1", torch.tensor(defaults.A1, **dd))
     a2 = param.get("a2", torch.tensor(defaults.A2, **dd))
     return 1.0 / (distances.pow(order) + (a1 * torch.sqrt(qq) + a2).pow(order))
```

### Comparing `tad_dftd4-0.0.4/src/tad_dftd4/data/r4r2.py` & `tad_dftd4-0.1.0/src/tad_dftd4/data/r4r2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # This file is part of tad-dftd4.
 #
-# SPDX-Identifier: LGPL-3.0
-# Copyright (C) 2022 Marvin Friede
+# SPDX-Identifier: Apache-2.0
+# Copyright (C) 2024 Grimme Group
 #
-# tad-dftd4 is free software: you can redistribute it and/or modify it under
-# the terms of the GNU Lesser General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# tad-dftd4 is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Lesser General Public License for more details.
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with tad-dftd4. If not, see <https://www.gnu.org/licenses/>.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 """
 Atomic data: Expectation values
 ===============================
 
 PBE0/def2-QZVP atomic values calculated by S. Grimme in Gaussian (2010).
 Rare gases recalculated by J. Mewes with PBE0/aug-cc-pVQZ in Dirac (2018).
 Also new super heavies Cn, Nh, Fl, Lv, Og and Am-Rg calculated at
 4c-PBE/Dyall-AE4Z level (Dirac 2022).
 """
-
 import torch
 
-__all__ = ["r4r2"]
+__all__ = ["R4R2"]
+
 
 # fmt: off
 r4_over_r2 = torch.tensor([
     0.0000,  # None
     8.0589, 3.4698,  # H,He
     29.0974,14.8517,11.8799, 7.8715, 5.5588, 4.7566, 3.8025, 3.1036,  # Li-Ne
     26.1552,17.2304,17.7210,12.7442, 9.5361, 8.1652, 6.7463, 5.6004,  # Na-Ar
@@ -52,13 +51,13 @@
     29.8135,26.3157,  # Fr,Ra
     19.1885,15.8542,16.1305,15.6161,15.1226,16.1576,14.6510,  # Ac-Am
     14.7178,13.9108,13.5623,13.2326,12.9189,12.6133,12.3142,  # Cm-No
     14.8326,12.3771,10.6378, 9.3638, 8.2297,  # Lr-
     7.5667, 6.9456, 6.3946, 5.9159, 5.4929,  # -Cn
     6.7286, 6.5144,10.9169,10.3600, 9.4723, 8.6641,  # Nh-Og
 ])
-"""Acutally calculated r⁴ over r² expectation values."""
+"""Actually calculated r⁴ over r² expectation values."""
 # fmt: on
 
 
-r4r2 = torch.sqrt(0.5 * (r4_over_r2 * torch.sqrt(torch.arange(r4_over_r2.shape[0]))))
+R4R2 = torch.sqrt(0.5 * (r4_over_r2 * torch.sqrt(torch.arange(r4_over_r2.shape[0]))))
 """r⁴ over r² expectation values."""
```

### Comparing `tad_dftd4-0.0.4/src/tad_dftd4/disp.py` & `tad_dftd4-0.1.0/src/tad_dftd4/disp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 # This file is part of tad-dftd4.
 #
-# SPDX-Identifier: LGPL-3.0
-# Copyright (C) 2022 Marvin Friede
+# SPDX-Identifier: Apache-2.0
+# Copyright (C) 2024 Grimme Group
 #
-# tad-dftd4 is free software: you can redistribute it and/or modify it under
-# the terms of the GNU Lesser General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# tad-dftd4 is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Lesser General Public License for more details.
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with tad-dftd4. If not, see <https://www.gnu.org/licenses/>.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 """
 Dispersion energy
 =================
 
 This module provides the dispersion energy evaluation for the pairwise
 interactions. It contains the main entrypoint for the dispersion energy
 (`dftd4`) as well as wrappers for the two-body (`dispersion2`) and the
 three-body (`dispersion3`) dispersion energy.
 """
 from __future__ import annotations
 
 import torch
+from tad_mctc import storch
+from tad_mctc.batch import real_pairs
+from tad_multicharge import get_eeq_charges
 
 from . import data, defaults
-from ._typing import Any, CountingFunction, DampingFunction, Tensor
-from .charges import get_charges
 from .cutoff import Cutoff
 from .damping import get_atm_dispersion, rational_damping
 from .model import D4Model
-from .ncoord import erf_count, get_coordination_number_d4
-from .utils import real_pairs
+from .ncoord import cn_d4, erf_count
+from .typing import DD, Any, CountingFunction, DampingFunction, Tensor
+
+__all__ = ["dftd4"]
 
 
 def dftd4(
     numbers: Tensor,
     positions: Tensor,
     charge: Tensor,
     param: dict[str, Tensor],
@@ -94,25 +96,27 @@
 
     Raises
     ------
     ValueError
         Shape inconsistencies between `numbers`, `positions`, `r4r2`, or,
         `rcov`.
     """
+    dd: DD = {"device": positions.device, "dtype": positions.dtype}
+
     if model is None:
-        model = D4Model(numbers, device=positions.device, dtype=positions.dtype)
+        model = D4Model(numbers, **dd)
     if cutoff is None:
-        cutoff = Cutoff(device=positions.device, dtype=positions.dtype)
+        cutoff = Cutoff(**dd)
 
     if rcov is None:
-        rcov = data.cov_rad_d3[numbers].type(positions.dtype).to(positions.device)
+        rcov = data.COV_D3.to(**dd)[numbers]
     if r4r2 is None:
-        r4r2 = data.r4r2[numbers].type(positions.dtype).to(positions.device)
+        r4r2 = data.R4R2.to(**dd)[numbers]
     if q is None:
-        q = get_charges(numbers, positions, charge, cutoff=cutoff.cn_eeq)
+        q = get_eeq_charges(numbers, positions, charge, cutoff=cutoff.cn_eeq)
 
     if numbers.shape != positions.shape[:-1]:
         raise ValueError(
             f"Shape of positions ({positions.shape}) is not consistent "
             f"with atomic numbers ({numbers.shape}).",
         )
     if numbers.shape != r4r2.shape:
@@ -127,16 +131,20 @@
         )
     if numbers.shape != q.shape:
         raise ValueError(
             f"Shape of atomic charges ({q.shape}) is not consistent with "
             f"atomic numbers ({numbers.shape}).",
         )
 
-    cn = get_coordination_number_d4(
-        numbers, positions, counting_function, rcov, cutoff=cutoff.cn
+    cn = cn_d4(
+        numbers,
+        positions,
+        counting_function=counting_function,
+        rcov=rcov,
+        cutoff=cutoff.cn,
     )
     weights = model.weight_references(cn, q)
     c6 = model.get_atomic_c6(weights)
 
     energy = dispersion2(
         numbers,
         positions,
@@ -191,24 +199,24 @@
         will be evaluated to `defaults.D4_DISP2_CUTOFF`.
 
     Returns
     -------
     Tensor
         Atom-resolved two-body dispersion energy.
     """
-    dd = {"device": positions.device, "dtype": positions.dtype}
+    dd: DD = {"device": positions.device, "dtype": positions.dtype}
     zero = torch.tensor(0.0, **dd)
 
     if cutoff is None:
         cutoff = torch.tensor(defaults.D4_DISP2_CUTOFF, **dd)
 
-    mask = real_pairs(numbers, diagonal=False)
+    mask = real_pairs(numbers, mask_diagonal=True)
     distances = torch.where(
         mask,
-        torch.cdist(positions, positions, p=2, compute_mode="use_mm_for_euclid_dist"),
+        storch.cdist(positions, positions, p=2),
         torch.tensor(torch.finfo(positions.dtype).eps, **dd),
     )
 
     qq = 3 * r4r2.unsqueeze(-1) * r4r2.unsqueeze(-2)
     c8 = c6 * qq
 
     t6 = torch.where(
@@ -226,15 +234,17 @@
     e8 = torch.sum(c8 * t8, dim=-1)
 
     s6 = param.get("s6", torch.tensor(defaults.S6, **dd))
     s8 = param.get("s8", torch.tensor(defaults.S8, **dd))
 
     edisp = s6 * e6 + s8 * e8
 
-    if "s10" in param and param["s10"] != 0.0:
+    # With `if "s10" in param and param["s10"] != 0.0`, the gradcheck tests fail
+    # if s10 is exactly 0 (other values are fine).
+    if "s10" in param:
         c10 = c6 * torch.pow(qq, 2) * 49.0 / 40.0
         t10 = torch.where(
             mask * (distances <= cutoff),
             damping_function(10, distances, qq, param, **kwargs),
             zero,
         )
         e10 = torch.sum(c10 * t10, dim=-1)
@@ -269,15 +279,15 @@
         Real-space cutoff. Defaults to `None`, i.e, `defaults.D4_DISP3_CUTOFF`.
 
     Returns
     -------
     Tensor
         Atom-resolved three-body dispersion energy.
     """
-    dd = {"device": positions.device, "dtype": positions.dtype}
+    dd: DD = {"device": positions.device, "dtype": positions.dtype}
 
     if cutoff is None:
         cutoff = torch.tensor(defaults.D4_DISP3_CUTOFF, **dd)
 
     s9 = param.get("s9", torch.tensor(defaults.S9, **dd))
     a1 = param.get("a1", torch.tensor(defaults.A1, **dd))
     a2 = param.get("a2", torch.tensor(defaults.A2, **dd))
```

### Comparing `tad_dftd4-0.0.4/src/tad_dftd4/model.py` & `tad_dftd4-0.1.0/src/tad_dftd4/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # This file is part of tad-dftd4.
 #
-# SPDX-Identifier: LGPL-3.0
-# Copyright (C) 2022 Marvin Friede
+# SPDX-Identifier: Apache-2.0
+# Copyright (C) 2024 Grimme Group
 #
-# tad-dftd4 is free software: you can redistribute it and/or modify it under
-# the terms of the GNU Lesser General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# tad-dftd4 is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Lesser General Public License for more details.
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with tad-dftd4. If not, see <https://www.gnu.org/licenses/>.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 """
 DFT-D4 Model
 ============
 
 This module contains the definition of the D4 dispersion model for the
 evaluation of C6 coefficients.
 
@@ -37,17 +36,21 @@
 >>> # calculate Gaussian weights, optionally pass CN and partial charges
 >>> gw = model.weight_references()
 >>> c6 = model.get_atomic_c6(gw)
 """
 from __future__ import annotations
 
 import torch
+from tad_mctc.math import einsum
 
 from . import data, params
-from ._typing import Tensor, TensorLike
+from .typing import Tensor, TensorLike
+
+__all__ = ["D4Model"]
+
 
 ga_default = 3.0
 gc_default = 2.0
 wf_default = 6.0
 
 
 class D4Model(TensorLike):
@@ -155,124 +158,134 @@
             Partial charge of every atom. Defaults to `None` (0).
 
         Returns
         -------
         Tensor
             Weights for the atomic reference systems.
         """
-        dd = {"device": self.device, "dtype": self.dtype}
-
         if cn is None:
-            cn = torch.zeros_like(self.numbers, dtype=self.dtype)
+            cn = torch.zeros(self.numbers.shape, **self.dd)
         if q is None:
-            q = torch.zeros_like(self.numbers, dtype=self.dtype)
+            q = torch.zeros(self.numbers.shape, **self.dd)
 
-        refc = params.refc[self.numbers].to(self.device)
-        refq = params.refq[self.numbers].type(self.dtype).to(self.device)
+        refc = params.refc.to(self.device)[self.numbers]
+        refq = params.refq.to(**self.dd)[self.numbers]
         mask = refc > 0
 
         # Due to the exponentiation, `norm` and `expw` may become very small
         # (down to 1e-300). This causes problems for the division by `norm`,
         # since single precision, i.e. `torch.float`, only goes to around 1e-38.
         # Consequently, some values become zero although the actual result
         # should be close to one. The problem does not arise when using `torch.
         # double`. In order to avoid this error, which is also difficult to
-        # detect, this part always uses `torch.double`. `params.refcn` is saved
-        # with `torch.double`.
-        refcn = params.refcn[self.numbers].to(self.device)
+        # detect, this part always uses `torch.double`. `params.refcovcn` is
+        # saved with `torch.double`, but I still made sure...
+        refcn = params.refcovcn.to(device=self.device, dtype=torch.double)[self.numbers]
 
         # For vectorization, we reformulate the Gaussian weighting function:
         # exp(-wf * igw * (cn - cn_ref)^2) = [exp(-(cn - cn_ref)^2)]^(wf * igw)
         # Gaussian weighting function part 1: exp(-(cn - cn_ref)^2)
         dcn = cn.unsqueeze(-1).type(torch.double) - refcn
         tmp = torch.exp(-dcn * dcn)
 
         # Gaussian weighting function part 2: tmp^(wf * igw)
         # (While the Fortran version just loops over the number of gaussian
         # weights `igw`, we have to use masks and explicitly implement the
         # formulas for exponentiation. Luckily, `igw` only takes on the values
         # 1 and 3.)
+        def refc_pow(n: int) -> Tensor:
+            return sum(
+                (torch.pow(tmp, i * self.wf) for i in range(1, n + 1)),
+                torch.tensor(0.0, device=tmp.device),
+            )
+
+        refc_pow_1 = torch.where(refc == 1, refc_pow(1), tmp)
+        refc_pow_final = torch.where(refc == 3, refc_pow(3), refc_pow_1)
+
         expw = torch.where(
             mask,
-            torch.where(
-                refc == 3,
-                torch.pow(tmp, self.wf)
-                + torch.pow(tmp, 2 * self.wf)
-                + torch.pow(tmp, 3 * self.wf),
-                torch.where(
-                    refc == 1,
-                    torch.pow(tmp, self.wf),
-                    tmp,
-                ),
-            ),
-            torch.tensor(0.0, device=self.device, dtype=refcn.dtype),  # double!
+            refc_pow_final,
+            torch.tensor(0.0, device=self.device, dtype=torch.double),  # double!
         )
 
         # normalize weights
-        norm = torch.sum(expw, dim=-1, keepdim=True)
-        gw_temp = (expw / norm).type(self.dtype)
+        norm = torch.where(
+            mask,
+            torch.sum(expw, dim=-1, keepdim=True),
+            torch.tensor(1e-300, device=self.device, dtype=torch.double),  # double!)
+        )
+        gw_temp = (expw / norm).type(self.dtype)  # back to real dtype
 
         # maximum reference CN for each atom
         maxcn = torch.max(refcn, dim=-1, keepdim=True)[0]
 
         # prevent division by 0 and small values
         exceptional = (torch.isnan(gw_temp)) | (gw_temp > torch.finfo(self.dtype).max)
 
         gw = torch.where(
             exceptional,
             torch.where(
                 refcn == maxcn,
-                torch.tensor(1.0, **dd),
-                torch.tensor(0.0, **dd),
+                torch.tensor(1.0, **self.dd),
+                torch.tensor(0.0, **self.dd),
             ),
             gw_temp,
         )
 
         # unsqueeze for reference dimension
-        zeff = data.zeff[self.numbers].unsqueeze(-1)
-        gam = data.gam[self.numbers].unsqueeze(-1) * self.gc
+        zeff = data.ZEFF.to(self.device)[self.numbers].unsqueeze(-1)
+        gam = data.GAM.to(**self.dd)[self.numbers].unsqueeze(-1) * self.gc
         q = q.unsqueeze(-1)
 
         # charge scaling
         zeta = torch.where(
             mask,
             self._zeta(gam, refq + zeff, q + zeff),
-            torch.tensor(0.0, **dd),
+            torch.tensor(0.0, **self.dd),
         )
 
         return zeta * gw
 
     def get_atomic_c6(self, gw: Tensor) -> Tensor:
         """
         Calculate atomic C6 dispersion coefficients.
 
         Parameters
         ----------
         gw : Tensor
-            Weights for the atomic reference systems.
+            Weights for the atomic reference systems of shape
+            `(..., nat, nref)`.
 
         Returns
         -------
         Tensor
-            C6 coefficients for all atom pairs.
+            C6 coefficients for all atom pairs of shape `(..., nat, nat)`.
         """
+        # (..., nunique, r, 23) -> (..., n, r, 23)
         alpha = self.alpha[self.atom_to_unique]
 
-        # shape of alpha: (b, nat, nref, 23)
-        # (b, 1, nat, 1, nref, 23) * (b, nat, 1, nref, 1, 23) =
-        # (b, nat, nat, nref, nref, 23)
-        rc6 = trapzd(
-            alpha.unsqueeze(-4).unsqueeze(-3) * alpha.unsqueeze(-3).unsqueeze(-2)
-        )
+        # (..., n, r, 23) -> (..., n, n, r, r)
+        rc6 = trapzd(alpha)
 
-        # shape of gw: (batch, natoms, nref)
-        # (b, 1, nat, 1, nref)*(b, nat, 1, nref, 1) = (b, nat, nat, nref, nref)
-        g = gw.unsqueeze(-3).unsqueeze(-2) * gw.unsqueeze(-2).unsqueeze(-1)
+        # The default einsum path is fastest if the large tensors comes first.
+        # (..., n1, n2, r1, r2) * (..., n1, r1) * (..., n2, r2) -> (..., n1, n2)
+        return einsum(
+            "...ijab,...ia,...jb->...ij",
+            *(rc6, gw, gw),
+            optimize=[(0, 1), (0, 1)],
+        )
 
-        return torch.sum(g * rc6, dim=(-2, -1))
+        # NOTE: This old version creates large intermediate tensors and builds
+        # the full matrix before the sum reduction, requiring a lot of memory.
+        #
+        # (..., 1, n, 1, r) * (..., n, 1, r, 1) = (..., n, n, r, r)
+        # g = gw.unsqueeze(-3).unsqueeze(-2) * gw.unsqueeze(-2).unsqueeze(-1)
+        #
+        # (..., n, n, r, r) * (..., n, n, r, r) -> (..., n, n)
+        # c6 = torch.sum(g * rc6, dim=(-2, -1))
 
     def _zeta(self, gam: Tensor, qref: Tensor, qmod: Tensor) -> Tensor:
         """
         charge scaling function.
 
         Parameters
         ----------
@@ -284,46 +297,48 @@
             Modified charges.
 
         Returns
         -------
         Tensor
             Scaled charges.
         """
+        eps = torch.tensor(torch.finfo(self.dtype).eps, **self.dd)
+        ga = torch.tensor(self.ga, **self.dd)
+        scale = torch.exp(gam * (1.0 - qref / (qmod - eps)))
+
         return torch.where(
             qmod > 0.0,
-            torch.exp(self.ga * (1.0 - torch.exp(gam * (1.0 - qref / qmod)))),
-            torch.exp(torch.tensor(self.ga, device=self.device, dtype=self.dtype)),
+            torch.exp(ga * (1.0 - scale)),
+            torch.exp(ga),
         )
 
     def _set_refalpha_eeq(self) -> Tensor:
         """
         Set the reference polarizibilities for unique species.
 
         Returns
         -------
         Tensor
             Reference polarizibilities for unique species (not all atoms).
         """
-        zero = torch.tensor(0.0, device=self.device, dtype=self.dtype)
+        zero = torch.tensor(0.0, **self.dd)
 
         numbers = self.unique
-        refsys = params.refsys[numbers].to(self.device)
-        refsq = params.refsq[numbers].type(self.dtype).to(self.device)
-        refascale = params.refascale[numbers].type(self.dtype).to(self.device)
-        refalpha = params.refalpha[numbers].type(self.dtype).to(self.device)
-        refscount = params.refscount[numbers].type(self.dtype).to(self.device)
-        secscale = params.secscale.type(self.dtype).to(self.device)
-        secalpha = params.secalpha.type(self.dtype).to(self.device)
+        refsys = params.refsys.to(self.device)[numbers]
+        refsq = params.refsq.to(**self.dd)[numbers]
+        refascale = params.refascale.to(**self.dd)[numbers]
+        refalpha = params.refalpha.to(**self.dd)[numbers]
+        refscount = params.refscount.to(**self.dd)[numbers]
+        secscale = params.secscale.to(**self.dd)
+        secalpha = params.secalpha.to(**self.dd)
 
         mask = refsys > 0
 
-        zeff = data.zeff[refsys].to(self.device)
-        gam = data.gam[refsys].type(self.dtype).to(self.device) * self.gc
-
-        aiw = secscale[refsys] * secalpha[refsys]
+        zeff = data.ZEFF.to(self.device)[refsys]
+        gam = data.GAM.to(**self.dd)[refsys] * self.gc
 
         # charge scaling
         zeta = torch.where(
             mask,
             self._zeta(gam, zeff, refsq + zeff),
             zero,
         )
@@ -338,15 +353,15 @@
 def trapzd(polarizability: Tensor) -> Tensor:
     """
     Numerical Casimir--Polder integration.
 
     Parameters
     ----------
     polarizability : Tensor
-        Polarizabilities.
+        Polarizabilities of shape `(..., nat, nref, 23)`
 
     Returns
     -------
     Tensor
         C6 coefficients.
     """
     thopi = 3.0 / 3.141592653589793238462643383279502884197
@@ -375,8 +390,20 @@
             1.0000000000000000,
             1.7500000000000000,
             2.5000000000000000,
             1.2500000000000000,
         ]
     )
 
-    return thopi * torch.sum(weights * polarizability, dim=-1)
+    # NOTE: In the old version, a memory inefficient intermediate tensor was
+    # created. The new version uses `einsum` to avoid this.
+    #
+    # (..., 1, nat, 1, nref, 23) * (..., nat, 1, nref, 1, 23) =
+    # (..., nat, nat, nref, nref, 23) -> (..., nat, nat, nref, nref)
+    # a = alpha.unsqueeze(-4).unsqueeze(-3) * alpha.unsqueeze(-3).unsqueeze(-2)
+    #
+    # rc6 = thopi * torch.sum(weights * a, dim=-1)
+
+    return thopi * einsum(
+        "w,...iaw,...jbw->...ijab",
+        *(weights, polarizability, polarizability),
+    )
```

### Comparing `tad_dftd4-0.0.4/src/tad_dftd4/params.py` & `tad_dftd4-0.1.0/src/tad_dftd4/params.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,68 @@
 # This file is part of tad-dftd4.
 #
-# SPDX-Identifier: LGPL-3.0
-# Copyright (C) 2022 Marvin Friede
+# SPDX-Identifier: Apache-2.0
+# Copyright (C) 2024 Grimme Group
 #
-# tad-dftd4 is free software: you can redistribute it and/or modify it under
-# the terms of the GNU Lesser General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# tad-dftd4 is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Lesser General Public License for more details.
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with tad-dftd4. If not, see <https://www.gnu.org/licenses/>.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 """
 Parameters
 ==========
 
-This module contains all parameters the computation of the C6 coefficients
+This module contains all parameters for the computation of the C6 coefficients
 (reference systems, reference polarizabilites, ...).
 """
 import torch
 
-refcn = torch.tensor(
+__all__ = [
+    "refcovcn",
+    "refcnd3",
+    "refq",
+    "refsq",
+    "refalpha",
+    "refascale",
+    "refscount",
+    "refsys",
+    "refc",
+    "secscale",
+    "secalpha",
+]
+
+# DFT-D4 CN (actual reference CN)
+refcovcn = torch.tensor(
     [
-        [
+        [  # dummy
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
         ],
-        [
+        [  # H
             0.00000000000000,
             0.89422436546040,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
         ],
-        [
+        [  # He
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
@@ -787,56 +801,370 @@
             0.93512916979697,
             1.87110482058901,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
         ],
-        [
+        [  # At
             0.00000000000000,
             0.97711087656722,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
         ],
-        [
+        [  # Rn
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+        ],
+        [  # Fr
+            0.00000000000000,
+            0.76514673233032,
+            0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
+        ],
+        [  # Ra
+            0.00000000000000,
+            0.77520757913589,
+            1.54451191425323,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+        ],
+        [  # Ac
+            0.00000000000000,
+            0.81221771240234,
+            1.61096704006195,
+            2.40822887420654,
+            3.16141414642334,
+            3.86818122863770,
+            4.60221958160400,
+        ],
+        [  # Th
+            0.00000000000000,
+            0.84210479259491,
+            1.67266535758972,
+            2.50573635101318,
+            3.33462429046631,
+            0.00000000000000,  # ThH5 missing (GEOM)
+            0.00000000000000,  # ThH6 missing (GEOM)
+        ],
+        [  # Pa
+            0.00000000000000,
+            0.85091900825500,
+            1.68243002891541,
+            2.56143164634705,
+            3.41472434997559,
+            4.33161783218384,
+            0.00000000000000,  # PaH6 missing (GEOM)
+        ],
+        [  # U
             0.00000000000000,
+            0.84563773870468,
+            0.00000000000000,  # UH2 missing
+            2.50075340270996,
+            3.38830232620239,
+            3.57048654556274,
+            5.12557458877563,
+        ],
+        [  # Np
             0.00000000000000,
+            0.84929960966110,
+            1.68312501907349,
+            2.51682710647583,
+            3.39772701263428,
+            4.23597240447998,
+            5.09381914138794,
+        ],
+        [  # Pu
             0.00000000000000,
+            0.81253784894943,
+            1.65689170360565,
+            2.49969720840454,
+            3.36243820190430,
+            4.19367313385010,
+            5.02024745941162,
+        ],
+        [  # Am
+            0.00000000000000,
+            0.78272187709808,
+            1.58581125736237,
+            2.46386861801147,
+            0.00000000000000,  # AmH4 missing
+            4.10353183746338,
+            4.94068670272827,
+        ],
+        [  # Cm
+            0.00000000000000,
+            0.8347442150116,
+            1.64897620677948,
+            2.47316074371338,
+            3.26227951049805,
+            4.05759239196777,
+            4.85972309112549,
+        ],
+        [  # Bk
+            0.00000000000000,
+            0.82979065179825,
+            1.66842269897461,
+            2.50224256515503,
+            3.36453199386597,
+            0.00000000000000,  # BkH5 missing (GEOM)
+            0.00000000000000,  # BkH6 missing (GEOM)
+        ],
+        [  # Cf
+            0.00000000000000,
+            0.81898736953735,
+            1.63452363014221,
+            2.50784802436829,
+            3.34391856193542,
+            0.00000000000000,  # CfH5 missing
+            4.98358106613159,
+        ],
+        [  # Es
+            0.00000000000000,
+            0.79849386215210,
+            1.60774898529053,
+            2.48593425750732,
+            3.30908131599426,
+            4.11455059051514,
+            4.89267015457153,
+        ],
+        [  # Fm
+            0.00000000000000,
+            0.81187158823013,
+            1.63818895816803,
+            2.51218342781067,
+            3.33093667030334,
+            4.15018892288208,
+            4.97273159027100,
+        ],
+        [  # Md
+            0.00000000000000,
+            0.83019560575485,
+            1.67299079895020,
+            2.52414393424988,
+            3.36544203758240,
+            0.00000000000000,  # MdH5 missing (GEOM)
+            0.00000000000000,  # MdH6 missing (GEOM)
+        ],
+        [  # No
+            0.00000000000000,
+            0.83132714033127,
+            1.67657399177551,
+            2.51869487762451,
+            3.36061143875122,
+            3.62583565711975,
+            3.85555744171143,
+        ],
+        [  # Lr
+            0.00000000000000,
+            0.81793087720871,
+            1.64256453514099,
+            2.47565555572510,
+            3.21661520004272,
+            3.99956941604614,
+            4.77920246124268,
         ],
     ],
     dtype=torch.float64,
 )
+
+# DFT-D3 CN (only Fortran: calculation of "ngw", named "refcn"; only actinides)
+refcnd3 = torch.tensor(
+    [
+        [  # Fr
+            0.00000000000000,
+            0.97049617767334,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+        ],
+        [  # Ra
+            0.00000000000000,
+            0.96613162755966,
+            1.92506694793701,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+        ],
+        [  # Ac
+            0.00000000000000,
+            0.98022586107254,
+            1.94446778297424,
+            2.90698194503784,
+            3.81743621826172,
+            4.67233896255493,
+            5.55994558334351,
+        ],
+        [  # Th
+            0.00000000000000,
+            0.98468047380447,
+            1.95599293708801,
+            2.93023586273193,
+            3.89967584609985,
+            0.00000000000000,  # ThH5 missing (GEOM)
+            0.00000000000000,  # ThH6 missing (GEOM)
+        ],
+        [  # Pa
+            0.00000000000000,
+            0.96470272541046,
+            1.90787398815155,
+            2.90372896194458,
+            3.87106418609619,
+            4.90939426422119,
+            0.00000000000000,  # PaH6 missing (GEOM)
+        ],
+        [  # U
+            0.00000000000000,
+            0.97657883167267,
+            0.00000000000000,  # UH2 missing
+            2.88882374763489,
+            3.91285228729248,
+            4.11813306808472,
+            5.91870355606079,
+        ],
+        [  # Np
+            0.00000000000000,
+            0.98379653692245,
+            1.94989669322968,
+            2.91591286659241,
+            3.93579626083374,
+            4.906907081604,
+            5.90049982070923,
+        ],
+        [  # Pu
+            0.00000000000000,
+            0.95366597175598,
+            1.94386768341064,
+            2.93234348297119,
+            3.9441020488739,
+            4.91923046112061,
+            5.88884162902832,
+        ],
+        [  # Am
+            0.00000000000000,
+            0.9163174033165,
+            1.85625433921814,
+            2.88227415084839,
+            0.00000000000000,  # AmH4 missing
+            4.80048131942749,
+            5.77936410903931,
+        ],
+        [  # Cm
+            0.00000000000000,
+            0.97616904973984,
+            1.92883539199829,
+            2.89290571212769,
+            3.81673455238342,
+            4.74775981903076,
+            5.68661880493164,
+        ],
+        [  # Bk
+            0.00000000000000,
+            0.97048676013947,
+            1.95111346244812,
+            2.92622041702271,
+            3.93419456481934,
+            0.00000000000000,  # BkH5 missing (GEOM)
+            0.00000000000000,  # BkH6 missing (GEOM)
+        ],
+        [  # Cf
+            0.00000000000000,
+            0.95812320709229,
+            1.91229522228241,
+            2.93266654014587,
+            3.91049480438232,
+            0.00000000000000,  # CfH5 missing
+            5.82847452163696,
+        ],
+        [  # Es
+            0.00000000000000,
+            0.93458300828934,
+            1.88156545162201,
+            2.90752410888672,
+            3.87045359611511,
+            4.81313467025757,
+            5.72440004348755,
+        ],
+        [  # Fm
+            0.00000000000000,
+            0.94997024536133,
+            1.91649174690247,
+            2.93766069412231,
+            3.89561820030212,
+            4.85404109954834,
+            5.81603574752808,
+        ],
+        [  # Md
+            0.00000000000000,
+            0.97095054388046,
+            1.95636773109436,
+            2.95153689384460,
+            3.93525266647339,
+            0.00000000000000,  # MdH5 missing (GEOM)
+            0.00000000000000,  # MdH6 missing (GEOM)
+        ],
+        [  # No
+            0.00000000000000,
+            0.97224730253220,
+            1.96050095558167,
+            2.94520807266235,
+            3.92964100837708,
+            4.25823402404785,
+            4.55113649368286,
+        ],
+        [  # Lr
+            0.00000000000000,
+            0.9569137096405,
+            1.92149925231934,
+            2.89576029777527,
+            3.76441621780396,
+            4.68083429336548,
+            5.59392404556274,
+        ],
+    ],
+    dtype=torch.float64,
+)
+
 refq = torch.tensor(
     [
-        [
+        [  # dummay
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
         ],
-        [
+        [  # H
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
         ],
-        [
+        [  # He
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
@@ -1593,47 +1921,201 @@
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
         ],
+        [  # Fr
+            0.00000000000000,
+            0.07920000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+        ],
+        [  # Ra
+            0.00000000000000,
+            0.23880000000000,
+            0.30820000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+        ],
+        [  # Ac
+            0.00000000000000,
+            0.11750000000000,
+            0.18970000000000,
+            0.23800000000000,
+            0.27140000000000,
+            0.29250000000000,
+            0.30940000000000,
+        ],
+        [  # Th
+            0.00000000000000,
+            0.08840000000000,
+            0.15380000000000,
+            0.20480000000000,
+            0.24330000000000,
+            0.00000000000000,  # ThH5 missing (GEOM)
+            0.00000000000000,  # ThH6 missing (GEOM)
+        ],
+        [  # Pa
+            0.00000000000000,
+            0.10670000000000,
+            0.18290000000000,
+            0.24670000000000,
+            0.29300000000000,
+            0.32920000000000,
+            0.00000000000000,  # PaH6 missing (GEOM)
+        ],
+        [  # U
+            0.00000000000000,
+            0.07960000000000,
+            0.00000000000000,  # UH2 missing
+            0.16920000000000,
+            0.20390000000000,
+            0.19490000000000,
+            0.24560000000000,
+        ],
+        [  # Np
+            0.00000000000000,
+            0.07660000000000,
+            0.13320000000000,
+            0.17550000000000,
+            0.21870000000000,
+            0.24240000000000,
+            0.26660000000000,
+        ],
+        [  # Pu
+            0.00000000000000,
+            0.14950000000000,
+            0.24790000000000,
+            0.31810000000000,
+            0.37790000000000,
+            0.40920000000000,
+            0.43640000000000,
+        ],
+        [  # Am
+            0.00000000000000,
+            0.15100000000000,
+            0.24100000000000,
+            0.30680000000000,
+            0.00000000000000,  # AmH4 missing
+            0.38010000000000,
+            0.40550000000000,
+        ],
+        [  # Cm
+            0.00000000000000,
+            0.07640000000000,
+            0.13380000000000,
+            0.17800000000000,
+            0.21120000000000,
+            0.23780000000000,
+            0.25950000000000,
+        ],
+        [  # Bk
+            0.00000000000000,
+            0.02210000000000,
+            0.04090000000000,
+            0.05620000000000,
+            0.07110000000000,
+            0.00000000000000,  # BkH5 missing (GEOM)
+            0.00000000000000,  # BkH6 missing (GEOM)
+        ],
+        [  # Cf
+            0.00000000000000,
+            0.15350000000000,
+            0.25390000000000,
+            0.33210000000000,
+            0.38680000000000,
+            0.00000000000000,  # CfH5 missing
+            0.45000000000000,
+        ],
+        [  # Es
+            0.00000000000000,
+            0.11350000000000,
+            0.19140000000000,
+            0.25500000000000,
+            0.29690000000000,
+            0.32680000000000,
+            0.34710000000000,
+        ],
+        [  # Fm
+            0.00000000000000,
+            0.09860000000000,
+            0.16690000000000,
+            0.22300000000000,
+            0.25830000000000,
+            0.28460000000000,
+            0.30460000000000,
+        ],
+        [  # Md
+            0.00000000000000,
+            0.06780000000000,
+            0.11580000000000,
+            0.15370000000000,
+            0.17900000000000,
+            0.00000000000000,  # MdH5 missing (GEOM)
+            0.00000000000000,  # MdH6 missing (GEOM)
+        ],
+        [  # No
+            0.00000000000000,
+            0.04800000000000,
+            0.08650000000000,
+            0.11740000000000,
+            0.14110000000000,
+            0.15770000000000,
+            0.17180000000000,
+        ],
+        [  # Lr
+            0.00000000000000,
+            0.05050000000000,
+            0.08900000000000,
+            0.11910000000000,
+            0.14090000000000,
+            0.15740000000000,
+            0.17080000000000,
+        ],
     ],
     dtype=torch.float64,
 )
+
 refsq = torch.tensor(
     [
-        [
+        [  # dummy
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
         ],
-        [
+        [  # H
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
         ],
-        [
+        [  # He
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
         ],
-        [
+        [  # Li
             0.00000000000000,
             -0.37061732228445,
             -0.50233549783851,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
@@ -2381,20 +2863,174 @@
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
         ],
+        [
+            0.00000000000000,  # Fr
+            -0.0792000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+        ],
+        [
+            0.00000000000000,  # Ra
+            -0.2388000000000,
+            -0.1541000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+        ],
+        [  # Ac
+            0.00000000000000,
+            -0.11750000000000,
+            -0.09485000000000,
+            -0.07933333333333,
+            -0.06785000000000,
+            -0.05850000000000,
+            -0.05156666666667,
+        ],
+        [  # Th
+            +0.00000000000000,
+            -0.08840000000000,
+            -0.07690000000000,
+            -0.06826666666667,
+            -0.06082500000000,
+            +0.00000000000000,  # ThH5 missing (GEOM)
+            +0.00000000000000,  # ThH6 missing (GEOM)
+        ],
+        [  # Pa
+            0.00000000000000,
+            -0.10670000000000,
+            -0.09145000000000,
+            -0.08223333333333,
+            -0.07325000000000,
+            -0.06584000000000,
+            0.00000000000000,  # PaH6 missing (GEOM)
+        ],
+        [  # U
+            0.00000000000000,
+            -0.07960000000000,
+            -0.00000000000000,  # UH2 missing
+            -0.05640000000000,
+            -0.05097500000000,
+            -0.03898000000000,
+            -0.04093333333333,
+        ],
+        [  # Np
+            0.00000000000000,
+            -0.07660000000000,
+            -0.06660000000000,
+            -0.05850000000000,
+            -0.05467500000000,
+            -0.04848000000000,
+            -0.04443333333333,
+        ],
+        [  # Pu
+            0.00000000000000,
+            -0.14950000000000,
+            -0.12395000000000,
+            -0.10603333333333,
+            -0.09447500000000,
+            -0.08184000000000,
+            -0.07273333333333,
+        ],
+        [  # Am
+            0.00000000000000,
+            -0.15100000000000,
+            -0.12050000000000,
+            -0.10226666666667,
+            -0.00000000000000,  # AmH4 missing
+            -0.07602000000000,
+            -0.06758333333333,
+        ],
+        [  # Cm
+            0.00000000000000,
+            -0.07640000000000,
+            -0.06690000000000,
+            -0.05933333333333,
+            -0.05280000000000,
+            -0.04756000000000,
+            -0.04325000000000,
+        ],
+        [  # Bk
+            0.00000000000000,
+            -0.02210000000000,
+            -0.02045000000000,
+            -0.01873333333333,
+            -0.01777500000000,
+            0.00000000000000,  # BkH5 missing (GEOM)
+            0.00000000000000,  # BkH6 missing (GEOM)
+        ],
+        [  # Cf
+            0.00000000000000,
+            -0.15350000000000,
+            -0.12695000000000,
+            -0.11070000000000,
+            -0.09670000000000,
+            -0.00000000000000,  # CfH5 missing
+            -0.07500000000000,
+        ],
+        [  # Es
+            0.00000000000000,
+            -0.11350000000000,
+            -0.09570000000000,
+            -0.08500000000000,
+            -0.07422500000000,
+            -0.06536000000000,
+            -0.05785000000000,
+        ],
+        [  # Fm
+            0.00000000000000,
+            -0.09860000000000,
+            -0.08345000000000,
+            -0.07433333333333,
+            -0.06457500000000,
+            -0.05692000000000,
+            -0.05076666666667,
+        ],
+        [  # Md
+            0.00000000000000,
+            -0.06780000000000,
+            -0.05790000000000,
+            -0.05123333333333,
+            -0.04475000000000,
+            0.00000000000000,  # MdH5 missing (GEOM)
+            0.00000000000000,  # MdH6 missing (GEOM)
+        ],
+        [  # No
+            0.00000000000000,
+            -0.04800000000000,
+            -0.04325000000000,
+            -0.03913333333333,
+            -0.03527500000000,
+            -0.03154000000000,
+            -0.02863333333333,
+        ],
+        [  # Lr
+            0.00000000000000,
+            -0.05050000000000,
+            -0.04450000000000,
+            -0.03970000000000,
+            -0.03522500000000,
+            -0.03148000000000,
+            -0.02846666666667,
+        ],
     ],
     dtype=torch.float64,
 )
+
 refalpha = torch.tensor(
     [
-        [
+        [  # dummy
             [
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
@@ -2563,15 +3199,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # H
             [
                 5.05401600000000e00,
                 4.96682100000000e00,
                 4.72443900000000e00,
                 3.97078600000000e00,
                 3.16550300000000e00,
                 2.48864600000000e00,
@@ -2740,15 +3376,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # He
             [
                 1.45463600000000e00,
                 1.45021300000000e00,
                 1.43714000000000e00,
                 1.38759000000000e00,
                 1.31354500000000e00,
                 1.22436000000000e00,
@@ -2917,15 +3553,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Li
             [
                 1.49684693000000e02,
                 1.01093775000000e02,
                 5.16672830000000e01,
                 1.80181080000000e01,
                 8.90934600000000e00,
                 5.33090300000000e00,
@@ -3094,15 +3730,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Be
             [
                 4.28790460000000e01,
                 3.99295910000000e01,
                 3.31319060000000e01,
                 1.98584460000000e01,
                 1.20562070000000e01,
                 7.87312400000000e00,
@@ -3271,15 +3907,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # B
             [
                 2.21068880000000e01,
                 2.13442260000000e01,
                 1.94317910000000e01,
                 1.46694210000000e01,
                 1.06975470000000e01,
                 7.90232000000000e00,
@@ -3448,15 +4084,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # C
             [
                 1.23555340000000e01,
                 1.21386640000000e01,
                 1.15492610000000e01,
                 9.79994900000000e00,
                 7.99168200000000e00,
                 6.46911200000000e00,
@@ -3625,15 +4261,15 @@
                 3.78403000000000e-01,
                 2.28799000000000e-01,
                 1.53550000000000e-01,
                 7.36385000000000e-02,
                 4.35460000000000e-02,
             ],
         ],
-        [
+        [  # N
             [
                 7.53850900000000e00,
                 7.46578400000000e00,
                 7.25922300000000e00,
                 6.57084200000000e00,
                 5.74120900000000e00,
                 4.94450400000000e00,
@@ -3802,15 +4438,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # O
             [
                 5.19670900000000e00,
                 5.16443000000000e00,
                 5.07156900000000e00,
                 4.74845000000000e00,
                 4.32735300000000e00,
                 3.88542600000000e00,
@@ -3979,15 +4615,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # F
             [
                 3.63383900000000e00,
                 3.61969600000000e00,
                 3.57839400000000e00,
                 3.42793800000000e00,
                 3.21737200000000e00,
                 2.97992900000000e00,
@@ -4156,15 +4792,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Ne
             [
                 2.62279400000000e00,
                 2.61608100000000e00,
                 2.59630100000000e00,
                 2.52211500000000e00,
                 2.41300700000000e00,
                 2.28318500000000e00,
@@ -4333,15 +4969,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Na
             [
                 1.70928531000000e02,
                 1.19194623000000e02,
                 6.28166710000000e01,
                 2.22250350000000e01,
                 1.10609650000000e01,
                 6.72256800000000e00,
@@ -5572,15 +6208,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Ar
             [
                 1.11080370000000e01,
                 1.10394140000000e01,
                 1.08402330000000e01,
                 1.01295640000000e01,
                 9.17337000000000e00,
                 8.14874700000000e00,
@@ -5749,15 +6385,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # K
             [
                 3.66617327000000e02,
                 1.95240726000000e02,
                 8.38654450000000e01,
                 2.88051330000000e01,
                 1.59216120000000e01,
                 1.09496410000000e01,
@@ -8758,15 +9394,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Kr
             [
                 1.68771250000000e01,
                 1.67404080000000e01,
                 1.63473440000000e01,
                 1.49868570000000e01,
                 1.32465280000000e01,
                 1.14802080000000e01,
@@ -8935,15 +9571,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Rb
             [
                 4.10157065000000e02,
                 2.14362942000000e02,
                 9.22189500000000e01,
                 3.30762760000000e01,
                 1.91702550000000e01,
                 1.36453490000000e01,
@@ -11944,15 +12580,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Xe
             [
                 2.73277050000000e01,
                 2.70110760000000e01,
                 2.61157860000000e01,
                 2.31734500000000e01,
                 1.97140260000000e01,
                 1.64952160000000e01,
@@ -12121,15 +12757,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Cs
             [
                 5.37089754000000e02,
                 2.51203112000000e02,
                 1.04671685000000e02,
                 4.01908390000000e01,
                 2.49381150000000e01,
                 1.83967650000000e01,
@@ -12298,15 +12934,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Ba
             [
                 2.88240883000000e02,
                 2.20124081000000e02,
                 1.31490276000000e02,
                 5.52586600000000e01,
                 3.15893280000000e01,
                 2.16257080000000e01,
@@ -12475,15 +13111,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # La
             [
                 2.15814022000000e02,
                 1.76844927000000e02,
                 1.18315876000000e02,
                 5.65506640000000e01,
                 3.37025040000000e01,
                 2.32152200000000e01,
@@ -12652,15 +13288,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Ce
             [
                 6.31803350000000e01,
                 6.08655150000000e01,
                 5.56077000000000e01,
                 4.29730420000000e01,
                 3.28160560000000e01,
                 2.56410650000000e01,
@@ -12829,15 +13465,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Pr
             [
                 2.53607583000000e02,
                 1.85347808000000e02,
                 1.17313120000000e02,
                 5.14986990000000e01,
                 2.95194860000000e01,
                 2.01469030000000e01,
@@ -13006,15 +13642,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Nd
             [
                 2.24576218000000e02,
                 1.79268440000000e02,
                 1.14550986000000e02,
                 5.07711900000000e01,
                 2.90959830000000e01,
                 1.98086410000000e01,
@@ -13183,15 +13819,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Pm
             [
                 2.16554028000000e02,
                 1.74068560000000e02,
                 1.12065720000000e02,
                 4.99521540000000e01,
                 2.85964740000000e01,
                 1.94194800000000e01,
@@ -13360,15 +13996,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Sm
             [
                 2.09482163000000e02,
                 1.69326427000000e02,
                 1.09749627000000e02,
                 4.91677750000000e01,
                 2.81221600000000e01,
                 1.90508730000000e01,
@@ -13537,15 +14173,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Eu
             [
                 2.03211190000000e02,
                 1.65077409000000e02,
                 1.07694135000000e02,
                 4.84835280000000e01,
                 2.77173710000000e01,
                 1.87379040000000e01,
@@ -13714,15 +14350,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Gd
             [
                 1.41842064000000e02,
                 1.16857104000000e02,
                 8.24531150000000e01,
                 4.28638860000000e01,
                 2.64230410000000e01,
                 1.85963810000000e01,
@@ -13891,15 +14527,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Tb
             [
                 2.29301596000000e02,
                 1.48757206000000e02,
                 8.38992590000000e01,
                 3.77525280000000e01,
                 2.30411680000000e01,
                 1.64030610000000e01,
@@ -14068,15 +14704,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Dy
             [
                 2.32465673000000e02,
                 1.35183600000000e02,
                 8.01286950000000e01,
                 3.77486970000000e01,
                 2.32434510000000e01,
                 1.65330840000000e01,
@@ -14245,15 +14881,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Ho
             [
                 1.74357971000000e02,
                 1.45347573000000e02,
                 9.83386140000000e01,
                 4.56653390000000e01,
                 2.61535730000000e01,
                 1.75697070000000e01,
@@ -14422,15 +15058,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Er
             [
                 1.69508670000000e02,
                 1.41831130000000e02,
                 9.64854630000000e01,
                 4.49898390000000e01,
                 2.57372660000000e01,
                 1.72457070000000e01,
@@ -14599,15 +15235,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Tm
             [
                 1.64874479000000e02,
                 1.38503417000000e02,
                 9.47797640000000e01,
                 4.44385580000000e01,
                 2.54312120000000e01,
                 1.70158970000000e01,
@@ -14776,15 +15412,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Yb
             [
                 1.63737907000000e02,
                 1.37401600000000e02,
                 9.38094750000000e01,
                 4.37828040000000e01,
                 2.49508110000000e01,
                 1.66301360000000e01,
@@ -14953,15 +15589,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Lu
             [
                 1.36853067000000e02,
                 1.04297562000000e02,
                 7.65562240000000e01,
                 4.02834860000000e01,
                 2.41515190000000e01,
                 1.64764390000000e01,
@@ -15130,15 +15766,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Hf
             [
                 1.06281621000000e02,
                 9.54891650000000e01,
                 7.53034870000000e01,
                 4.41393100000000e01,
                 2.81355730000000e01,
                 1.96843670000000e01,
@@ -15307,15 +15943,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Ta
             [
                 8.89256120000000e01,
                 8.19318660000000e01,
                 6.73277280000000e01,
                 4.19543150000000e01,
                 2.77130410000000e01,
                 1.98298060000000e01,
@@ -15484,15 +16120,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # W
             [
                 7.26835210000000e01,
                 6.65725390000000e01,
                 5.45218660000000e01,
                 3.51042250000000e01,
                 2.43743050000000e01,
                 1.81885020000000e01,
@@ -15661,15 +16297,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Re
             [
                 7.09067150000000e01,
                 6.57037140000000e01,
                 5.52189840000000e01,
                 3.68309030000000e01,
                 2.56365300000000e01,
                 1.90080410000000e01,
@@ -15838,15 +16474,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Os
             [
                 5.96083520000000e01,
                 5.62806020000000e01,
                 4.88648650000000e01,
                 3.41600550000000e01,
                 2.44374970000000e01,
                 1.84318460000000e01,
@@ -16015,15 +16651,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Ir
             [
                 5.15493740000000e01,
                 4.92234270000000e01,
                 4.37106450000000e01,
                 3.17225470000000e01,
                 2.32089290000000e01,
                 1.77566590000000e01,
@@ -16192,15 +16828,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Pt
             [
                 4.11424820000000e01,
                 3.93180510000000e01,
                 3.50148090000000e01,
                 2.58710280000000e01,
                 1.95216660000000e01,
                 1.54256100000000e01,
@@ -16369,15 +17005,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Au
             [
                 3.77290460000000e01,
                 3.61091840000000e01,
                 3.22722340000000e01,
                 2.40716250000000e01,
                 1.83385860000000e01,
                 1.46143630000000e01,
@@ -16546,15 +17182,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Hg
             [
                 3.71668150000000e01,
                 3.59903170000000e01,
                 3.29876470000000e01,
                 2.55237630000000e01,
                 1.95407590000000e01,
                 1.54358360000000e01,
@@ -16723,15 +17359,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Tl
             [
                 7.54787320000000e01,
                 6.69797680000000e01,
                 5.27293310000000e01,
                 3.32800020000000e01,
                 2.31647510000000e01,
                 1.73598020000000e01,
@@ -16900,15 +17536,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Pb
             [
                 6.32905510000000e01,
                 5.95286430000000e01,
                 5.12607860000000e01,
                 3.54025850000000e01,
                 2.51394190000000e01,
                 1.87947900000000e01,
@@ -17077,15 +17713,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Bi
             [
                 5.11916750000000e01,
                 4.94069930000000e01,
                 4.49458450000000e01,
                 3.41505430000000e01,
                 2.55045870000000e01,
                 1.95073500000000e01,
@@ -17254,15 +17890,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Po
             [
                 4.57354800000000e01,
                 4.45177550000000e01,
                 4.13554830000000e01,
                 3.29793560000000e01,
                 2.55092680000000e01,
                 1.99242900000000e01,
@@ -17431,15 +18067,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # At
             [
                 3.91638670000000e01,
                 3.84250150000000e01,
                 3.64213580000000e01,
                 3.05411780000000e01,
                 2.46134160000000e01,
                 1.97657890000000e01,
@@ -17608,15 +18244,15 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
-        [
+        [  # Rn
             [
                 3.36514050000000e01,
                 3.31852420000000e01,
                 3.18852830000000e01,
                 2.77786920000000e01,
                 2.32154680000000e01,
                 1.91736050000000e01,
@@ -17785,17 +18421,3027 @@
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
                 0.00000000000000e00,
             ],
         ],
+        [  # Fr
+            [
+                4.32714790000000e02,
+                2.33557930000000e02,
+                1.07018270000000e02,
+                4.40853000000000e01,
+                2.81033000000000e01,
+                2.09345200000000e01,
+                1.66243700000000e01,
+                1.36315900000000e01,
+                1.13991600000000e01,
+                9.66771000000000e00,
+                8.29195000000000e00,
+                7.17998000000000e00,
+                5.51460000000000e00,
+                4.35085000000000e00,
+                3.50978000000000e00,
+                2.88466000000000e00,
+                2.40886000000000e00,
+                1.62326000000000e00,
+                1.16311000000000e00,
+                6.77280000000000e-01,
+                4.41240000000000e-01,
+                1.99950000000000e-01,
+                1.13310000000000e-01,
+            ],
+            [
+                7.17862700000000e01,
+                6.55632800000000e01,
+                5.41920400000000e01,
+                3.73256900000000e01,
+                2.78786200000000e01,
+                2.19222000000000e01,
+                1.77602400000000e01,
+                1.46759000000000e01,
+                1.23098200000000e01,
+                1.04527500000000e01,
+                8.97005000000000e00,
+                7.76957000000000e00,
+                5.97098000000000e00,
+                4.71460000000000e00,
+                3.80673000000000e00,
+                3.13178000000000e00,
+                2.61774000000000e00,
+                1.76774000000000e00,
+                1.26867000000000e00,
+                7.40250000000000e-01,
+                4.82800000000000e-01,
+                2.19040000000000e-01,
+                1.24180000000000e-01,
+            ],
+            [
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+            [
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+            [
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+            [
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+            [
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+        ],
+        [  # Ra
+            [
+                2.64194690000000e02,
+                2.08712820000000e02,
+                1.31086720000000e02,
+                5.85103700000000e01,
+                3.45223400000000e01,
+                2.40579200000000e01,
+                1.83378700000000e01,
+                1.47007500000000e01,
+                1.21522900000000e01,
+                1.02528100000000e01,
+                8.77892000000000e00,
+                7.60345000000000e00,
+                5.85760000000000e00,
+                4.64014000000000e00,
+                3.75788000000000e00,
+                3.09941000000000e00,
+                2.59606000000000e00,
+                1.75958000000000e00,
+                1.26574000000000e00,
+                7.40410000000000e-01,
+                4.83490000000000e-01,
+                2.19640000000000e-01,
+                1.24600000000000e-01,
+            ],
+            [
+                2.65139660000000e02,
+                1.69950980000000e02,
+                9.81252400000000e01,
+                4.99054300000000e01,
+                3.29673500000000e01,
+                2.43765600000000e01,
+                1.91292900000000e01,
+                1.55551100000000e01,
+                1.29496000000000e01,
+                1.09644700000000e01,
+                9.40558000000000e00,
+                8.15430000000000e00,
+                6.28793000000000e00,
+                4.98366000000000e00,
+                4.03792000000000e00,
+                3.33190000000000e00,
+                2.79206000000000e00,
+                1.89439000000000e00,
+                1.36384000000000e00,
+                7.98670000000000e-01,
+                5.21850000000000e-01,
+                2.37220000000000e-01,
+                1.34600000000000e-01,
+            ],
+            [
+                7.15606700000000e01,
+                6.78481200000000e01,
+                5.96614200000000e01,
+                4.35416700000000e01,
+                3.25219600000000e01,
+                2.52514100000000e01,
+                2.02337300000000e01,
+                1.66050300000000e01,
+                1.38797700000000e01,
+                1.17724500000000e01,
+                1.01056100000000e01,
+                8.76316000000000e00,
+                6.75754000000000e00,
+                5.35573000000000e00,
+                4.33974000000000e00,
+                3.58158000000000e00,
+                3.00196000000000e00,
+                2.03809000000000e00,
+                1.46811000000000e00,
+                8.60380000000000e-01,
+                5.62420000000000e-01,
+                2.55780000000000e-01,
+                1.45150000000000e-01,
+            ],
+            [
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+            [
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+            [
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+            [
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+        ],
+        [  # Ac
+            [
+                2.04401840000000e02,
+                1.67213570000000e02,
+                1.16697680000000e02,
+                5.89801600000000e01,
+                3.55482400000000e01,
+                2.45444200000000e01,
+                1.84663300000000e01,
+                1.46614600000000e01,
+                1.20557600000000e01,
+                1.01553600000000e01,
+                8.70674000000000e00,
+                7.56712000000000e00,
+                5.89647000000000e00,
+                4.74234000000000e00,
+                3.90760000000000e00,
+                3.28264000000000e00,
+                2.80160000000000e00,
+                1.98810000000000e00,
+                1.49118000000000e00,
+                9.33350000000000e-01,
+                6.39980000000000e-01,
+                3.12280000000000e-01,
+                1.83660000000000e-01,
+            ],
+            [
+                1.83413630000000e02,
+                1.51781680000000e02,
+                1.06812860000000e02,
+                5.73476600000000e01,
+                3.66708800000000e01,
+                2.62420200000000e01,
+                2.01262600000000e01,
+                1.61394300000000e01,
+                1.33398900000000e01,
+                1.12678800000000e01,
+                9.67509000000000e00,
+                8.41584000000000e00,
+                6.56300000000000e00,
+                5.27983000000000e00,
+                4.35060000000000e00,
+                3.65434000000000e00,
+                3.11813000000000e00,
+                2.21093000000000e00,
+                1.65679000000000e00,
+                1.03537000000000e00,
+                7.09170000000000e-01,
+                3.45550000000000e-01,
+                2.03080000000000e-01,
+            ],
+            [
+                1.61407990000000e02,
+                1.15714320000000e02,
+                8.17711600000000e01,
+                5.00677900000000e01,
+                3.49561700000000e01,
+                2.61999400000000e01,
+                2.05872400000000e01,
+                1.67260600000000e01,
+                1.39261300000000e01,
+                1.18135400000000e01,
+                1.01705400000000e01,
+                8.86227000000000e00,
+                6.92589000000000e00,
+                5.57893000000000e00,
+                4.60112000000000e00,
+                3.86728000000000e00,
+                3.30142000000000e00,
+                2.34264000000000e00,
+                1.75612000000000e00,
+                1.09774000000000e00,
+                7.51960000000000e-01,
+                3.66430000000000e-01,
+                2.15350000000000e-01,
+            ],
+            [
+                6.73757700000000e01,
+                6.51171500000000e01,
+                5.94934200000000e01,
+                4.58749400000000e01,
+                3.48544000000000e01,
+                2.70905200000000e01,
+                2.16503900000000e01,
+                1.77357500000000e01,
+                1.48287300000000e01,
+                1.26068900000000e01,
+                1.08666700000000e01,
+                9.47547000000000e00,
+                7.41036000000000e00,
+                5.97113000000000e00,
+                4.92538000000000e00,
+                4.14008000000000e00,
+                3.53428000000000e00,
+                2.50734000000000e00,
+                1.87893000000000e00,
+                1.17370000000000e00,
+                8.03600000000000e-01,
+                3.91330000000000e-01,
+                2.29900000000000e-01,
+            ],
+            [
+                1.64999540000000e02,
+                9.19493300000000e01,
+                6.88420500000000e01,
+                4.96464500000000e01,
+                3.76575900000000e01,
+                2.93281700000000e01,
+                2.34479400000000e01,
+                1.91936000000000e01,
+                1.60278600000000e01,
+                1.36085200000000e01,
+                1.17157200000000e01,
+                1.02048100000000e01,
+                7.96689000000000e00,
+                6.41109000000000e00,
+                5.28270000000000e00,
+                4.43647000000000e00,
+                3.78433000000000e00,
+                2.68023000000000e00,
+                2.00572000000000e00,
+                1.25030000000000e00,
+                8.54830000000000e-01,
+                4.15460000000000e-01,
+                2.43830000000000e-01,
+            ],
+            [
+                1.71248130000000e02,
+                1.34670270000000e02,
+                9.49592200000000e01,
+                5.88184700000000e01,
+                4.22048900000000e01,
+                3.21668700000000e01,
+                2.54549400000000e01,
+                2.07156500000000e01,
+                1.72342600000000e01,
+                1.45947900000000e01,
+                1.25409800000000e01,
+                1.09080400000000e01,
+                8.49912000000000e00,
+                6.83056000000000e00,
+                5.62305000000000e00,
+                4.71872000000000e00,
+                4.02243000000000e00,
+                2.84476000000000e00,
+                2.12618000000000e00,
+                1.32267000000000e00,
+                9.02950000000000e-01,
+                4.37860000000000e-01,
+                2.56680000000000e-01,
+            ],
+            [
+                2.13470340000000e02,
+                1.68241850000000e02,
+                1.14200900000000e02,
+                6.58443700000000e01,
+                4.60049400000000e01,
+                3.47217600000000e01,
+                2.73472300000000e01,
+                2.21892600000000e01,
+                1.84196600000000e01,
+                1.55715000000000e01,
+                1.33612300000000e01,
+                1.16077400000000e01,
+                9.02748000000000e00,
+                7.24492000000000e00,
+                5.95731000000000e00,
+                4.99428000000000e00,
+                4.25357000000000e00,
+                3.00247000000000e00,
+                2.24037000000000e00,
+                1.39005000000000e00,
+                9.47110000000000e-01,
+                4.57920000000000e-01,
+                2.68030000000000e-01,
+            ],
+        ],
+        [  # Th
+            [
+                1.51305490000000e02,
+                1.32022430000000e02,
+                1.00344620000000e02,
+                5.71424100000000e01,
+                3.68572000000000e01,
+                2.63120900000000e01,
+                2.00921500000000e01,
+                1.60586100000000e01,
+                1.32526600000000e01,
+                1.11956600000000e01,
+                9.62671000000000e00,
+                8.39348000000000e00,
+                6.58810000000000e00,
+                5.34141000000000e00,
+                4.43881000000000e00,
+                3.76176000000000e00,
+                3.23935000000000e00,
+                2.35140000000000e00,
+                1.80344000000000e00,
+                1.17559000000000e00,
+                8.33310000000000e-01,
+                4.29200000000000e-01,
+                2.59690000000000e-01,
+            ],
+            [
+                1.42015310000000e02,
+                1.21733050000000e02,
+                9.18672700000000e01,
+                5.46347100000000e01,
+                3.69218200000000e01,
+                2.71645700000000e01,
+                2.11160700000000e01,
+                1.70503600000000e01,
+                1.41521300000000e01,
+                1.19928500000000e01,
+                1.03287100000000e01,
+                9.01188000000000e00,
+                7.07334000000000e00,
+                5.72966000000000e00,
+                4.75532000000000e00,
+                4.02410000000000e00,
+                3.45992000000000e00,
+                2.50181000000000e00,
+                1.91190000000000e00,
+                1.23895000000000e00,
+                8.74480000000000e-01,
+                4.47660000000000e-01,
+                2.70060000000000e-01,
+            ],
+            [
+                1.17310950000000e02,
+                9.92297800000000e01,
+                7.68788200000000e01,
+                5.03595500000000e01,
+                3.64314400000000e01,
+                2.78344800000000e01,
+                2.20825100000000e01,
+                1.80276800000000e01,
+                1.50511500000000e01,
+                1.27931800000000e01,
+                1.10336600000000e01,
+                9.63193000000000e00,
+                7.55769000000000e00,
+                6.11549000000000e00,
+                5.06884000000000e00,
+                4.28341000000000e00,
+                3.67772000000000e00,
+                2.65041000000000e00,
+                2.01942000000000e00,
+                1.30240000000000e00,
+                9.16170000000000e-01,
+                4.66750000000000e-01,
+                2.80940000000000e-01,
+            ],
+            [
+                9.43173000000000e01,
+                8.38298000000000e01,
+                6.92480800000000e01,
+                4.95421600000000e01,
+                3.73912000000000e01,
+                2.91786500000000e01,
+                2.33999800000000e01,
+                1.92059800000000e01,
+                1.60744500000000e01,
+                1.36753400000000e01,
+                1.17953000000000e01,
+                1.02929700000000e01,
+                8.06570000000000e00,
+                6.51639000000000e00,
+                5.39264000000000e00,
+                4.55010000000000e00,
+                3.90099000000000e00,
+                2.80190000000000e00,
+                2.12859000000000e00,
+                1.36644000000000e00,
+                9.58020000000000e-01,
+                4.85760000000000e-01,
+                2.91700000000000e-01,
+            ],
+            [
+                6.39384900000000e01,
+                6.24467300000000e01,
+                5.85371300000000e01,
+                4.79250300000000e01,
+                3.80867400000000e01,
+                3.04192900000000e01,
+                2.46745200000000e01,
+                2.03673800000000e01,
+                1.70925200000000e01,
+                1.45573700000000e01,
+                1.25588400000000e01,
+                1.09564600000000e01,
+                8.57566000000000e00,
+                6.91831000000000e00,
+                5.71673000000000e00,
+                4.81658000000000e00,
+                4.12376000000000e00,
+                2.95260000000000e00,
+                2.23700000000000e00,
+                1.42991000000000e00,
+                9.99500000000000e-01,
+                5.04590000000000e-01,
+                3.02380000000000e-01,
+            ],
+            [  # ThH5 missing (GEOM)
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+            [  # ThH6 missing (GEOM)
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+        ],
+        [  # Pa
+            [
+                1.66627770000000e02,
+                1.41284220000000e02,
+                1.02456720000000e02,
+                5.44640100000000e01,
+                3.41796000000000e01,
+                2.43027300000000e01,
+                1.86668300000000e01,
+                1.50570800000000e01,
+                1.25481800000000e01,
+                1.06993500000000e01,
+                9.27773000000000e00,
+                8.14965000000000e00,
+                6.47415000000000e00,
+                5.29500000000000e00,
+                4.42690000000000e00,
+                3.76659000000000e00,
+                3.25135000000000e00,
+                2.36411000000000e00,
+                1.81047000000000e00,
+                1.17369000000000e00,
+                8.27720000000000e-01,
+                4.22970000000000e-01,
+                2.54970000000000e-01,
+            ],
+            [
+                1.57076070000000e02,
+                1.29941710000000e02,
+                9.40821000000000e01,
+                5.26866900000000e01,
+                3.47765300000000e01,
+                2.54911900000000e01,
+                1.99067900000000e01,
+                1.61943000000000e01,
+                1.35495700000000e01,
+                1.15701000000000e01,
+                1.00337700000000e01,
+                8.80823000000000e00,
+                6.98220000000000e00,
+                5.69646000000000e00,
+                4.75126000000000e00,
+                4.03374000000000e00,
+                3.47501000000000e00,
+                2.51593000000000e00,
+                1.92001000000000e00,
+                1.23818000000000e00,
+                8.70030000000000e-01,
+                4.42320000000000e-01,
+                2.65980000000000e-01,
+            ],
+            [
+                1.25357500000000e02,
+                9.78437100000000e01,
+                7.23248100000000e01,
+                4.63109800000000e01,
+                3.36240800000000e01,
+                2.59618100000000e01,
+                2.08399900000000e01,
+                1.71993700000000e01,
+                1.44962900000000e01,
+                1.24214900000000e01,
+                1.07866200000000e01,
+                9.47086000000000e00,
+                7.49829000000000e00,
+                6.10563000000000e00,
+                5.08225000000000e00,
+                4.30651000000000e00,
+                3.70349000000000e00,
+                2.67136000000000e00,
+                2.03256000000000e00,
+                1.30504000000000e00,
+                9.14350000000000e-01,
+                4.62990000000000e-01,
+                2.77890000000000e-01,
+            ],
+            [
+                8.59686200000000e01,
+                7.65627700000000e01,
+                6.42651600000000e01,
+                4.69223500000000e01,
+                3.58900500000000e01,
+                2.83126800000000e01,
+                2.29032600000000e01,
+                1.89260700000000e01,
+                1.59240300000000e01,
+                1.36038600000000e01,
+                1.17728300000000e01,
+                1.03012100000000e01,
+                8.10477000000000e00,
+                6.56553000000000e00,
+                5.44249000000000e00,
+                4.59647000000000e00,
+                3.94224000000000e00,
+                2.82988000000000e00,
+                2.14641000000000e00,
+                1.37302000000000e00,
+                9.60020000000000e-01,
+                4.84970000000000e-01,
+                2.90780000000000e-01,
+            ],
+            [
+                6.82275000000000e01,
+                6.56186000000000e01,
+                6.00315200000000e01,
+                4.76359800000000e01,
+                3.75304200000000e01,
+                2.99830600000000e01,
+                2.43945000000000e01,
+                2.02072400000000e01,
+                1.70133900000000e01,
+                1.45306100000000e01,
+                1.25652700000000e01,
+                1.09835700000000e01,
+                8.62243000000000e00,
+                6.96983000000000e00,
+                5.76635000000000e00,
+                4.86152000000000e00,
+                4.16310000000000e00,
+                2.97872000000000e00,
+                2.25344000000000e00,
+                1.43591000000000e00,
+                1.00130000000000e00,
+                5.03920000000000e-01,
+                3.01590000000000e-01,
+            ],
+            [
+                6.46792300000000e01,
+                6.27768600000000e01,
+                5.83981800000000e01,
+                4.80808200000000e01,
+                3.88769800000000e01,
+                3.15484100000000e01,
+                2.58960300000000e01,
+                2.15514400000000e01,
+                1.81846400000000e01,
+                1.55419400000000e01,
+                1.34379700000000e01,
+                1.17392400000000e01,
+                9.19861000000000e00,
+                7.42021000000000e00,
+                6.12678000000000e00,
+                5.15602000000000e00,
+                4.40809000000000e00,
+                3.14348000000000e00,
+                2.37214000000000e00,
+                1.50652000000000e00,
+                1.04847000000000e00,
+                5.26390000000000e-01,
+                3.14710000000000e-01,
+            ],
+            [  # PaH6 missing (GEOM)
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+        ],
+        [  # U
+            [
+                1.59650180000000e02,
+                1.35896100000000e02,
+                9.85086800000000e01,
+                5.23884600000000e01,
+                3.29239600000000e01,
+                2.34920600000000e01,
+                1.81199800000000e01,
+                1.46740300000000e01,
+                1.22716700000000e01,
+                1.04952600000000e01,
+                9.12474000000000e00,
+                8.03373000000000e00,
+                6.40609000000000e00,
+                5.25397000000000e00,
+                4.40118000000000e00,
+                3.74937000000000e00,
+                3.23868000000000e00,
+                2.35491000000000e00,
+                1.80117000000000e00,
+                1.16396000000000e00,
+                8.18810000000000e-01,
+                4.17100000000000e-01,
+                2.51170000000000e-01,
+            ],
+            [
+                1.52026140000000e02,
+                1.28001400000000e02,
+                9.27351000000000e01,
+                5.15592200000000e01,
+                3.37876600000000e01,
+                2.46849400000000e01,
+                1.92730100000000e01,
+                1.57026800000000e01,
+                1.31693600000000e01,
+                1.12756900000000e01,
+                9.80510000000000e00,
+                8.62992000000000e00,
+                6.87215000000000e00,
+                5.62670000000000e00,
+                4.70527000000000e00,
+                4.00174000000000e00,
+                3.45118000000000e00,
+                2.50039000000000e00,
+                1.90650000000000e00,
+                1.22593000000000e00,
+                8.59300000000000e-01,
+                4.35410000000000e-01,
+                2.61510000000000e-01,
+            ],
+            [  # UH2 missing
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+            [
+                6.14627600000000e01,
+                5.81569300000000e01,
+                5.25979400000000e01,
+                4.11735600000000e01,
+                3.21632900000000e01,
+                2.56872500000000e01,
+                2.10129300000000e01,
+                1.75503200000000e01,
+                1.49129800000000e01,
+                1.28533700000000e01,
+                1.12101300000000e01,
+                9.87514000000000e00,
+                7.85336000000000e00,
+                6.41132000000000e00,
+                5.34378000000000e00,
+                4.53007000000000e00,
+                3.89490000000000e00,
+                2.80302000000000e00,
+                2.12548000000000e00,
+                1.35531000000000e00,
+                9.44420000000000e-01,
+                4.74530000000000e-01,
+                2.83820000000000e-01,
+            ],
+            [
+                5.77404400000000e01,
+                5.68541900000000e01,
+                5.30160000000000e01,
+                4.34071000000000e01,
+                3.48271900000000e01,
+                2.81717400000000e01,
+                2.31478600000000e01,
+                1.93339400000000e01,
+                1.63930700000000e01,
+                1.40847800000000e01,
+                1.22416000000000e01,
+                1.07465100000000e01,
+                8.49245000000000e00,
+                6.89665000000000e00,
+                5.72389000000000e00,
+                4.83575000000000e00,
+                4.14631000000000e00,
+                2.96957000000000e00,
+                2.24502000000000e00,
+                1.42686000000000e00,
+                9.92710000000000e-01,
+                4.98010000000000e-01,
+                2.97700000000000e-01,
+            ],
+            [
+                7.94643700000000e01,
+                6.61195700000000e01,
+                5.83424900000000e01,
+                4.58165000000000e01,
+                3.62236200000000e01,
+                2.91719600000000e01,
+                2.39622200000000e01,
+                2.00392100000000e01,
+                1.70204000000000e01,
+                1.46497200000000e01,
+                1.27534500000000e01,
+                1.12117900000000e01,
+                8.87969000000000e00,
+                7.22090000000000e00,
+                5.99789000000000e00,
+                5.06873000000000e00,
+                4.34586000000000e00,
+                3.10918000000000e00,
+                2.34654000000000e00,
+                1.48582000000000e00,
+                1.03041000000000e00,
+                5.14230000000000e-01,
+                3.06560000000000e-01,
+            ],
+            [
+                7.04499300000000e01,
+                6.84799400000000e01,
+                6.34736400000000e01,
+                5.08489300000000e01,
+                4.01019100000000e01,
+                3.21246100000000e01,
+                2.62551100000000e01,
+                2.18601000000000e01,
+                1.84967500000000e01,
+                1.58683700000000e01,
+                1.37750900000000e01,
+                1.20799000000000e01,
+                9.52755000000000e00,
+                7.72245000000000e00,
+                6.39687000000000e00,
+                5.39380000000000e00,
+                4.61589000000000e00,
+                3.29081000000000e00,
+                2.47785000000000e00,
+                1.56486000000000e00,
+                1.08390000000000e00,
+                5.40420000000000e-01,
+                3.22120000000000e-01,
+            ],
+        ],
+        [  # Np
+            [
+                1.52128390000000e02,
+                1.12603310000000e02,
+                7.54650300000000e01,
+                4.07348500000000e01,
+                2.73560900000000e01,
+                2.06809600000000e01,
+                1.66270800000000e01,
+                1.38529700000000e01,
+                1.18126700000000e01,
+                1.02408900000000e01,
+                8.99068000000000e00,
+                7.97264000000000e00,
+                6.41871000000000e00,
+                5.29541000000000e00,
+                4.45260000000000e00,
+                3.80231000000000e00,
+                3.28928000000000e00,
+                2.39479000000000e00,
+                1.83085000000000e00,
+                1.18051000000000e00,
+                8.28830000000000e-01,
+                4.21240000000000e-01,
+                2.53500000000000e-01,
+            ],
+            [
+                1.34237390000000e02,
+                1.04391380000000e02,
+                7.37094800000000e01,
+                4.28461500000000e01,
+                2.97209900000000e01,
+                2.26356900000000e01,
+                1.81746800000000e01,
+                1.50874400000000e01,
+                1.28155700000000e01,
+                1.10712300000000e01,
+                9.68988000000000e00,
+                8.57003000000000e00,
+                6.87038000000000e00,
+                5.64955000000000e00,
+                4.73801000000000e00,
+                4.03733000000000e00,
+                3.48618000000000e00,
+                2.52878000000000e00,
+                1.92769000000000e00,
+                1.23750000000000e00,
+                8.66120000000000e-01,
+                4.38120000000000e-01,
+                2.63030000000000e-01,
+            ],
+            [
+                1.14725700000000e02,
+                8.97632500000000e01,
+                6.66972100000000e01,
+                4.29194500000000e01,
+                3.11632400000000e01,
+                2.41344200000000e01,
+                1.94813300000000e01,
+                1.61874400000000e01,
+                1.37402200000000e01,
+                1.18546900000000e01,
+                1.03605200000000e01,
+                9.14997000000000e00,
+                7.31603000000000e00,
+                6.00250000000000e00,
+                5.02432000000000e00,
+                4.27413000000000e00,
+                3.68517000000000e00,
+                2.66473000000000e00,
+                2.02605000000000e00,
+                1.29529000000000e00,
+                9.03780000000000e-01,
+                4.55000000000000e-01,
+                2.72500000000000e-01,
+            ],
+            [
+                6.00193300000000e01,
+                5.77069100000000e01,
+                5.24809600000000e01,
+                4.08285800000000e01,
+                3.17259300000000e01,
+                2.52753700000000e01,
+                2.06624400000000e01,
+                1.72654300000000e01,
+                1.46871900000000e01,
+                1.26773600000000e01,
+                1.10746900000000e01,
+                9.77215000000000e00,
+                7.79620000000000e00,
+                6.38202000000000e00,
+                5.33098000000000e00,
+                4.52671000000000e00,
+                3.89666000000000e00,
+                2.80840000000000e00,
+                2.12984000000000e00,
+                1.35656000000000e00,
+                9.44080000000000e-01,
+                4.73510000000000e-01,
+                2.83050000000000e-01,
+            ],
+            [
+                5.76363300000000e01,
+                5.57487000000000e01,
+                5.16348100000000e01,
+                4.21036900000000e01,
+                3.38112200000000e01,
+                2.74066600000000e01,
+                2.25760500000000e01,
+                1.89076000000000e01,
+                1.60757400000000e01,
+                1.38491000000000e01,
+                1.20671800000000e01,
+                1.06181700000000e01,
+                8.42496000000000e00,
+                6.86375000000000e00,
+                5.71049000000000e00,
+                4.83309000000000e00,
+                4.14925000000000e00,
+                2.97614000000000e00,
+                2.25024000000000e00,
+                1.42846000000000e00,
+                9.92490000000000e-01,
+                4.96980000000000e-01,
+                2.96900000000000e-01,
+            ],
+            [
+                7.98320500000000e01,
+                7.51734800000000e01,
+                6.60772100000000e01,
+                4.92762900000000e01,
+                3.77995500000000e01,
+                2.99549600000000e01,
+                2.43770500000000e01,
+                2.02708100000000e01,
+                1.71576200000000e01,
+                1.47371100000000e01,
+                1.28142200000000e01,
+                1.12583100000000e01,
+                8.91396000000000e00,
+                7.25124000000000e00,
+                6.02546000000000e00,
+                5.09404000000000e00,
+                4.36877000000000e00,
+                3.12612000000000e00,
+                2.35856000000000e00,
+                1.49187000000000e00,
+                1.03377000000000e00,
+                5.15570000000000e-01,
+                3.07390000000000e-01,
+            ],
+            [
+                9.08035900000000e01,
+                8.56049900000000e01,
+                7.45057100000000e01,
+                5.41947900000000e01,
+                4.09874200000000e01,
+                3.22515300000000e01,
+                2.61389000000000e01,
+                2.16751400000000e01,
+                1.83064600000000e01,
+                1.56954400000000e01,
+                1.36261600000000e01,
+                1.19551600000000e01,
+                9.44349000000000e00,
+                7.66703000000000e00,
+                6.36036000000000e00,
+                5.36936000000000e00,
+                4.59895000000000e00,
+                3.28198000000000e00,
+                2.47087000000000e00,
+                1.55800000000000e00,
+                1.07727000000000e00,
+                5.35640000000000e-01,
+                3.18890000000000e-01,
+            ],
+        ],
+        [  # Pu
+            [
+                1.72740680000000e02,
+                1.45604780000000e02,
+                1.01760140000000e02,
+                5.01348300000000e01,
+                2.99893400000000e01,
+                2.08783400000000e01,
+                1.59825000000000e01,
+                1.29731100000000e01,
+                1.09295300000000e01,
+                9.43743000000000e00,
+                8.28943000000000e00,
+                7.37207000000000e00,
+                5.98626000000000e00,
+                4.98306000000000e00,
+                4.22293000000000e00,
+                3.62924000000000e00,
+                3.15521000000000e00,
+                2.31466000000000e00,
+                1.77495000000000e00,
+                1.14438000000000e00,
+                8.01380000000000e-01,
+                4.04890000000000e-01,
+                2.42910000000000e-01,
+            ],
+            [
+                1.40659240000000e02,
+                1.09308290000000e02,
+                7.29347700000000e01,
+                3.99873900000000e01,
+                2.70421600000000e01,
+                2.03958100000000e01,
+                1.63706000000000e01,
+                1.36552700000000e01,
+                1.16835500000000e01,
+                1.01759300000000e01,
+                8.97967000000000e00,
+                8.00428000000000e00,
+                6.50611000000000e00,
+                5.40993000000000e00,
+                4.57661000000000e00,
+                3.92566000000000e00,
+                3.40651000000000e00,
+                2.48861000000000e00,
+                1.90186000000000e00,
+                1.22001000000000e00,
+                8.51400000000000e-01,
+                4.28050000000000e-01,
+                2.56190000000000e-01,
+            ],
+            [
+                9.77401900000000e01,
+                7.66673600000000e01,
+                5.94821600000000e01,
+                3.95056600000000e01,
+                2.89200100000000e01,
+                2.25125400000000e01,
+                1.82688400000000e01,
+                1.52650100000000e01,
+                1.30297600000000e01,
+                1.13019800000000e01,
+                9.92682000000000e00,
+                8.80704000000000e00,
+                7.09721000000000e00,
+                5.85928000000000e00,
+                4.92812000000000e00,
+                4.20758000000000e00,
+                3.63754000000000e00,
+                2.64001000000000e00,
+                2.00929000000000e00,
+                1.28295000000000e00,
+                8.93130000000000e-01,
+                4.47770000000000e-01,
+                2.67660000000000e-01,
+            ],
+            [
+                5.53410200000000e01,
+                5.33923900000000e01,
+                4.91137600000000e01,
+                3.89121200000000e01,
+                3.05323900000000e01,
+                2.44542300000000e01,
+                2.00613900000000e01,
+                1.68098900000000e01,
+                1.43347700000000e01,
+                1.24010300000000e01,
+                1.08558900000000e01,
+                9.59757000000000e00,
+                7.68289000000000e00,
+                6.30672000000000e00,
+                5.27963000000000e00,
+                4.49058000000000e00,
+                3.87024000000000e00,
+                2.79355000000000e00,
+                2.11881000000000e00,
+                1.34758000000000e00,
+                9.36160000000000e-01,
+                4.68220000000000e-01,
+                2.79590000000000e-01,
+            ],
+            [
+                6.44204800000000e01,
+                5.78758900000000e01,
+                5.16984400000000e01,
+                4.13225200000000e01,
+                3.30419600000000e01,
+                2.67589700000000e01,
+                2.20508700000000e01,
+                1.84869900000000e01,
+                1.57401000000000e01,
+                1.35812100000000e01,
+                1.18528500000000e01,
+                1.04460800000000e01,
+                8.31250000000000e00,
+                6.78861000000000e00,
+                5.65888000000000e00,
+                4.79638000000000e00,
+                4.12202000000000e00,
+                2.96021000000000e00,
+                2.23808000000000e00,
+                1.41850000000000e00,
+                9.83790000000000e-01,
+                4.91240000000000e-01,
+                2.93160000000000e-01,
+            ],
+            [
+                8.48162300000000e01,
+                7.92047800000000e01,
+                6.81430500000000e01,
+                4.92446000000000e01,
+                3.72617800000000e01,
+                2.93656200000000e01,
+                2.38516500000000e01,
+                1.98304800000000e01,
+                1.67967800000000e01,
+                1.44437200000000e01,
+                1.25760100000000e01,
+                1.10645900000000e01,
+                8.78442000000000e00,
+                7.16280000000000e00,
+                5.96342000000000e00,
+                5.04907000000000e00,
+                4.33488000000000e00,
+                3.10599000000000e00,
+                2.34348000000000e00,
+                1.48016000000000e00,
+                1.02381000000000e00,
+                5.09110000000000e-01,
+                3.03180000000000e-01,
+            ],
+            [
+                1.04800850000000e02,
+                9.65146400000000e01,
+                8.05042500000000e01,
+                5.54090700000000e01,
+                4.09972200000000e01,
+                3.19652500000000e01,
+                2.58009100000000e01,
+                2.13575000000000e01,
+                1.80287900000000e01,
+                1.54598100000000e01,
+                1.34288200000000e01,
+                1.17907500000000e01,
+                9.32951000000000e00,
+                7.58707000000000e00,
+                6.30301000000000e00,
+                5.32695000000000e00,
+                4.56642000000000e00,
+                3.26192000000000e00,
+                2.45545000000000e00,
+                1.54578000000000e00,
+                1.06682000000000e00,
+                5.28810000000000e-01,
+                3.14420000000000e-01,
+            ],
+        ],
+        [  # Am
+            [
+                1.65602040000000e02,
+                1.40497900000000e02,
+                9.90178200000000e01,
+                4.93590700000000e01,
+                2.96192400000000e01,
+                2.06060600000000e01,
+                1.57483000000000e01,
+                1.27644400000000e01,
+                1.07432900000000e01,
+                9.27216000000000e00,
+                8.14368000000000e00,
+                7.24416000000000e00,
+                5.88867000000000e00,
+                4.90888000000000e00,
+                4.16626000000000e00,
+                3.58539000000000e00,
+                3.12064000000000e00,
+                2.29340000000000e00,
+                1.75963000000000e00,
+                1.13363000000000e00,
+                7.92730000000000e-01,
+                3.99540000000000e-01,
+                2.39500000000000e-01,
+            ],
+            [
+                1.33035510000000e02,
+                1.04920150000000e02,
+                7.14375700000000e01,
+                3.97059900000000e01,
+                2.67872400000000e01,
+                2.01190900000000e01,
+                1.60990800000000e01,
+                1.34053800000000e01,
+                1.14612800000000e01,
+                9.98176000000000e00,
+                8.81165000000000e00,
+                7.85960000000000e00,
+                6.39932000000000e00,
+                5.33090000000000e00,
+                4.51755000000000e00,
+                3.88082000000000e00,
+                3.37176000000000e00,
+                2.46801000000000e00,
+                1.88739000000000e00,
+                1.21006000000000e00,
+                8.43380000000000e-01,
+                4.23060000000000e-01,
+                2.53010000000000e-01,
+            ],
+            [
+                6.00171500000000e01,
+                5.60454500000000e01,
+                4.85551000000000e01,
+                3.51426600000000e01,
+                2.64217100000000e01,
+                2.08389700000000e01,
+                1.70639300000000e01,
+                1.43636900000000e01,
+                1.23396900000000e01,
+                1.07652600000000e01,
+                9.50448000000000e00,
+                8.47165000000000e00,
+                6.88110000000000e00,
+                5.71677000000000e00,
+                4.83222000000000e00,
+                4.14172000000000e00,
+                3.59127000000000e00,
+                2.61826000000000e00,
+                1.99642000000000e00,
+                1.27477000000000e00,
+                8.86100000000000e-01,
+                4.42800000000000e-01,
+                2.64300000000000e-01,
+            ],
+            [
+                5.46144300000000e01,
+                5.11618600000000e01,
+                4.71127900000000e01,
+                3.75251800000000e01,
+                2.95311700000000e01,
+                2.36871500000000e01,
+                1.94572200000000e01,
+                1.63294500000000e01,
+                1.39514500000000e01,
+                1.20946300000000e01,
+                1.06104900000000e01,
+                9.40057000000000e00,
+                7.55488000000000e00,
+                6.22254000000000e00,
+                5.22356000000000e00,
+                4.45266000000000e00,
+                3.84409000000000e00,
+                2.78182000000000e00,
+                2.11193000000000e00,
+                1.34279000000000e00,
+                9.31770000000000e-01,
+                4.65030000000000e-01,
+                2.77480000000000e-01,
+            ],
+            [  # AmH4 missing
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+            [
+                9.84837900000000e01,
+                8.86034800000000e01,
+                7.23488700000000e01,
+                4.95093900000000e01,
+                3.67445600000000e01,
+                2.87272700000000e01,
+                2.32551600000000e01,
+                1.93161900000000e01,
+                1.63678900000000e01,
+                1.40916600000000e01,
+                1.22892600000000e01,
+                1.08318700000000e01,
+                8.63152000000000e00,
+                7.06198000000000e00,
+                5.89640000000000e00,
+                5.00396000000000e00,
+                4.30398000000000e00,
+                3.09233000000000e00,
+                2.33546000000000e00,
+                1.47434000000000e00,
+                1.01829000000000e00,
+                5.04900000000000e-01,
+                3.00300000000000e-01,
+            ],
+            [
+                1.13335150000000e02,
+                1.02516090000000e02,
+                8.30136200000000e01,
+                5.52298300000000e01,
+                4.03635400000000e01,
+                3.13181900000000e01,
+                2.52331600000000e01,
+                2.08827200000000e01,
+                1.76395700000000e01,
+                1.51435500000000e01,
+                1.31727500000000e01,
+                1.15836000000000e01,
+                9.19352000000000e00,
+                7.49702000000000e00,
+                6.24268000000000e00,
+                5.28594000000000e00,
+                4.53799000000000e00,
+                3.24901000000000e00,
+                2.44786000000000e00,
+                1.54055000000000e00,
+                1.06204000000000e00,
+                5.25310000000000e-01,
+                3.12070000000000e-01,
+            ],
+        ],
+        [  # Cm
+            [
+                1.34397870000000e02,
+                1.16174320000000e02,
+                8.63865200000000e01,
+                4.71493500000000e01,
+                2.97740500000000e01,
+                2.12860100000000e01,
+                1.64817600000000e01,
+                1.34221500000000e01,
+                1.12973100000000e01,
+                9.72665000000000e00,
+                8.51214000000000e00,
+                7.54147000000000e00,
+                6.08224000000000e00,
+                5.03649000000000e00,
+                4.25215000000000e00,
+                3.64471000000000e00,
+                3.16276000000000e00,
+                2.31365000000000e00,
+                1.77098000000000e00,
+                1.13848000000000e00,
+                7.95370000000000e-01,
+                4.00560000000000e-01,
+                2.40110000000000e-01,
+            ],
+            [
+                1.26612030000000e02,
+                1.09321250000000e02,
+                8.15723600000000e01,
+                4.70010300000000e01,
+                3.12023600000000e01,
+                2.28860500000000e01,
+                1.78996500000000e01,
+                1.46120400000000e01,
+                1.22877600000000e01,
+                1.05566200000000e01,
+                9.21542000000000e00,
+                8.14449000000000e00,
+                6.54005000000000e00,
+                5.39650000000000e00,
+                4.54305000000000e00,
+                3.88481000000000e00,
+                3.36435000000000e00,
+                2.45147000000000e00,
+                1.87098000000000e00,
+                1.19772000000000e00,
+                8.34320000000000e-01,
+                4.18350000000000e-01,
+                2.50210000000000e-01,
+            ],
+            [
+                9.92439600000000e01,
+                7.90151500000000e01,
+                6.03295100000000e01,
+                4.00819000000000e01,
+                2.93585500000000e01,
+                2.27763000000000e01,
+                1.83964100000000e01,
+                1.53028700000000e01,
+                1.30129200000000e01,
+                1.12536800000000e01,
+                9.86184000000000e00,
+                8.73456000000000e00,
+                7.02436000000000e00,
+                5.79428000000000e00,
+                4.87283000000000e00,
+                4.16137000000000e00,
+                3.59896000000000e00,
+                2.61408000000000e00,
+                1.98975000000000e00,
+                1.26865000000000e00,
+                8.81300000000000e-01,
+                4.40150000000000e-01,
+                2.62710000000000e-01,
+            ],
+            [
+                5.46754500000000e01,
+                5.29826400000000e01,
+                4.87627000000000e01,
+                3.84660300000000e01,
+                2.99916200000000e01,
+                2.38921900000000e01,
+                1.95266100000000e01,
+                1.63253800000000e01,
+                1.39077500000000e01,
+                1.20304700000000e01,
+                1.05370300000000e01,
+                9.32432000000000e00,
+                7.48280000000000e00,
+                6.15946000000000e00,
+                5.17002000000000e00,
+                4.40767000000000e00,
+                3.80624000000000e00,
+                2.75616000000000e00,
+                2.09296000000000e00,
+                1.32994000000000e00,
+                9.21720000000000e-01,
+                4.58740000000000e-01,
+                2.73310000000000e-01,
+            ],
+            [
+                8.45347300000000e01,
+                7.57999500000000e01,
+                6.27375400000000e01,
+                4.44811000000000e01,
+                3.35258000000000e01,
+                2.63562200000000e01,
+                2.13871200000000e01,
+                1.77920400000000e01,
+                1.50970200000000e01,
+                1.30153700000000e01,
+                1.13665700000000e01,
+                1.00328800000000e01,
+                8.01758000000000e00,
+                6.57766000000000e00,
+                5.50607000000000e00,
+                4.68359000000000e00,
+                4.03679000000000e00,
+                2.91224000000000e00,
+                2.20546000000000e00,
+                1.39615000000000e00,
+                9.65210000000000e-01,
+                4.78710000000000e-01,
+                2.84710000000000e-01,
+            ],
+            [
+                1.10667900000000e02,
+                9.67153000000000e01,
+                7.59750200000000e01,
+                5.03030900000000e01,
+                3.69564000000000e01,
+                2.87507400000000e01,
+                2.31990700000000e01,
+                1.92245300000000e01,
+                1.62621200000000e01,
+                1.39830200000000e01,
+                1.21836800000000e01,
+                1.07323800000000e01,
+                8.54739000000000e00,
+                6.99301000000000e00,
+                5.84043000000000e00,
+                4.95847000000000e00,
+                4.26669000000000e00,
+                3.06810000000000e00,
+                2.31785000000000e00,
+                1.46231000000000e00,
+                1.00866000000000e00,
+                4.98650000000000e-01,
+                2.96080000000000e-01,
+            ],
+            [
+                1.33958250000000e02,
+                1.16031480000000e02,
+                8.86352200000000e01,
+                5.60350700000000e01,
+                4.03477900000000e01,
+                3.11150200000000e01,
+                2.49872400000000e01,
+                2.06390300000000e01,
+                1.74139100000000e01,
+                1.49408800000000e01,
+                1.29935600000000e01,
+                1.14264900000000e01,
+                9.07407000000000e00,
+                7.40641000000000e00,
+                6.17347000000000e00,
+                5.23239000000000e00,
+                4.49583000000000e00,
+                3.22345000000000e00,
+                2.42985000000000e00,
+                1.52819000000000e00,
+                1.05191000000000e00,
+                5.18470000000000e-01,
+                3.07390000000000e-01,
+            ],
+        ],
+        [  # Bk
+            [
+                1.50084160000000e02,
+                1.29489300000000e02,
+                9.33386400000000e01,
+                4.75743700000000e01,
+                2.87210300000000e01,
+                1.99726200000000e01,
+                1.52301700000000e01,
+                1.23184200000000e01,
+                1.03534300000000e01,
+                8.93024000000000e00,
+                7.84391000000000e00,
+                6.98171000000000e00,
+                5.68827000000000e00,
+                4.75626000000000e00,
+                4.04986000000000e00,
+                3.49608000000000e00,
+                3.05137000000000e00,
+                2.25387000000000e00,
+                1.73367000000000e00,
+                1.11727000000000e00,
+                7.79580000000000e-01,
+                3.90750000000000e-01,
+                2.33590000000000e-01,
+            ],
+            [
+                1.25927410000000e02,
+                1.04072830000000e02,
+                7.58864500000000e01,
+                4.32369500000000e01,
+                2.87502800000000e01,
+                2.11786000000000e01,
+                1.66537700000000e01,
+                1.36738100000000e01,
+                1.15652200000000e01,
+                9.99085000000000e00,
+                8.76671000000000e00,
+                7.78499000000000e00,
+                6.30383000000000e00,
+                5.23750000000000e00,
+                4.43390000000000e00,
+                3.80850000000000e00,
+                3.30998000000000e00,
+                2.42570000000000e00,
+                1.85628000000000e00,
+                1.18927000000000e00,
+                8.27280000000000e-01,
+                4.13210000000000e-01,
+                2.46640000000000e-01,
+            ],
+            [
+                9.42400900000000e01,
+                7.75243900000000e01,
+                5.89429600000000e01,
+                3.90623400000000e01,
+                2.86154000000000e01,
+                2.22014200000000e01,
+                1.79361600000000e01,
+                1.49285100000000e01,
+                1.27060600000000e01,
+                1.10009500000000e01,
+                9.65288000000000e00,
+                8.56113000000000e00,
+                6.90353000000000e00,
+                5.70875000000000e00,
+                4.81127000000000e00,
+                4.11626000000000e00,
+                3.56521000000000e00,
+                2.59587000000000e00,
+                1.97800000000000e00,
+                1.26105000000000e00,
+                8.74990000000000e-01,
+                4.35810000000000e-01,
+                2.59800000000000e-01,
+            ],
+            [
+                5.29670000000000e01,
+                5.12081000000000e01,
+                4.72097200000000e01,
+                3.73875500000000e01,
+                2.92191000000000e01,
+                2.33037200000000e01,
+                1.90603100000000e01,
+                1.59482500000000e01,
+                1.35995200000000e01,
+                1.17770200000000e01,
+                1.03277100000000e01,
+                9.15081000000000e00,
+                7.36232000000000e00,
+                6.07461000000000e00,
+                5.10935000000000e00,
+                4.36353000000000e00,
+                3.77348000000000e00,
+                2.73883000000000e00,
+                2.08194000000000e00,
+                1.32281000000000e00,
+                9.15730000000000e-01,
+                4.54560000000000e-01,
+                2.70500000000000e-01,
+            ],
+            [
+                6.40310000000000e01,
+                5.76315700000000e01,
+                5.04511300000000e01,
+                3.99025500000000e01,
+                3.17426200000000e01,
+                2.56004300000000e01,
+                2.10403300000000e01,
+                1.76213600000000e01,
+                1.50076100000000e01,
+                1.29656800000000e01,
+                1.13372000000000e01,
+                1.00142700000000e01,
+                8.00811000000000e00,
+                6.57121000000000e00,
+                5.50088000000000e00,
+                4.67913000000000e00,
+                4.03290000000000e00,
+                2.90939000000000e00,
+                2.20320000000000e00,
+                1.39432000000000e00,
+                9.63550000000000e-01,
+                4.77560000000000e-01,
+                2.84030000000000e-01,
+            ],
+            [  # BkH5 missing (GEOM)
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+            [  # BkH6 missing (GEOM)
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+        ],
+        [  # Cf
+            [
+                1.48009190000000e02,
+                1.27668280000000e02,
+                9.18844400000000e01,
+                4.66738900000000e01,
+                2.81153000000000e01,
+                1.95155900000000e01,
+                1.48547000000000e01,
+                1.19926300000000e01,
+                1.00613000000000e01,
+                8.66330000000000e00,
+                7.59745000000000e00,
+                6.75291000000000e00,
+                5.48976000000000e00,
+                4.58350000000000e00,
+                3.89923000000000e00,
+                3.36439000000000e00,
+                2.93578000000000e00,
+                2.16854000000000e00,
+                1.66849000000000e00,
+                1.07587000000000e00,
+                7.51200000000000e-01,
+                3.77540000000000e-01,
+                2.26470000000000e-01,
+            ],
+            [
+                1.30798730000000e02,
+                1.03869160000000e02,
+                7.09979000000000e01,
+                3.93130600000000e01,
+                2.62475400000000e01,
+                1.94913500000000e01,
+                1.54458200000000e01,
+                1.27645500000000e01,
+                1.08527200000000e01,
+                9.41456000000000e00,
+                8.28890000000000e00,
+                7.38110000000000e00,
+                6.00267000000000e00,
+                5.00367000000000e00,
+                4.24702000000000e00,
+                3.65571000000000e00,
+                3.18266000000000e00,
+                2.33930000000000e00,
+                1.79304000000000e00,
+                1.15014000000000e00,
+                8.00340000000000e-01,
+                4.00330000000000e-01,
+                2.39540000000000e-01,
+            ],
+            [
+                5.33942300000000e01,
+                5.04801000000000e01,
+                4.47056500000000e01,
+                3.30884500000000e01,
+                2.49852400000000e01,
+                1.96813400000000e01,
+                1.60762000000000e01,
+                1.35014100000000e01,
+                1.15794600000000e01,
+                1.00917600000000e01,
+                8.90614000000000e00,
+                7.93899000000000e00,
+                6.45670000000000e00,
+                5.37602000000000e00,
+                4.55606000000000e00,
+                3.91539000000000e00,
+                3.40338000000000e00,
+                2.49290000000000e00,
+                1.90548000000000e00,
+                1.21734000000000e00,
+                8.44790000000000e-01,
+                4.20840000000000e-01,
+                2.51250000000000e-01,
+            ],
+            [
+                5.04030000000000e01,
+                4.88894600000000e01,
+                4.51750100000000e01,
+                3.60185500000000e01,
+                2.82961100000000e01,
+                2.26345400000000e01,
+                1.85399200000000e01,
+                1.55218100000000e01,
+                1.32371200000000e01,
+                1.14612700000000e01,
+                1.00478300000000e01,
+                8.89968000000000e00,
+                7.15518000000000e00,
+                5.90016000000000e00,
+                4.96036000000000e00,
+                4.23493000000000e00,
+                3.66146000000000e00,
+                2.65675000000000e00,
+                2.01927000000000e00,
+                1.28290000000000e00,
+                8.88320000000000e-01,
+                4.41810000000000e-01,
+                2.63650000000000e-01,
+            ],
+            [
+                8.15874700000000e01,
+                6.86608200000000e01,
+                5.65880100000000e01,
+                4.13108400000000e01,
+                3.17640400000000e01,
+                2.52149100000000e01,
+                2.05502500000000e01,
+                1.71270100000000e01,
+                1.45428400000000e01,
+                1.25405500000000e01,
+                1.09527700000000e01,
+                9.66819000000000e00,
+                7.72784000000000e00,
+                6.34239000000000e00,
+                5.31173000000000e00,
+                4.52060000000000e00,
+                3.89818000000000e00,
+                2.81464000000000e00,
+                2.13212000000000e00,
+                1.34898000000000e00,
+                9.31800000000000e-01,
+                4.61940000000000e-01,
+                2.75210000000000e-01,
+            ],
+            [  # CfH5 missing
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+            [
+                1.29701490000000e02,
+                1.11196890000000e02,
+                8.43720000000000e01,
+                5.39448000000000e01,
+                3.91948300000000e01,
+                3.03204900000000e01,
+                2.43568100000000e01,
+                2.01026300000000e01,
+                1.69427700000000e01,
+                1.45209100000000e01,
+                1.26163400000000e01,
+                1.10860700000000e01,
+                8.79404000000000e00,
+                7.17342000000000e00,
+                5.97752000000000e00,
+                5.06580000000000e00,
+                4.35269000000000e00,
+                3.12102000000000e00,
+                2.35235000000000e00,
+                1.47826000000000e00,
+                1.01662000000000e00,
+                5.00830000000000e-01,
+                2.97400000000000e-01,
+            ],
+        ],
+        [  # Es
+            [
+                1.41220170000000e02,
+                1.22520680000000e02,
+                8.90107400000000e01,
+                4.57447300000000e01,
+                2.77131900000000e01,
+                1.92896700000000e01,
+                1.46962900000000e01,
+                1.18616100000000e01,
+                9.94153000000000e00,
+                8.54826000000000e00,
+                7.48478000000000e00,
+                6.64205000000000e00,
+                5.38322000000000e00,
+                4.48284000000000e00,
+                3.80542000000000e00,
+                3.27772000000000e00,
+                2.85606000000000e00,
+                2.10408000000000e00,
+                1.61590000000000e00,
+                1.03939000000000e00,
+                7.24710000000000e-01,
+                3.64000000000000e-01,
+                2.18650000000000e-01,
+            ],
+            [
+                1.27119070000000e02,
+                1.01167160000000e02,
+                6.90944700000000e01,
+                3.84335200000000e01,
+                2.57933500000000e01,
+                1.92100200000000e01,
+                1.52410000000000e01,
+                1.25963000000000e01,
+                1.07033800000000e01,
+                9.27613000000000e00,
+                8.15778000000000e00,
+                7.25573000000000e00,
+                5.88731000000000e00,
+                4.89785000000000e00,
+                4.15039000000000e00,
+                3.56770000000000e00,
+                3.10252000000000e00,
+                2.27543000000000e00,
+                1.74123000000000e00,
+                1.11427000000000e00,
+                7.74260000000000e-01,
+                3.86930000000000e-01,
+                2.31780000000000e-01,
+            ],
+            [
+                5.15499300000000e01,
+                4.91951700000000e01,
+                4.38725300000000e01,
+                3.27274200000000e01,
+                2.47930800000000e01,
+                1.95486400000000e01,
+                1.59633400000000e01,
+                1.33936100000000e01,
+                1.14716600000000e01,
+                9.98283000000000e00,
+                8.79652000000000e00,
+                7.82961000000000e00,
+                6.35059000000000e00,
+                5.27574000000000e00,
+                4.46283000000000e00,
+                3.82948000000000e00,
+                3.32455000000000e00,
+                2.42938000000000e00,
+                1.85373000000000e00,
+                1.18144000000000e00,
+                8.18690000000000e-01,
+                4.07470000000000e-01,
+                2.43510000000000e-01,
+            ],
+            [
+                4.87142300000000e01,
+                4.71908400000000e01,
+                4.36761400000000e01,
+                3.51176500000000e01,
+                2.77848700000000e01,
+                2.23133400000000e01,
+                1.83099600000000e01,
+                1.53383400000000e01,
+                1.30793500000000e01,
+                1.13191000000000e01,
+                9.91614000000000e00,
+                8.77583000000000e00,
+                7.04338000000000e00,
+                5.79839000000000e00,
+                4.86763000000000e00,
+                4.15045000000000e00,
+                3.58445000000000e00,
+                2.59517000000000e00,
+                1.96924000000000e00,
+                1.24831000000000e00,
+                8.63240000000000e-01,
+                4.29020000000000e-01,
+                2.56290000000000e-01,
+            ],
+            [
+                8.53606600000000e01,
+                7.04284500000000e01,
+                5.68603800000000e01,
+                4.09584000000000e01,
+                3.13950300000000e01,
+                2.49036700000000e01,
+                2.02901400000000e01,
+                1.69042800000000e01,
+                1.43470300000000e01,
+                1.23646900000000e01,
+                1.07923500000000e01,
+                9.52025000000000e00,
+                7.59949000000000e00,
+                6.22938000000000e00,
+                5.21138000000000e00,
+                4.43095000000000e00,
+                3.81765000000000e00,
+                2.75169000000000e00,
+                2.08152000000000e00,
+                1.31416000000000e00,
+                9.06490000000000e-01,
+                4.48930000000000e-01,
+                2.67670000000000e-01,
+            ],
+            [
+                1.17457620000000e02,
+                9.40368600000000e01,
+                7.06831300000000e01,
+                4.71236300000000e01,
+                3.51066300000000e01,
+                2.75008100000000e01,
+                2.22441900000000e01,
+                1.84361400000000e01,
+                1.55817300000000e01,
+                1.33811300000000e01,
+                1.16435800000000e01,
+                1.02434300000000e01,
+                8.14007000000000e00,
+                6.64869000000000e00,
+                5.54605000000000e00,
+                4.70421000000000e00,
+                4.04495000000000e00,
+                2.90435000000000e00,
+                2.19103000000000e00,
+                1.37833000000000e00,
+                9.48560000000000e-01,
+                4.68210000000000e-01,
+                2.78670000000000e-01,
+            ],
+            [
+                1.50763530000000e02,
+                1.17597930000000e02,
+                8.50999300000000e01,
+                5.37332400000000e01,
+                3.89845200000000e01,
+                3.01309200000000e01,
+                2.41804600000000e01,
+                1.99356900000000e01,
+                1.67838100000000e01,
+                1.43694000000000e01,
+                1.24720300000000e01,
+                1.09487800000000e01,
+                8.67021000000000e00,
+                7.06206000000000e00,
+                5.87746000000000e00,
+                4.97579000000000e00,
+                4.27151000000000e00,
+                3.05728000000000e00,
+                2.30104000000000e00,
+                1.44292000000000e00,
+                9.90930000000000e-01,
+                4.87620000000000e-01,
+                2.89730000000000e-01,
+            ],
+        ],
+        [  # Fm
+            [
+                1.34513240000000e02,
+                1.17365110000000e02,
+                8.60922200000000e01,
+                4.48044200000000e01,
+                2.73252700000000e01,
+                1.90895400000000e01,
+                1.45664700000000e01,
+                1.17577800000000e01,
+                9.84597000000000e00,
+                8.45414000000000e00,
+                7.38996000000000e00,
+                6.54636000000000e00,
+                5.28777000000000e00,
+                4.39055000000000e00,
+                3.71821000000000e00,
+                3.19646000000000e00,
+                2.78094000000000e00,
+                2.04308000000000e00,
+                1.56620000000000e00,
+                1.00519000000000e00,
+                7.00110000000000e-01,
+                3.51650000000000e-01,
+                2.11570000000000e-01,
+            ],
+            [
+                1.23419780000000e02,
+                9.80796000000000e01,
+                6.73261100000000e01,
+                3.77049500000000e01,
+                2.54441800000000e01,
+                1.90089500000000e01,
+                1.50992900000000e01,
+                1.24780100000000e01,
+                1.05937400000000e01,
+                9.16938000000000e00,
+                8.05210000000000e00,
+                7.15094000000000e00,
+                5.78578000000000e00,
+                4.80168000000000e00,
+                4.06079000000000e00,
+                3.48505000000000e00,
+                3.02668000000000e00,
+                2.21450000000000e00,
+                1.69184000000000e00,
+                1.08041000000000e00,
+                7.49900000000000e-01,
+                3.74680000000000e-01,
+                2.24750000000000e-01,
+            ],
+            [
+                4.92489800000000e01,
+                4.71164900000000e01,
+                4.23467900000000e01,
+                3.20194900000000e01,
+                2.44465800000000e01,
+                1.93482600000000e01,
+                1.58217100000000e01,
+                1.32748600000000e01,
+                1.13611400000000e01,
+                9.87499000000000e00,
+                8.68970000000000e00,
+                7.72376000000000e00,
+                6.24831000000000e00,
+                5.17919000000000e00,
+                4.37315000000000e00,
+                3.74698000000000e00,
+                3.24901000000000e00,
+                2.36894000000000e00,
+                1.80486000000000e00,
+                1.14803000000000e00,
+                7.94700000000000e-01,
+                3.95420000000000e-01,
+                2.36620000000000e-01,
+            ],
+            [
+                4.88289600000000e01,
+                4.67101500000000e01,
+                4.27341700000000e01,
+                3.42569100000000e01,
+                2.71850100000000e01,
+                2.18934500000000e01,
+                1.79996100000000e01,
+                1.50945700000000e01,
+                1.28774400000000e01,
+                1.11448400000000e01,
+                9.76124000000000e00,
+                8.63533000000000e00,
+                6.92358000000000e00,
+                5.69363000000000e00,
+                4.77490000000000e00,
+                4.06773000000000e00,
+                3.51025000000000e00,
+                2.53738000000000e00,
+                1.92303000000000e00,
+                1.21689000000000e00,
+                8.40670000000000e-01,
+                4.17690000000000e-01,
+                2.49810000000000e-01,
+            ],
+            [
+                8.99278200000000e01,
+                7.07326700000000e01,
+                5.59993400000000e01,
+                4.02168300000000e01,
+                3.09059100000000e01,
+                2.45634500000000e01,
+                2.00342000000000e01,
+                1.66975800000000e01,
+                1.41706300000000e01,
+                1.22082400000000e01,
+                1.06500500000000e01,
+                9.38878000000000e00,
+                7.48444000000000e00,
+                6.12720000000000e00,
+                5.12004000000000e00,
+                4.34896000000000e00,
+                3.74380000000000e00,
+                2.69385000000000e00,
+                2.03514000000000e00,
+                1.28258000000000e00,
+                8.83790000000000e-01,
+                4.37520000000000e-01,
+                2.61150000000000e-01,
+            ],
+            [
+                1.16817350000000e02,
+                9.32645400000000e01,
+                7.00509200000000e01,
+                4.66547100000000e01,
+                3.47567800000000e01,
+                2.72346500000000e01,
+                2.20313300000000e01,
+                1.82566300000000e01,
+                1.54237200000000e01,
+                1.32378500000000e01,
+                1.15111700000000e01,
+                1.01196800000000e01,
+                8.03016000000000e00,
+                6.55020000000000e00,
+                5.45752000000000e00,
+                4.62446000000000e00,
+                3.97292000000000e00,
+                2.84776000000000e00,
+                2.14560000000000e00,
+                1.34738000000000e00,
+                9.26340000000000e-01,
+                4.57060000000000e-01,
+                2.72310000000000e-01,
+            ],
+            [
+                1.35612200000000e02,
+                1.12692760000000e02,
+                8.38706100000000e01,
+                5.33717400000000e01,
+                3.87175500000000e01,
+                2.99159300000000e01,
+                2.40013000000000e01,
+                1.97798800000000e01,
+                1.66432600000000e01,
+                1.42393700000000e01,
+                1.23498800000000e01,
+                1.08330400000000e01,
+                8.56521000000000e00,
+                6.96653000000000e00,
+                5.79060000000000e00,
+                4.89689000000000e00,
+                4.19981000000000e00,
+                3.00047000000000e00,
+                2.25534000000000e00,
+                1.41191000000000e00,
+                9.68800000000000e-01,
+                4.76650000000000e-01,
+                2.83530000000000e-01,
+            ],
+        ],
+        [  # Md
+            [
+                1.30207200000000e02,
+                1.14111530000000e02,
+                8.43232500000000e01,
+                4.41735800000000e01,
+                2.69219800000000e01,
+                1.87618300000000e01,
+                1.42890700000000e01,
+                1.15253100000000e01,
+                9.65452000000000e00,
+                8.29885000000000e00,
+                7.26543000000000e00,
+                6.44733000000000e00,
+                5.22619000000000e00,
+                4.35283000000000e00,
+                3.69532000000000e00,
+                3.18262000000000e00,
+                2.77250000000000e00,
+                2.03981000000000e00,
+                1.56323000000000e00,
+                1.00019000000000e00,
+                6.93780000000000e-01,
+                3.45450000000000e-01,
+                2.06730000000000e-01,
+            ],
+            [
+                1.22358400000000e02,
+                9.67485900000000e01,
+                6.68292500000000e01,
+                3.73575000000000e01,
+                2.51065100000000e01,
+                1.86943300000000e01,
+                1.48200100000000e01,
+                1.22392800000000e01,
+                1.03950300000000e01,
+                9.00699000000000e00,
+                7.92101000000000e00,
+                7.04601000000000e00,
+                5.71955000000000e00,
+                4.76033000000000e00,
+                4.03508000000000e00,
+                3.46900000000000e00,
+                3.01648000000000e00,
+                2.21020000000000e00,
+                1.68822000000000e00,
+                1.07509000000000e00,
+                7.43390000000000e-01,
+                3.68410000000000e-01,
+                2.19860000000000e-01,
+            ],
+            [
+                5.05776500000000e01,
+                4.82323300000000e01,
+                4.31074800000000e01,
+                3.21977700000000e01,
+                2.43573900000000e01,
+                1.91617800000000e01,
+                1.56147000000000e01,
+                1.30800000000000e01,
+                1.11905700000000e01,
+                9.73130000000000e00,
+                8.57131000000000e00,
+                7.62750000000000e00,
+                6.18597000000000e00,
+                5.13923000000000e00,
+                4.34747000000000e00,
+                3.73022000000000e00,
+                3.23772000000000e00,
+                2.36333000000000e00,
+                1.80006000000000e00,
+                1.14193000000000e00,
+                7.87670000000000e-01,
+                3.88930000000000e-01,
+                2.31620000000000e-01,
+            ],
+            [
+                7.12250100000000e01,
+                5.94085900000000e01,
+                4.89787800000000e01,
+                3.55944200000000e01,
+                2.71964200000000e01,
+                2.15383500000000e01,
+                1.75689600000000e01,
+                1.46827100000000e01,
+                1.25133600000000e01,
+                1.08340600000000e01,
+                9.50074000000000e00,
+                8.41922000000000e00,
+                6.77716000000000e00,
+                5.59528000000000e00,
+                4.70881000000000e00,
+                4.02301000000000e00,
+                3.47951000000000e00,
+                2.52352000000000e00,
+                1.91421000000000e00,
+                1.20886000000000e00,
+                8.31960000000000e-01,
+                4.09750000000000e-01,
+                2.43690000000000e-01,
+            ],
+            [
+                1.00338530000000e02,
+                8.43364300000000e01,
+                6.43830000000000e01,
+                4.21400900000000e01,
+                3.08493900000000e01,
+                2.39708700000000e01,
+                1.93555900000000e01,
+                1.60717600000000e01,
+                1.36333100000000e01,
+                1.17603700000000e01,
+                1.02817000000000e01,
+                9.08764000000000e00,
+                7.28416000000000e00,
+                5.99359000000000e00,
+                5.03012000000000e00,
+                4.28763000000000e00,
+                3.70116000000000e00,
+                2.67423000000000e00,
+                2.02313000000000e00,
+                1.27316000000000e00,
+                8.74250000000000e-01,
+                4.29160000000000e-01,
+                2.54760000000000e-01,
+            ],
+            [  # MdH5 missing (GEOM)
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+            [  # MdH6 missing (GEOM)
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+                0.00000000000000e00,
+            ],
+        ],
+        [  # No
+            [
+                1.24805280000000e02,
+                1.10004500000000e02,
+                8.21183900000000e01,
+                4.35324100000000e01,
+                2.66190500000000e01,
+                1.85568300000000e01,
+                1.41261500000000e01,
+                1.13882900000000e01,
+                9.53719000000000e00,
+                8.19771000000000e00,
+                7.17785000000000e00,
+                6.37109000000000e00,
+                5.16720000000000e00,
+                4.30564000000000e00,
+                3.65622000000000e00,
+                3.14915000000000e00,
+                2.74301000000000e00,
+                2.01619000000000e00,
+                1.54266000000000e00,
+                9.83030000000000e-01,
+                6.79080000000000e-01,
+                3.35580000000000e-01,
+                2.00020000000000e-01,
+            ],
+            [
+                1.16764440000000e02,
+                9.57311100000000e01,
+                6.71224100000000e01,
+                3.76422800000000e01,
+                2.51782600000000e01,
+                1.86618300000000e01,
+                1.47429700000000e01,
+                1.21468300000000e01,
+                1.03010700000000e01,
+                8.91776000000000e00,
+                7.83892000000000e00,
+                6.97156000000000e00,
+                5.65895000000000e00,
+                4.71043000000000e00,
+                3.99304000000000e00,
+                3.43269000000000e00,
+                2.98437000000000e00,
+                2.18458000000000e00,
+                1.66616000000000e00,
+                1.05708000000000e00,
+                7.28160000000000e-01,
+                3.58320000000000e-01,
+                2.13050000000000e-01,
+            ],
+            [
+                5.01539300000000e01,
+                4.79467800000000e01,
+                4.28472600000000e01,
+                3.20060400000000e01,
+                2.41919600000000e01,
+                1.90043700000000e01,
+                1.54660100000000e01,
+                1.29435000000000e01,
+                1.10680800000000e01,
+                9.62290000000000e00,
+                8.47600000000000e00,
+                7.54380000000000e00,
+                6.12081000000000e00,
+                5.08723000000000e00,
+                4.30470000000000e00,
+                3.69396000000000e00,
+                3.20611000000000e00,
+                2.33862000000000e00,
+                1.77892000000000e00,
+                1.12462000000000e00,
+                7.72950000000000e-01,
+                3.79090000000000e-01,
+                2.24940000000000e-01,
+            ],
+            [
+                9.13663900000000e01,
+                6.90314800000000e01,
+                5.36426300000000e01,
+                3.65348500000000e01,
+                2.71761000000000e01,
+                2.12644300000000e01,
+                1.72504600000000e01,
+                1.43838400000000e01,
+                1.22513400000000e01,
+                1.06102800000000e01,
+                9.31146000000000e00,
+                8.25946000000000e00,
+                6.66245000000000e00,
+                5.51106000000000e00,
+                4.64514000000000e00,
+                3.97324000000000e00,
+                3.43925000000000e00,
+                2.49618000000000e00,
+                1.89245000000000e00,
+                1.19160000000000e00,
+                8.17120000000000e-01,
+                3.99530000000000e-01,
+                2.36660000000000e-01,
+            ],
+            [
+                1.24250160000000e02,
+                9.36045400000000e01,
+                6.68688500000000e01,
+                4.21117700000000e01,
+                3.04955400000000e01,
+                2.35931200000000e01,
+                1.90153800000000e01,
+                1.57803700000000e01,
+                1.33883600000000e01,
+                1.15557700000000e01,
+                1.01109200000000e01,
+                8.94473000000000e00,
+                7.18260000000000e00,
+                5.91944000000000e00,
+                4.97419000000000e00,
+                4.24392000000000e00,
+                3.66572000000000e00,
+                2.64986000000000e00,
+                2.00341000000000e00,
+                1.25714000000000e00,
+                8.60310000000000e-01,
+                4.19460000000000e-01,
+                2.48070000000000e-01,
+            ],
+            [
+                1.29447610000000e02,
+                9.78022200000000e01,
+                7.05399100000000e01,
+                4.49644600000000e01,
+                3.27582600000000e01,
+                2.54115300000000e01,
+                2.04944800000000e01,
+                1.70008300000000e01,
+                1.44106000000000e01,
+                1.24242700000000e01,
+                1.08583100000000e01,
+                9.59515000000000e00,
+                7.68910000000000e00,
+                6.32555000000000e00,
+                5.30715000000000e00,
+                4.52174000000000e00,
+                3.90087000000000e00,
+                2.81260000000000e00,
+                2.12219000000000e00,
+                1.32783000000000e00,
+                9.06890000000000e-01,
+                4.40840000000000e-01,
+                2.60250000000000e-01,
+            ],
+            [
+                1.34820670000000e02,
+                1.02188720000000e02,
+                7.44006500000000e01,
+                4.79164700000000e01,
+                3.50575700000000e01,
+                2.72357800000000e01,
+                2.19652600000000e01,
+                1.82071400000000e01,
+                1.54169700000000e01,
+                1.32770900000000e01,
+                1.15910500000000e01,
+                1.02322400000000e01,
+                8.18488000000000e00,
+                6.72313000000000e00,
+                5.63325000000000e00,
+                4.79398000000000e00,
+                4.13142000000000e00,
+                2.97234000000000e00,
+                2.23886000000000e00,
+                1.39734000000000e00,
+                9.52720000000000e-01,
+                4.61880000000000e-01,
+                2.72240000000000e-01,
+            ],
+        ],
+        [  # Lr
+            [
+                2.06653320000000e02,
+                8.36937500000000e01,
+                6.48432200000000e01,
+                3.87234300000000e01,
+                2.51567100000000e01,
+                1.80960100000000e01,
+                1.40318300000000e01,
+                1.14483000000000e01,
+                9.66738000000000e00,
+                8.36011000000000e00,
+                7.35352000000000e00,
+                6.54992000000000e00,
+                5.33800000000000e00,
+                4.46120000000000e00,
+                3.79540000000000e00,
+                3.27300000000000e00,
+                2.85329000000000e00,
+                2.09996000000000e00,
+                1.60786000000000e00,
+                1.02469000000000e00,
+                7.07000000000000e-01,
+                3.47460000000000e-01,
+                2.05910000000000e-01,
+            ],
+            [
+                9.23161300000000e01,
+                8.29673800000000e01,
+                6.58155800000000e01,
+                4.09485200000000e01,
+                2.79903000000000e01,
+                2.06982400000000e01,
+                1.61941600000000e01,
+                1.31960200000000e01,
+                1.10779900000000e01,
+                9.50865000000000e00,
+                8.30041000000000e00,
+                7.34103000000000e00,
+                5.91147000000000e00,
+                4.89525000000000e00,
+                4.13545000000000e00,
+                3.54680000000000e00,
+                3.07861000000000e00,
+                2.24866000000000e00,
+                1.71340000000000e00,
+                1.08574000000000e00,
+                7.46680000000000e-01,
+                3.65350000000000e-01,
+                2.16000000000000e-01,
+            ],
+            [
+                8.45082300000000e01,
+                7.08844100000000e01,
+                5.46073800000000e01,
+                3.67023400000000e01,
+                2.69875800000000e01,
+                2.08759700000000e01,
+                1.67762200000000e01,
+                1.38910500000000e01,
+                1.17749600000000e01,
+                1.01664300000000e01,
+                8.90597000000000e00,
+                7.89279000000000e00,
+                6.36602000000000e00,
+                5.27133000000000e00,
+                4.44973000000000e00,
+                3.81233000000000e00,
+                3.30536000000000e00,
+                2.40784000000000e00,
+                1.83068000000000e00,
+                1.15650000000000e00,
+                7.93790000000000e-01,
+                3.87320000000000e-01,
+                2.28620000000000e-01,
+            ],
+            [
+                4.75131300000000e01,
+                4.61744600000000e01,
+                4.28144500000000e01,
+                3.43869400000000e01,
+                2.71100000000000e01,
+                2.16792100000000e01,
+                1.77218900000000e01,
+                1.48050900000000e01,
+                1.26061100000000e01,
+                1.09063200000000e01,
+                9.56063000000000e00,
+                8.47226000000000e00,
+                6.82493000000000e00,
+                5.64154000000000e00,
+                4.75381000000000e00,
+                4.06613000000000e00,
+                3.52014000000000e00,
+                2.55652000000000e00,
+                1.93941000000000e00,
+                1.22164000000000e00,
+                8.37020000000000e-01,
+                4.07400000000000e-01,
+                2.40130000000000e-01,
+            ],
+            [
+                2.42422010000000e02,
+                5.17872100000000e01,
+                4.62957100000000e01,
+                3.67861900000000e01,
+                2.92534000000000e01,
+                2.35192300000000e01,
+                1.92597900000000e01,
+                1.60851700000000e01,
+                1.36784800000000e01,
+                1.18139300000000e01,
+                1.03373100000000e01,
+                9.14394000000000e00,
+                7.34146000000000e00,
+                6.05112000000000e00,
+                5.08654000000000e00,
+                4.34171000000000e00,
+                3.75204000000000e00,
+                2.71549000000000e00,
+                2.05487000000000e00,
+                1.29012000000000e00,
+                8.82130000000000e-01,
+                4.28140000000000e-01,
+                2.51940000000000e-01,
+            ],
+            [
+                1.43635660000000e02,
+                9.60464200000000e01,
+                6.86157000000000e01,
+                4.55604500000000e01,
+                3.39675300000000e01,
+                2.65910500000000e01,
+                2.14849100000000e01,
+                1.77937700000000e01,
+                1.50381700000000e01,
+                1.29231500000000e01,
+                1.12595600000000e01,
+                9.92270000000000e00,
+                7.91779000000000e00,
+                6.49467000000000e00,
+                5.43838000000000e00,
+                4.62759000000000e00,
+                3.98889000000000e00,
+                2.87345000000000e00,
+                2.16766000000000e00,
+                1.35586000000000e00,
+                9.25140000000000e-01,
+                4.47800000000000e-01,
+                2.63150000000000e-01,
+            ],
+            [
+                1.76310910000000e02,
+                1.22395460000000e02,
+                8.30180800000000e01,
+                5.16133400000000e01,
+                3.73991000000000e01,
+                2.88827900000000e01,
+                2.31674700000000e01,
+                1.91031400000000e01,
+                1.60971100000000e01,
+                1.38030600000000e01,
+                1.20054900000000e01,
+                1.05648400000000e01,
+                8.41032000000000e00,
+                6.88539000000000e00,
+                5.75609000000000e00,
+                4.89097000000000e00,
+                4.21068000000000e00,
+                3.02566000000000e00,
+                2.27829000000000e00,
+                1.42157000000000e00,
+                9.68480000000000e-01,
+                4.67770000000000e-01,
+                2.74550000000000e-01,
+            ],
+        ],
     ],
     dtype=torch.float64,
 )
+
 refascale = torch.tensor(
     [
         [
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
@@ -18573,38 +22219,192 @@
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
         ],
+        [
+            1.00000000000000,  # Fr
+            1.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+        ],
+        [
+            1.00000000000000,  # Ra
+            1.00000000000000,
+            1.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+        ],
+        [
+            1.00000000000000,  # Ac
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+        ],
+        [
+            1.00000000000000,  # Th
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            0.00000000000000,  # ThH5 missing (GEOM)
+            0.00000000000000,  # ThH6 missing (GEOM)
+        ],
+        [
+            1.00000000000000,  # Pa
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            0.00000000000000,  # PaH6 missing (GEOM)
+        ],
+        [
+            1.00000000000000,  # U
+            1.00000000000000,
+            0.00000000000000,  # UH2 missing
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+        ],
+        [
+            1.00000000000000,  # Np
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+        ],
+        [
+            1.00000000000000,  # Pu
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+        ],
+        [
+            1.00000000000000,  # Am
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            0.00000000000000,  # AmH4 missing
+            1.00000000000000,
+            1.00000000000000,
+        ],
+        [
+            1.00000000000000,  # Cm
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+        ],
+        [
+            1.00000000000000,  # Bk
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            0.00000000000000,  # BkH5 missing (GEOM)
+            0.00000000000000,  # BkH6 missing (GEOM)
+        ],
+        [
+            1.00000000000000,  # Cf
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            0.00000000000000,  # CfH5 missing
+            1.00000000000000,
+        ],
+        [
+            1.00000000000000,  # Es
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+        ],
+        [
+            1.00000000000000,  # Fm
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+        ],
+        [
+            1.00000000000000,  # Md
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            0.00000000000000,  # MdH5 missing (GEOM)
+            0.00000000000000,  # MdH6 missing (GEOM)
+        ],
+        [
+            1.00000000000000,  # No
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+        ],
+        [
+            1.00000000000000,  # Lr
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+            1.00000000000000,
+        ],
     ],
     dtype=torch.float64,
 )
+
 refscount = torch.tensor(
     [
-        [
+        [  # dummy
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
         ],
-        [
+        [  # H
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
         ],
-        [
+        [  # He
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
@@ -19361,122 +23161,294 @@
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
             0.00000000000000,
         ],
+        [
+            0.00000000000000,  # Fr
+            1.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+        ],
+        [
+            0.00000000000000,  # Ra
+            1.00000000000000,
+            2.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+            0.00000000000000,
+        ],
+        [
+            0.00000000000000,  # Ac
+            1.00000000000000,
+            2.00000000000000,
+            3.00000000000000,
+            4.00000000000000,
+            5.00000000000000,
+            6.00000000000000,
+        ],
+        [
+            0.00000000000000,  # Th
+            1.00000000000000,
+            2.00000000000000,
+            3.00000000000000,
+            4.00000000000000,
+            0.00000000000000,  # ThH5 missing (GEOM)
+            0.00000000000000,  # ThH6 missing (GEOM)
+        ],
+        [
+            0.00000000000000,  # Pa
+            1.00000000000000,
+            2.00000000000000,
+            3.00000000000000,
+            4.00000000000000,
+            5.00000000000000,
+            0.00000000000000,  # PaH6 missing (GEOM)
+        ],
+        [
+            0.00000000000000,  # U
+            1.00000000000000,
+            0.00000000000000,  # UH2 missing
+            3.00000000000000,
+            4.00000000000000,
+            5.00000000000000,
+            6.00000000000000,
+        ],
+        [
+            0.00000000000000,  # Np
+            1.00000000000000,
+            2.00000000000000,
+            3.00000000000000,
+            4.00000000000000,
+            5.00000000000000,
+            6.00000000000000,
+        ],
+        [
+            0.00000000000000,  # Pu
+            1.00000000000000,
+            2.00000000000000,
+            3.00000000000000,
+            4.00000000000000,
+            5.00000000000000,
+            6.00000000000000,
+        ],
+        [
+            0.00000000000000,  # Am
+            1.00000000000000,
+            2.00000000000000,
+            3.00000000000000,
+            0.00000000000000,  # AmH4 missing
+            5.00000000000000,
+            6.00000000000000,
+        ],
+        [
+            0.00000000000000,  # Cm
+            1.00000000000000,
+            2.00000000000000,
+            3.00000000000000,
+            4.00000000000000,
+            5.00000000000000,
+            6.00000000000000,
+        ],
+        [
+            0.00000000000000,  # Bk
+            1.00000000000000,
+            2.00000000000000,
+            3.00000000000000,
+            4.00000000000000,
+            0.00000000000000,  # BkH5 missing (GEOM)
+            0.00000000000000,  # BkH6 missing (GEOM)
+        ],
+        [
+            0.00000000000000,  # Cf
+            1.00000000000000,
+            2.00000000000000,
+            3.00000000000000,
+            4.00000000000000,
+            0.00000000000000,  # CfH5 missing
+            6.00000000000000,
+        ],
+        [
+            0.00000000000000,  # Es
+            1.00000000000000,
+            2.00000000000000,
+            3.00000000000000,
+            4.00000000000000,
+            5.00000000000000,
+            6.00000000000000,
+        ],
+        [
+            0.00000000000000,  # Fm
+            1.00000000000000,
+            2.00000000000000,
+            3.00000000000000,
+            4.00000000000000,
+            5.00000000000000,
+            6.00000000000000,
+        ],
+        [
+            0.00000000000000,  # Md
+            1.00000000000000,
+            2.00000000000000,
+            3.00000000000000,
+            4.00000000000000,
+            0.00000000000000,  # MdH5 missing (GEOM)
+            0.00000000000000,  # MdH6 missing (GEOM)
+        ],
+        [
+            0.00000000000000,  # No
+            1.00000000000000,
+            2.00000000000000,
+            3.00000000000000,
+            4.00000000000000,
+            5.00000000000000,
+            6.00000000000000,
+        ],
+        [
+            0.00000000000000,  # Lr
+            1.00000000000000,
+            2.00000000000000,
+            3.00000000000000,
+            4.00000000000000,
+            5.00000000000000,
+            6.00000000000000,
+        ],
     ],
     dtype=torch.float64,
 )
+
 refsys = torch.tensor(
     [
-        [0, 0, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 0, 0, 0, 0, 0, 0],
-        [1, 1, 17, 0, 0, 0, 0],
-        [1, 1, 1, 9, 0, 0, 0],
-        [1, 1, 1, 1, 1, 0, 0],
-        [1, 1, 1, 1, 1, 1, 2],
-        [1, 1, 1, 1, 1, 0, 0],
-        [1, 1, 1, 1, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 0, 0, 0, 0, 0, 0],
-        [1, 1, 17, 0, 0, 0, 0],
-        [1, 1, 1, 9, 0, 0, 0],
-        [1, 1, 1, 1, 0, 0, 0],
-        [1, 1, 1, 1, 1, 0, 0],
-        [1, 1, 1, 1, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 0, 0, 0, 0, 0, 0],
-        [1, 1, 17, 0, 0, 0, 0],
-        [1, 1, 1, 9, 0, 0, 0],
-        [1, 1, 1, 11, 0, 0, 0],
-        [1, 1, 1, 11, 0, 0, 0],
-        [1, 1, 1, 11, 0, 0, 0],
-        [1, 1, 1, 8, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 1, 1, 1, 0, 0, 0],
-        [1, 1, 1, 1, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 1, 1, 1, 1, 0, 0],
-        [1, 1, 1, 1, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 0, 0, 0, 0, 0, 0],
-        [1, 1, 17, 0, 0, 0, 0],
-        [1, 1, 1, 9, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 1, 1, 11, 0, 0, 0],
-        [1, 1, 1, 11, 0, 0, 0],
-        [1, 1, 1, 1, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 1, 1, 1, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 1, 1, 0, 0, 0],
-        [1, 1, 1, 1, 1, 0, 0],
-        [1, 1, 1, 1, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 0, 0, 0, 0, 0, 0],
-        [1, 1, 17, 0, 0, 0, 0],
-        [1, 1, 1, 9, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 0, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 1, 11, 0, 0, 0],
-        [1, 1, 1, 11, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 1, 1, 1, 1, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 1, 1, 1, 0, 0, 0],
-        [1, 1, 1, 1, 1, 0, 0],
-        [1, 1, 1, 1, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [1, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0],  # dummy
+        [1, 1, 0, 0, 0, 0, 0],  # H
+        [1, 0, 0, 0, 0, 0, 0],  # He
+        [1, 1, 17, 0, 0, 0, 0],  # Li
+        [1, 1, 1, 9, 0, 0, 0],  # Be
+        [1, 1, 1, 1, 1, 0, 0],  # B
+        [1, 1, 1, 1, 1, 1, 2],  # C
+        [1, 1, 1, 1, 1, 0, 0],  # N
+        [1, 1, 1, 1, 0, 0, 0],  # O
+        [1, 1, 0, 0, 0, 0, 0],  # F
+        [1, 0, 0, 0, 0, 0, 0],  # Ne
+        [1, 1, 17, 0, 0, 0, 0],  # Na
+        [1, 1, 1, 9, 0, 0, 0],  # Mg
+        [1, 1, 1, 1, 0, 0, 0],  # Al
+        [1, 1, 1, 1, 1, 0, 0],  # Si
+        [1, 1, 1, 1, 0, 0, 0],  # P
+        [1, 1, 1, 0, 0, 0, 0],  # S
+        [1, 1, 0, 0, 0, 0, 0],  # Cl
+        [1, 0, 0, 0, 0, 0, 0],  # Ar
+        [1, 1, 17, 0, 0, 0, 0],  # K
+        [1, 1, 1, 9, 0, 0, 0],  # Ca
+        [1, 1, 1, 11, 0, 0, 0],  # Sc
+        [1, 1, 1, 11, 0, 0, 0],  # Ti
+        [1, 1, 1, 11, 0, 0, 0],  # V
+        [1, 1, 1, 8, 0, 0, 0],  # Cr
+        [1, 1, 1, 0, 0, 0, 0],  # Mn
+        [1, 1, 1, 0, 0, 0, 0],  # Fe
+        [1, 1, 1, 1, 0, 0, 0],  # Co
+        [1, 1, 1, 1, 0, 0, 0],  # Ni
+        [1, 1, 0, 0, 0, 0, 0],  # Cu
+        [1, 1, 0, 0, 0, 0, 0],  # Zn
+        [1, 1, 1, 0, 0, 0, 0],  # Ga
+        [1, 1, 1, 1, 1, 0, 0],  # Ge
+        [1, 1, 1, 1, 0, 0, 0],  # As
+        [1, 1, 1, 0, 0, 0, 0],  # Se
+        [1, 1, 0, 0, 0, 0, 0],  # Br
+        [1, 0, 0, 0, 0, 0, 0],  # Kr
+        [1, 1, 17, 0, 0, 0, 0],  # Rb
+        [1, 1, 1, 9, 0, 0, 0],  # Sr
+        [1, 1, 1, 0, 0, 0, 0],  # Y
+        [1, 1, 1, 11, 0, 0, 0],  # Zr
+        [1, 1, 1, 11, 0, 0, 0],  # Nb
+        [1, 1, 1, 1, 0, 0, 0],  # Mo
+        [1, 1, 1, 0, 0, 0, 0],  # Tc
+        [1, 1, 1, 0, 0, 0, 0],  # Ru
+        [1, 1, 1, 1, 0, 0, 0],  # Rh
+        [1, 1, 1, 0, 0, 0, 0],  # Pd
+        [1, 1, 0, 0, 0, 0, 0],  # Ag
+        [1, 1, 0, 0, 0, 0, 0],  # Cd
+        [1, 1, 1, 1, 0, 0, 0],  # In
+        [1, 1, 1, 1, 1, 0, 0],  # Sn
+        [1, 1, 1, 1, 0, 0, 0],  # Sb
+        [1, 1, 1, 0, 0, 0, 0],  # Te
+        [1, 1, 0, 0, 0, 0, 0],  # I
+        [1, 0, 0, 0, 0, 0, 0],  # Xe
+        [1, 1, 17, 0, 0, 0, 0],  # Cs
+        [1, 1, 1, 9, 0, 0, 0],  # Ba
+        [1, 1, 1, 0, 0, 0, 0],  # La (Lanthanides start)
+        [1, 0, 0, 0, 0, 0, 0],  # Ce
+        [1, 1, 0, 0, 0, 0, 0],  # Pr
+        [1, 1, 0, 0, 0, 0, 0],  # Nd
+        [1, 1, 0, 0, 0, 0, 0],  # Pm
+        [1, 1, 0, 0, 0, 0, 0],  # Sm
+        [1, 1, 0, 0, 0, 0, 0],  # Eu
+        [1, 1, 0, 0, 0, 0, 0],  # Gd
+        [1, 1, 0, 0, 0, 0, 0],  # Tb
+        [1, 1, 0, 0, 0, 0, 0],  # Dy
+        [1, 1, 0, 0, 0, 0, 0],  # Ho
+        [1, 1, 0, 0, 0, 0, 0],  # Er
+        [1, 1, 0, 0, 0, 0, 0],  # Tm
+        [1, 1, 0, 0, 0, 0, 0],  # Yb
+        [1, 1, 0, 0, 0, 0, 0],  # Lu (Lanthanides end)
+        [1, 1, 1, 11, 0, 0, 0],  # Hf
+        [1, 1, 1, 11, 0, 0, 0],  # Ta
+        [1, 1, 1, 0, 0, 0, 0],  # W
+        [1, 1, 1, 0, 0, 0, 0],  # Re
+        [1, 1, 1, 0, 0, 0, 0],  # Os
+        [1, 1, 1, 1, 1, 0, 0],  # Ir
+        [1, 1, 1, 0, 0, 0, 0],  # Pt
+        [1, 1, 0, 0, 0, 0, 0],  # Au
+        [1, 1, 0, 0, 0, 0, 0],  # Hg
+        [1, 1, 1, 1, 0, 0, 0],  # Tl
+        [1, 1, 1, 1, 1, 0, 0],  # Pb
+        [1, 1, 1, 1, 0, 0, 0],  # Bi
+        [1, 1, 1, 0, 0, 0, 0],  # Po
+        [1, 1, 0, 0, 0, 0, 0],  # At
+        [1, 0, 0, 0, 0, 0, 0],  # Rn
+        [1, 1, 0, 0, 0, 0, 0],  # Fr
+        [1, 1, 1, 0, 0, 0, 0],  # Ra
+        [1, 1, 1, 1, 1, 1, 1],  # Ac (Actinides start)
+        [1, 1, 1, 1, 1, 0, 0],  # Th (ThH5, ThH6 missing)
+        [1, 1, 1, 1, 1, 1, 0],  # Pa
+        [1, 1, 0, 1, 1, 1, 1],  # U (UH2 missing)
+        [1, 1, 1, 1, 1, 1, 1],  # Np
+        [1, 1, 1, 1, 1, 1, 1],  # Pu
+        [1, 1, 1, 1, 0, 1, 1],  # Am (AmH4 missing)
+        [1, 1, 1, 1, 1, 1, 1],  # Cm
+        [1, 1, 1, 1, 1, 0, 0],  # Bk (BkH5, BkH6 missing)
+        [1, 1, 1, 1, 1, 0, 1],  # Cf (CfH5 missing)
+        [1, 1, 1, 1, 1, 1, 1],  # Es
+        [1, 1, 1, 1, 1, 1, 1],  # Fm
+        [1, 1, 1, 1, 1, 0, 0],  # Md (MdH5, MdH6 missing)
+        [1, 1, 1, 1, 1, 1, 1],  # No
+        [1, 1, 1, 1, 1, 1, 1],  # Lr (Actinides end)
     ],
     dtype=torch.long,
 )
+
 refc = torch.tensor(
     [
-        [0, 0, 0, 0, 0, 0, 0],
-        [3, 1, 0, 0, 0, 0, 0],
-        [3, 0, 0, 0, 0, 0, 0],
-        [3, 1, 1, 0, 0, 0, 0],
-        [3, 1, 1, 1, 0, 0, 0],
-        [3, 1, 1, 1, 1, 0, 0],
-        [3, 3, 1, 3, 1, 3, 3],
-        [3, 3, 1, 1, 3, 0, 0],
-        [3, 3, 1, 3, 0, 0, 0],
-        [3, 1, 0, 0, 0, 0, 0],
-        [3, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0],  # dummy
+        [3, 1, 0, 0, 0, 0, 0],  # H
+        [3, 0, 0, 0, 0, 0, 0],  # He
+        [3, 1, 1, 0, 0, 0, 0],  # Li
+        [3, 1, 1, 1, 0, 0, 0],  # Be
+        [3, 1, 1, 1, 1, 0, 0],  # B
+        [3, 3, 1, 3, 1, 3, 3],  # C
+        [3, 3, 1, 1, 3, 0, 0],  # N
+        [3, 3, 1, 3, 0, 0, 0],  # O
+        [3, 1, 0, 0, 0, 0, 0],  # F
+        [3, 0, 0, 0, 0, 0, 0],  # Ne
         [3, 1, 1, 0, 0, 0, 0],
         [3, 1, 1, 1, 0, 0, 0],
         [3, 1, 1, 1, 0, 0, 0],
         [3, 1, 1, 1, 1, 0, 0],
         [3, 1, 1, 1, 0, 0, 0],
         [3, 1, 1, 0, 0, 0, 0],
         [3, 1, 0, 0, 0, 0, 0],
@@ -19545,16 +23517,34 @@
         [3, 1, 0, 0, 0, 0, 0],
         [3, 1, 1, 1, 0, 0, 0],
         [3, 1, 1, 1, 1, 0, 0],
         [3, 1, 1, 1, 0, 0, 0],
         [3, 1, 1, 0, 0, 0, 0],
         [3, 1, 0, 0, 0, 0, 0],
         [3, 0, 0, 0, 0, 0, 0],
+        [3, 1, 0, 0, 0, 0, 0],  # Fr
+        [3, 1, 1, 0, 0, 0, 0],  # Ra
+        [3, 1, 1, 1, 1, 1, 1],  # Ac
+        [3, 1, 1, 1, 1, 0, 0],  # Th (ThH5, ThH6 missing)
+        [3, 1, 1, 1, 1, 1, 0],  # Pa (PaH6 missing)
+        [3, 1, 0, 1, 3, 3, 1],  # U (UH2 missing)
+        [3, 1, 1, 1, 1, 1, 1],  # Np
+        [3, 1, 1, 1, 1, 1, 1],  # Pu
+        [3, 1, 1, 1, 0, 1, 1],  # Am (AmH4 missing)
+        [3, 1, 1, 1, 1, 1, 1],  # Cm
+        [3, 1, 1, 1, 1, 0, 0],  # Bk (BkH5, BkH6 missing)
+        [3, 1, 1, 1, 1, 0, 1],  # Cf (CfH5 missing)
+        [3, 1, 1, 1, 1, 1, 1],  # Es
+        [3, 1, 1, 1, 1, 1, 1],  # Fm
+        [3, 1, 1, 1, 1, 0, 0],  # Md (MdH5, MdH6 missing)
+        [3, 1, 1, 1, 3, 3, 1],  # No
+        [3, 1, 1, 1, 1, 1, 1],  # Lr
     ]
 )
+
 secscale = torch.tensor(
     [
         [0.00000000000000],
         [0.50000000000000],
         [0.00000000000000],
         [0.00000000000000],
         [0.00000000000000],
@@ -19570,14 +23560,15 @@
         [0.00000000000000],
         [0.00000000000000],
         [0.00000000000000],
         [0.50000000000000],
     ],
     dtype=torch.float64,
 )
+
 secalpha = torch.tensor(
     [
         [
             0.00000000000000e00,
             0.00000000000000e00,
             0.00000000000000e00,
             0.00000000000000e00,
```

### Comparing `tad_dftd4-0.0.4/src/tad_dftd4.egg-info/PKG-INFO` & `tad_dftd4-0.1.0/src/tad_dftd4.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,631 +1,689 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7461 642d  : 2.1.Name: tad-
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7461 645f  : 2.1.Name: tad_
 00000020: 6466 7464 340a 5665 7273 696f 6e3a 2030  dftd4.Version: 0
-00000030: 2e30 2e34 0a53 756d 6d61 7279 3a20 546f  .0.4.Summary: To
+00000030: 2e31 2e30 0a53 756d 6d61 7279 3a20 546f  .1.0.Summary: To
 00000040: 7263 6820 6175 746f 6469 6666 2044 4654  rch autodiff DFT
 00000050: 2d44 3420 696d 706c 656d 656e 7461 7469  -D4 implementati
 00000060: 6f6e 0a41 7574 686f 723a 2022 4d61 7276  on.Author: "Marv
 00000070: 696e 2046 7269 6564 6522 0a4c 6963 656e  in Friede".Licen
-00000080: 7365 3a20 4c47 504c 2d33 2e30 0a43 6c61  se: LGPL-3.0.Cla
-00000090: 7373 6966 6965 723a 2046 7261 6d65 776f  ssifier: Framewo
-000000a0: 726b 203a 3a20 5079 7465 7374 0a43 6c61  rk :: Pytest.Cla
-000000b0: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
-000000c0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000000d0: 203a 3a20 474e 5520 4c65 7373 6572 2047   :: GNU Lesser G
-000000e0: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
-000000f0: 6365 6e73 6520 7633 2028 4c47 504c 7633  cense v3 (LGPLv3
-00000100: 290a 436c 6173 7369 6669 6572 3a20 4e61  ).Classifier: Na
-00000110: 7475 7261 6c20 4c61 6e67 7561 6765 203a  tural Language :
-00000120: 3a20 456e 676c 6973 680a 436c 6173 7369  : English.Classi
-00000130: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000140: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000150: 7468 6f6e 203a 3a20 330a 436c 6173 7369  thon :: 3.Classi
-00000160: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000170: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000180: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
-00000190: 790a 436c 6173 7369 6669 6572 3a20 5072  y.Classifier: Pr
-000001a0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001b0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001c0: 332e 380a 436c 6173 7369 6669 6572 3a20  3.8.Classifier: 
-000001d0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001e0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001f0: 3a20 332e 390a 436c 6173 7369 6669 6572  : 3.9.Classifier
-00000200: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000210: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000220: 203a 3a20 332e 3130 0a43 6c61 7373 6966   :: 3.10.Classif
-00000230: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000240: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000250: 686f 6e20 3a3a 2033 2e31 310a 436c 6173  hon :: 3.11.Clas
-00000260: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000270: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000280: 5079 7468 6f6e 203a 3a20 496d 706c 656d  Python :: Implem
-00000290: 656e 7461 7469 6f6e 203a 3a20 4350 7974  entation :: CPyt
-000002a0: 686f 6e0a 436c 6173 7369 6669 6572 3a20  hon.Classifier: 
-000002b0: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
-000002c0: 6669 632f 456e 6769 6e65 6572 696e 670a  fic/Engineering.
-000002d0: 436c 6173 7369 6669 6572 3a20 5479 7069  Classifier: Typi
-000002e0: 6e67 203a 3a20 5479 7065 640a 5265 7175  ng :: Typed.Requ
-000002f0: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
-00000300: 2e38 0a44 6573 6372 6970 7469 6f6e 2d43  .8.Description-C
-00000310: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-00000320: 742f 782d 7273 740a 5072 6f76 6964 6573  t/x-rst.Provides
-00000330: 2d45 7874 7261 3a20 6465 760a 4c69 6365  -Extra: dev.Lice
-00000340: 6e73 652d 4669 6c65 3a20 434f 5059 494e  nse-File: COPYIN
-00000350: 470a 4c69 6365 6e73 652d 4669 6c65 3a20  G.License-File: 
-00000360: 434f 5059 494e 472e 4c45 5353 4552 0a0a  COPYING.LESSER..
-00000370: 546f 7263 6820 6175 746f 6469 6666 2066  Torch autodiff f
-00000380: 6f72 2044 4654 2d44 340a 3d3d 3d3d 3d3d  or DFT-D4.======
-00000390: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000003a0: 3d3d 3d0a 0a2e 2e20 696d 6167 653a 3a20  ===.... image:: 
-000003b0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000003c0: 6c64 732e 696f 2f62 6164 6765 2f70 7974  lds.io/badge/pyt
-000003d0: 686f 6e2d 2533 453d 332e 382d 626c 7565  hon-%3E=3.8-blue
-000003e0: 2e73 7667 0a20 2020 203a 7461 7267 6574  .svg.    :target
-000003f0: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00000400: 6965 6c64 732e 696f 2f62 6164 6765 2f70  ields.io/badge/p
-00000410: 7974 686f 6e2d 332e 3825 3230 7c25 3230  ython-3.8%20|%20
-00000420: 332e 3925 3230 7c25 3230 332e 3130 2532  3.9%20|%203.10%2
-00000430: 307c 2532 3033 2e31 312d 626c 7565 2e73  0|%203.11-blue.s
-00000440: 7667 0a20 2020 203a 616c 743a 2050 7974  vg.    :alt: Pyt
-00000450: 686f 6e20 5665 7273 696f 6e73 0a0a 2e2e  hon Versions....
-00000460: 2069 6d61 6765 3a3a 2068 7474 7073 3a2f   image:: https:/
-00000470: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000480: 6769 7468 7562 2f76 2f72 656c 6561 7365  github/v/release
-00000490: 2f64 6674 6434 2f74 6164 2d64 6674 6434  /dftd4/tad-dftd4
-000004a0: 0a20 2020 203a 7461 7267 6574 3a20 6874  .    :target: ht
-000004b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000004c0: 2f64 6674 6434 2f74 6164 2d64 6674 6434  /dftd4/tad-dftd4
-000004d0: 2f72 656c 6561 7365 732f 6c61 7465 7374  /releases/latest
-000004e0: 0a20 2020 203a 616c 743a 2052 656c 6561  .    :alt: Relea
-000004f0: 7365 0a0a 2e2e 2069 6d61 6765 3a3a 2068  se.... image:: h
-00000500: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000510: 6473 2e69 6f2f 7079 7069 2f76 2f74 6164  ds.io/pypi/v/tad
-00000520: 2d64 6674 6434 0a20 2020 203a 7461 7267  -dftd4.    :targ
-00000530: 6574 3a20 6874 7470 733a 2f2f 7079 7069  et: https://pypi
-00000540: 2e6f 7267 2f70 726f 6a65 6374 2f74 6164  .org/project/tad
-00000550: 2d64 6674 6434 2f0a 2020 2020 3a61 6c74  -dftd4/.    :alt
-00000560: 3a20 5079 5049 0a0a 2e2e 2069 6d61 6765  : PyPI.... image
-00000570: 3a3a 2068 7474 7073 3a2f 2f69 6d67 2e73  :: https://img.s
-00000580: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000590: 4c69 6365 6e73 652d 4c47 504c 5f76 332d  License-LGPL_v3-
-000005a0: 626c 7565 2e73 7667 0a20 2020 203a 7461  blue.svg.    :ta
-000005b0: 7267 6574 3a20 6874 7470 733a 2f2f 7777  rget: https://ww
-000005c0: 772e 676e 752e 6f72 672f 6c69 6365 6e73  w.gnu.org/licens
-000005d0: 6573 2f6c 6770 6c2d 332e 300a 2020 2020  es/lgpl-3.0.    
-000005e0: 3a61 6c74 3a20 4c47 504c 2d33 2e30 0a0a  :alt: LGPL-3.0..
-000005f0: 2e2e 2069 6d61 6765 3a3a 2068 7474 7073  .. image:: https
-00000600: 3a2f 2f67 6974 6875 622e 636f 6d2f 6466  ://github.com/df
-00000610: 7464 342f 6466 7464 342f 776f 726b 666c  td4/dftd4/workfl
-00000620: 6f77 732f 4349 2f62 6164 6765 2e73 7667  ows/CI/badge.svg
-00000630: 0a20 2020 203a 7461 7267 6574 3a20 6874  .    :target: ht
-00000640: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000650: 2f64 6674 6434 2f64 6674 6434 2f61 6374  /dftd4/dftd4/act
-00000660: 696f 6e73 0a20 2020 203a 616c 743a 2043  ions.    :alt: C
-00000670: 490a 0a2e 2e20 696d 6167 653a 3a20 6874  I.... image:: ht
-00000680: 7470 733a 2f2f 7265 6164 7468 6564 6f63  tps://readthedoc
-00000690: 732e 6f72 672f 7072 6f6a 6563 7473 2f74  s.org/projects/t
-000006a0: 6164 2d64 6674 6434 2f62 6164 6765 2f3f  ad-dftd4/badge/?
-000006b0: 7665 7273 696f 6e3d 6c61 7465 7374 0a20  version=latest. 
-000006c0: 2020 203a 7461 7267 6574 3a20 6874 7470     :target: http
-000006d0: 733a 2f2f 7461 642d 6466 7464 342e 7265  s://tad-dftd4.re
-000006e0: 6164 7468 6564 6f63 732e 696f 0a20 2020  adthedocs.io.   
-000006f0: 203a 616c 743a 2044 6f63 756d 656e 7461   :alt: Documenta
-00000700: 7469 6f6e 2053 7461 7475 730a 0a2e 2e20  tion Status.... 
-00000710: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
-00000720: 636f 6465 636f 762e 696f 2f67 682f 6466  codecov.io/gh/df
-00000730: 7464 342f 7461 642d 6466 7464 342f 6272  td4/tad-dftd4/br
-00000740: 616e 6368 2f6d 6169 6e2f 6772 6170 682f  anch/main/graph/
-00000750: 6261 6467 652e 7376 673f 746f 6b65 6e3d  badge.svg?token=
-00000760: 4f47 4a4a 6e5a 3674 3447 0a20 2020 203a  OGJJnZ6t4G.    :
-00000770: 7461 7267 6574 3a20 6874 7470 733a 2f2f  target: https://
-00000780: 636f 6465 636f 762e 696f 2f67 682f 6466  codecov.io/gh/df
-00000790: 7464 342f 7461 642d 6466 7464 340a 2020  td4/tad-dftd4.  
-000007a0: 2020 3a61 6c74 3a20 436f 7665 7261 6765    :alt: Coverage
-000007b0: 0a0a 2e2e 2069 6d61 6765 3a3a 2068 7474  .... image:: htt
-000007c0: 7073 3a2f 2f72 6573 756c 7473 2e70 7265  ps://results.pre
-000007d0: 2d63 6f6d 6d69 742e 6369 2f62 6164 6765  -commit.ci/badge
-000007e0: 2f67 6974 6875 622f 6466 7464 342f 7461  /github/dftd4/ta
-000007f0: 642d 6466 7464 342f 6d61 696e 2e73 7667  d-dftd4/main.svg
-00000800: 0a20 2020 203a 7461 7267 6574 3a20 6874  .    :target: ht
-00000810: 7470 733a 2f2f 7265 7375 6c74 732e 7072  tps://results.pr
-00000820: 652d 636f 6d6d 6974 2e63 692f 6c61 7465  e-commit.ci/late
-00000830: 7374 2f67 6974 6875 622f 6466 7464 342f  st/github/dftd4/
-00000840: 7461 642d 6466 7464 342f 6d61 696e 0a20  tad-dftd4/main. 
-00000850: 2020 203a 616c 743a 2070 7265 2d63 6f6d     :alt: pre-com
-00000860: 6d69 742e 6369 2073 7461 7475 730a 0a49  mit.ci status..I
-00000870: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
-00000880: 2074 6865 2044 4654 2d44 3420 6469 7370   the DFT-D4 disp
-00000890: 6572 7369 6f6e 206d 6f64 656c 2069 6e20  ersion model in 
-000008a0: 5079 546f 7263 682e 0a54 6869 7320 6d6f  PyTorch..This mo
-000008b0: 6475 6c65 2061 6c6c 6f77 7320 746f 2070  dule allows to p
-000008c0: 726f 6365 7373 2061 2073 696e 676c 6520  rocess a single 
-000008d0: 7374 7275 6374 7572 6520 6f72 2061 2062  structure or a b
-000008e0: 6174 6368 206f 6620 7374 7275 6374 7572  atch of structur
-000008f0: 6573 2066 6f72 2074 6865 2063 616c 6375  es for the calcu
-00000900: 6c61 7469 6f6e 206f 6620 6174 6f6d 2d72  lation of atom-r
-00000910: 6573 6f6c 7665 6420 6469 7370 6572 7369  esolved dispersi
-00000920: 6f6e 2065 6e65 7267 6965 732e 0a0a 466f  on energies...Fo
-00000930: 7220 6465 7461 696c 7320 6f6e 2074 6865  r details on the
-00000940: 2044 3420 6469 7370 6572 7369 6f6e 206d   D4 dispersion m
-00000950: 6f64 656c 2c20 7365 650a 0a2d 205c 452e  odel, see..- \E.
-00000960: 2043 616c 6465 7765 7968 6572 2c20 432e   Caldeweyher, C.
-00000970: 2042 616e 6e77 6172 7468 2061 6e64 2053   Bannwarth and S
-00000980: 2e20 4772 696d 6d65 2c20 2a4a 2e20 4368  . Grimme, *J. Ch
-00000990: 656d 2e20 5068 7973 2e2a 2c20 2a2a 3230  em. Phys.*, **20
-000009a0: 3137 2a2a 2c20 2a31 3437 2a2c 2030 3334  17**, *147*, 034
-000009b0: 3131 322e 2044 4f49 3a20 6031 302e 3130  112. DOI: `10.10
-000009c0: 3633 2f31 2e34 3939 3332 3135 203c 6874  63/1.4993215 <ht
-000009d0: 7470 733a 2f2f 6478 2e64 6f69 2e6f 7267  tps://dx.doi.org
-000009e0: 2f31 302e 3130 3633 2f31 2e34 3939 3332  /10.1063/1.49932
-000009f0: 3135 3e60 5f5f 0a0a 2d20 5c45 2e20 4361  15>`__..- \E. Ca
-00000a00: 6c64 6577 6579 6865 722c 2053 2e20 4568  ldeweyher, S. Eh
-00000a10: 6c65 7274 2c20 412e 2048 616e 7365 6e2c  lert, A. Hansen,
-00000a20: 2048 2e20 4e65 7567 6562 6175 6572 2c20   H. Neugebauer, 
-00000a30: 532e 2053 7069 6368 6572 2c20 432e 2042  S. Spicher, C. B
-00000a40: 616e 6e77 6172 7468 2061 6e64 2053 2e20  annwarth and S. 
-00000a50: 4772 696d 6d65 2c20 2a4a 2e20 4368 656d  Grimme, *J. Chem
-00000a60: 2e20 5068 7973 2e2a 2c20 2a2a 3230 3139  . Phys.*, **2019
-00000a70: 2a2a 2c20 2a31 3530 2a2c 2031 3534 3132  **, *150*, 15412
-00000a80: 322e 2044 4f49 3a20 6031 302e 3130 3633  2. DOI: `10.1063
-00000a90: 2f31 2e35 3039 3032 3232 203c 6874 7470  /1.5090222 <http
-00000aa0: 733a 2f2f 6478 2e64 6f69 2e6f 7267 2f31  s://dx.doi.org/1
-00000ab0: 302e 3130 3633 2f31 2e35 3039 3032 3232  0.1063/1.5090222
-00000ac0: 3e60 5f5f 0a0a 2d20 5c45 2e20 4361 6c64  >`__..- \E. Cald
-00000ad0: 6577 6579 6865 722c 204a 2e2d 4d2e 204d  eweyher, J.-M. M
-00000ae0: 6577 6573 2c20 532e 2045 686c 6572 7420  ewes, S. Ehlert 
-00000af0: 616e 6420 532e 2047 7269 6d6d 652c 202a  and S. Grimme, *
-00000b00: 5068 7973 2e20 4368 656d 2e20 4368 656d  Phys. Chem. Chem
-00000b10: 2e20 5068 7973 2e2a 2c20 2a2a 3230 3230  . Phys.*, **2020
-00000b20: 2a2a 2c20 2a32 322a 2c20 3834 3939 2d38  **, *22*, 8499-8
-00000b30: 3531 322e 2044 4f49 3a20 6031 302e 3130  512. DOI: `10.10
-00000b40: 3339 2f44 3043 5030 3035 3032 4120 3c68  39/D0CP00502A <h
-00000b50: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-00000b60: 302e 3130 3339 2f44 3043 5030 3035 3032  0.1039/D0CP00502
-00000b70: 413e 605f 5f0a 0a46 6f72 2061 6c74 6572  A>`__..For alter
-00000b80: 6e61 7469 7665 2069 6d70 6c65 6d65 6e74  native implement
-00000b90: 6174 696f 6e73 2c20 616c 736f 2063 6865  ations, also che
-00000ba0: 636b 206f 7574 0a0a 6064 6674 6434 203c  ck out..`dftd4 <
-00000bb0: 6874 7470 733a 2f2f 6466 7464 342e 7265  https://dftd4.re
-00000bc0: 6164 7468 6564 6f63 732e 696f 3e60 5f5f  adthedocs.io>`__
-00000bd0: 3a0a 2020 496d 706c 656d 656e 7461 7469  :.  Implementati
-00000be0: 6f6e 206f 6620 7468 6520 4446 542d 4434  on of the DFT-D4
-00000bf0: 2064 6973 7065 7273 696f 6e20 6d6f 6465   dispersion mode
-00000c00: 6c20 696e 2046 6f72 7472 616e 2077 6974  l in Fortran wit
-00000c10: 6820 5079 7468 6f6e 2062 696e 6469 6e67  h Python binding
-00000c20: 732e 0a0a 6063 7070 2d64 3420 3c68 7474  s...`cpp-d4 <htt
-00000c30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000c40: 6466 7464 342f 6370 702d 6434 3e60 5f5f  dftd4/cpp-d4>`__
-00000c50: 3a0a 2020 496d 706c 656d 656e 7461 7469  :.  Implementati
-00000c60: 6f6e 206f 6620 7468 6520 4446 542d 4434  on of the DFT-D4
-00000c70: 2064 6973 7065 7273 696f 6e20 6d6f 6465   dispersion mode
-00000c80: 6c20 696e 2043 2b2b 2e0a 0a49 6e73 7461  l in C++...Insta
-00000c90: 6c6c 6174 696f 6e0a 2d2d 2d2d 2d2d 2d2d  llation.--------
-00000ca0: 2d2d 2d2d 0a0a 7069 700a 7e7e 7e0a 0a2a  ----..pip.~~~..*
-00000cb0: 7461 642d 6466 7464 342a 2063 616e 2065  tad-dftd4* can e
-00000cc0: 6173 696c 7920 6265 2069 6e73 7461 6c6c  asily be install
-00000cd0: 6564 2077 6974 6820 6060 7069 7060 602e  ed with ``pip``.
-00000ce0: 0a0a 2e2e 2063 6f64 653a 3a0a 0a20 2020  .... code::..   
-00000cf0: 2070 6970 2069 6e73 7461 6c6c 2074 6164   pip install tad
-00000d00: 2d64 6674 6434 0a0a 0a46 726f 6d20 736f  -dftd4...From so
-00000d10: 7572 6365 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  urce.~~~~~~~~~~~
-00000d20: 0a0a 5468 6973 2070 726f 6a65 6374 2069  ..This project i
-00000d30: 7320 686f 7374 6564 206f 6e20 4769 7448  s hosted on GitH
-00000d40: 7562 2061 7420 6064 6674 6434 2f74 6164  ub at `dftd4/tad
-00000d50: 2d64 6674 6434 203c 6874 7470 733a 2f2f  -dftd4 <https://
-00000d60: 6769 7468 7562 2e63 6f6d 2f64 6674 6434  github.com/dftd4
-00000d70: 2f74 6164 2d64 6674 6434 3e60 5f5f 2e0a  /tad-dftd4>`__..
-00000d80: 4f62 7461 696e 2074 6865 2073 6f75 7263  Obtain the sourc
-00000d90: 6520 6279 2063 6c6f 6e69 6e67 2074 6865  e by cloning the
-00000da0: 2072 6570 6f73 6974 6f72 7920 7769 7468   repository with
-00000db0: 0a0a 2e2e 2063 6f64 653a 3a0a 0a20 2020  .... code::..   
-00000dc0: 2067 6974 2063 6c6f 6e65 2068 7474 7073   git clone https
-00000dd0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6466  ://github.com/df
-00000de0: 7464 342f 7461 642d 6466 7464 340a 2020  td4/tad-dftd4.  
-00000df0: 2020 6364 2074 6164 2d64 6674 6434 0a0a    cd tad-dftd4..
-00000e00: 5765 2072 6563 6f6d 6d65 6e64 2075 7369  We recommend usi
-00000e10: 6e67 2061 2060 636f 6e64 6120 3c68 7474  ng a `conda <htt
-00000e20: 7073 3a2f 2f63 6f6e 6461 2e69 6f2f 3e60  ps://conda.io/>`
-00000e30: 5f5f 2065 6e76 6972 6f6e 6d65 6e74 2074  __ environment t
-00000e40: 6f20 696e 7374 616c 6c20 7468 6520 7061  o install the pa
-00000e50: 636b 6167 652e 0a59 6f75 2063 616e 2073  ckage..You can s
-00000e60: 6574 7570 2074 6865 2065 6e76 6972 6f6e  etup the environ
-00000e70: 6d65 6e74 206d 616e 6167 6572 2075 7369  ment manager usi
-00000e80: 6e67 2061 2060 6d61 6d62 6166 6f72 6765  ng a `mambaforge
-00000e90: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-00000ea0: 2e63 6f6d 2f63 6f6e 6461 2d66 6f72 6765  .com/conda-forge
-00000eb0: 2f6d 696e 6966 6f72 6765 3e60 5f5f 2069  /miniforge>`__ i
-00000ec0: 6e73 7461 6c6c 6572 2e0a 496e 7374 616c  nstaller..Instal
-00000ed0: 6c20 7468 6520 7265 7175 6972 6564 2064  l the required d
-00000ee0: 6570 656e 6465 6e63 6965 7320 6672 6f6d  ependencies from
-00000ef0: 2074 6865 2063 6f6e 6461 2d66 6f72 6765   the conda-forge
-00000f00: 2063 6861 6e6e 656c 2e0a 0a2e 2e20 636f   channel..... co
-00000f10: 6465 3a3a 0a0a 2020 2020 6d61 6d62 6120  de::..    mamba 
-00000f20: 656e 7620 6372 6561 7465 202d 6e20 746f  env create -n to
-00000f30: 7263 6820 2d66 2065 6e76 6972 6f6e 6d65  rch -f environme
-00000f40: 6e74 2e79 616d 6c0a 2020 2020 6d61 6d62  nt.yaml.    mamb
-00000f50: 6120 6163 7469 7661 7465 2074 6f72 6368  a activate torch
-00000f60: 0a0a 496e 7374 616c 6c20 7468 6973 2070  ..Install this p
-00000f70: 726f 6a65 6374 2077 6974 6820 6060 7069  roject with ``pi
-00000f80: 7060 6020 696e 2074 6865 2065 6e76 6972  p`` in the envir
-00000f90: 6f6e 6d65 6e74 0a0a 2e2e 2063 6f64 653a  onment.... code:
-00000fa0: 3a0a 0a20 2020 2070 6970 2069 6e73 7461  :..    pip insta
-00000fb0: 6c6c 202e 0a0a 5468 6520 666f 6c6c 6f77  ll ...The follow
-00000fc0: 696e 6720 6465 7065 6e64 656e 6369 6573  ing dependencies
-00000fd0: 2061 7265 2072 6571 7569 7265 640a 0a2d   are required..-
-00000fe0: 2060 6e75 6d70 7920 3c68 7474 7073 3a2f   `numpy <https:/
-00000ff0: 2f6e 756d 7079 2e6f 7267 2f3e 605f 5f0a  /numpy.org/>`__.
-00001000: 2d20 6074 6f72 6368 203c 6874 7470 733a  - `torch <https:
-00001010: 2f2f 7079 746f 7263 682e 6f72 672f 3e60  //pytorch.org/>`
-00001020: 5f5f 0a2d 2060 7079 7465 7374 203c 6874  __.- `pytest <ht
-00001030: 7470 733a 2f2f 646f 6373 2e70 7974 6573  tps://docs.pytes
-00001040: 742e 6f72 672f 3e60 5f5f 2028 7465 7374  t.org/>`__ (test
-00001050: 7320 6f6e 6c79 290a 0a44 6576 656c 6f70  s only)..Develop
-00001060: 6d65 6e74 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ment.-----------
-00001070: 0a0a 466f 7220 6465 7665 6c6f 706d 656e  ..For developmen
-00001080: 742c 2061 6464 6974 696f 6e61 6c6c 7920  t, additionally 
-00001090: 696e 7374 616c 6c20 7468 6520 666f 6c6c  install the foll
-000010a0: 6f77 696e 6720 746f 6f6c 7320 696e 2079  owing tools in y
-000010b0: 6f75 7220 656e 7669 726f 6e6d 656e 742e  our environment.
-000010c0: 0a0a 2e2e 2063 6f64 653a 3a0a 0a20 2020  .... code::..   
-000010d0: 206d 616d 6261 2069 6e73 7461 6c6c 2062   mamba install b
-000010e0: 6c61 636b 2063 6f76 6465 6661 756c 7473  lack covdefaults
-000010f0: 2063 6f76 6572 6167 6520 6d79 7079 2070   coverage mypy p
-00001100: 7265 2d63 6f6d 6d69 7420 7079 6c69 6e74  re-commit pylint
-00001110: 2074 6f78 0a0a 5769 7468 2070 6970 2c20   tox..With pip, 
-00001120: 6164 6420 7468 6520 6f70 7469 6f6e 2060  add the option `
-00001130: 602d 6560 6020 666f 7220 696e 7374 616c  `-e`` for instal
-00001140: 6c69 6e67 2069 6e20 6465 7665 6c6f 706d  ling in developm
-00001150: 656e 7420 6d6f 6465 2c20 616e 6420 6164  ent mode, and ad
-00001160: 6420 6060 5b64 6576 5d60 6020 666f 7220  d ``[dev]`` for 
-00001170: 7468 6520 6465 7665 6c6f 706d 656e 7420  the development 
-00001180: 6465 7065 6e64 656e 6369 6573 0a0a 2e2e  dependencies....
-00001190: 2063 6f64 653a 3a0a 0a20 2020 2070 6970   code::..    pip
-000011a0: 2069 6e73 7461 6c6c 202d 6520 2e5b 6465   install -e .[de
-000011b0: 765d 0a0a 5468 6520 7072 652d 636f 6d6d  v]..The pre-comm
-000011c0: 6974 2068 6f6f 6b73 2061 7265 2069 6e69  it hooks are ini
-000011d0: 7469 616c 697a 6564 2062 7920 7275 6e6e  tialized by runn
-000011e0: 696e 6720 7468 6520 666f 6c6c 6f77 696e  ing the followin
-000011f0: 6720 636f 6d6d 616e 6420 696e 2074 6865  g command in the
-00001200: 2072 6f6f 7420 6f66 2074 6865 2072 6570   root of the rep
-00001210: 6f73 6974 6f72 792e 0a0a 2e2e 2063 6f64  ository..... cod
-00001220: 653a 3a0a 0a20 2020 2070 7265 2d63 6f6d  e::..    pre-com
-00001230: 6d69 7420 696e 7374 616c 6c0a 0a46 6f72  mit install..For
-00001240: 2074 6573 7469 6e67 2061 6c6c 2050 7974   testing all Pyt
-00001250: 686f 6e20 656e 7669 726f 6e6d 656e 7473  hon environments
-00001260: 2c20 7369 6d70 6c79 2072 756e 2060 746f  , simply run `to
-00001270: 7860 2e0a 0a2e 2e20 636f 6465 3a3a 0a0a  x`..... code::..
-00001280: 2020 2020 746f 780a 0a4e 6f74 6520 7468      tox..Note th
-00001290: 6174 2074 6869 7320 7261 6e64 6f6d 697a  at this randomiz
-000012a0: 6573 2074 6865 206f 7264 6572 206f 6620  es the order of 
-000012b0: 7465 7374 7320 6275 7420 736b 6970 7320  tests but skips 
-000012c0: 226c 6172 6765 2220 7465 7374 732e 2054  "large" tests. T
-000012d0: 6f20 6d6f 6469 6679 2074 6869 7320 6265  o modify this be
-000012e0: 6861 7669 6f72 2c20 6074 6f78 6020 6861  havior, `tox` ha
-000012f0: 7320 746f 2073 6b69 7020 7468 6520 6f70  s to skip the op
-00001300: 7469 6f6e 616c 202a 706f 7361 7267 732a  tional *posargs*
-00001310: 2e0a 0a2e 2e20 636f 6465 3a3a 0a0a 2020  ..... code::..  
-00001320: 2020 746f 7820 2d2d 2074 6573 740a 0a45    tox -- test..E
-00001330: 7861 6d70 6c65 730a 2d2d 2d2d 2d2d 2d2d  xamples.--------
-00001340: 0a0a 5468 6520 666f 6c6c 6f77 696e 6720  ..The following 
-00001350: 6578 616d 706c 6520 7368 6f77 7320 686f  example shows ho
-00001360: 7720 746f 2063 616c 6375 6c61 7465 2074  w to calculate t
-00001370: 6865 2044 4654 2d44 3420 6469 7370 6572  he DFT-D4 disper
-00001380: 7369 6f6e 2065 6e65 7267 7920 666f 7220  sion energy for 
-00001390: 6120 7369 6e67 6c65 2073 7472 7563 7475  a single structu
-000013a0: 7265 2e0a 0a2e 2e20 636f 6465 3a3a 2070  re..... code:: p
-000013b0: 7974 686f 6e0a 0a20 2020 2069 6d70 6f72  ython..    impor
-000013c0: 7420 746f 7263 680a 2020 2020 696d 706f  t torch.    impo
-000013d0: 7274 2074 6164 5f64 6674 6434 2061 7320  rt tad_dftd4 as 
-000013e0: 6434 0a0a 2020 2020 6e75 6d62 6572 7320  d4..    numbers 
-000013f0: 3d20 6434 2e75 7469 6c73 2e74 6f5f 6e75  = d4.utils.to_nu
-00001400: 6d62 6572 2873 796d 626f 6c73 3d22 4320  mber(symbols="C 
-00001410: 4320 4320 4320 4e20 4320 5320 4820 4820  C C C N C S H H 
-00001420: 4820 4820 4822 2e73 706c 6974 2829 290a  H H H".split()).
-00001430: 0a20 2020 2023 2063 6f6f 7264 696e 6174  .    # coordinat
-00001440: 6573 2069 6e20 426f 6872 0a20 2020 2070  es in Bohr.    p
-00001450: 6f73 6974 696f 6e73 203d 2074 6f72 6368  ositions = torch
-00001460: 2e74 656e 736f 7228 0a20 2020 2020 2020  .tensor(.       
-00001470: 205b 0a20 2020 2020 2020 2020 2020 205b   [.            [
-00001480: 2d32 2e35 3637 3435 3638 3535 3634 3637  -2.5674568556467
-00001490: 312c 202d 302e 3032 3530 3939 3835 3937  1, -0.0250998597
-000014a0: 3939 3130 2c20 302e 3030 3030 3030 3030  9910, 0.00000000
-000014b0: 3030 3030 3030 5d2c 0a20 2020 2020 2020  000000],.       
-000014c0: 2020 2020 205b 2d31 2e33 3931 3737 3538       [-1.3917758
-000014d0: 3234 3535 3739 372c 202b 322e 3237 3639  2455797, +2.2769
-000014e0: 3631 3838 3838 3030 3134 2c20 302e 3030  6188880014, 0.00
-000014f0: 3030 3030 3030 3030 3030 3030 5d2c 0a20  000000000000],. 
-00001500: 2020 2020 2020 2020 2020 205b 2b31 2e32             [+1.2
-00001510: 3737 3834 3939 3536 3234 3839 342c 202b  7784995624894, +
-00001520: 322e 3435 3130 3734 3739 3735 3933 3836  2.45107479759386
-00001530: 2c20 302e 3030 3030 3030 3030 3030 3030  , 0.000000000000
-00001540: 3030 5d2c 0a20 2020 2020 2020 2020 2020  00],.           
-00001550: 205b 2b32 2e36 3238 3031 3933 3736 3135   [+2.62801937615
-00001560: 3739 332c 202b 302e 3235 3932 3737 3237  793, +0.25927727
-00001570: 3032 3831 3230 2c20 302e 3030 3030 3030  028120, 0.000000
-00001580: 3030 3030 3030 3030 5d2c 0a20 2020 2020  00000000],.     
-00001590: 2020 2020 2020 205b 2b31 2e34 3130 3937         [+1.41097
-000015a0: 3033 3336 3631 3132 332c 202d 312e 3939  033661123, -1.99
-000015b0: 3839 3039 3936 3037 3734 3132 2c20 302e  890996077412, 0.
-000015c0: 3030 3030 3030 3030 3030 3030 3030 5d2c  00000000000000],
-000015d0: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
-000015e0: 2e31 3731 3836 3130 3232 3938 3834 392c  .17186102298849,
-000015f0: 202d 322e 3334 3232 3035 3736 3238 3431   -2.342205762841
-00001600: 3830 2c20 302e 3030 3030 3030 3030 3030  80, 0.0000000000
-00001610: 3030 3030 5d2c 0a20 2020 2020 2020 2020  0000],.         
-00001620: 2020 205b 2d32 2e33 3935 3035 3939 3033     [-2.395059903
-00001630: 3638 3337 382c 202d 352e 3232 3633 3538  68378, -5.226358
-00001640: 3338 3333 3233 3632 2c20 302e 3030 3030  38332362, 0.0000
-00001650: 3030 3030 3030 3030 3030 5d2c 0a20 2020  0000000000],.   
-00001660: 2020 2020 2020 2020 205b 2b32 2e34 3139           [+2.419
-00001670: 3631 3938 3034 3535 3435 372c 202d 332e  61980455457, -3.
-00001680: 3632 3135 3830 3139 3235 3330 3435 2c20  62158019253045, 
-00001690: 302e 3030 3030 3030 3030 3030 3030 3030  0.00000000000000
-000016a0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-000016b0: 2d32 2e35 3137 3434 3337 3438 3436 3036  -2.5174437484606
-000016c0: 352c 202b 332e 3938 3138 3137 3133 3638  5, +3.9818171368
-000016d0: 3637 3436 2c20 302e 3030 3030 3030 3030  6746, 0.00000000
-000016e0: 3030 3030 3030 5d2c 0a20 2020 2020 2020  000000],.       
-000016f0: 2020 2020 205b 2b32 2e32 3432 3639 3034       [+2.2426904
-00001700: 3833 3834 3737 352c 202b 342e 3234 3338  8384775, +4.2438
-00001710: 3934 3733 3230 3336 3437 2c20 302e 3030  9473203647, 0.00
-00001720: 3030 3030 3030 3030 3030 3030 5d2c 0a20  000000000000],. 
-00001730: 2020 2020 2020 2020 2020 205b 2b34 2e36             [+4.6
-00001740: 3634 3838 3938 3435 3733 3935 362c 202b  6488984573956, +
-00001750: 302e 3137 3930 3735 3638 3030 3634 3039  0.17907568006409
-00001760: 2c20 302e 3030 3030 3030 3030 3030 3030  , 0.000000000000
-00001770: 3030 5d2c 0a20 2020 2020 2020 2020 2020  00],.           
-00001780: 205b 2d34 2e36 3030 3434 3234 3437 3832   [-4.60044244782
-00001790: 3233 372c 202d 302e 3137 3739 3437 3334  237, -0.17794734
-000017a0: 3633 3734 3133 2c20 302e 3030 3030 3030  637413, 0.000000
-000017b0: 3030 3030 3030 3030 5d2c 0a20 2020 2020  00000000],.     
-000017c0: 2020 205d 0a20 2020 2029 0a0a 2020 2020     ].    )..    
-000017d0: 2320 746f 7461 6c20 6368 6172 6765 206f  # total charge o
-000017e0: 6620 7468 6520 7379 7374 656d 0a20 2020  f the system.   
-000017f0: 2063 6861 7267 6520 3d20 746f 7263 682e   charge = torch.
-00001800: 7465 6e73 6f72 2830 2e30 290a 0a20 2020  tensor(0.0)..   
-00001810: 2023 2054 5053 5330 2d44 342d 4154 4d20   # TPSS0-D4-ATM 
-00001820: 7061 7261 6d65 7465 7273 0a20 2020 2070  parameters.    p
-00001830: 6172 616d 203d 207b 0a20 2020 2020 2020  aram = {.       
-00001840: 2022 7336 223a 2070 6f73 6974 696f 6e73   "s6": positions
-00001850: 2e6e 6577 5f74 656e 736f 7228 312e 3029  .new_tensor(1.0)
-00001860: 2c0a 2020 2020 2020 2020 2273 3822 3a20  ,.        "s8": 
-00001870: 706f 7369 7469 6f6e 732e 6e65 775f 7465  positions.new_te
-00001880: 6e73 6f72 2831 2e38 3538 3937 3735 3029  nsor(1.85897750)
-00001890: 2c0a 2020 2020 2020 2020 2273 3922 3a20  ,.        "s9": 
-000018a0: 706f 7369 7469 6f6e 732e 6e65 775f 7465  positions.new_te
-000018b0: 6e73 6f72 2831 2e30 292c 0a20 2020 2020  nsor(1.0),.     
-000018c0: 2020 2022 6131 223a 2070 6f73 6974 696f     "a1": positio
-000018d0: 6e73 2e6e 6577 5f74 656e 736f 7228 302e  ns.new_tensor(0.
-000018e0: 3434 3238 3639 3636 292c 0a20 2020 2020  44286966),.     
-000018f0: 2020 2022 6132 223a 2070 6f73 6974 696f     "a2": positio
-00001900: 6e73 2e6e 6577 5f74 656e 736f 7228 342e  ns.new_tensor(4.
-00001910: 3630 3233 3035 3334 292c 0a20 2020 207d  60230534),.    }
-00001920: 0a0a 2020 2020 656e 6572 6779 203d 2064  ..    energy = d
-00001930: 342e 6466 7464 3428 6e75 6d62 6572 732c  4.dftd4(numbers,
-00001940: 2070 6f73 6974 696f 6e73 2c20 6368 6172   positions, char
-00001950: 6765 2c20 7061 7261 6d29 0a20 2020 2074  ge, param).    t
-00001960: 6f72 6368 2e73 6574 5f70 7269 6e74 6f70  orch.set_printop
-00001970: 7469 6f6e 7328 7072 6563 6973 696f 6e3d  tions(precision=
-00001980: 3130 290a 2020 2020 7072 696e 7428 656e  10).    print(en
-00001990: 6572 6779 290a 2020 2020 2320 7465 6e73  ergy).    # tens
-000019a0: 6f72 285b 2d30 2e30 3032 3038 3431 3334  or([-0.002084134
-000019b0: 342c 202d 302e 3030 3138 3937 3131 3935  4, -0.0018971195
-000019c0: 2c20 2d30 2e30 3031 3831 3037 3531 332c  , -0.0018107513,
-000019d0: 202d 302e 3030 3138 3330 3536 3935 2c0a   -0.0018305695,.
-000019e0: 2020 2020 2320 2020 2020 2020 2020 2d30      #         -0
-000019f0: 2e30 3032 3137 3337 3639 332c 202d 302e  .0021737693, -0.
-00001a00: 3030 3139 3438 3432 3336 2c20 2d30 2e30  0019484236, -0.0
-00001a10: 3032 3237 3838 3235 332c 202d 302e 3030  022788253, -0.00
-00001a20: 3034 3038 3036 3538 2c0a 2020 2020 2320  04080658,.    # 
-00001a30: 2020 2020 2020 2020 2d30 2e30 3030 3432          -0.00042
-00001a40: 3631 3836 362c 202d 302e 3030 3034 3139  61866, -0.000419
-00001a50: 3938 3339 2c20 2d30 2e30 3030 3432 3830  9839, -0.0004280
-00001a60: 3736 382c 202d 302e 3030 3035 3130 3839  768, -0.00051089
-00001a70: 3335 5d29 0a0a 5468 6520 6e65 7874 2065  35])..The next e
-00001a80: 7861 6d70 6c65 2073 686f 7773 2074 6865  xample shows the
-00001a90: 2063 616c 6375 6c61 7469 6f6e 206f 6620   calculation of 
-00001aa0: 6469 7370 6572 7369 6f6e 2065 6e65 7267  dispersion energ
-00001ab0: 6965 7320 666f 7220 6120 6261 7463 6820  ies for a batch 
-00001ac0: 6f66 2073 7472 7563 7475 7265 732e 0a0a  of structures...
-00001ad0: 2e2e 2063 6f64 653a 3a20 7079 7468 6f6e  .. code:: python
-00001ae0: 0a0a 2020 2020 696d 706f 7274 2074 6f72  ..    import tor
-00001af0: 6368 0a20 2020 2069 6d70 6f72 7420 7461  ch.    import ta
-00001b00: 645f 6466 7464 3420 6173 2064 340a 0a20  d_dftd4 as d4.. 
-00001b10: 2020 2023 2053 3232 2073 7973 7465 6d20     # S22 system 
-00001b20: 343a 2066 6f72 6d61 6d69 6465 2064 696d  4: formamide dim
-00001b30: 6572 0a20 2020 206e 756d 6265 7273 203d  er.    numbers =
-00001b40: 2064 342e 7574 696c 732e 7061 636b 2828   d4.utils.pack((
-00001b50: 0a20 2020 2020 2020 2064 342e 7574 696c  .        d4.util
-00001b60: 732e 746f 5f6e 756d 6265 7228 2243 2043  s.to_number("C C
-00001b70: 204e 204e 2048 2048 2048 2048 2048 2048   N N H H H H H H
-00001b80: 204f 204f 222e 7370 6c69 7428 2929 2c0a   O O".split()),.
-00001b90: 2020 2020 2020 2020 6434 2e75 7469 6c73          d4.utils
-00001ba0: 2e74 6f5f 6e75 6d62 6572 2822 4320 4f20  .to_number("C O 
-00001bb0: 4e20 4820 4820 4822 2e73 706c 6974 2829  N H H H".split()
-00001bc0: 292c 0a20 2020 2029 290a 0a20 2020 2023  ),.    ))..    #
-00001bd0: 2063 6f6f 7264 696e 6174 6573 2069 6e20   coordinates in 
-00001be0: 426f 6872 0a20 2020 2070 6f73 6974 696f  Bohr.    positio
-00001bf0: 6e73 203d 2064 342e 7574 696c 732e 7061  ns = d4.utils.pa
-00001c00: 636b 2828 0a20 2020 2020 2020 2074 6f72  ck((.        tor
-00001c10: 6368 2e74 656e 736f 7228 5b0a 2020 2020  ch.tensor([.    
-00001c20: 2020 2020 2020 2020 5b2d 332e 3831 3436          [-3.8146
-00001c30: 3934 3838 3134 3339 3231 2c20 2b30 2e30  9488143921, +0.0
-00001c40: 3939 3933 3434 3134 3032 3931 322c 2030  9993441402912, 0
-00001c50: 2e30 3030 3030 3030 3030 3030 3030 305d  .00000000000000]
-00001c60: 2c0a 2020 2020 2020 2020 2020 2020 5b2b  ,.            [+
-00001c70: 332e 3831 3436 3934 3838 3134 3339 3231  3.81469488143921
-00001c80: 2c20 2d30 2e30 3939 3933 3434 3134 3032  , -0.09993441402
-00001c90: 3931 322c 2030 2e30 3030 3030 3030 3030  912, 0.000000000
-00001ca0: 3030 3030 305d 2c0a 2020 2020 2020 2020  00000],.        
-00001cb0: 2020 2020 5b2d 322e 3636 3033 3030 3439      [-2.66030049
-00001cc0: 3332 3430 3336 2c20 2d32 2e31 3538 3938  324036, -2.15898
-00001cd0: 3235 3135 3333 3530 382c 2030 2e30 3030  251533508, 0.000
-00001ce0: 3030 3030 3030 3030 3030 305d 2c0a 2020  00000000000],.  
-00001cf0: 2020 2020 2020 2020 2020 5b2b 322e 3636            [+2.66
-00001d00: 3033 3030 3439 3332 3430 3336 2c20 2b32  030049324036, +2
-00001d10: 2e31 3538 3938 3235 3135 3333 3530 382c  .15898251533508,
-00001d20: 2030 2e30 3030 3030 3030 3030 3030 3030   0.0000000000000
-00001d30: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
-00001d40: 5b2d 302e 3733 3137 3835 3239 3733 3933  [-0.731785297393
-00001d50: 3830 2c20 2d32 2e32 3832 3337 3739 3538  80, -2.282377958
-00001d60: 3239 3737 332c 2030 2e30 3030 3030 3030  29773, 0.0000000
-00001d70: 3030 3030 3030 305d 2c0a 2020 2020 2020  0000000],.      
-00001d80: 2020 2020 2020 5b2d 352e 3839 3033 3933        [-5.890393
-00001d90: 3235 3731 3431 3131 2c20 2d30 2e30 3235  25714111, -0.025
-00001da0: 3839 3131 3435 3639 3132 382c 2030 2e30  89114569128, 0.0
-00001db0: 3030 3030 3030 3030 3030 3030 305d 2c0a  0000000000000],.
-00001dc0: 2020 2020 2020 2020 2020 2020 5b2d 332e              [-3.
-00001dd0: 3731 3235 3439 3434 3830 3133 3331 2c20  71254944801331, 
-00001de0: 2d33 2e37 3336 3035 3737 3538 3333 3133  -3.7360577583313
-00001df0: 302c 2030 2e30 3030 3030 3030 3030 3030  0, 0.00000000000
-00001e00: 3030 305d 2c0a 2020 2020 2020 2020 2020  000],.          
-00001e10: 2020 5b2b 332e 3731 3235 3439 3434 3830    [+3.7125494480
-00001e20: 3133 3331 2c20 2b33 2e37 3336 3035 3737  1331, +3.7360577
-00001e30: 3538 3333 3133 302c 2030 2e30 3030 3030  5833130, 0.00000
-00001e40: 3030 3030 3030 3030 305d 2c0a 2020 2020  000000000],.    
-00001e50: 2020 2020 2020 2020 5b2b 302e 3733 3137          [+0.7317
-00001e60: 3835 3239 3733 3933 3830 2c20 2b32 2e32  8529739380, +2.2
-00001e70: 3832 3337 3739 3538 3239 3737 332c 2030  8237795829773, 0
-00001e80: 2e30 3030 3030 3030 3030 3030 3030 305d  .00000000000000]
-00001e90: 2c0a 2020 2020 2020 2020 2020 2020 5b2b  ,.            [+
-00001ea0: 352e 3839 3033 3933 3235 3731 3431 3131  5.89039325714111
-00001eb0: 2c20 2b30 2e30 3235 3839 3131 3435 3639  , +0.02589114569
-00001ec0: 3132 382c 2030 2e30 3030 3030 3030 3030  128, 0.000000000
-00001ed0: 3030 3030 305d 2c0a 2020 2020 2020 2020  00000],.        
-00001ee0: 2020 2020 5b2d 322e 3734 3432 3631 3032      [-2.74426102
-00001ef0: 3633 3832 3435 2c20 2b32 2e31 3631 3135  638245, +2.16115
-00001f00: 3537 3030 3638 3335 392c 2030 2e30 3030  570068359, 0.000
-00001f10: 3030 3030 3030 3030 3030 305d 2c0a 2020  00000000000],.  
-00001f20: 2020 2020 2020 2020 2020 5b2b 322e 3734            [+2.74
-00001f30: 3432 3631 3032 3633 3832 3435 2c20 2d32  426102638245, -2
-00001f40: 2e31 3631 3135 3537 3030 3638 3335 392c  .16115570068359,
-00001f50: 2030 2e30 3030 3030 3030 3030 3030 3030   0.0000000000000
-00001f60: 305d 2c0a 2020 2020 2020 2020 5d29 2c0a  0],.        ]),.
-00001f70: 2020 2020 2020 2020 746f 7263 682e 7465          torch.te
-00001f80: 6e73 6f72 285b 0a20 2020 2020 2020 2020  nsor([.         
-00001f90: 2020 205b 2d30 2e35 3535 3639 3734 3332     [-0.555697432
-00001fa0: 3033 3430 362c 202b 312e 3039 3033 3034  03406, +1.090304
-00001fb0: 3235 3436 3835 3537 2c20 302e 3030 3030  25468557, 0.0000
-00001fc0: 3030 3030 3030 3030 3030 5d2c 0a20 2020  0000000000],.   
-00001fd0: 2020 2020 2020 2020 205b 2b30 2e35 3134           [+0.514
-00001fe0: 3733 3633 3436 3738 3436 392c 202b 332e  73634678469, +3.
-00001ff0: 3135 3135 3235 3530 3236 3336 3131 2c20  15152550263611, 
-00002000: 302e 3030 3030 3030 3030 3030 3030 3030  0.00000000000000
-00002010: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-00002020: 2b30 2e35 3938 3639 3639 3032 3434 3434  +0.5986969024444
-00002030: 362c 202d 312e 3136 3836 3132 3633 3738  6, -1.1686126378
-00002040: 3934 3737 2c20 302e 3030 3030 3030 3030  9477, 0.00000000
-00002050: 3030 3030 3030 5d2c 0a20 2020 2020 2020  000000],.       
-00002060: 2020 2020 205b 2d30 2e34 3533 3535 3230       [-0.4535520
-00002070: 3336 3639 3133 342c 202d 322e 3734 3536  3669134, -2.7456
-00002080: 3837 3830 3433 3830 3634 2c20 302e 3030  8780438064, 0.00
-00002090: 3030 3030 3030 3030 3030 3030 5d2c 0a20  000000000000],. 
-000020a0: 2020 2020 2020 2020 2020 205b 2b32 2e35             [+2.5
-000020b0: 3237 3231 3230 3935 3434 3939 392c 202d  2721209544999, -
-000020c0: 312e 3239 3230 3038 3030 3935 3638 3637  1.29200800956867
-000020d0: 2c20 302e 3030 3030 3030 3030 3030 3030  , 0.000000000000
-000020e0: 3030 5d2c 0a20 2020 2020 2020 2020 2020  00],.           
-000020f0: 205b 2d32 2e36 3331 3339 3538 3735 3935   [-2.63139587595
-00002100: 3337 362c 202b 302e 3936 3434 3738 3639  376, +0.96447869
-00002110: 3435 3232 3430 2c20 302e 3030 3030 3030  452240, 0.000000
-00002120: 3030 3030 3030 3030 5d2c 0a20 2020 2020  00000000],.     
-00002130: 2020 205d 292c 0a20 2020 2029 290a 0a20     ]),.    )).. 
-00002140: 2020 2023 2074 6f74 616c 2063 6861 7267     # total charg
-00002150: 6520 6f66 2062 6f74 6820 7379 7374 656d  e of both system
-00002160: 0a20 2020 2063 6861 7267 6520 3d20 746f  .    charge = to
-00002170: 7263 682e 7465 6e73 6f72 285b 302e 302c  rch.tensor([0.0,
-00002180: 2030 2e30 5d29 0a0a 2020 2020 2320 5450   0.0])..    # TP
-00002190: 5353 302d 4434 2d41 544d 2070 6172 616d  SS0-D4-ATM param
-000021a0: 6574 6572 730a 2020 2020 7061 7261 6d20  eters.    param 
-000021b0: 3d20 7b0a 2020 2020 2020 2020 2273 3622  = {.        "s6"
-000021c0: 3a20 706f 7369 7469 6f6e 732e 6e65 775f  : positions.new_
-000021d0: 7465 6e73 6f72 2831 2e30 292c 0a20 2020  tensor(1.0),.   
-000021e0: 2020 2020 2022 7338 223a 2070 6f73 6974       "s8": posit
-000021f0: 696f 6e73 2e6e 6577 5f74 656e 736f 7228  ions.new_tensor(
-00002200: 312e 3835 3839 3737 3530 292c 0a20 2020  1.85897750),.   
-00002210: 2020 2020 2022 7339 223a 2070 6f73 6974       "s9": posit
-00002220: 696f 6e73 2e6e 6577 5f74 656e 736f 7228  ions.new_tensor(
-00002230: 312e 3029 2c0a 2020 2020 2020 2020 2261  1.0),.        "a
-00002240: 3122 3a20 706f 7369 7469 6f6e 732e 6e65  1": positions.ne
-00002250: 775f 7465 6e73 6f72 2830 2e34 3432 3836  w_tensor(0.44286
-00002260: 3936 3629 2c0a 2020 2020 2020 2020 2261  966),.        "a
-00002270: 3222 3a20 706f 7369 7469 6f6e 732e 6e65  2": positions.ne
-00002280: 775f 7465 6e73 6f72 2834 2e36 3032 3330  w_tensor(4.60230
-00002290: 3533 3429 2c0a 2020 2020 7d0a 0a20 2020  534),.    }..   
-000022a0: 2023 2063 616c 6375 6c61 7465 2064 6973   # calculate dis
-000022b0: 7065 7273 696f 6e20 656e 6572 6779 2069  persion energy i
-000022c0: 6e20 4861 7274 7265 650a 2020 2020 656e  n Hartree.    en
-000022d0: 6572 6779 203d 2074 6f72 6368 2e73 756d  ergy = torch.sum
-000022e0: 2864 342e 6466 7464 3428 6e75 6d62 6572  (d4.dftd4(number
-000022f0: 732c 2070 6f73 6974 696f 6e73 2c20 6368  s, positions, ch
-00002300: 6172 6765 2c20 7061 7261 6d29 2c20 2d31  arge, param), -1
-00002310: 290a 2020 2020 746f 7263 682e 7365 745f  ).    torch.set_
-00002320: 7072 696e 746f 7074 696f 6e73 2870 7265  printoptions(pre
-00002330: 6369 7369 6f6e 3d31 3029 0a20 2020 2070  cision=10).    p
-00002340: 7269 6e74 2865 6e65 7267 7929 0a20 2020  rint(energy).   
-00002350: 2023 2074 656e 736f 7228 5b2d 302e 3030   # tensor([-0.00
-00002360: 3838 3334 3134 3332 2c20 2d30 2e30 3032  88341432, -0.002
-00002370: 3730 3133 3630 375d 290a 2020 2020 7072  7013607]).    pr
-00002380: 696e 7428 656e 6572 6779 5b30 5d20 2d20  int(energy[0] - 
-00002390: 322a 656e 6572 6779 5b31 5d29 0a20 2020  2*energy[1]).   
-000023a0: 2023 2074 656e 736f 7228 2d30 2e30 3033   # tensor(-0.003
-000023b0: 3433 3134 3231 3729 0a0a 436f 6e74 7269  4314217)..Contri
-000023c0: 6275 7469 6e67 0a2d 2d2d 2d2d 2d2d 2d2d  buting.---------
-000023d0: 2d2d 2d0a 0a54 6869 7320 6973 2061 2076  ---..This is a v
-000023e0: 6f6c 756e 7465 6572 206f 7065 6e20 736f  olunteer open so
-000023f0: 7572 6365 2070 726f 6a65 6374 7320 616e  urce projects an
-00002400: 6420 636f 6e74 7269 6275 7469 6f6e 7320  d contributions 
-00002410: 6172 6520 616c 7761 7973 2077 656c 636f  are always welco
-00002420: 6d65 2e0a 506c 6561 7365 2c20 7461 6b65  me..Please, take
-00002430: 2061 206d 6f6d 656e 7420 746f 2072 6561   a moment to rea
-00002440: 6420 7468 6520 6063 6f6e 7472 6962 7574  d the `contribut
-00002450: 696e 6720 6775 6964 656c 696e 6573 203c  ing guidelines <
-00002460: 434f 4e54 5249 4255 5449 4e47 2e6d 643e  CONTRIBUTING.md>
-00002470: 605f 5f2e 0a0a 4c69 6365 6e73 650a 2d2d  `__...License.--
-00002480: 2d2d 2d2d 2d0a 0a54 6869 7320 7072 6f6a  -----..This proj
-00002490: 6563 7420 6973 2066 7265 6520 736f 6674  ect is free soft
-000024a0: 7761 7265 3a20 796f 7520 6361 6e20 7265  ware: you can re
-000024b0: 6469 7374 7269 6275 7465 2069 7420 616e  distribute it an
-000024c0: 642f 6f72 206d 6f64 6966 7920 6974 2075  d/or modify it u
-000024d0: 6e64 6572 2074 6865 2074 6572 6d73 206f  nder the terms o
-000024e0: 6620 7468 6520 4c65 7373 6572 2047 4e55  f the Lesser GNU
-000024f0: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
-00002500: 4c69 6365 6e73 6520 6173 2070 7562 6c69  License as publi
-00002510: 7368 6564 2062 7920 7468 6520 4672 6565  shed by the Free
-00002520: 2053 6f66 7477 6172 6520 466f 756e 6461   Software Founda
-00002530: 7469 6f6e 2c20 6569 7468 6572 2076 6572  tion, either ver
-00002540: 7369 6f6e 2033 206f 6620 7468 6520 4c69  sion 3 of the Li
-00002550: 6365 6e73 652c 206f 7220 2861 7420 796f  cense, or (at yo
-00002560: 7572 206f 7074 696f 6e29 2061 6e79 206c  ur option) any l
-00002570: 6174 6572 2076 6572 7369 6f6e 2e0a 0a54  ater version...T
-00002580: 6869 7320 7072 6f6a 6563 7420 6973 2064  his project is d
-00002590: 6973 7472 6962 7574 6564 2069 6e20 7468  istributed in th
-000025a0: 6520 686f 7065 2074 6861 7420 6974 2077  e hope that it w
-000025b0: 696c 6c20 6265 2075 7365 6675 6c2c 2062  ill be useful, b
-000025c0: 7574 2077 6974 686f 7574 2061 6e79 2077  ut without any w
-000025d0: 6172 7261 6e74 793b 2077 6974 686f 7574  arranty; without
-000025e0: 2065 7665 6e20 7468 6520 696d 706c 6965   even the implie
-000025f0: 6420 7761 7272 616e 7479 206f 6620 6d65  d warranty of me
-00002600: 7263 6861 6e74 6162 696c 6974 7920 6f72  rchantability or
-00002610: 2066 6974 6e65 7373 2066 6f72 2061 2070   fitness for a p
-00002620: 6172 7469 6375 6c61 7220 7075 7270 6f73  articular purpos
-00002630: 652e 2053 6565 2074 6865 204c 6573 7365  e. See the Lesse
-00002640: 7220 474e 5520 4765 6e65 7261 6c20 5075  r GNU General Pu
-00002650: 626c 6963 204c 6963 656e 7365 2066 6f72  blic License for
-00002660: 206d 6f72 6520 6465 7461 696c 732e 0a0a   more details...
-00002670: 556e 6c65 7373 2079 6f75 2065 7870 6c69  Unless you expli
-00002680: 6369 746c 7920 7374 6174 6520 6f74 6865  citly state othe
-00002690: 7277 6973 652c 2061 6e79 2063 6f6e 7472  rwise, any contr
-000026a0: 6962 7574 696f 6e20 696e 7465 6e74 696f  ibution intentio
-000026b0: 6e61 6c6c 7920 7375 626d 6974 7465 6420  nally submitted 
-000026c0: 666f 7220 696e 636c 7573 696f 6e20 696e  for inclusion in
-000026d0: 2074 6869 7320 7072 6f6a 6563 7420 6279   this project by
-000026e0: 2079 6f75 2c20 6173 2064 6566 696e 6564   you, as defined
-000026f0: 2069 6e20 7468 6520 4c65 7373 6572 2047   in the Lesser G
-00002700: 4e55 2047 656e 6572 616c 2050 7562 6c69  NU General Publi
-00002710: 6320 6c69 6365 6e73 652c 2073 6861 6c6c  c license, shall
-00002720: 2062 6520 6c69 6365 6e73 6564 2061 7320   be licensed as 
-00002730: 6162 6f76 652c 2077 6974 686f 7574 2061  above, without a
-00002740: 6e79 2061 6464 6974 696f 6e61 6c20 7465  ny additional te
-00002750: 726d 7320 6f72 2063 6f6e 6469 7469 6f6e  rms or condition
-00002760: 732e 0a                                  s..
+00000080: 7365 3a20 4170 6163 6865 2d32 2e30 0a43  se: Apache-2.0.C
+00000090: 6c61 7373 6966 6965 723a 2046 7261 6d65  lassifier: Frame
+000000a0: 776f 726b 203a 3a20 5079 7465 7374 0a43  work :: Pytest.C
+000000b0: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
+000000c0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+000000d0: 6564 203a 3a20 4170 6163 6865 2053 6f66  ed :: Apache Sof
+000000e0: 7477 6172 6520 4c69 6365 6e73 650a 436c  tware License.Cl
+000000f0: 6173 7369 6669 6572 3a20 4e61 7475 7261  assifier: Natura
+00000100: 6c20 4c61 6e67 7561 6765 203a 3a20 456e  l Language :: En
+00000110: 676c 6973 680a 436c 6173 7369 6669 6572  glish.Classifier
+00000120: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000130: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000140: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
+00000150: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000160: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000170: 203a 3a20 3320 3a3a 204f 6e6c 790a 436c   :: 3 :: Only.Cl
+00000180: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000190: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000001a0: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
+000001b0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000001c0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001d0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000001e0: 390a 436c 6173 7369 6669 6572 3a20 5072  9.Classifier: Pr
+000001f0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000200: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000210: 332e 3130 0a43 6c61 7373 6966 6965 723a  3.10.Classifier:
+00000220: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000230: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000240: 3a3a 2033 2e31 310a 436c 6173 7369 6669  :: 3.11.Classifi
+00000250: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000260: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000270: 6f6e 203a 3a20 496d 706c 656d 656e 7461  on :: Implementa
+00000280: 7469 6f6e 203a 3a20 4350 7974 686f 6e0a  tion :: CPython.
+00000290: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+000002a0: 6320 3a3a 2053 6369 656e 7469 6669 632f  c :: Scientific/
+000002b0: 456e 6769 6e65 6572 696e 670a 436c 6173  Engineering.Clas
+000002c0: 7369 6669 6572 3a20 5479 7069 6e67 203a  sifier: Typing :
+000002d0: 3a20 5479 7065 640a 5265 7175 6972 6573  : Typed.Requires
+000002e0: 2d50 7974 686f 6e3a 203e 3d33 2e38 0a44  -Python: >=3.8.D
+000002f0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+00000300: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+00000310: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
+00000320: 696c 653a 204c 4943 454e 5345 0a52 6571  ile: LICENSE.Req
+00000330: 7569 7265 732d 4469 7374 3a20 6e75 6d70  uires-Dist: nump
+00000340: 790a 5265 7175 6972 6573 2d44 6973 743a  y.Requires-Dist:
+00000350: 2074 6164 2d6d 6374 630a 5265 7175 6972   tad-mctc.Requir
+00000360: 6573 2d44 6973 743a 2074 6164 2d6d 756c  es-Dist: tad-mul
+00000370: 7469 6368 6172 6765 0a52 6571 7569 7265  ticharge.Require
+00000380: 732d 4469 7374 3a20 746f 7263 683e 3d31  s-Dist: torch>=1
+00000390: 2e31 310a 5072 6f76 6964 6573 2d45 7874  .11.Provides-Ext
+000003a0: 7261 3a20 6465 760a 5265 7175 6972 6573  ra: dev.Requires
+000003b0: 2d44 6973 743a 2062 6c61 636b 3b20 6578  -Dist: black; ex
+000003c0: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+000003d0: 7569 7265 732d 4469 7374 3a20 636f 7664  uires-Dist: covd
+000003e0: 6566 6175 6c74 733b 2065 7874 7261 203d  efaults; extra =
+000003f0: 3d20 2264 6576 220a 5265 7175 6972 6573  = "dev".Requires
+00000400: 2d44 6973 743a 206d 7970 793b 2065 7874  -Dist: mypy; ext
+00000410: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+00000420: 6972 6573 2d44 6973 743a 2070 7265 2d63  ires-Dist: pre-c
+00000430: 6f6d 6d69 743b 2065 7874 7261 203d 3d20  ommit; extra == 
+00000440: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
+00000450: 6973 743a 2070 796c 696e 743b 2065 7874  ist: pylint; ext
+00000460: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+00000470: 6972 6573 2d44 6973 743a 2070 7974 6573  ires-Dist: pytes
+00000480: 743b 2065 7874 7261 203d 3d20 2264 6576  t; extra == "dev
+00000490: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+000004a0: 2070 7974 6573 742d 636f 763b 2065 7874   pytest-cov; ext
+000004b0: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+000004c0: 6972 6573 2d44 6973 743a 2070 7974 6573  ires-Dist: pytes
+000004d0: 742d 7261 6e64 6f6d 2d6f 7264 6572 3b20  t-random-order; 
+000004e0: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
+000004f0: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
+00000500: 7465 7374 2d78 6469 7374 3b20 6578 7472  test-xdist; extr
+00000510: 6120 3d3d 2022 6465 7622 0a52 6571 7569  a == "dev".Requi
+00000520: 7265 732d 4469 7374 3a20 746f 783b 2065  res-Dist: tox; e
+00000530: 7874 7261 203d 3d20 2264 6576 220a 5072  xtra == "dev".Pr
+00000540: 6f76 6964 6573 2d45 7874 7261 3a20 746f  ovides-Extra: to
+00000550: 780a 5265 7175 6972 6573 2d44 6973 743a  x.Requires-Dist:
+00000560: 2063 6f76 6465 6661 756c 7473 3b20 6578   covdefaults; ex
+00000570: 7472 6120 3d3d 2022 746f 7822 0a52 6571  tra == "tox".Req
+00000580: 7569 7265 732d 4469 7374 3a20 7079 7465  uires-Dist: pyte
+00000590: 7374 3b20 6578 7472 6120 3d3d 2022 746f  st; extra == "to
+000005a0: 7822 0a52 6571 7569 7265 732d 4469 7374  x".Requires-Dist
+000005b0: 3a20 7079 7465 7374 2d63 6f76 3b20 6578  : pytest-cov; ex
+000005c0: 7472 6120 3d3d 2022 746f 7822 0a52 6571  tra == "tox".Req
+000005d0: 7569 7265 732d 4469 7374 3a20 7079 7465  uires-Dist: pyte
+000005e0: 7374 2d72 616e 646f 6d2d 6f72 6465 723b  st-random-order;
+000005f0: 2065 7874 7261 203d 3d20 2274 6f78 220a   extra == "tox".
+00000600: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
+00000610: 7974 6573 742d 7864 6973 743b 2065 7874  ytest-xdist; ext
+00000620: 7261 203d 3d20 2274 6f78 220a 0a23 2054  ra == "tox"..# T
+00000630: 6f72 6368 2041 7574 6f64 6966 6620 666f  orch Autodiff fo
+00000640: 7220 4446 542d 4434 0a0a 3c74 6162 6c65  r DFT-D4..<table
+00000650: 3e0a 2020 3c74 723e 0a20 2020 203c 7464  >.  <tr>.    <td
+00000660: 3e43 6f6d 7061 7469 6269 6c69 7479 3a3c  >Compatibility:<
+00000670: 2f74 643e 0a20 2020 203c 7464 3e0a 2020  /td>.    <td>.  
+00000680: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000690: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000006a0: 732e 696f 2f62 6164 6765 2f50 7974 686f  s.io/badge/Pytho
+000006b0: 6e2d 332e 3825 3230 7c25 3230 332e 3925  n-3.8%20|%203.9%
+000006c0: 3230 7c25 3230 332e 3130 2532 307c 2532  20|%203.10%20|%2
+000006d0: 3033 2e31 312d 626c 7565 2e73 7667 2220  03.11-blue.svg" 
+000006e0: 616c 743d 2250 7974 686f 6e20 5665 7273  alt="Python Vers
+000006f0: 696f 6e73 222f 3e0a 2020 2020 2020 3c69  ions"/>.      <i
+00000700: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000710: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000720: 6164 6765 2f50 7954 6f72 6368 2d25 3345  adge/PyTorch-%3E
+00000730: 3d31 2e31 312e 302d 626c 7565 2e73 7667  =1.11.0-blue.svg
+00000740: 2220 616c 743d 2250 7954 6f72 6368 2056  " alt="PyTorch V
+00000750: 6572 7369 6f6e 7322 2f3e 0a20 2020 203c  ersions"/>.    <
+00000760: 2f74 643e 0a20 203c 2f74 723e 0a20 203c  /td>.  </tr>.  <
+00000770: 7472 3e0a 2020 2020 3c74 643e 4176 6169  tr>.    <td>Avai
+00000780: 6c61 6269 6c69 7479 3a3c 2f74 643e 0a20  lability:</td>. 
+00000790: 2020 203c 7464 3e0a 2020 2020 2020 3c61     <td>.      <a
+000007a0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000007b0: 6974 6875 622e 636f 6d2f 6466 7464 342f  ithub.com/dftd4/
+000007c0: 7461 642d 6466 7464 342f 7265 6c65 6173  tad-dftd4/releas
+000007d0: 6573 2f6c 6174 6573 7422 3e0a 2020 2020  es/latest">.    
+000007e0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+000007f0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000800: 732e 696f 2f67 6974 6875 622f 762f 7265  s.io/github/v/re
+00000810: 6c65 6173 652f 6466 7464 342f 7461 642d  lease/dftd4/tad-
+00000820: 6466 7464 343f 636f 6c6f 723d 6f72 616e  dftd4?color=oran
+00000830: 6765 2220 616c 743d 2252 656c 6561 7365  ge" alt="Release
+00000840: 222f 3e0a 2020 2020 2020 3c2f 613e 0a20  "/>.      </a>. 
+00000850: 2020 2020 203c 6120 6872 6566 3d22 6874       <a href="ht
+00000860: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000870: 726f 6a65 6374 2f74 6164 2d64 6674 6434  roject/tad-dftd4
+00000880: 2f22 3e0a 2020 2020 2020 2020 3c69 6d67  /">.        <img
+00000890: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+000008a0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+000008b0: 692f 762f 7461 642d 6466 7464 343f 636f  i/v/tad-dftd4?co
+000008c0: 6c6f 723d 6f72 616e 6765 2220 616c 743d  lor=orange" alt=
+000008d0: 2250 7950 4922 2f3e 0a20 2020 2020 203c  "PyPI"/>.      <
+000008e0: 2f61 3e0a 2020 2020 2020 3c61 2068 7265  /a>.      <a hre
+000008f0: 663d 2268 7474 703a 2f2f 7777 772e 6170  f="http://www.ap
+00000900: 6163 6865 2e6f 7267 2f6c 6963 656e 7365  ache.org/license
+00000910: 732f 4c49 4345 4e53 452d 322e 3022 3e0a  s/LICENSE-2.0">.
+00000920: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000930: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000940: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
+00000950: 6963 656e 7365 2d41 7061 6368 6525 3230  icense-Apache%20
+00000960: 322e 302d 6f72 616e 6765 2e73 7667 2220  2.0-orange.svg" 
+00000970: 616c 743d 2241 7061 6368 652d 322e 3022  alt="Apache-2.0"
+00000980: 2f3e 0a20 2020 2020 203c 2f61 3e0a 2020  />.      </a>.  
+00000990: 2020 3c2f 7464 3e0a 2020 3c2f 7472 3e0a    </td>.  </tr>.
+000009a0: 2020 3c74 723e 0a20 2020 203c 7464 3e53    <tr>.    <td>S
+000009b0: 7461 7475 733a 3c2f 7464 3e0a 2020 2020  tatus:</td>.    
+000009c0: 3c74 643e 0a20 2020 2020 203c 6120 6872  <td>.      <a hr
+000009d0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000009e0: 7562 2e63 6f6d 2f64 6674 6434 2f74 6164  ub.com/dftd4/tad
+000009f0: 2d64 6674 6434 2f61 6374 696f 6e73 2f77  -dftd4/actions/w
+00000a00: 6f72 6b66 6c6f 7773 2f70 7974 686f 6e2e  orkflows/python.
+00000a10: 7961 6d6c 223e 0a20 2020 2020 2020 203c  yaml">.        <
+00000a20: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000a30: 2f67 6974 6875 622e 636f 6d2f 6466 7464  /github.com/dftd
+00000a40: 342f 7461 642d 6466 7464 342f 6163 7469  4/tad-dftd4/acti
+00000a50: 6f6e 732f 776f 726b 666c 6f77 732f 7079  ons/workflows/py
+00000a60: 7468 6f6e 2e79 616d 6c2f 6261 6467 652e  thon.yaml/badge.
+00000a70: 7376 6722 2061 6c74 3d22 5465 7374 2053  svg" alt="Test S
+00000a80: 7461 7475 7322 2f3e 0a20 2020 2020 203c  tatus"/>.      <
+00000a90: 2f61 3e0a 2020 2020 2020 3c61 2068 7265  /a>.      <a hre
+00000aa0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00000ab0: 622e 636f 6d2f 6466 7464 342f 7461 642d  b.com/dftd4/tad-
+00000ac0: 6466 7464 342f 6163 7469 6f6e 732f 776f  dftd4/actions/wo
+00000ad0: 726b 666c 6f77 732f 7265 6c65 6173 652e  rkflows/release.
+00000ae0: 7961 6d6c 223e 0a20 2020 2020 2020 203c  yaml">.        <
+00000af0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000b00: 2f67 6974 6875 622e 636f 6d2f 6466 7464  /github.com/dftd
+00000b10: 342f 7461 642d 6466 7464 342f 6163 7469  4/tad-dftd4/acti
+00000b20: 6f6e 732f 776f 726b 666c 6f77 732f 7265  ons/workflows/re
+00000b30: 6c65 6173 652e 7961 6d6c 2f62 6164 6765  lease.yaml/badge
+00000b40: 2e73 7667 2220 616c 743d 2242 7569 6c64  .svg" alt="Build
+00000b50: 2053 7461 7475 7322 2f3e 0a20 2020 2020   Status"/>.     
+00000b60: 203c 2f61 3e0a 2020 2020 2020 3c61 2068   </a>.      <a h
+00000b70: 7265 663d 2268 7474 7073 3a2f 2f74 6164  ref="https://tad
+00000b80: 2d64 6674 6434 2e72 6561 6474 6865 646f  -dftd4.readthedo
+00000b90: 6373 2e69 6f22 3e0a 2020 2020 2020 2020  cs.io">.        
+00000ba0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000bb0: 2f2f 7265 6164 7468 6564 6f63 732e 6f72  //readthedocs.or
+00000bc0: 672f 7072 6f6a 6563 7473 2f74 6164 2d64  g/projects/tad-d
+00000bd0: 6674 6434 2f62 6164 6765 2f3f 7665 7273  ftd4/badge/?vers
+00000be0: 696f 6e3d 6c61 7465 7374 2220 616c 743d  ion=latest" alt=
+00000bf0: 2244 6f63 756d 656e 7461 7469 6f6e 2053  "Documentation S
+00000c00: 7461 7475 7322 2f3e 0a20 2020 2020 203c  tatus"/>.      <
+00000c10: 2f61 3e0a 2020 2020 2020 3c61 2068 7265  /a>.      <a hre
+00000c20: 663d 2268 7474 7073 3a2f 2f72 6573 756c  f="https://resul
+00000c30: 7473 2e70 7265 2d63 6f6d 6d69 742e 6369  ts.pre-commit.ci
+00000c40: 2f6c 6174 6573 742f 6769 7468 7562 2f64  /latest/github/d
+00000c50: 6674 6434 2f74 6164 2d64 6674 6434 2f6d  ftd4/tad-dftd4/m
+00000c60: 6169 6e22 3e0a 2020 2020 2020 2020 3c69  ain">.        <i
+00000c70: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000c80: 7265 7375 6c74 732e 7072 652d 636f 6d6d  results.pre-comm
+00000c90: 6974 2e63 692f 6261 6467 652f 6769 7468  it.ci/badge/gith
+00000ca0: 7562 2f64 6674 6434 2f74 6164 2d64 6674  ub/dftd4/tad-dft
+00000cb0: 6434 2f6d 6169 6e2e 7376 6722 2061 6c74  d4/main.svg" alt
+00000cc0: 3d22 7072 652d 636f 6d6d 6974 2e63 6920  ="pre-commit.ci 
+00000cd0: 5374 6174 7573 222f 3e0a 2020 2020 2020  Status"/>.      
+00000ce0: 3c2f 613e 0a20 2020 2020 203c 6120 6872  </a>.      <a hr
+00000cf0: 6566 3d22 6874 7470 733a 2f2f 636f 6465  ef="https://code
+00000d00: 636f 762e 696f 2f67 682f 6466 7464 342f  cov.io/gh/dftd4/
+00000d10: 7461 642d 6466 7464 3422 3e0a 2020 2020  tad-dftd4">.    
+00000d20: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000d30: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00000d40: 2f67 682f 6466 7464 342f 7461 642d 6466  /gh/dftd4/tad-df
+00000d50: 7464 342f 6272 616e 6368 2f6d 6169 6e2f  td4/branch/main/
+00000d60: 6772 6170 682f 6261 6467 652e 7376 673f  graph/badge.svg?
+00000d70: 746f 6b65 6e3d 4f47 4a4a 6e5a 3674 3447  token=OGJJnZ6t4G
+00000d80: 2220 616c 743d 2243 6f76 6572 6167 6522  " alt="Coverage"
+00000d90: 2f3e 0a20 2020 2020 203c 2f61 3e0a 2020  />.      </a>.  
+00000da0: 2020 3c2f 7464 3e0a 2020 3c2f 7472 3e0a    </td>.  </tr>.
+00000db0: 3c2f 7461 626c 653e 0a0a 3c62 723e 0a0a  </table>..<br>..
+00000dc0: 496d 706c 656d 656e 7461 7469 6f6e 206f  Implementation o
+00000dd0: 6620 7468 6520 4446 542d 4434 2064 6973  f the DFT-D4 dis
+00000de0: 7065 7273 696f 6e20 6d6f 6465 6c20 696e  persion model in
+00000df0: 2050 7954 6f72 6368 2e20 5468 6973 206d   PyTorch. This m
+00000e00: 6f64 756c 6520 616c 6c6f 7773 2074 6f20  odule allows to 
+00000e10: 7072 6f63 6573 7320 6120 7369 6e67 6c65  process a single
+00000e20: 2073 7472 7563 7475 7265 206f 7220 6120   structure or a 
+00000e30: 6261 7463 6820 6f66 2073 7472 7563 7475  batch of structu
+00000e40: 7265 7320 666f 7220 7468 6520 6361 6c63  res for the calc
+00000e50: 756c 6174 696f 6e20 6f66 2061 746f 6d2d  ulation of atom-
+00000e60: 7265 736f 6c76 6564 2064 6973 7065 7273  resolved dispers
+00000e70: 696f 6e20 656e 6572 6769 6573 2e0a 0a46  ion energies...F
+00000e80: 6f72 2064 6574 6169 6c73 206f 6e20 7468  or details on th
+00000e90: 6520 4434 2064 6973 7065 7273 696f 6e20  e D4 dispersion 
+00000ea0: 6d6f 6465 6c2c 2073 6565 3a0a 0a2d 2045  model, see:..- E
+00000eb0: 2e20 4361 6c64 6577 6579 6865 722c 2043  . Caldeweyher, C
+00000ec0: 2e20 4261 6e6e 7761 7274 6820 616e 6420  . Bannwarth and 
+00000ed0: 532e 2047 7269 6d6d 652c 202a 4a2e 2043  S. Grimme, *J. C
+00000ee0: 6865 6d2e 2050 6879 732e 2a2c 2032 3031  hem. Phys.*, 201
+00000ef0: 372c 2031 3437 2c20 3033 3431 3132 2e20  7, 147, 034112. 
+00000f00: 5b44 4f49 3a20 3130 2e31 3036 332f 312e  [DOI: 10.1063/1.
+00000f10: 3439 3933 3231 355d 2868 7474 7073 3a2f  4993215](https:/
+00000f20: 2f64 782e 646f 692e 6f72 672f 3130 2e31  /dx.doi.org/10.1
+00000f30: 3036 332f 312e 3439 3933 3231 3529 0a2d  063/1.4993215).-
+00000f40: 2045 2e20 4361 6c64 6577 6579 6865 722c   E. Caldeweyher,
+00000f50: 2053 2e20 4568 6c65 7274 2c20 412e 2048   S. Ehlert, A. H
+00000f60: 616e 7365 6e2c 2048 2e20 4e65 7567 6562  ansen, H. Neugeb
+00000f70: 6175 6572 2c20 532e 2053 7069 6368 6572  auer, S. Spicher
+00000f80: 2c20 432e 2042 616e 6e77 6172 7468 2061  , C. Bannwarth a
+00000f90: 6e64 2053 2e20 4772 696d 6d65 2c20 2a4a  nd S. Grimme, *J
+00000fa0: 2e20 4368 656d 2e20 5068 7973 2e2a 2c20  . Chem. Phys.*, 
+00000fb0: 3230 3139 2c20 3135 302c 2031 3534 3132  2019, 150, 15412
+00000fc0: 322e 205b 444f 493a 2031 302e 3130 3633  2. [DOI: 10.1063
+00000fd0: 2f31 2e35 3039 3032 3232 5d28 6874 7470  /1.5090222](http
+00000fe0: 733a 2f2f 6478 2e64 6f69 2e6f 7267 2f31  s://dx.doi.org/1
+00000ff0: 302e 3130 3633 2f31 2e35 3039 3032 3232  0.1063/1.5090222
+00001000: 290a 2d20 452e 2043 616c 6465 7765 7968  ).- E. Caldeweyh
+00001010: 6572 2c20 4a2e 2d4d 2e20 4d65 7765 732c  er, J.-M. Mewes,
+00001020: 2053 2e20 4568 6c65 7274 2061 6e64 2053   S. Ehlert and S
+00001030: 2e20 4772 696d 6d65 2c20 2a50 6879 732e  . Grimme, *Phys.
+00001040: 2043 6865 6d2e 2043 6865 6d2e 2050 6879   Chem. Chem. Phy
+00001050: 732e 2a2c 2032 3032 302c 2032 322c 2038  s.*, 2020, 22, 8
+00001060: 3439 392d 3835 3132 2e20 5b44 4f49 3a20  499-8512. [DOI: 
+00001070: 3130 2e31 3033 392f 4430 4350 3030 3530  10.1039/D0CP0050
+00001080: 3241 5d28 6874 7470 733a 2f2f 646f 692e  2A](https://doi.
+00001090: 6f72 672f 3130 2e31 3033 392f 4430 4350  org/10.1039/D0CP
+000010a0: 3030 3530 3241 290a 0a46 6f72 2061 6c74  00502A)..For alt
+000010b0: 6572 6e61 7469 7665 2069 6d70 6c65 6d65  ernative impleme
+000010c0: 6e74 6174 696f 6e73 2c20 616c 736f 2063  ntations, also c
+000010d0: 6865 636b 206f 7574 3a0a 0a2d 205b 6466  heck out:..- [df
+000010e0: 7464 345d 2868 7474 7073 3a2f 2f64 6674  td4](https://dft
+000010f0: 6434 2e72 6561 6474 6865 646f 6373 2e69  d4.readthedocs.i
+00001100: 6f29 3a20 496d 706c 656d 656e 7461 7469  o): Implementati
+00001110: 6f6e 206f 6620 7468 6520 4446 542d 4434  on of the DFT-D4
+00001120: 2064 6973 7065 7273 696f 6e20 6d6f 6465   dispersion mode
+00001130: 6c20 696e 2046 6f72 7472 616e 2077 6974  l in Fortran wit
+00001140: 6820 5079 7468 6f6e 2062 696e 6469 6e67  h Python binding
+00001150: 732e 0a2d 205b 6370 702d 6434 5d28 6874  s..- [cpp-d4](ht
+00001160: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001170: 2f64 6674 6434 2f63 7070 2d64 3429 3a20  /dftd4/cpp-d4): 
+00001180: 496d 706c 656d 656e 7461 7469 6f6e 206f  Implementation o
+00001190: 6620 7468 6520 4446 542d 4434 2064 6973  f the DFT-D4 dis
+000011a0: 7065 7273 696f 6e20 6d6f 6465 6c20 696e  persion model in
+000011b0: 2043 2b2b 2e0a 0a23 2320 496e 7374 616c   C++...## Instal
+000011c0: 6c61 7469 6f6e 0a0a 2323 2320 7069 700a  lation..### pip.
+000011d0: 0a2a 7461 642d 6466 7464 342a 2063 616e  .*tad-dftd4* can
+000011e0: 2065 6173 696c 7920 6265 2069 6e73 7461   easily be insta
+000011f0: 6c6c 6564 2077 6974 6820 6060 7069 7060  lled with ``pip`
+00001200: 602e 0a0a 6060 6073 680a 7069 7020 696e  `...```sh.pip in
+00001210: 7374 616c 6c20 7461 642d 6466 7464 340a  stall tad-dftd4.
+00001220: 6060 600a 0a23 2323 2046 726f 6d20 736f  ```..### From so
+00001230: 7572 6365 0a0a 5468 6973 2070 726f 6a65  urce..This proje
+00001240: 6374 2069 7320 686f 7374 6564 206f 6e20  ct is hosted on 
+00001250: 4769 7448 7562 2061 7420 5b64 6674 6434  GitHub at [dftd4
+00001260: 2f74 6164 2d64 6674 6434 5d28 6874 7470  /tad-dftd4](http
+00001270: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00001280: 6674 6434 2f74 6164 2d64 6674 6434 292e  ftd4/tad-dftd4).
+00001290: 0a4f 6274 6169 6e20 7468 6520 736f 7572  .Obtain the sour
+000012a0: 6365 2062 7920 636c 6f6e 696e 6720 7468  ce by cloning th
+000012b0: 6520 7265 706f 7369 746f 7279 2077 6974  e repository wit
+000012c0: 680a 0a60 6060 7368 0a67 6974 2063 6c6f  h..```sh.git clo
+000012d0: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
+000012e0: 622e 636f 6d2f 6466 7464 342f 7461 642d  b.com/dftd4/tad-
+000012f0: 6466 7464 340a 6364 2074 6164 2d64 6674  dftd4.cd tad-dft
+00001300: 6434 0a60 6060 0a0a 5765 2072 6563 6f6d  d4.```..We recom
+00001310: 6d65 6e64 2075 7369 6e67 2061 205b 636f  mend using a [co
+00001320: 6e64 615d 2868 7474 7073 3a2f 2f63 6f6e  nda](https://con
+00001330: 6461 2e69 6f2f 2920 656e 7669 726f 6e6d  da.io/) environm
+00001340: 656e 7420 746f 2069 6e73 7461 6c6c 2074  ent to install t
+00001350: 6865 2070 6163 6b61 6765 2e0a 596f 7520  he package..You 
+00001360: 6361 6e20 7365 7475 7020 7468 6520 656e  can setup the en
+00001370: 7669 726f 6e6d 656e 7420 6d61 6e61 6765  vironment manage
+00001380: 7220 7573 696e 6720 6120 5b6d 616d 6261  r using a [mamba
+00001390: 666f 7267 655d 2868 7474 7073 3a2f 2f67  forge](https://g
+000013a0: 6974 6875 622e 636f 6d2f 636f 6e64 612d  ithub.com/conda-
+000013b0: 666f 7267 652f 6d69 6e69 666f 7267 6529  forge/miniforge)
+000013c0: 2069 6e73 7461 6c6c 6572 2e0a 496e 7374   installer..Inst
+000013d0: 616c 6c20 7468 6520 7265 7175 6972 6564  all the required
+000013e0: 2064 6570 656e 6465 6e63 6965 7320 6672   dependencies fr
+000013f0: 6f6d 2074 6865 2063 6f6e 6461 2d66 6f72  om the conda-for
+00001400: 6765 2063 6861 6e6e 656c 2e0a 0a60 6060  ge channel...```
+00001410: 7368 0a6d 616d 6261 2065 6e76 2063 7265  sh.mamba env cre
+00001420: 6174 6520 2d6e 2074 6f72 6368 202d 6620  ate -n torch -f 
+00001430: 656e 7669 726f 6e6d 656e 742e 7961 6d6c  environment.yaml
+00001440: 0a6d 616d 6261 2061 6374 6976 6174 6520  .mamba activate 
+00001450: 746f 7263 680a 6060 600a 0a49 6e73 7461  torch.```..Insta
+00001460: 6c6c 2074 6869 7320 7072 6f6a 6563 7420  ll this project 
+00001470: 7769 7468 2060 6070 6970 6060 2069 6e20  with ``pip`` in 
+00001480: 7468 6520 656e 7669 726f 6e6d 656e 740a  the environment.
+00001490: 0a60 6060 7368 0a70 6970 2069 6e73 7461  .```sh.pip insta
+000014a0: 6c6c 202e 0a60 6060 0a0a 5468 6520 666f  ll ..```..The fo
+000014b0: 6c6c 6f77 696e 6720 6465 7065 6e64 656e  llowing dependen
+000014c0: 6369 6573 2061 7265 2072 6571 7569 7265  cies are require
+000014d0: 640a 0a2d 205b 6e75 6d70 795d 2868 7474  d..- [numpy](htt
+000014e0: 7073 3a2f 2f6e 756d 7079 2e6f 7267 2f29  ps://numpy.org/)
+000014f0: 0a2d 205b 7461 642d 6d63 7463 5d28 6874  .- [tad-mctc](ht
+00001500: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001510: 2f74 6164 2d6d 6374 632f 7461 642d 6d63  /tad-mctc/tad-mc
+00001520: 7463 2f29 0a2d 205b 7461 642d 6d75 6c74  tc/).- [tad-mult
+00001530: 6963 6861 7267 655d 2868 7474 7073 3a2f  icharge](https:/
+00001540: 2f67 6974 6875 622e 636f 6d2f 7461 642d  /github.com/tad-
+00001550: 6d63 7463 2f74 6164 2d6d 756c 7469 6368  mctc/tad-multich
+00001560: 6172 6765 2f29 0a2d 205b 746f 7263 685d  arge/).- [torch]
+00001570: 2868 7474 7073 3a2f 2f70 7974 6f72 6368  (https://pytorch
+00001580: 2e6f 7267 2f29 0a2d 205b 7079 7465 7374  .org/).- [pytest
+00001590: 5d28 6874 7470 733a 2f2f 646f 6373 2e70  ](https://docs.p
+000015a0: 7974 6573 742e 6f72 672f 2920 2874 6573  ytest.org/) (tes
+000015b0: 7473 206f 6e6c 7929 0a0a 2323 2044 6576  ts only)..## Dev
+000015c0: 656c 6f70 6d65 6e74 0a0a 466f 7220 6465  elopment..For de
+000015d0: 7665 6c6f 706d 656e 742c 2061 6464 6974  velopment, addit
+000015e0: 696f 6e61 6c6c 7920 696e 7374 616c 6c20  ionally install 
+000015f0: 7468 6520 666f 6c6c 6f77 696e 6720 746f  the following to
+00001600: 6f6c 7320 696e 2079 6f75 7220 656e 7669  ols in your envi
+00001610: 726f 6e6d 656e 742e 0a0a 6060 6073 680a  ronment...```sh.
+00001620: 6d61 6d62 6120 696e 7374 616c 6c20 626c  mamba install bl
+00001630: 6163 6b20 636f 7664 6566 6175 6c74 7320  ack covdefaults 
+00001640: 6d79 7079 2070 7265 2d63 6f6d 6d69 7420  mypy pre-commit 
+00001650: 7079 6c69 6e74 2070 7974 6573 7420 7079  pylint pytest py
+00001660: 7465 7374 2d63 6f76 2070 7974 6573 742d  test-cov pytest-
+00001670: 7864 6973 7420 746f 780a 7069 7020 696e  xdist tox.pip in
+00001680: 7374 616c 6c20 7079 7465 7374 2d72 616e  stall pytest-ran
+00001690: 646f 6d2d 6f72 6465 720a 6060 600a 0a57  dom-order.```..W
+000016a0: 6974 6820 7069 702c 2061 6464 2074 6865  ith pip, add the
+000016b0: 206f 7074 696f 6e20 6060 2d65 6060 2066   option ``-e`` f
+000016c0: 6f72 2069 6e73 7461 6c6c 696e 6720 696e  or installing in
+000016d0: 2064 6576 656c 6f70 6d65 6e74 206d 6f64   development mod
+000016e0: 652c 2061 6e64 2061 6464 2060 605b 6465  e, and add ``[de
+000016f0: 765d 6060 2066 6f72 2074 6865 2064 6576  v]`` for the dev
+00001700: 656c 6f70 6d65 6e74 2064 6570 656e 6465  elopment depende
+00001710: 6e63 6965 730a 0a60 6060 7368 0a70 6970  ncies..```sh.pip
+00001720: 2069 6e73 7461 6c6c 202d 6520 2e5b 6465   install -e .[de
+00001730: 765d 0a60 6060 0a0a 5468 6520 7072 652d  v].```..The pre-
+00001740: 636f 6d6d 6974 2068 6f6f 6b73 2061 7265  commit hooks are
+00001750: 2069 6e69 7469 616c 697a 6564 2062 7920   initialized by 
+00001760: 7275 6e6e 696e 6720 7468 6520 666f 6c6c  running the foll
+00001770: 6f77 696e 6720 636f 6d6d 616e 6420 696e  owing command in
+00001780: 2074 6865 2072 6f6f 7420 6f66 2074 6865   the root of the
+00001790: 2072 6570 6f73 6974 6f72 792e 0a0a 6060   repository...``
+000017a0: 6073 680a 7072 652d 636f 6d6d 6974 2069  `sh.pre-commit i
+000017b0: 6e73 7461 6c6c 0a60 6060 0a0a 466f 7220  nstall.```..For 
+000017c0: 7465 7374 696e 6720 616c 6c20 5079 7468  testing all Pyth
+000017d0: 6f6e 2065 6e76 6972 6f6e 6d65 6e74 732c  on environments,
+000017e0: 2073 696d 706c 7920 7275 6e20 6074 6f78   simply run `tox
+000017f0: 602e 0a0a 6060 6073 680a 746f 780a 6060  `...```sh.tox.``
+00001800: 600a 0a4e 6f74 6520 7468 6174 2074 6869  `..Note that thi
+00001810: 7320 7261 6e64 6f6d 697a 6573 2074 6865  s randomizes the
+00001820: 206f 7264 6572 206f 6620 7465 7374 7320   order of tests 
+00001830: 6275 7420 736b 6970 7320 226c 6172 6765  but skips "large
+00001840: 2220 7465 7374 732e 2054 6f20 6d6f 6469  " tests. To modi
+00001850: 6679 2074 6869 7320 6265 6861 7669 6f72  fy this behavior
+00001860: 2c20 6074 6f78 6020 6861 7320 746f 2073  , `tox` has to s
+00001870: 6b69 7020 7468 6520 6f70 7469 6f6e 616c  kip the optional
+00001880: 202a 706f 7361 7267 732a 2e0a 0a60 6060   *posargs*...```
+00001890: 7368 0a74 6f78 202d 2d20 7465 7374 0a60  sh.tox -- test.`
+000018a0: 6060 0a0a 2323 2045 7861 6d70 6c65 730a  ``..## Examples.
+000018b0: 0a54 6865 2066 6f6c 6c6f 7769 6e67 2065  .The following e
+000018c0: 7861 6d70 6c65 2073 686f 7773 2068 6f77  xample shows how
+000018d0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+000018e0: 6520 4446 542d 4434 2064 6973 7065 7273  e DFT-D4 dispers
+000018f0: 696f 6e20 656e 6572 6779 2066 6f72 2061  ion energy for a
+00001900: 2073 696e 676c 6520 7374 7275 6374 7572   single structur
+00001910: 652e 0a0a 6060 6070 7974 686f 6e0a 696d  e...```python.im
+00001920: 706f 7274 2074 6f72 6368 0a69 6d70 6f72  port torch.impor
+00001930: 7420 7461 645f 6466 7464 3420 6173 2064  t tad_dftd4 as d
+00001940: 340a 696d 706f 7274 2074 6164 5f6d 6374  4.import tad_mct
+00001950: 6320 6173 206d 6374 630a 0a6e 756d 6265  c as mctc..numbe
+00001960: 7273 203d 206d 6374 632e 636f 6e76 6572  rs = mctc.conver
+00001970: 742e 7379 6d62 6f6c 5f74 6f5f 6e75 6d62  t.symbol_to_numb
+00001980: 6572 2873 796d 626f 6c73 3d22 4320 4320  er(symbols="C C 
+00001990: 4320 4320 4e20 4320 5320 4820 4820 4820  C C N C S H H H 
+000019a0: 4820 4822 2e73 706c 6974 2829 290a 0a23  H H".split())..#
+000019b0: 2063 6f6f 7264 696e 6174 6573 2069 6e20   coordinates in 
+000019c0: 426f 6872 0a70 6f73 6974 696f 6e73 203d  Bohr.positions =
+000019d0: 2074 6f72 6368 2e74 656e 736f 7228 0a20   torch.tensor(. 
+000019e0: 2020 205b 0a20 2020 2020 2020 205b 2d32     [.        [-2
+000019f0: 2e35 3637 3435 3638 3535 3634 3637 312c  .56745685564671,
+00001a00: 202d 302e 3032 3530 3939 3835 3937 3939   -0.025099859799
+00001a10: 3130 2c20 302e 3030 3030 3030 3030 3030  10, 0.0000000000
+00001a20: 3030 3030 5d2c 0a20 2020 2020 2020 205b  0000],.        [
+00001a30: 2d31 2e33 3931 3737 3538 3234 3535 3739  -1.3917758245579
+00001a40: 372c 202b 322e 3237 3639 3631 3838 3838  7, +2.2769618888
+00001a50: 3030 3134 2c20 302e 3030 3030 3030 3030  0014, 0.00000000
+00001a60: 3030 3030 3030 5d2c 0a20 2020 2020 2020  000000],.       
+00001a70: 205b 2b31 2e32 3737 3834 3939 3536 3234   [+1.27784995624
+00001a80: 3839 342c 202b 322e 3435 3130 3734 3739  894, +2.45107479
+00001a90: 3735 3933 3836 2c20 302e 3030 3030 3030  759386, 0.000000
+00001aa0: 3030 3030 3030 3030 5d2c 0a20 2020 2020  00000000],.     
+00001ab0: 2020 205b 2b32 2e36 3238 3031 3933 3736     [+2.628019376
+00001ac0: 3135 3739 332c 202b 302e 3235 3932 3737  15793, +0.259277
+00001ad0: 3237 3032 3831 3230 2c20 302e 3030 3030  27028120, 0.0000
+00001ae0: 3030 3030 3030 3030 3030 5d2c 0a20 2020  0000000000],.   
+00001af0: 2020 2020 205b 2b31 2e34 3130 3937 3033       [+1.4109703
+00001b00: 3336 3631 3132 332c 202d 312e 3939 3839  3661123, -1.9989
+00001b10: 3039 3936 3037 3734 3132 2c20 302e 3030  0996077412, 0.00
+00001b20: 3030 3030 3030 3030 3030 3030 5d2c 0a20  000000000000],. 
+00001b30: 2020 2020 2020 205b 2d31 2e31 3731 3836         [-1.17186
+00001b40: 3130 3232 3938 3834 392c 202d 322e 3334  102298849, -2.34
+00001b50: 3232 3035 3736 3238 3431 3830 2c20 302e  220576284180, 0.
+00001b60: 3030 3030 3030 3030 3030 3030 3030 5d2c  00000000000000],
+00001b70: 0a20 2020 2020 2020 205b 2d32 2e33 3935  .        [-2.395
+00001b80: 3035 3939 3033 3638 3337 382c 202d 352e  05990368378, -5.
+00001b90: 3232 3633 3538 3338 3333 3233 3632 2c20  22635838332362, 
+00001ba0: 302e 3030 3030 3030 3030 3030 3030 3030  0.00000000000000
+00001bb0: 5d2c 0a20 2020 2020 2020 205b 2b32 2e34  ],.        [+2.4
+00001bc0: 3139 3631 3938 3034 3535 3435 372c 202d  1961980455457, -
+00001bd0: 332e 3632 3135 3830 3139 3235 3330 3435  3.62158019253045
+00001be0: 2c20 302e 3030 3030 3030 3030 3030 3030  , 0.000000000000
+00001bf0: 3030 5d2c 0a20 2020 2020 2020 205b 2d32  00],.        [-2
+00001c00: 2e35 3137 3434 3337 3438 3436 3036 352c  .51744374846065,
+00001c10: 202b 332e 3938 3138 3137 3133 3638 3637   +3.981817136867
+00001c20: 3436 2c20 302e 3030 3030 3030 3030 3030  46, 0.0000000000
+00001c30: 3030 3030 5d2c 0a20 2020 2020 2020 205b  0000],.        [
+00001c40: 2b32 2e32 3432 3639 3034 3833 3834 3737  +2.2426904838477
+00001c50: 352c 202b 342e 3234 3338 3934 3733 3230  5, +4.2438947320
+00001c60: 3336 3437 2c20 302e 3030 3030 3030 3030  3647, 0.00000000
+00001c70: 3030 3030 3030 5d2c 0a20 2020 2020 2020  000000],.       
+00001c80: 205b 2b34 2e36 3634 3838 3938 3435 3733   [+4.66488984573
+00001c90: 3935 362c 202b 302e 3137 3930 3735 3638  956, +0.17907568
+00001ca0: 3030 3634 3039 2c20 302e 3030 3030 3030  006409, 0.000000
+00001cb0: 3030 3030 3030 3030 5d2c 0a20 2020 2020  00000000],.     
+00001cc0: 2020 205b 2d34 2e36 3030 3434 3234 3437     [-4.600442447
+00001cd0: 3832 3233 372c 202d 302e 3137 3739 3437  82237, -0.177947
+00001ce0: 3334 3633 3734 3133 2c20 302e 3030 3030  34637413, 0.0000
+00001cf0: 3030 3030 3030 3030 3030 5d2c 0a20 2020  0000000000],.   
+00001d00: 205d 0a29 0a0a 2320 746f 7461 6c20 6368   ].)..# total ch
+00001d10: 6172 6765 206f 6620 7468 6520 7379 7374  arge of the syst
+00001d20: 656d 0a63 6861 7267 6520 3d20 746f 7263  em.charge = torc
+00001d30: 682e 7465 6e73 6f72 2830 2e30 290a 0a23  h.tensor(0.0)..#
+00001d40: 2054 5053 5368 2d44 342d 4154 4d20 7061   TPSSh-D4-ATM pa
+00001d50: 7261 6d65 7465 7273 0a70 6172 616d 203d  rameters.param =
+00001d60: 207b 0a20 2020 2022 7336 223a 2070 6f73   {.    "s6": pos
+00001d70: 6974 696f 6e73 2e6e 6577 5f74 656e 736f  itions.new_tenso
+00001d80: 7228 312e 3029 2c0a 2020 2020 2273 3822  r(1.0),.    "s8"
+00001d90: 3a20 706f 7369 7469 6f6e 732e 6e65 775f  : positions.new_
+00001da0: 7465 6e73 6f72 2831 2e38 3538 3937 3735  tensor(1.8589775
+00001db0: 3029 2c0a 2020 2020 2273 3922 3a20 706f  0),.    "s9": po
+00001dc0: 7369 7469 6f6e 732e 6e65 775f 7465 6e73  sitions.new_tens
+00001dd0: 6f72 2831 2e30 292c 0a20 2020 2022 6131  or(1.0),.    "a1
+00001de0: 223a 2070 6f73 6974 696f 6e73 2e6e 6577  ": positions.new
+00001df0: 5f74 656e 736f 7228 302e 3434 3238 3639  _tensor(0.442869
+00001e00: 3636 292c 0a20 2020 2022 6132 223a 2070  66),.    "a2": p
+00001e10: 6f73 6974 696f 6e73 2e6e 6577 5f74 656e  ositions.new_ten
+00001e20: 736f 7228 342e 3630 3233 3035 3334 292c  sor(4.60230534),
+00001e30: 0a7d 0a0a 656e 6572 6779 203d 2064 342e  .}..energy = d4.
+00001e40: 6466 7464 3428 6e75 6d62 6572 732c 2070  dftd4(numbers, p
+00001e50: 6f73 6974 696f 6e73 2c20 6368 6172 6765  ositions, charge
+00001e60: 2c20 7061 7261 6d29 0a74 6f72 6368 2e73  , param).torch.s
+00001e70: 6574 5f70 7269 6e74 6f70 7469 6f6e 7328  et_printoptions(
+00001e80: 7072 6563 6973 696f 6e3d 3130 290a 7072  precision=10).pr
+00001e90: 696e 7428 656e 6572 6779 290a 2320 7465  int(energy).# te
+00001ea0: 6e73 6f72 285b 2d30 2e30 3032 3038 3431  nsor([-0.0020841
+00001eb0: 3334 342c 202d 302e 3030 3138 3937 3131  344, -0.00189711
+00001ec0: 3935 2c20 2d30 2e30 3031 3831 3037 3531  95, -0.001810751
+00001ed0: 332c 202d 302e 3030 3138 3330 3536 3935  3, -0.0018305695
+00001ee0: 2c0a 2320 2020 2020 2020 2020 2d30 2e30  ,.#         -0.0
+00001ef0: 3032 3137 3337 3639 332c 202d 302e 3030  021737693, -0.00
+00001f00: 3139 3438 3432 3336 2c20 2d30 2e30 3032  19484236, -0.002
+00001f10: 3237 3838 3235 332c 202d 302e 3030 3034  2788253, -0.0004
+00001f20: 3038 3036 3538 2c0a 2320 2020 2020 2020  080658,.#       
+00001f30: 2020 2d30 2e30 3030 3432 3631 3836 362c    -0.0004261866,
+00001f40: 202d 302e 3030 3034 3139 3938 3339 2c20   -0.0004199839, 
+00001f50: 2d30 2e30 3030 3432 3830 3736 382c 202d  -0.0004280768, -
+00001f60: 302e 3030 3035 3130 3839 3335 5d29 0a60  0.0005108935]).`
+00001f70: 6060 0a0a 5468 6520 6e65 7874 2065 7861  ``..The next exa
+00001f80: 6d70 6c65 2073 686f 7773 2074 6865 2063  mple shows the c
+00001f90: 616c 6375 6c61 7469 6f6e 206f 6620 6469  alculation of di
+00001fa0: 7370 6572 7369 6f6e 2065 6e65 7267 6965  spersion energie
+00001fb0: 7320 666f 7220 6120 6261 7463 6820 6f66  s for a batch of
+00001fc0: 2073 7472 7563 7475 7265 732e 0a0a 6060   structures...``
+00001fd0: 6070 7974 686f 6e0a 0a69 6d70 6f72 7420  `python..import 
+00001fe0: 746f 7263 680a 696d 706f 7274 2074 6164  torch.import tad
+00001ff0: 5f64 6674 6434 2061 7320 6434 0a69 6d70  _dftd4 as d4.imp
+00002000: 6f72 7420 7461 645f 6d63 7463 2061 7320  ort tad_mctc as 
+00002010: 6d63 7463 0a0a 2320 5332 3220 7379 7374  mctc..# S22 syst
+00002020: 656d 2034 3a20 666f 726d 616d 6964 6520  em 4: formamide 
+00002030: 6469 6d65 720a 6e75 6d62 6572 7320 3d20  dimer.numbers = 
+00002040: 6d63 7463 2e62 6174 6368 2e70 6163 6b28  mctc.batch.pack(
+00002050: 280a 2020 2020 6d63 7463 2e63 6f6e 7665  (.    mctc.conve
+00002060: 7274 2e73 796d 626f 6c5f 746f 5f6e 756d  rt.symbol_to_num
+00002070: 6265 7228 2243 2043 204e 204e 2048 2048  ber("C C N N H H
+00002080: 2048 2048 2048 2048 204f 204f 222e 7370   H H H H O O".sp
+00002090: 6c69 7428 2929 2c0a 2020 2020 6d63 7463  lit()),.    mctc
+000020a0: 2e63 6f6e 7665 7274 2e73 796d 626f 6c5f  .convert.symbol_
+000020b0: 746f 5f6e 756d 6265 7228 2243 204f 204e  to_number("C O N
+000020c0: 2048 2048 2048 222e 7370 6c69 7428 2929   H H H".split())
+000020d0: 2c0a 2929 0a0a 2320 636f 6f72 6469 6e61  ,.))..# coordina
+000020e0: 7465 7320 696e 2042 6f68 720a 706f 7369  tes in Bohr.posi
+000020f0: 7469 6f6e 7320 3d20 6d63 7463 2e62 6174  tions = mctc.bat
+00002100: 6368 2e70 6163 6b28 280a 2020 2020 746f  ch.pack((.    to
+00002110: 7263 682e 7465 6e73 6f72 285b 0a20 2020  rch.tensor([.   
+00002120: 2020 2020 205b 2d33 2e38 3134 3639 3438       [-3.8146948
+00002130: 3831 3433 3932 312c 202b 302e 3039 3939  8143921, +0.0999
+00002140: 3334 3431 3430 3239 3132 2c20 302e 3030  3441402912, 0.00
+00002150: 3030 3030 3030 3030 3030 3030 5d2c 0a20  000000000000],. 
+00002160: 2020 2020 2020 205b 2b33 2e38 3134 3639         [+3.81469
+00002170: 3438 3831 3433 3932 312c 202d 302e 3039  488143921, -0.09
+00002180: 3939 3334 3431 3430 3239 3132 2c20 302e  993441402912, 0.
+00002190: 3030 3030 3030 3030 3030 3030 3030 5d2c  00000000000000],
+000021a0: 0a20 2020 2020 2020 205b 2d32 2e36 3630  .        [-2.660
+000021b0: 3330 3034 3933 3234 3033 362c 202d 322e  30049324036, -2.
+000021c0: 3135 3839 3832 3531 3533 3335 3038 2c20  15898251533508, 
+000021d0: 302e 3030 3030 3030 3030 3030 3030 3030  0.00000000000000
+000021e0: 5d2c 0a20 2020 2020 2020 205b 2b32 2e36  ],.        [+2.6
+000021f0: 3630 3330 3034 3933 3234 3033 362c 202b  6030049324036, +
+00002200: 322e 3135 3839 3832 3531 3533 3335 3038  2.15898251533508
+00002210: 2c20 302e 3030 3030 3030 3030 3030 3030  , 0.000000000000
+00002220: 3030 5d2c 0a20 2020 2020 2020 205b 2d30  00],.        [-0
+00002230: 2e37 3331 3738 3532 3937 3339 3338 302c  .73178529739380,
+00002240: 202d 322e 3238 3233 3737 3935 3832 3937   -2.282377958297
+00002250: 3733 2c20 302e 3030 3030 3030 3030 3030  73, 0.0000000000
+00002260: 3030 3030 5d2c 0a20 2020 2020 2020 205b  0000],.        [
+00002270: 2d35 2e38 3930 3339 3332 3537 3134 3131  -5.8903932571411
+00002280: 312c 202d 302e 3032 3538 3931 3134 3536  1, -0.0258911456
+00002290: 3931 3238 2c20 302e 3030 3030 3030 3030  9128, 0.00000000
+000022a0: 3030 3030 3030 5d2c 0a20 2020 2020 2020  000000],.       
+000022b0: 205b 2d33 2e37 3132 3534 3934 3438 3031   [-3.71254944801
+000022c0: 3333 312c 202d 332e 3733 3630 3537 3735  331, -3.73605775
+000022d0: 3833 3331 3330 2c20 302e 3030 3030 3030  833130, 0.000000
+000022e0: 3030 3030 3030 3030 5d2c 0a20 2020 2020  00000000],.     
+000022f0: 2020 205b 2b33 2e37 3132 3534 3934 3438     [+3.712549448
+00002300: 3031 3333 312c 202b 332e 3733 3630 3537  01331, +3.736057
+00002310: 3735 3833 3331 3330 2c20 302e 3030 3030  75833130, 0.0000
+00002320: 3030 3030 3030 3030 3030 5d2c 0a20 2020  0000000000],.   
+00002330: 2020 2020 205b 2b30 2e37 3331 3738 3532       [+0.7317852
+00002340: 3937 3339 3338 302c 202b 322e 3238 3233  9739380, +2.2823
+00002350: 3737 3935 3832 3937 3733 2c20 302e 3030  7795829773, 0.00
+00002360: 3030 3030 3030 3030 3030 3030 5d2c 0a20  000000000000],. 
+00002370: 2020 2020 2020 205b 2b35 2e38 3930 3339         [+5.89039
+00002380: 3332 3537 3134 3131 312c 202b 302e 3032  325714111, +0.02
+00002390: 3538 3931 3134 3536 3931 3238 2c20 302e  589114569128, 0.
+000023a0: 3030 3030 3030 3030 3030 3030 3030 5d2c  00000000000000],
+000023b0: 0a20 2020 2020 2020 205b 2d32 2e37 3434  .        [-2.744
+000023c0: 3236 3130 3236 3338 3234 352c 202b 322e  26102638245, +2.
+000023d0: 3136 3131 3535 3730 3036 3833 3539 2c20  16115570068359, 
+000023e0: 302e 3030 3030 3030 3030 3030 3030 3030  0.00000000000000
+000023f0: 5d2c 0a20 2020 2020 2020 205b 2b32 2e37  ],.        [+2.7
+00002400: 3434 3236 3130 3236 3338 3234 352c 202d  4426102638245, -
+00002410: 322e 3136 3131 3535 3730 3036 3833 3539  2.16115570068359
+00002420: 2c20 302e 3030 3030 3030 3030 3030 3030  , 0.000000000000
+00002430: 3030 5d2c 0a20 2020 205d 292c 0a20 2020  00],.    ]),.   
+00002440: 2074 6f72 6368 2e74 656e 736f 7228 5b0a   torch.tensor([.
+00002450: 2020 2020 2020 2020 5b2d 302e 3535 3536          [-0.5556
+00002460: 3937 3433 3230 3334 3036 2c20 2b31 2e30  9743203406, +1.0
+00002470: 3930 3330 3432 3534 3638 3535 372c 2030  9030425468557, 0
+00002480: 2e30 3030 3030 3030 3030 3030 3030 305d  .00000000000000]
+00002490: 2c0a 2020 2020 2020 2020 5b2b 302e 3531  ,.        [+0.51
+000024a0: 3437 3336 3334 3637 3834 3639 2c20 2b33  473634678469, +3
+000024b0: 2e31 3531 3532 3535 3032 3633 3631 312c  .15152550263611,
+000024c0: 2030 2e30 3030 3030 3030 3030 3030 3030   0.0000000000000
+000024d0: 305d 2c0a 2020 2020 2020 2020 5b2b 302e  0],.        [+0.
+000024e0: 3539 3836 3936 3930 3234 3434 3436 2c20  59869690244446, 
+000024f0: 2d31 2e31 3638 3631 3236 3337 3839 3437  -1.1686126378947
+00002500: 372c 2030 2e30 3030 3030 3030 3030 3030  7, 0.00000000000
+00002510: 3030 305d 2c0a 2020 2020 2020 2020 5b2d  000],.        [-
+00002520: 302e 3435 3335 3532 3033 3636 3931 3334  0.45355203669134
+00002530: 2c20 2d32 2e37 3435 3638 3738 3034 3338  , -2.74568780438
+00002540: 3036 342c 2030 2e30 3030 3030 3030 3030  064, 0.000000000
+00002550: 3030 3030 305d 2c0a 2020 2020 2020 2020  00000],.        
+00002560: 5b2b 322e 3532 3732 3132 3039 3534 3439  [+2.527212095449
+00002570: 3939 2c20 2d31 2e32 3932 3030 3830 3039  99, -1.292008009
+00002580: 3536 3836 372c 2030 2e30 3030 3030 3030  56867, 0.0000000
+00002590: 3030 3030 3030 305d 2c0a 2020 2020 2020  0000000],.      
+000025a0: 2020 5b2d 322e 3633 3133 3935 3837 3539    [-2.6313958759
+000025b0: 3533 3736 2c20 2b30 2e39 3634 3437 3836  5376, +0.9644786
+000025c0: 3934 3532 3234 302c 2030 2e30 3030 3030  9452240, 0.00000
+000025d0: 3030 3030 3030 3030 305d 2c0a 2020 2020  000000000],.    
+000025e0: 5d29 2c0a 2929 0a0a 2320 746f 7461 6c20  ]),.))..# total 
+000025f0: 6368 6172 6765 206f 6620 626f 7468 2073  charge of both s
+00002600: 7973 7465 6d0a 6368 6172 6765 203d 2074  ystem.charge = t
+00002610: 6f72 6368 2e74 656e 736f 7228 5b30 2e30  orch.tensor([0.0
+00002620: 2c20 302e 305d 290a 0a23 2054 5053 5368  , 0.0])..# TPSSh
+00002630: 2d44 342d 4154 4d20 7061 7261 6d65 7465  -D4-ATM paramete
+00002640: 7273 0a70 6172 616d 203d 207b 0a20 2020  rs.param = {.   
+00002650: 2022 7336 223a 2070 6f73 6974 696f 6e73   "s6": positions
+00002660: 2e6e 6577 5f74 656e 736f 7228 312e 3029  .new_tensor(1.0)
+00002670: 2c0a 2020 2020 2273 3822 3a20 706f 7369  ,.    "s8": posi
+00002680: 7469 6f6e 732e 6e65 775f 7465 6e73 6f72  tions.new_tensor
+00002690: 2831 2e38 3538 3937 3735 3029 2c0a 2020  (1.85897750),.  
+000026a0: 2020 2273 3922 3a20 706f 7369 7469 6f6e    "s9": position
+000026b0: 732e 6e65 775f 7465 6e73 6f72 2831 2e30  s.new_tensor(1.0
+000026c0: 292c 0a20 2020 2022 6131 223a 2070 6f73  ),.    "a1": pos
+000026d0: 6974 696f 6e73 2e6e 6577 5f74 656e 736f  itions.new_tenso
+000026e0: 7228 302e 3434 3238 3639 3636 292c 0a20  r(0.44286966),. 
+000026f0: 2020 2022 6132 223a 2070 6f73 6974 696f     "a2": positio
+00002700: 6e73 2e6e 6577 5f74 656e 736f 7228 342e  ns.new_tensor(4.
+00002710: 3630 3233 3035 3334 292c 0a7d 0a0a 2320  60230534),.}..# 
+00002720: 6361 6c63 756c 6174 6520 6469 7370 6572  calculate disper
+00002730: 7369 6f6e 2065 6e65 7267 7920 696e 2048  sion energy in H
+00002740: 6172 7472 6565 0a65 6e65 7267 7920 3d20  artree.energy = 
+00002750: 746f 7263 682e 7375 6d28 6434 2e64 6674  torch.sum(d4.dft
+00002760: 6434 286e 756d 6265 7273 2c20 706f 7369  d4(numbers, posi
+00002770: 7469 6f6e 732c 2063 6861 7267 652c 2070  tions, charge, p
+00002780: 6172 616d 292c 202d 3129 0a74 6f72 6368  aram), -1).torch
+00002790: 2e73 6574 5f70 7269 6e74 6f70 7469 6f6e  .set_printoption
+000027a0: 7328 7072 6563 6973 696f 6e3d 3130 290a  s(precision=10).
+000027b0: 7072 696e 7428 656e 6572 6779 290a 2320  print(energy).# 
+000027c0: 7465 6e73 6f72 285b 2d30 2e30 3038 3833  tensor([-0.00883
+000027d0: 3431 3433 322c 202d 302e 3030 3237 3031  41432, -0.002701
+000027e0: 3336 3037 5d29 0a70 7269 6e74 2865 6e65  3607]).print(ene
+000027f0: 7267 795b 305d 202d 2032 2a65 6e65 7267  rgy[0] - 2*energ
+00002800: 795b 315d 290a 2320 7465 6e73 6f72 282d  y[1]).# tensor(-
+00002810: 302e 3030 3334 3331 3432 3137 290a 6060  0.0034314217).``
+00002820: 600a 0a23 2320 436f 6e74 7269 6275 7469  `..## Contributi
+00002830: 6e67 0a0a 5468 6973 2069 7320 6120 766f  ng..This is a vo
+00002840: 6c75 6e74 6565 7220 6f70 656e 2073 6f75  lunteer open sou
+00002850: 7263 6520 7072 6f6a 6563 7473 2061 6e64  rce projects and
+00002860: 2063 6f6e 7472 6962 7574 696f 6e73 2061   contributions a
+00002870: 7265 2061 6c77 6179 7320 7765 6c63 6f6d  re always welcom
+00002880: 652e 0a50 6c65 6173 652c 2074 616b 6520  e..Please, take 
+00002890: 6120 6d6f 6d65 6e74 2074 6f20 7265 6164  a moment to read
+000028a0: 2074 6865 205b 636f 6e74 7269 6275 7469   the [contributi
+000028b0: 6e67 2067 7569 6465 6c69 6e65 735d 2843  ng guidelines](C
+000028c0: 4f4e 5452 4942 5554 494e 472e 6d64 292e  ONTRIBUTING.md).
+000028d0: 0a0a 2323 204c 6963 656e 7365 0a0a 5468  ..## License..Th
+000028e0: 6973 2070 726f 6a65 6374 2069 7320 6c69  is project is li
+000028f0: 6365 6e73 6564 2075 6e64 6572 2074 6865  censed under the
+00002900: 2041 7061 6368 6520 4c69 6365 6e73 652c   Apache License,
+00002910: 2056 6572 7369 6f6e 2032 2e30 2028 7468   Version 2.0 (th
+00002920: 6520 224c 6963 656e 7365 2229 3b20 796f  e "License"); yo
+00002930: 7520 6d61 7920 6e6f 7420 7573 6520 7468  u may not use th
+00002940: 6973 2070 726f 6a65 6374 2773 2066 696c  is project's fil
+00002950: 6573 2065 7863 6570 7420 696e 2063 6f6d  es except in com
+00002960: 706c 6961 6e63 6520 7769 7468 2074 6865  pliance with the
+00002970: 204c 6963 656e 7365 2e20 596f 7520 6d61   License. You ma
+00002980: 7920 6f62 7461 696e 2061 2063 6f70 7920  y obtain a copy 
+00002990: 6f66 2074 6865 204c 6963 656e 7365 2061  of the License a
+000029a0: 740a 0a68 7474 703a 2f2f 7777 772e 6170  t..http://www.ap
+000029b0: 6163 6865 2e6f 7267 2f6c 6963 656e 7365  ache.org/license
+000029c0: 732f 4c49 4345 4e53 452d 322e 300a 0a55  s/LICENSE-2.0..U
+000029d0: 6e6c 6573 7320 7265 7175 6972 6564 2062  nless required b
+000029e0: 7920 6170 706c 6963 6162 6c65 206c 6177  y applicable law
+000029f0: 206f 7220 6167 7265 6564 2074 6f20 696e   or agreed to in
+00002a00: 2077 7269 7469 6e67 2c20 736f 6674 7761   writing, softwa
+00002a10: 7265 2064 6973 7472 6962 7574 6564 2075  re distributed u
+00002a20: 6e64 6572 2074 6865 204c 6963 656e 7365  nder the License
+00002a30: 2069 7320 6469 7374 7269 6275 7465 6420   is distributed 
+00002a40: 6f6e 2061 6e20 2241 5320 4953 2220 4241  on an "AS IS" BA
+00002a50: 5349 532c 2057 4954 484f 5554 2057 4152  SIS, WITHOUT WAR
+00002a60: 5241 4e54 4945 5320 4f52 2043 4f4e 4449  RANTIES OR CONDI
+00002a70: 5449 4f4e 5320 4f46 2041 4e59 204b 494e  TIONS OF ANY KIN
+00002a80: 442c 2065 6974 6865 7220 6578 7072 6573  D, either expres
+00002a90: 7320 6f72 2069 6d70 6c69 6564 2e20 5365  s or implied. Se
+00002aa0: 6520 7468 6520 4c69 6365 6e73 6520 666f  e the License fo
+00002ab0: 7220 7468 6520 7370 6563 6966 6963 206c  r the specific l
+00002ac0: 616e 6775 6167 6520 676f 7665 726e 696e  anguage governin
+00002ad0: 6720 7065 726d 6973 7369 6f6e 7320 616e  g permissions an
+00002ae0: 6420 6c69 6d69 7461 7469 6f6e 7320 756e  d limitations un
+00002af0: 6465 7220 7468 6520 4c69 6365 6e73 652e  der the License.
+00002b00: 0a                                       .
```

