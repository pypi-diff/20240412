# Comparing `tmp/stginga-1.5.0.tar.gz` & `tmp/stginga-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stginga-1.5.0.tar", last modified: Thu Mar 21 15:31:12 2024, max compression
+gzip compressed data, was "stginga-1.5.1.tar", last modified: Fri Apr 12 02:08:33 2024, max compression
```

## Comparing `stginga-1.5.0.tar` & `stginga-1.5.1.tar`

### file list

```diff
@@ -1,121 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.625707 stginga-1.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.605706 stginga-1.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.605706 stginga-1.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-03-21 15:30:58.000000 stginga-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-21 15:30:58.000000 stginga-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-03-21 15:30:58.000000 stginga-1.5.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-21 15:30:58.000000 stginga-1.5.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-21 15:30:58.000000 stginga-1.5.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-21 15:30:58.000000 stginga-1.5.0/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.605706 stginga-1.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-03-21 15:30:58.000000 stginga-1.5.0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-03-21 15:30:58.000000 stginga-1.5.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-21 15:30:58.000000 stginga-1.5.0/.github/workflows/open_actions.yml
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-21 15:30:58.000000 stginga-1.5.0/.github/workflows/predeps_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-21 15:30:58.000000 stginga-1.5.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-21 15:30:58.000000 stginga-1.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-21 15:30:58.000000 stginga-1.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-03-21 15:30:58.000000 stginga-1.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-21 15:30:58.000000 stginga-1.5.0/CITATION
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-03-21 15:30:58.000000 stginga-1.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-03-21 15:30:58.000000 stginga-1.5.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-21 15:30:58.000000 stginga-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-21 15:31:12.625707 stginga-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-21 15:30:58.000000 stginga-1.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-21 15:30:58.000000 stginga-1.5.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.605706 stginga-1.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.605706 stginga-1.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    19012 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/_static/stsci_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.605706 stginga-1.5.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/_templates/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.605706 stginga-1.5.0/docs/stginga/
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.609706 stginga-1.5.0/docs/stginga/plugins_manual/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/backgroundsub.rst
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/badpixcorr.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/dqinspect.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.613706 stginga-1.5.0/docs/stginga/plugins_manual/images/
--rw-r--r--   0 runner    (1001) docker     (127)   219289 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/images/backgroundsub_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)   111640 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/images/badpixcorr_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)   270366 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/images/dqinspect_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)   723120 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/images/mipick_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)   100428 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/images/mosaicauto_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)  1831524 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/images/multiimage_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)   111413 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/images/smoothing_after.png
--rw-r--r--   0 runner    (1001) docker     (127)   418997 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/images/smoothing_before.png
--rw-r--r--   0 runner    (1001) docker     (127)   104596 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/images/snrcalc_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/mipick.rst
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/mosaicauto.rst
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/multiimage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/smoothing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/plugins_manual/snrcalc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/ref_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-21 15:30:58.000000 stginga-1.5.0/docs/stginga/run.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.617706 stginga-1.5.0/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-21 15:30:58.000000 stginga-1.5.0/experimental/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.617706 stginga-1.5.0/experimental/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-21 15:30:58.000000 stginga-1.5.0/experimental/configs/plugin_Smoothing.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-03-21 15:30:58.000000 stginga-1.5.0/experimental/ginga_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.617706 stginga-1.5.0/experimental/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-03-21 15:30:58.000000 stginga-1.5.0/experimental/notebooks/astrowidgets_asdf_in_fits.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.617706 stginga-1.5.0/experimental/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-03-21 15:30:58.000000 stginga-1.5.0/experimental/plugins/MIPick.py
--rw-r--r--   0 runner    (1001) docker     (127)    16236 2024-03-21 15:30:58.000000 stginga-1.5.0/experimental/plugins/MultiImage.py
--rw-r--r--   0 runner    (1001) docker     (127)    11085 2024-03-21 15:30:58.000000 stginga-1.5.0/experimental/plugins/Smoothing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.617706 stginga-1.5.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-21 15:30:58.000000 stginga-1.5.0/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-21 15:30:58.000000 stginga-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-21 15:31:12.625707 stginga-1.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1067 2024-03-21 15:30:58.000000 stginga-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.617706 stginga-1.5.0/stginga/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/_astropy_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.621707 stginga-1.5.0/stginga/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/data/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/data/dqflags_acs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/data/dqflags_hstgen.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/data/dqflags_jwst.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/data/dqflags_wfc3.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.601706 stginga-1.5.0/stginga/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.621707 stginga-1.5.0/stginga/examples/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/examples/configs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/examples/configs/channel_Image.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/examples/configs/general.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/examples/configs/ginga_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/examples/configs/plugin_BackgroundSub.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/examples/configs/plugin_BadPixCorr.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/examples/configs/plugin_Contents.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/examples/configs/plugin_DQInspect.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/examples/configs/plugin_Mosaic.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/examples/configs/plugin_SNRCalc.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/examples/configs/plugin_Thumbs.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/gingawrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/plugin_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.621707 stginga-1.5.0/stginga/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)    29891 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/plugins/BackgroundSub.py
--rw-r--r--   0 runner    (1001) docker     (127)    36421 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/plugins/BadPixCorr.py
--rw-r--r--   0 runner    (1001) docker     (127)    24567 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/plugins/DQInspect.py
--rw-r--r--   0 runner    (1001) docker     (127)    19247 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/plugins/MosaicAuto.py
--rw-r--r--   0 runner    (1001) docker     (127)    40058 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/plugins/SNRCalc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/plugins/local_plugin_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.625707 stginga-1.5.0/stginga/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-03-21 15:30:58.000000 stginga-1.5.0/stginga/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-21 15:31:12.000000 stginga-1.5.0/stginga/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:31:12.625707 stginga-1.5.0/stginga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-21 15:31:12.000000 stginga-1.5.0/stginga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-03-21 15:31:12.000000 stginga-1.5.0/stginga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 15:31:12.000000 stginga-1.5.0/stginga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-21 15:31:12.000000 stginga-1.5.0/stginga.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 15:31:12.000000 stginga-1.5.0/stginga.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-21 15:31:12.000000 stginga-1.5.0/stginga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-21 15:31:12.000000 stginga-1.5.0/stginga.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.960585 stginga-1.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.944585 stginga-1.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.944585 stginga-1.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-12 02:08:25.000000 stginga-1.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-12 02:08:25.000000 stginga-1.5.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-12 02:08:25.000000 stginga-1.5.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-12 02:08:25.000000 stginga-1.5.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-12 02:08:25.000000 stginga-1.5.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-12 02:08:25.000000 stginga-1.5.1/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.944585 stginga-1.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-12 02:08:25.000000 stginga-1.5.1/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-12 02:08:25.000000 stginga-1.5.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-12 02:08:25.000000 stginga-1.5.1/.github/workflows/open_actions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-12 02:08:25.000000 stginga-1.5.1/.github/workflows/predeps_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-12 02:08:25.000000 stginga-1.5.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-12 02:08:25.000000 stginga-1.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-12 02:08:25.000000 stginga-1.5.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-12 02:08:25.000000 stginga-1.5.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-12 02:08:25.000000 stginga-1.5.1/CITATION
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-12 02:08:25.000000 stginga-1.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-12 02:08:25.000000 stginga-1.5.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-12 02:08:25.000000 stginga-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-12 02:08:33.960585 stginga-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-12 02:08:25.000000 stginga-1.5.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-12 02:08:25.000000 stginga-1.5.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.944585 stginga-1.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.944585 stginga-1.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    19012 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/_static/stsci_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.944585 stginga-1.5.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/_templates/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.944585 stginga-1.5.1/docs/stginga/
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.948585 stginga-1.5.1/docs/stginga/plugins_manual/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/backgroundsub.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/badpixcorr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/dqinspect.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.952585 stginga-1.5.1/docs/stginga/plugins_manual/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   219289 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/images/backgroundsub_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)   111640 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/images/badpixcorr_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)   270366 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/images/dqinspect_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)   723120 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/images/mipick_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)   100428 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/images/mosaicauto_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1831524 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/images/multiimage_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)   111413 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/images/smoothing_after.png
+-rw-r--r--   0 runner    (1001) docker     (127)   418997 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/images/smoothing_before.png
+-rw-r--r--   0 runner    (1001) docker     (127)   104596 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/images/snrcalc_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/mipick.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/mosaicauto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/multiimage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/smoothing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/plugins_manual/snrcalc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/ref_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-12 02:08:25.000000 stginga-1.5.1/docs/stginga/run.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.952585 stginga-1.5.1/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-12 02:08:25.000000 stginga-1.5.1/experimental/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.952585 stginga-1.5.1/experimental/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 02:08:25.000000 stginga-1.5.1/experimental/configs/plugin_Smoothing.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-12 02:08:25.000000 stginga-1.5.1/experimental/ginga_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.952585 stginga-1.5.1/experimental/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-12 02:08:25.000000 stginga-1.5.1/experimental/notebooks/astrowidgets_asdf_in_fits.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.956585 stginga-1.5.1/experimental/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-12 02:08:25.000000 stginga-1.5.1/experimental/plugins/MIPick.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16236 2024-04-12 02:08:25.000000 stginga-1.5.1/experimental/plugins/MultiImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11085 2024-04-12 02:08:25.000000 stginga-1.5.1/experimental/plugins/Smoothing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.956585 stginga-1.5.1/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-12 02:08:25.000000 stginga-1.5.1/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 02:08:25.000000 stginga-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-12 02:08:33.960585 stginga-1.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1067 2024-04-12 02:08:25.000000 stginga-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.956585 stginga-1.5.1/stginga/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/_astropy_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.956585 stginga-1.5.1/stginga/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/data/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/data/dqflags_acs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/data/dqflags_hstgen.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/data/dqflags_jwst.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/data/dqflags_wfc3.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.940585 stginga-1.5.1/stginga/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.960585 stginga-1.5.1/stginga/examples/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/examples/configs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/examples/configs/channel_Image.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/examples/configs/general.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/examples/configs/ginga_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/examples/configs/plugin_BackgroundSub.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/examples/configs/plugin_BadPixCorr.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/examples/configs/plugin_Contents.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/examples/configs/plugin_DQInspect.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/examples/configs/plugin_Mosaic.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/examples/configs/plugin_SNRCalc.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/examples/configs/plugin_Thumbs.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/gingawrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/plugin_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.960585 stginga-1.5.1/stginga/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)    29891 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/plugins/BackgroundSub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36421 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/plugins/BadPixCorr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24567 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/plugins/DQInspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19247 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/plugins/MosaicAuto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40058 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/plugins/SNRCalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/plugins/local_plugin_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.960585 stginga-1.5.1/stginga/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-04-12 02:08:25.000000 stginga-1.5.1/stginga/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:08:33.960585 stginga-1.5.1/stginga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-12 02:08:33.000000 stginga-1.5.1/stginga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-12 02:08:33.000000 stginga-1.5.1/stginga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 02:08:33.000000 stginga-1.5.1/stginga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-12 02:08:33.000000 stginga-1.5.1/stginga.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 02:08:33.000000 stginga-1.5.1/stginga.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-12 02:08:33.000000 stginga-1.5.1/stginga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 02:08:33.000000 stginga-1.5.1/stginga.egg-info/top_level.txt
```

### Comparing `stginga-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `stginga-1.5.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `stginga-1.5.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/.github/ISSUE_TEMPLATE/question.md` & `stginga-1.5.1/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/.github/PULL_REQUEST_TEMPLATE.md` & `stginga-1.5.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/.github/dependabot.yml` & `stginga-1.5.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/.github/labeler.yml` & `stginga-1.5.1/.github/labeler.yml`

 * *Files 1% similar despite different names*

```diff
@@ -57,8 +57,10 @@
 
 SNRCalc:
 - changed-files:
   - any-glob-to-any-file:
     - stginga/plugins/SNRCalc.py
 
 utils:
