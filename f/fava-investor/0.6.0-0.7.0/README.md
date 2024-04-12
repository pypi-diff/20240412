# Comparing `tmp/fava_investor-0.6.0.tar.gz` & `tmp/fava_investor-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fava_investor-0.6.0.tar", last modified: Sat Feb  3 05:58:24 2024, max compression
+gzip compressed data, was "fava_investor-0.7.tar", last modified: Fri Apr 12 17:23:50 2024, max compression
```

## Comparing `fava_investor-0.6.0.tar` & `fava_investor-0.7.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.774938 fava_investor-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-02-03 05:58:12.000000 fava_investor-0.6.0/.gitchangelog.rc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.750939 fava_investor-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.758938 fava_investor-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-03 05:58:12.000000 fava_investor-0.6.0/.github/workflows/conventionalcommits.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-02-03 05:58:12.000000 fava_investor-0.6.0/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-03 05:58:12.000000 fava_investor-0.6.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-02-03 05:58:12.000000 fava_investor-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-02-03 05:58:12.000000 fava_investor-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-02-03 05:58:12.000000 fava_investor-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-03 05:58:12.000000 fava_investor-0.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-03 05:58:12.000000 fava_investor-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-02-03 05:58:24.774938 fava_investor-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-02-03 05:58:12.000000 fava_investor-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:12.000000 fava_investor-0.6.0/TODO.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-03 05:58:12.000000 fava_investor-0.6.0/design.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.758938 fava_investor-0.6.0/fava_investor/
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.758938 fava_investor-0.6.0/fava_investor/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/cli/investor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.758938 fava_investor-0.6.0/fava_investor/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/common/beancountinvestorapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/common/clicommon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/common/favainvestorapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/common/libinvestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.758938 fava_investor-0.6.0/fava_investor/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/examples/beancount-example.config
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/examples/example.beancount
--rw-r--r--   0 runner    (1001) docker     (127)   913210 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/examples/huge-example.beancount
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.762938 fava_investor-0.6.0/fava_investor/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.762938 fava_investor-0.6.0/fava_investor/modules/assetalloc_account/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/assetalloc_account/TODO.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/assetalloc_account/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2583 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/assetalloc_account/assetalloc_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/assetalloc_account/libaaacc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.762938 fava_investor-0.6.0/fava_investor/modules/assetalloc_class/
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/assetalloc_class/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/assetalloc_class/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2437 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/assetalloc_class/assetalloc_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/assetalloc_class/example.beancount
--rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/assetalloc_class/libassetalloc.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/assetalloc_class/multicurrency.beancount
--rw-r--r--   0 runner    (1001) docker     (127)     8812 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/assetalloc_class/test_asset_allocation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.762938 fava_investor-0.6.0/fava_investor/modules/cashdrag/
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/cashdrag/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/cashdrag/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1414 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/cashdrag/cashdrag.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/cashdrag/design.md
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/cashdrag/libcashdrag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.766938 fava_investor-0.6.0/fava_investor/modules/minimizegains/
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/minimizegains/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/minimizegains/TODO.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/minimizegains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/minimizegains/example.beancount
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/minimizegains/libminimizegains.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2549 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/minimizegains/minimizegains.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/minimizegains/test_minimizegains.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.766938 fava_investor-0.6.0/fava_investor/modules/summarizer/
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/summarizer/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/summarizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/summarizer/design.md
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/summarizer/example.beancount
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/summarizer/libsummarizer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1570 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/summarizer/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.770938 fava_investor-0.6.0/fava_investor/modules/tlh/
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/tlh/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/tlh/TODO.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/tlh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/tlh/example.beancount
--rw-r--r--   0 runner    (1001) docker     (127)    10919 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/tlh/libtlh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/tlh/test_libtlh.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   393735 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/tlh/tlh.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2200 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/tlh/tlh.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/modules/tlh/wash_substantially_identical.beancount
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.770938 fava_investor-0.6.0/fava_investor/pythonanywhere/
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/pythonanywhere/commodities.beancount
--rw-r--r--   0 runner    (1001) docker     (127)   316964 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/pythonanywhere/example.beancount
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/pythonanywhere/fava_config.beancount
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/pythonanywhere/favainvestor_pythonanywhere_com_wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/pythonanywhere/scripts
--rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/pythonanywhere/update.bash
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.770938 fava_investor-0.6.0/fava_investor/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/templates/Investor.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.770938 fava_investor-0.6.0/fava_investor/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/util/cachedtickerinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.770938 fava_investor-0.6.0/fava_investor/util/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/util/experimental/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6890 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/util/experimental/scaled_navs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/util/relatetickers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/util/test_relatetickers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12522 2024-02-03 05:58:12.000000 fava_investor-0.6.0/fava_investor/util/ticker_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 05:58:24.770938 fava_investor-0.6.0/fava_investor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-02-03 05:58:24.000000 fava_investor-0.6.0/fava_investor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-02-03 05:58:24.000000 fava_investor-0.6.0/fava_investor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 05:58:24.000000 fava_investor-0.6.0/fava_investor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-03 05:58:24.000000 fava_investor-0.6.0/fava_investor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 05:58:24.000000 fava_investor-0.6.0/fava_investor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-03 05:58:24.000000 fava_investor-0.6.0/fava_investor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-03 05:58:24.000000 fava_investor-0.6.0/fava_investor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-02-03 05:58:12.000000 fava_investor-0.6.0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    57629 2024-02-03 05:58:12.000000 fava_investor-0.6.0/screenshot-assetalloc.png
--rwxr-xr-x   0 runner    (1001) docker     (127)   111266 2024-02-03 05:58:12.000000 fava_investor-0.6.0/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-03 05:58:24.774938 fava_investor-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-03 05:58:12.000000 fava_investor-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.584261 fava_investor-0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-12 17:23:36.000000 fava_investor-0.7/.gitchangelog.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.560261 fava_investor-0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.568261 fava_investor-0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-12 17:23:36.000000 fava_investor-0.7/.github/workflows/conventionalcommits.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-12 17:23:36.000000 fava_investor-0.7/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-12 17:23:36.000000 fava_investor-0.7/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-12 17:23:36.000000 fava_investor-0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-04-12 17:23:36.000000 fava_investor-0.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-12 17:23:36.000000 fava_investor-0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 17:23:36.000000 fava_investor-0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 17:23:36.000000 fava_investor-0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-12 17:23:50.580261 fava_investor-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-12 17:23:36.000000 fava_investor-0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:36.000000 fava_investor-0.7/TODO.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-12 17:23:36.000000 fava_investor-0.7/design.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.568261 fava_investor-0.7/fava_investor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.568261 fava_investor-0.7/fava_investor/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/cli/investor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.568261 fava_investor-0.7/fava_investor/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/common/beancountinvestorapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/common/clicommon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/common/favainvestorapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/common/libinvestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.568261 fava_investor-0.7/fava_investor/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/examples/beancount-example.config
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/examples/example.beancount
+-rw-r--r--   0 runner    (1001) docker     (127)   913210 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/examples/huge-example.beancount
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.572261 fava_investor-0.7/fava_investor/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.572261 fava_investor-0.7/fava_investor/modules/assetalloc_account/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/assetalloc_account/TODO.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/assetalloc_account/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2583 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/assetalloc_account/assetalloc_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/assetalloc_account/libaaacc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.572261 fava_investor-0.7/fava_investor/modules/assetalloc_class/
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/assetalloc_class/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/assetalloc_class/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2437 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/assetalloc_class/assetalloc_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/assetalloc_class/example.beancount
+-rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/assetalloc_class/libassetalloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/assetalloc_class/multicurrency.beancount
+-rw-r--r--   0 runner    (1001) docker     (127)     8812 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/assetalloc_class/test_asset_allocation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.572261 fava_investor-0.7/fava_investor/modules/cashdrag/
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/cashdrag/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/cashdrag/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1414 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/cashdrag/cashdrag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/cashdrag/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/cashdrag/libcashdrag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.576261 fava_investor-0.7/fava_investor/modules/minimizegains/
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/minimizegains/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/minimizegains/TODO.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/minimizegains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/minimizegains/example.beancount
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/minimizegains/libminimizegains.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2549 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/minimizegains/minimizegains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/minimizegains/test_minimizegains.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.576261 fava_investor-0.7/fava_investor/modules/summarizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/summarizer/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/summarizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/summarizer/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/summarizer/example.beancount
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/summarizer/libsummarizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1570 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/summarizer/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.580261 fava_investor-0.7/fava_investor/modules/tlh/
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/tlh/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/tlh/TODO.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/tlh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/tlh/example.beancount
+-rw-r--r--   0 runner    (1001) docker     (127)    10919 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/tlh/libtlh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/tlh/test_libtlh.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   393735 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/tlh/tlh.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2200 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/tlh/tlh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/modules/tlh/wash_substantially_identical.beancount
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.580261 fava_investor-0.7/fava_investor/pythonanywhere/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/pythonanywhere/commodities.beancount
+-rw-r--r--   0 runner    (1001) docker     (127)   316964 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/pythonanywhere/example.beancount
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/pythonanywhere/fava_config.beancount
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/pythonanywhere/favainvestor_pythonanywhere_com_wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/pythonanywhere/scripts
+-rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/pythonanywhere/update.bash
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.580261 fava_investor-0.7/fava_investor/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/templates/Investor.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.580261 fava_investor-0.7/fava_investor/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/util/cachedtickerinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.580261 fava_investor-0.7/fava_investor/util/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/util/experimental/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6890 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/util/experimental/scaled_navs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/util/relatetickers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/util/test_relatetickers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12522 2024-04-12 17:23:36.000000 fava_investor-0.7/fava_investor/util/ticker_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:50.580261 fava_investor-0.7/fava_investor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-12 17:23:50.000000 fava_investor-0.7/fava_investor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-12 17:23:50.000000 fava_investor-0.7/fava_investor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:23:50.000000 fava_investor-0.7/fava_investor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-12 17:23:50.000000 fava_investor-0.7/fava_investor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:23:50.000000 fava_investor-0.7/fava_investor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-12 17:23:50.000000 fava_investor-0.7/fava_investor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 17:23:50.000000 fava_investor-0.7/fava_investor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-12 17:23:36.000000 fava_investor-0.7/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57629 2024-04-12 17:23:36.000000 fava_investor-0.7/screenshot-assetalloc.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)   111266 2024-04-12 17:23:36.000000 fava_investor-0.7/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:23:50.584261 fava_investor-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-12 17:23:36.000000 fava_investor-0.7/setup.py
```

### Comparing `fava_investor-0.6.0/.gitchangelog.rc` & `fava_investor-0.7/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/.github/workflows/pythonpackage.yml` & `fava_investor-0.7/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/.github/workflows/pythonpublish.yml` & `fava_investor-0.7/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/.gitignore` & `fava_investor-0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/CHANGELOG.md` & `fava_investor-0.7/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # Changelog
 