-  - stginga/utils.py
+- changed-files:
+  - any-glob-to-any-file:
+    - stginga/utils.py
```

### Comparing `stginga-1.5.0/.github/workflows/ci_workflows.yml` & `stginga-1.5.1/.github/workflows/ci_workflows.yml`

 * *Files 7% similar despite different names*

```diff
@@ -90,16 +90,18 @@
         fetch-depth: 0
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Install and build
       run: |
-        python -m pip install --upgrade pip setuptools wheel
-        python -m pip install -U numpy pyerfa astropy-iers-data PyYAML packaging
+        python -m pip install -U pip setuptools wheel
+        python -m pip install -U -i https://pypi.anaconda.org/scientific-python-nightly-wheels/simple numpy --pre
+        python -m pip install -U astropy-iers-data PyYAML packaging
+        python -m pip install -U -i https://pypi.anaconda.org/liberfa/simple pyerfa --pre
         python -m pip install -U -i https://pypi.anaconda.org/astropy/simple astropy --pre
         python -m pip install git+https://github.com/ejeschke/ginga.git@main#egg=ginga
         python -m pip install -e .[test]
     - name: Test with dev deps
       run: pytest
 
   link_check:
```

### Comparing `stginga-1.5.0/.github/workflows/codeql-analysis.yml` & `stginga-1.5.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/.github/workflows/open_actions.yml` & `stginga-1.5.1/.github/workflows/open_actions.yml`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/.github/workflows/predeps_workflow.yml` & `stginga-1.5.1/.github/workflows/predeps_workflow.yml`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/.github/workflows/publish-to-pypi.yml` & `stginga-1.5.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/.gitignore` & `stginga-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/CHANGES.rst` & `stginga-1.5.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+1.5.1 (2024-04-11)
+------------------
+
+- Compatibility with NumPy 2.0. [#238]
+
 1.5 (2024-03-21)
 ----------------
 
 Other Changes and Additions
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 - Compatibility with Ginga 5. [#234]
```

### Comparing `stginga-1.5.0/CITATION` & `stginga-1.5.1/CITATION`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/CODE_OF_CONDUCT.md` & `stginga-1.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/LICENSE.rst` & `stginga-1.5.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/PKG-INFO` & `stginga-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stginga
-Version: 1.5.0
+Version: 1.5.1
 Summary: Ginga products specific to STScI data analysis
 Home-page: https://github.com/spacetelescope/stginga
 Author: STScI
 Author-email: help@stsci.edu
 License: BSD
 Keywords: astronomy,astrophysics,image,visualization,HST,JWST
 Classifier: Intended Audience :: Science/Research
```

### Comparing `stginga-1.5.0/README.rst` & `stginga-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/conftest.py` & `stginga-1.5.1/conftest.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/Makefile` & `stginga-1.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/_static/stsci_logo.png` & `stginga-1.5.1/docs/_static/stsci_logo.png`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/conf.py` & `stginga-1.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/index.rst` & `stginga-1.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/make.bat` & `stginga-1.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/config.rst` & `stginga-1.5.1/docs/stginga/config.rst`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/install.rst` & `stginga-1.5.1/docs/stginga/install.rst`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/plugins_manual/images/backgroundsub_screenshot.png` & `stginga-1.5.1/docs/stginga/plugins_manual/images/backgroundsub_screenshot.png`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/plugins_manual/images/badpixcorr_screenshot.png` & `stginga-1.5.1/docs/stginga/plugins_manual/images/badpixcorr_screenshot.png`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/plugins_manual/images/dqinspect_screenshot.png` & `stginga-1.5.1/docs/stginga/plugins_manual/images/dqinspect_screenshot.png`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/plugins_manual/images/mipick_screenshot.png` & `stginga-1.5.1/docs/stginga/plugins_manual/images/mipick_screenshot.png`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/plugins_manual/images/mosaicauto_screenshot.png` & `stginga-1.5.1/docs/stginga/plugins_manual/images/mosaicauto_screenshot.png`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/plugins_manual/images/multiimage_screenshot.png` & `stginga-1.5.1/docs/stginga/plugins_manual/images/multiimage_screenshot.png`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/plugins_manual/images/smoothing_after.png` & `stginga-1.5.1/docs/stginga/plugins_manual/images/smoothing_after.png`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/plugins_manual/images/smoothing_before.png` & `stginga-1.5.1/docs/stginga/plugins_manual/images/smoothing_before.png`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/plugins_manual/images/snrcalc_screenshot.png` & `stginga-1.5.1/docs/stginga/plugins_manual/images/snrcalc_screenshot.png`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/plugins_manual/index.rst` & `stginga-1.5.1/docs/stginga/plugins_manual/index.rst`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/plugins_manual/mipick.rst` & `stginga-1.5.1/docs/stginga/plugins_manual/mipick.rst`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/plugins_manual/multiimage.rst` & `stginga-1.5.1/docs/stginga/plugins_manual/multiimage.rst`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/plugins_manual/smoothing.rst` & `stginga-1.5.1/docs/stginga/plugins_manual/smoothing.rst`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/docs/stginga/run.rst` & `stginga-1.5.1/docs/stginga/run.rst`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/experimental/README.rst` & `stginga-1.5.1/experimental/README.rst`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/experimental/ginga_config.py` & `stginga-1.5.1/experimental/ginga_config.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/experimental/notebooks/astrowidgets_asdf_in_fits.ipynb` & `stginga-1.5.1/experimental/notebooks/astrowidgets_asdf_in_fits.ipynb`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/experimental/plugins/MIPick.py` & `stginga-1.5.1/experimental/plugins/MIPick.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/experimental/plugins/MultiImage.py` & `stginga-1.5.1/experimental/plugins/MultiImage.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/experimental/plugins/Smoothing.py` & `stginga-1.5.1/experimental/plugins/Smoothing.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/setup.cfg` & `stginga-1.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/setup.py` & `stginga-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/data/dqflags_acs.txt` & `stginga-1.5.1/stginga/data/dqflags_acs.txt`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/data/dqflags_hstgen.txt` & `stginga-1.5.1/stginga/data/dqflags_hstgen.txt`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/data/dqflags_jwst.txt` & `stginga-1.5.1/stginga/data/dqflags_jwst.txt`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/data/dqflags_wfc3.txt` & `stginga-1.5.1/stginga/data/dqflags_wfc3.txt`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/examples/configs/general.cfg` & `stginga-1.5.1/stginga/examples/configs/general.cfg`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/examples/configs/ginga_config.py` & `stginga-1.5.1/stginga/examples/configs/ginga_config.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/examples/configs/plugin_BackgroundSub.cfg` & `stginga-1.5.1/stginga/examples/configs/plugin_BackgroundSub.cfg`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/examples/configs/plugin_BadPixCorr.cfg` & `stginga-1.5.1/stginga/examples/configs/plugin_BadPixCorr.cfg`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/examples/configs/plugin_DQInspect.cfg` & `stginga-1.5.1/stginga/examples/configs/plugin_DQInspect.cfg`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/examples/configs/plugin_Mosaic.cfg` & `stginga-1.5.1/stginga/examples/configs/plugin_Mosaic.cfg`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/examples/configs/plugin_SNRCalc.cfg` & `stginga-1.5.1/stginga/examples/configs/plugin_SNRCalc.cfg`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/gingawrapper.py` & `stginga-1.5.1/stginga/gingawrapper.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/plugin_info.py` & `stginga-1.5.1/stginga/plugin_info.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/plugins/BackgroundSub.py` & `stginga-1.5.1/stginga/plugins/BackgroundSub.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/plugins/BadPixCorr.py` & `stginga-1.5.1/stginga/plugins/BadPixCorr.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/plugins/DQInspect.py` & `stginga-1.5.1/stginga/plugins/DQInspect.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/plugins/MosaicAuto.py` & `stginga-1.5.1/stginga/plugins/MosaicAuto.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/plugins/SNRCalc.py` & `stginga-1.5.1/stginga/plugins/SNRCalc.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/plugins/local_plugin_mixin.py` & `stginga-1.5.1/stginga/plugins/local_plugin_mixin.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/tests/test_utils.py` & `stginga-1.5.1/stginga/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `stginga-1.5.0/stginga/utils.py` & `stginga-1.5.1/stginga/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         Returns
         -------
         dqs_by_flag : dict
             Dictionary mapping each interpreted DQ value to indices
             of affected array elements.
 
         """
-        data = np.asarray(data, dtype=int)  # Ensure int array
+        data = np.asarray(data, dtype=np.uint)  # Ensure uint array
         dqs_by_flag = {}
 
         def _one_flag(vf):
             dqs_by_flag[vf] = np.where((data & vf) != 0)
 
         # Skip good flag
         list(map(_one_flag, self._valid_flags[1:]))
```

### Comparing `stginga-1.5.0/stginga.egg-info/PKG-INFO` & `stginga-1.5.1/stginga.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stginga
-Version: 1.5.0
+Version: 1.5.1
 Summary: Ginga products specific to STScI data analysis
 Home-page: https://github.com/spacetelescope/stginga
 Author: STScI
 Author-email: help@stsci.edu
 License: BSD
 Keywords: astronomy,astrophysics,image,visualization,HST,JWST
 Classifier: Intended Audience :: Science/Research
```

### Comparing `stginga-1.5.0/stginga.egg-info/SOURCES.txt` & `stginga-1.5.1/stginga.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 experimental/plugins/Smoothing.py
 licenses/README.rst
 stginga/__init__.py
 stginga/_astropy_init.py
 stginga/gingawrapper.py
 stginga/plugin_info.py
 stginga/utils.py
-stginga/version.py
 stginga.egg-info/PKG-INFO
 stginga.egg-info/SOURCES.txt
 stginga.egg-info/dependency_links.txt
 stginga.egg-info/entry_points.txt
 stginga.egg-info/not-zip-safe
 stginga.egg-info/requires.txt
 stginga.egg-info/top_level.txt
```