-## (unreleased)
+## 0.7.0 (2024-02-02)
 
+This release brings fava_investor up to date with upstream changes in Fava. Primarily,
+asset allocation by class was fixed. Thanks to contributors below.
+
+### Fixes
+
+- Fix assetalloc_class chart (#93) [Adriano Di Luzio]
+- remove dead code for Fava <v1.18 (#91) [Jakob Schnitzer]
+- hierarchy chart: remove now uneeded modifier (#90) [Jakob Schnitzer]
+- libsummarizer crash in Fava (wrong pricemap) [Red S]
+- build_beancount_pricemap() was missing in cli version. [Red S]
+
+
+## 0.6.0 (2024-02-02)
 
 ### Improvements
 
 - Fix to work with upstream changes (Fava 1.25+)
 
 - Make currency regex not incorrectly match substrings (#88) [Tyler Schicke]
```

### Comparing `fava_investor-0.6.0/CONTRIBUTING.md` & `fava_investor-0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/LICENSE.md` & `fava_investor-0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/PKG-INFO` & `fava_investor-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fava_investor
-Version: 0.6.0
+Version: 0.7.0
 Summary: Fava extension and beancount libraries for investing
 Home-page: https://github.com/redstreet/fava_investor
 Author: Red S
 Author-email: redstreet@users.noreply.github.com
 License: GPL-3.0
 Keywords: fava beancount accounting investment
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: Click>=7.0
 Requires-Dist: beancount>=2.3.2
 Requires-Dist: click_aliases>=1.0.1
-Requires-Dist: fava>=1.23
+Requires-Dist: fava>=1.26
 Requires-Dist: packaging>=20.3
 Requires-Dist: python_dateutil>=2.8.1
 Requires-Dist: tabulate>=0.8.9
 Requires-Dist: yfinance>=0.1.70
 
 # Fava Investor
```

### Comparing `fava_investor-0.6.0/README.md` & `fava_investor-0.7/README.md`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/design.md` & `fava_investor-0.7/design.md`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/cli/investor.py` & `fava_investor-0.7/fava_investor/cli/investor.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/common/beancountinvestorapi.py` & `fava_investor-0.7/fava_investor/common/beancountinvestorapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 
     def end_date(self):
         return None  # Only used in fava (UI selection context)
 
     def build_price_map(self):
         return prices.build_price_map(self.entries)
 
+    def build_beancount_price_map(self):
+        return self.build_price_map
+
     def build_filtered_price_map(self, pos, base_currency):
         """Ignore filtering since we are not in fava. Return all prices"""
         return prices.build_price_map(self.entries)
 
     def get_commodity_directives(self):
         return getters.get_commodity_directives(self.entries)
```

### Comparing `fava_investor-0.6.0/fava_investor/common/clicommon.py` & `fava_investor-0.7/fava_investor/common/clicommon.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/common/favainvestorapi.py` & `fava_investor-0.7/fava_investor/common/favainvestorapi.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/common/libinvestor.py` & `fava_investor-0.7/fava_investor/common/libinvestor.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/examples/beancount-example.config` & `fava_investor-0.7/fava_investor/examples/beancount-example.config`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/examples/example.beancount` & `fava_investor-0.7/fava_investor/examples/example.beancount`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/examples/huge-example.beancount` & `fava_investor-0.7/fava_investor/examples/huge-example.beancount`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/assetalloc_account/assetalloc_account.py` & `fava_investor-0.7/fava_investor/modules/assetalloc_account/assetalloc_account.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/assetalloc_account/libaaacc.py` & `fava_investor-0.7/fava_investor/modules/assetalloc_account/libaaacc.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/assetalloc_class/README.md` & `fava_investor-0.7/fava_investor/modules/assetalloc_class/README.md`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/assetalloc_class/assetalloc_class.py` & `fava_investor-0.7/fava_investor/modules/assetalloc_class/assetalloc_class.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/assetalloc_class/example.beancount` & `fava_investor-0.7/fava_investor/modules/assetalloc_class/example.beancount`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/assetalloc_class/libassetalloc.py` & `fava_investor-0.7/fava_investor/modules/assetalloc_class/libassetalloc.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
         children = [child.serialise(currency) for child in self.children]
         return {
             "account": self.name,
             "balance_children": {currency: self.balance_children},
             "balance": {currency: self.balance},
             "children": children,
+            "has_txns": False,
         }
 
     def pretty_print(self, indent=0):
         fmt = "{}{} {:4.2f} {:4.2f} {:4.2f} {:4.2f} {:4.2f}"
         print(fmt.format('-' * indent, self.name,
                          self.balance, self.balance_children,
                          self.percentage, self.percentage_children, self.percentage_parent))
```

### Comparing `fava_investor-0.6.0/fava_investor/modules/assetalloc_class/multicurrency.beancount` & `fava_investor-0.7/fava_investor/modules/assetalloc_class/multicurrency.beancount`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/assetalloc_class/test_asset_allocation.py` & `fava_investor-0.7/fava_investor/modules/assetalloc_class/test_asset_allocation.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/cashdrag/README.md` & `fava_investor-0.7/fava_investor/modules/cashdrag/README.md`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/cashdrag/cashdrag.py` & `fava_investor-0.7/fava_investor/modules/cashdrag/cashdrag.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/cashdrag/libcashdrag.py` & `fava_investor-0.7/fava_investor/modules/cashdrag/libcashdrag.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/minimizegains/README.md` & `fava_investor-0.7/fava_investor/modules/minimizegains/README.md`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/minimizegains/TODO.md` & `fava_investor-0.7/fava_investor/modules/minimizegains/TODO.md`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/minimizegains/libminimizegains.py` & `fava_investor-0.7/fava_investor/modules/minimizegains/libminimizegains.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/minimizegains/minimizegains.py` & `fava_investor-0.7/fava_investor/modules/minimizegains/minimizegains.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/minimizegains/test_minimizegains.py` & `fava_investor-0.7/fava_investor/modules/minimizegains/test_minimizegains.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/summarizer/README.md` & `fava_investor-0.7/fava_investor/modules/summarizer/README.md`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/summarizer/example.beancount` & `fava_investor-0.7/fava_investor/modules/summarizer/example.beancount`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/summarizer/libsummarizer.py` & `fava_investor-0.7/fava_investor/modules/summarizer/libsummarizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import collections
 import re
 import fava_investor.common.libinvestor as libinvestor
 from beancount.core.data import Close
 from beancount.core import realization
 from beancount.core import convert
-from fava.core.conversion import convert_position
 from fava_investor.common.libinvestor import build_table_footer
 
 
 # TODO:
 # - print balances nicely, sort by them, show what percent is complete
 #   - for each commodity_leaf account, ensure there is a parent, else print
 
@@ -133,15 +132,15 @@
 
 
 def active_accounts_metadata(accapi, options):
     """Build metadata table for accounts that are open"""
 
     # balances = get_balances(accapi)
     realacc = accapi.realize()
-    pm = accapi.build_price_map()
+    pm = accapi.build_beancount_price_map()
     currency = accapi.get_operating_currencies()[0]
 
     p_acc_pattern = re.compile(options['acc_pattern'])
     meta_prefix = options.get('meta_prefix', '')
     specified_cols = options.get('columns', [])
     meta_skip = options.get('meta_skip', '')
     retval = []
@@ -164,15 +163,15 @@
     return retval
 
 
 def get_balance(realacc, account, pm, currency):
     subtree = realization.get(realacc, account)
     balance = realization.compute_balance(subtree)
     vbalance = balance.reduce(convert.get_units)
-    market_value = vbalance.reduce(convert_position, currency, pm)
+    market_value = vbalance.reduce(convert.convert_position, currency, pm)
     val = libinvestor.val(market_value)
     return val
     # return int(val)
 
 
 def get_balances(accapi):
     """Find all balances"""
```

### Comparing `fava_investor-0.6.0/fava_investor/modules/summarizer/summarizer.py` & `fava_investor-0.7/fava_investor/modules/summarizer/summarizer.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/tlh/README.md` & `fava_investor-0.7/fava_investor/modules/tlh/README.md`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/tlh/TODO.txt` & `fava_investor-0.7/fava_investor/modules/tlh/TODO.txt`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/tlh/example.beancount` & `fava_investor-0.7/fava_investor/modules/tlh/example.beancount`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/tlh/libtlh.py` & `fava_investor-0.7/fava_investor/modules/tlh/libtlh.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/tlh/test_libtlh.py` & `fava_investor-0.7/fava_investor/modules/tlh/test_libtlh.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/tlh/tlh.jpg` & `fava_investor-0.7/fava_investor/modules/tlh/tlh.jpg`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/tlh/tlh.py` & `fava_investor-0.7/fava_investor/modules/tlh/tlh.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/modules/tlh/wash_substantially_identical.beancount` & `fava_investor-0.7/fava_investor/modules/tlh/wash_substantially_identical.beancount`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/pythonanywhere/commodities.beancount` & `fava_investor-0.7/fava_investor/pythonanywhere/commodities.beancount`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/pythonanywhere/example.beancount` & `fava_investor-0.7/fava_investor/pythonanywhere/example.beancount`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/pythonanywhere/fava_config.beancount` & `fava_investor-0.7/fava_investor/pythonanywhere/fava_config.beancount`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/templates/Investor.html` & `fava_investor-0.7/fava_investor/templates/Investor.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 {% import "_query_table.html" as querytable with context %}
-{% set new_querytable = extension.use_new_querytable() %}
 
 {% set module = request.args.get('module') %}
 <div class="headerline">
   {% for key, label in [('aa_class', _('Asset Allocation Classes')),
                         ('aa_account', _('Asset Allocation Accounts')),
                         ('cashdrag', _('Cash Drag')),
                         ('tlh', _('Tax Loss Harvestor')),
@@ -26,19 +25,15 @@
 {% macro table_list_renderer(title, tables) -%}
 <h2>{{ title }}</h2>
 {% if tables|length == 0 %}
    Module not configured. See example.beancount for how to configure this module.
 {% endif %}
 {% for table in tables %}
   <h2>{{table[0]}}</h2>
-  {% if new_querytable %}
-    {{ querytable.querytable(ledger, None, *table[1]) }}
-  {% else %}
-    {{ querytable.querytable(None, *table[1]) }}
-  {% endif %}
+  {{ querytable.querytable(ledger, None, *table[1]) }}
 {% endfor %}
 {% endmacro %}
 <!-- -------------------------------------------------------------------------------- -->
 
 {% if (module == 'aa_account') %}
   {{ table_list_renderer('Portfolio: Asset Allocation by Accounts', extension.build_aa_by_account()) }}
 {% endif %}
@@ -80,63 +75,48 @@
           {% endfor %}
         </tbody>
       </table>
       <br />
     </div>
     <div class="column">
       <h3 style="text-align:left">Losses by Commodity</h3>
-      {% if new_querytable %}
-        {{ querytable.querytable(ledger, None, *harvests[3]) }}
-      {% else %}
-        {{ querytable.querytable(None, *harvests[3]) }}
-      {% endif %}
+      {{ querytable.querytable(ledger, None, *harvests[3]) }}
       <br />
     </div>
   </div>
 
 
   <h3>Candidates for tax loss harvesting</h3>
-  {% if new_querytable %}
-    {{ querytable.querytable(ledger, None, *harvests[0]) }}
-  {% else %}
-    {{ querytable.querytable(None, *harvests[0]) }}
-  {% endif %}
+  {{ querytable.querytable(ledger, None, *harvests[0]) }}
+
   <br />
 
 
   <h3>Potential wash sales: purchases within the past 30 days</h3>
 
   <i>Below is a list of purchases with the past 30 days. "earliest_sale" is the date on
     which a loss of the ticker shown can be harvested without resulting in a wash sale.</i>
 
   {% set table_empty_msg = None %}
   {% if harvests[2][0]|length == 0 %}
     {% set table_empty_msg = 'No purchases of the candidates above found within the last 30 days!' %}
   {% endif %}
-  {% if new_querytable %}
-    {{ querytable.querytable(ledger, table_empty_msg, *harvests[2]) }}
-  {% else %}
-    {{ querytable.querytable(table_empty_msg, *harvests[2]) }}
-  {% endif %}
+  {{ querytable.querytable(ledger, table_empty_msg, *harvests[2]) }}
   <br />
 
   <h3>What not to buy</h3>
   <i>Below is a list of recent sales with losses. Assuming these losses were harvested,
     purchasing these within 30 days of the sale could result in the loss becoming a wash
     sale.</i>
   {% set lossy_sales = extension.recently_sold_at_loss() %}
   {% set table_empty_msg = None %}
   {% if lossy_sales[1]|length == 0 %}
     {% set table_empty_msg = 'No sales with losses found in the last 30 days!' %}
   {% endif %}
-  {% if new_querytable %}
-    {{ querytable.querytable(ledger, table_empty_msg, *lossy_sales) }}
-  {% else %}
-    {{ querytable.querytable(table_empty_msg, *lossy_sales) }}
-  {% endif %}
+  {{ querytable.querytable(ledger, table_empty_msg, *lossy_sales) }}
 
   <br>
   <i>None of the above is meant to be financial, legal, tax, or other advice.</i>
 
 
 {% endif %}
 
@@ -198,30 +178,22 @@
     {% endif %}
   </li>
   {% endfor %}
 </ol>
 </tree-table>
 {% endmacro %}
 
-{% macro asset_allocation_hierarchy(serialised_tree, label='Asset Allocation') %}
-{% do chart_data.append({
-'type': 'hierarchy',
-'label': label,
-'data': {
-  'modifier': 1,
-  'root': serialised_tree,
-},
-}) %}
-{% endmacro %}
-
 {% if (module == 'aa_class') %}
   <h2>Portfolio: Asset Allocation by Class</h2>
 
-  {% set chart_data = [] %}
   {% set results = extension.build_assetalloc_by_class() %}
-
-  {{ asset_allocation_hierarchy(results[0].serialise(results[0]['currency']), label='Asset Allocation') }}
+  {% set chart_data = [{
+    'type': 'hierarchy',
+    'label': "Asset Allocation",
+    'data': results[0].serialise(results[0]['currency'])
+    }]
+  %}
   <svelte-component type="charts"><script type="application/json">{{ chart_data|tojson }}</script></svelte-component>
 
   {{ asset_tree(results[0]) }}
 
 {% endif %}
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
-{% import "_query_table.html" as querytable with context %} {% set
-new_querytable = extension.use_new_querytable() %} {% set module =
+{% import "_query_table.html" as querytable with context %} {% set module =
 request.args.get('module') %}
 {% for key, label in [('aa_class', _('Asset Allocation Classes')),
 ('aa_account', _('Asset Allocation Accounts')), ('cashdrag', _('Cash Drag')),
 ('tlh', _('Tax Loss Harvestor')), ('summarizer', _('Summarizer')),
 ('minimizegains', _('Gains Minimizer')) ] %}
 ******** {{%% iiff nnoott ((mmoodduullee ==== kkeeyy)) %%}}_{{_{{_ _ll_aa_bb_ee_ll_ _}}_}}{{%% eellssee %%}} {{{{ llaabbeell }}}}{{%% eennddiiff %%}}
 ********
@@ -12,52 +11,46 @@
 and tools for investments. It implemented as a collection of modules. Use the
 tabs on the top to navigate to each module. {% endif %} {% macro
 table_list_renderer(title, tables) -%}
 ********** {{{{ ttiittllee }}}} **********
 {% if tables|length == 0 %} Module not configured. See example.beancount for
 how to configure this module. {% endif %} {% for table in tables %}
 ********** {{{{ttaabbllee[[00]]}}}} **********
-{% if new_querytable %} {{ querytable.querytable(ledger, None, *table[1]) }} {%
-else %} {{ querytable.querytable(None, *table[1]) }} {% endif %} {% endfor %}
-{% endmacro %} {% if (module == 'aa_account') %} {{ table_list_renderer
-('Portfolio: Asset Allocation by Accounts', extension.build_aa_by_account()) }}
-{% endif %} {% if (module == 'cashdrag') %} {{ table_list_renderer('',
-extension.build_cashdrag()) }} {% endif %} {% if (module == 'summarizer') %} {
-{ table_list_renderer('', extension.build_summarizer()) }} {% endif %} {% if
-(module == 'minimizegains') %} {{ table_list_renderer('',
-extension.build_minimizegains()) }} {% endif %} {% if (module == 'tlh') %}
+{{ querytable.querytable(ledger, None, *table[1]) }} {% endfor %} {% endmacro
+%} {% if (module == 'aa_account') %} {{ table_list_renderer('Portfolio: Asset
+Allocation by Accounts', extension.build_aa_by_account()) }} {% endif %} {% if
+(module == 'cashdrag') %} {{ table_list_renderer('', extension.build_cashdrag
+()) }} {% endif %} {% if (module == 'summarizer') %} {{ table_list_renderer('',
+extension.build_summarizer()) }} {% endif %} {% if (module == 'minimizegains')
+%} {{ table_list_renderer('', extension.build_minimizegains()) }} {% endif %}
+{% if (module == 'tlh') %}
 ********** TTaaxx LLoossss HHaarrvveesstteerr **********
 {% set harvests = extension.build_tlh_tables() %}
 ******** SSuummmmaarryy ********
 {{{{?Â? __((''SSuummmmaarryy'')) }}}} {{{{?Â? __((''VVaall'')) }}}}
 {{Â key }}             {{Â value }}
 
 ******** LLoosssseess bbyy CCoommmmooddiittyy ********
-{% if new_querytable %} {{ querytable.querytable(ledger, None, *harvests[3]) }}
-{% else %} {{ querytable.querytable(None, *harvests[3]) }} {% endif %}
+{{ querytable.querytable(ledger, None, *harvests[3]) }}
 ******** CCaannddiiddaatteess ffoorr ttaaxx lloossss hhaarrvveessttiinngg ********
-{% if new_querytable %} {{ querytable.querytable(ledger, None, *harvests[0]) }}
-{% else %} {{ querytable.querytable(None, *harvests[0]) }} {% endif %}
+{{ querytable.querytable(ledger, None, *harvests[0]) }}
 ******** PPootteennttiiaall wwaasshh ssaalleess:: ppuurrcchhaasseess wwiitthhiinn tthhee ppaasstt 3300 ddaayyss ********
 Below is a list of purchases with the past 30 days. "earliest_sale" is the date
 on which a loss of the ticker shown can be harvested without resulting in a
 wash sale. {% set table_empty_msg = None %} {% if harvests[2][0]|length == 0 %}
 {% set table_empty_msg = 'No purchases of the candidates above found within the
-last 30 days!' %} {% endif %} {% if new_querytable %} {{ querytable.querytable
-(ledger, table_empty_msg, *harvests[2]) }} {% else %} {{ querytable.querytable
-(table_empty_msg, *harvests[2]) }} {% endif %}
+last 30 days!' %} {% endif %} {{ querytable.querytable(ledger, table_empty_msg,
+*harvests[2]) }}
 ******** WWhhaatt nnoott ttoo bbuuyy ********
 Below is a list of recent sales with losses. Assuming these losses were
 harvested, purchasing these within 30 days of the sale could result in the loss
 becoming a wash sale. {% set lossy_sales = extension.recently_sold_at_loss() %}
 {% set table_empty_msg = None %} {% if lossy_sales[1]|length == 0 %} {% set
 table_empty_msg = 'No sales with losses found in the last 30 days!' %} {% endif
-%} {% if new_querytable %} {{ querytable.querytable(ledger, table_empty_msg,
-*lossy_sales) }} {% else %} {{ querytable.querytable(table_empty_msg,
-*lossy_sales) }} {% endif %}
+%} {{ querytable.querytable(ledger, table_empty_msg, *lossy_sales) }}
 None of the above is meant to be financial, legal, tax, or other advice. {%
 endif %} {% set table_hover_text = _('Hold Shift while clicking to expand all
 children. Hold Ctrl or Cmd while clicking to expand one level.') %} {# TODO: -
 add a format_percentage() to fava's template_filters, and use that here -
 display 0 decimal places for assets (needed for all of fava_investor) - fix:
 asset bucket spacing is too wide - get currency from libassetalloc instead of
 looping: {% for currency in ledger.options.operating_currency %} - remove links
@@ -77,16 +70,13 @@
       '' %} {{ '{:6.2f} %'.format(account.percentage) if account.percentage
       else '' }} {{ '{:6.2f} %'.format(account.percentage_children) if
       account.percentage_children else '' }}
    5. {% if account.children %}
          1. {{ loop(account.children|sort(attribute='name')) }}
    6. {% endif %}
    7. {% endfor %}
-{% endmacro %} {% macro asset_allocation_hierarchy(serialised_tree,
-label='Asset Allocation') %} {% do chart_data.append({ 'type': 'hierarchy',
-'label': label, 'data': { 'modifier': 1, 'root': serialised_tree, }, }) %} {%
-endmacro %} {% if (module == 'aa_class') %}
+{% endmacro %} {% if (module == 'aa_class') %}
 ********** PPoorrttffoolliioo:: AAsssseett AAllllooccaattiioonn bbyy CCllaassss **********
-{% set chart_data = [] %} {% set results = extension.build_assetalloc_by_class
-() %} {{ asset_allocation_hierarchy(results[0].serialise(results[0]
-['currency']), label='Asset Allocation') }}
+{% set results = extension.build_assetalloc_by_class() %} {% set chart_data = [
+{ 'type': 'hierarchy', 'label': "Asset Allocation", 'data': results
+[0].serialise(results[0]['currency']) }] %}
 {{ asset_tree(results[0]) }} {% endif %}
```

### Comparing `fava_investor-0.6.0/fava_investor/util/cachedtickerinfo.py` & `fava_investor-0.7/fava_investor/util/cachedtickerinfo.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/util/experimental/scaled_navs.py` & `fava_investor-0.7/fava_investor/util/experimental/scaled_navs.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/util/relatetickers.py` & `fava_investor-0.7/fava_investor/util/relatetickers.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/util/test_relatetickers.py` & `fava_investor-0.7/fava_investor/util/test_relatetickers.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor/util/ticker_util.py` & `fava_investor-0.7/fava_investor/util/ticker_util.py`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/fava_investor.egg-info/PKG-INFO` & `fava_investor-0.7/fava_investor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fava_investor
-Version: 0.6.0
+Version: 0.7.0
 Summary: Fava extension and beancount libraries for investing
 Home-page: https://github.com/redstreet/fava_investor
 Author: Red S
 Author-email: redstreet@users.noreply.github.com
 License: GPL-3.0
 Keywords: fava beancount accounting investment
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: Click>=7.0
 Requires-Dist: beancount>=2.3.2
 Requires-Dist: click_aliases>=1.0.1
-Requires-Dist: fava>=1.23
+Requires-Dist: fava>=1.26
 Requires-Dist: packaging>=20.3
 Requires-Dist: python_dateutil>=2.8.1
 Requires-Dist: tabulate>=0.8.9
 Requires-Dist: yfinance>=0.1.70
 
 # Fava Investor
```

### Comparing `fava_investor-0.6.0/fava_investor.egg-info/SOURCES.txt` & `fava_investor-0.7/fava_investor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/requirements.txt` & `fava_investor-0.7/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 # fava_investor/build/lib/fava_investor/__init__.py: 3,4
 # fava_investor/build/lib/fava_investor/common/beancountinvestorapi.py: 29
 # fava_investor/build/lib/fava_investor/common/favainvestorapi.py: 2,3
 # fava_investor/fava_investor/__init__.py: 3,4
 # fava_investor/fava_investor/common/beancountinvestorapi.py: 29
 # fava_investor/fava_investor/common/favainvestorapi.py: 2,3
-fava>=1.25
+fava>=1.27
 
 # fava_investor/.eggs/setuptools_scm-7.0.4-py3.8.egg/setuptools_scm/_entrypoints.py: 77
 importlib_metadata >= 1.5.0
 
 # fava_investor/.eggs/setuptools_scm-7.0.4-py3.8.egg/setuptools_scm/_version_cls.py: 5,6
 # fava_investor/build/lib/fava_investor/common/favainvestorapi.py: 4
 # fava_investor/fava_investor/common/favainvestorapi.py: 4
```

### Comparing `fava_investor-0.6.0/screenshot-assetalloc.png` & `fava_investor-0.7/screenshot-assetalloc.png`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/screenshot.png` & `fava_investor-0.7/screenshot.png`

 * *Files identical despite different names*

### Comparing `fava_investor-0.6.0/setup.py` & `fava_investor-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     keywords='fava beancount accounting investment',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'Click >= 7.0',
         'beancount >= 2.3.2',
         'click_aliases >= 1.0.1',
-        'fava >= 1.23',
+        'fava >= 1.26',
         'packaging >= 20.3',
         'python_dateutil >= 2.8.1',
         'tabulate >= 0.8.9',
         'yfinance >= 0.1.70',
     ],
     entry_points={
         'console_scripts': [
```

