# Comparing `tmp/quantify-core-0.7.4.tar.gz` & `tmp/quantify-core-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantify-core-0.7.4.tar", last modified: Fri Dec 15 16:23:50 2023, max compression
+gzip compressed data, was "quantify-core-0.7.5.tar", last modified: Fri Apr 12 08:57:01 2024, max compression
```

## Comparing `quantify-core-0.7.4.tar` & `quantify-core-0.7.5.tar`

### file list

```diff
@@ -1,278 +1,320 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.555151 quantify-core-0.7.4/
--rw-rw-rw-   0 root         (0) root         (0)     1834 2023-12-15 16:23:37.000000 quantify-core-0.7.4/AUTHORS.md
--rw-rw-rw-   0 root         (0) root         (0)    26415 2023-12-15 16:23:37.000000 quantify-core-0.7.4/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    14826 2023-12-15 16:23:37.000000 quantify-core-0.7.4/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-12-15 16:23:37.000000 quantify-core-0.7.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-12-15 16:23:37.000000 quantify-core-0.7.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6385 2023-12-15 16:23:50.555151 quantify-core-0.7.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3217 2023-12-15 16:23:37.000000 quantify-core-0.7.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.499152 quantify-core-0.7.4/docs/
--rw-rw-rw-   0 root         (0) root         (0)      788 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     1162 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.499152 quantify-core-0.7.4/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.501152 quantify-core-0.7.4/docs/source/api/
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/api/analysis.md
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/api/data.md
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/api/index.md
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/api/measurement.md
--rw-rw-rw-   0 root         (0) root         (0)      473 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/api/utilities.md
--rw-rw-rw-   0 root         (0) root         (0)      794 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/api/visualization.md
--rwxrwxrwx   0 root         (0) root         (0)    14228 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.501152 quantify-core-0.7.4/docs/source/dev/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.501152 quantify-core-0.7.4/docs/source/dev/design/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.502152 quantify-core-0.7.4/docs/source/dev/design/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      543 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/dev/design/dataset/index.md
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/dev/design/index.md
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/dev/guide.md
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/dev/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.502152 quantify-core-0.7.4/docs/source/howto/
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/howto/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.502152 quantify-core-0.7.4/docs/source/images/
--rw-rw-rw-   0 root         (0) root         (0)     2254 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/images/QUANTIFY-FAVICON_16.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.506152 quantify-core-0.7.4/docs/source/images/install/
--rw-rw-rw-   0 root         (0) root         (0)  2452484 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/images/install/conda_activate.gif
--rw-rw-rw-   0 root         (0) root         (0)   858347 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/images/install/conda_install.gif
--rw-rw-rw-   0 root         (0) root         (0)  1669689 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/images/install/conda_source_installed_all_users.gif
--rw-rw-rw-   0 root         (0) root         (0)    27025 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/images/surface-7-sched.png
--rw-rw-rw-   0 root         (0) root         (0)     1850 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.507152 quantify-core-0.7.4/docs/source/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/tutorials/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.509152 quantify-core-0.7.4/docs/source/user/
--rw-rw-rw-   0 root         (0) root         (0)     1851 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/user/about.md
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/user/authors.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/user/bibliography.md
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/user/changelog.md
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/user/index.md
--rw-rw-rw-   0 root         (0) root         (0)    13399 2023-12-15 16:23:37.000000 quantify-core-0.7.4/docs/source/user/installation.md
--rw-rw-rw-   0 root         (0) root         (0)    17794 2023-12-15 16:23:37.000000 quantify-core-0.7.4/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.556151 quantify-core-0.7.4/quantify_core/
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)       60 2023-12-15 16:23:50.556151 quantify-core-0.7.4/quantify_core/_static_version.py
--rw-rw-rw-   0 root         (0) root         (0)     5795 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.515152 quantify-core-0.7.4/quantify_core/analysis/
--rw-rw-rw-   0 root         (0) root         (0)      693 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/analysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    35475 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/analysis/base_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5079 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/analysis/calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     3413 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/analysis/cosine_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    22433 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/analysis/fitting_models.py
--rw-rw-rw-   0 root         (0) root         (0)     2573 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/analysis/interpolation_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     4339 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/analysis/optimization_analysis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.515152 quantify-core-0.7.4/quantify_core/analysis/schemas/
--rw-rw-rw-   0 root         (0) root         (0)     1152 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/analysis/schemas/AnalysisSettings.json
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/analysis/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26708 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/analysis/single_qubit_timedomain.py
--rw-rw-rw-   0 root         (0) root         (0)    10613 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/analysis/spectroscopy_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5762 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/analysis/time_of_flight_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/analysis/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.517152 quantify-core-0.7.4/quantify_core/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5853 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/data/dataset_adapters.py
--rw-rw-rw-   0 root         (0) root         (0)    12630 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/data/dataset_attrs.py
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/data/experiment.py
--rw-rw-rw-   0 root         (0) root         (0)    45558 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/data/handling.py
--rw-rw-rw-   0 root         (0) root         (0)     2961 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/data/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.518152 quantify-core-0.7.4/quantify_core/measurement/
--rw-rw-rw-   0 root         (0) root         (0)      725 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/measurement/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39295 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/measurement/control.py
--rw-rw-rw-   0 root         (0) root         (0)      946 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/measurement/gettables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.519152 quantify-core-0.7.4/quantify_core/measurement/schemas/
--rw-rw-rw-   0 root         (0) root         (0)     2516 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/measurement/schemas/Gettable.json
--rw-rw-rw-   0 root         (0) root         (0)     1646 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/measurement/schemas/Settable.json
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/measurement/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3133 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/measurement/types.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.521152 quantify-core-0.7.4/quantify_core/utilities/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1849 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/utilities/_docs_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1209 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/utilities/_tests_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    19538 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/utilities/dataset_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     5005 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/utilities/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)    11085 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/utilities/examples_support.py
--rw-rw-rw-   0 root         (0) root         (0)     9674 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/utilities/experiment_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     5882 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/utilities/general.py
--rw-rw-rw-   0 root         (0) root         (0)     2883 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/utilities/inspect_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.524151 quantify-core-0.7.4/quantify_core/visualization/
--rw-rw-rw-   0 root         (0) root         (0)    16761 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/visualization/SI_utilities.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/visualization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/visualization/_appnope.py
--rw-rw-rw-   0 root         (0) root         (0)     1979 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/visualization/color_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.524151 quantify-core-0.7.4/quantify_core/visualization/ins_mon_widget/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/visualization/ins_mon_widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9725 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/visualization/ins_mon_widget/qc_snapshot_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     8121 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/visualization/instrument_monitor.py
--rw-rw-rw-   0 root         (0) root         (0)    19888 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/visualization/mpl_plotting.py
--rw-rw-rw-   0 root         (0) root         (0)     4369 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/visualization/plot_interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)    10576 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/visualization/pyqt_plotmon.py
--rw-rw-rw-   0 root         (0) root         (0)    28755 2023-12-15 16:23:37.000000 quantify-core-0.7.4/quantify_core/visualization/pyqt_plotmon_remote.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.552151 quantify-core-0.7.4/quantify_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6385 2023-12-15 16:23:50.000000 quantify-core-0.7.4/quantify_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9370 2023-12-15 16:23:50.000000 quantify-core-0.7.4/quantify_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-15 16:23:50.000000 quantify-core-0.7.4/quantify_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-15 16:23:42.000000 quantify-core-0.7.4/quantify_core.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      586 2023-12-15 16:23:50.000000 quantify-core-0.7.4/quantify_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-12-15 16:23:50.000000 quantify-core-0.7.4/quantify_core.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-15 16:23:50.555151 quantify-core-0.7.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      667 2023-12-15 16:23:37.000000 quantify-core-0.7.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.525152 quantify-core-0.7.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.527151 quantify-core-0.7.4/tests/analysis/
--rw-rw-rw-   0 root         (0) root         (0)     9901 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/analysis/test_base_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     3385 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/analysis/test_calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     3176 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/analysis/test_fitting_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1134 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/analysis/test_interpolation_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/analysis/test_optimization_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     2192 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/analysis/test_qubit_spectroscopy.py
--rw-rw-rw-   0 root         (0) root         (0)    18050 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/analysis/test_single_qubit_timedomain.py
--rw-rw-rw-   0 root         (0) root         (0)     3628 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/analysis/test_spectroscopy_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     2499 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/analysis/test_time_of_flight_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/analysis/test_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.528151 quantify-core-0.7.4/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    31985 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/data/test_data_handling.py
--rw-rw-rw-   0 root         (0) root         (0)     3534 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/data/test_experiment.py
--rw-rw-rw-   0 root         (0) root         (0)     1849 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/data/test_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.529152 quantify-core-0.7.4/tests/measurement/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/measurement/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    50533 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/measurement/test_measurement_control.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/measurement/test_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.530151 quantify-core-0.7.4/tests/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.483152 quantify-core-0.7.4/tests/test_data/20200430/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.530151 quantify-core-0.7.4/tests/test_data/20200430/20200430-170837-001-315f36-Cosine test/
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20200430/20200430-170837-001-315f36-Cosine test/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.484152 quantify-core-0.7.4/tests/test_data/20200504/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.530151 quantify-core-0.7.4/tests/test_data/20200504/20200504-191556-002-4209ee-2D Cosine test/
--rw-rw-rw-   0 root         (0) root         (0)    13868 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20200504/20200504-191556-002-4209ee-2D Cosine test/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.484152 quantify-core-0.7.4/tests/test_data/20200814/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.531151 quantify-core-0.7.4/tests/test_data/20200814/20200814-134652-492-fbf254-save/
--rw-rw-rw-   0 root         (0) root         (0)     4037 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20200814/20200814-134652-492-fbf254-save/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.485152 quantify-core-0.7.4/tests/test_data/20201124/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.531151 quantify-core-0.7.4/tests/test_data/20201124/20201124-184709-137-8a5112-(0) Spec IF=0.000 MHz/
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20201124/20201124-184709-137-8a5112-(0) Spec IF=0.000 MHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.531151 quantify-core-0.7.4/tests/test_data/20201124/20201124-184716-237-918bee-(1) Spec IF=20.000 MHz/
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20201124/20201124-184716-237-918bee-(1) Spec IF=20.000 MHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.531151 quantify-core-0.7.4/tests/test_data/20201124/20201124-184722-988-0463d4-(2) Spec IF=-20.000 MHz/
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20201124/20201124-184722-988-0463d4-(2) Spec IF=-20.000 MHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.532151 quantify-core-0.7.4/tests/test_data/20201124/20201124-184729-618-85970f-(3) Spec IF=40.000 MHz/
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20201124/20201124-184729-618-85970f-(3) Spec IF=40.000 MHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.532151 quantify-core-0.7.4/tests/test_data/20201124/20201124-184736-341-3628d4-(4) Spec IF=-40.000 MHz/
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20201124/20201124-184736-341-3628d4-(4) Spec IF=-40.000 MHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.485152 quantify-core-0.7.4/tests/test_data/20210118/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.533151 quantify-core-0.7.4/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/
--rw-rw-rw-   0 root         (0) root         (0)   240636 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/dataset.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    36780 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.485152 quantify-core-0.7.4/tests/test_data/20210126/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.534151 quantify-core-0.7.4/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/
--rw-rw-rw-   0 root         (0) root         (0)   244060 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/dataset.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    30350 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.486152 quantify-core-0.7.4/tests/test_data/20210227/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.534151 quantify-core-0.7.4/tests/test_data/20210227/20210227-172939-723-53d82c-Resonator_power_id6_4.612GHz/
--rw-rw-rw-   0 root         (0) root         (0)    73496 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210227/20210227-172939-723-53d82c-Resonator_power_id6_4.612GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.534151 quantify-core-0.7.4/tests/test_data/20210227/20210227-174714-680-31df85-Resonator_id7_4.660GHz/
--rw-rw-rw-   0 root         (0) root         (0)    13616 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210227/20210227-174714-680-31df85-Resonator_id7_4.660GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.535151 quantify-core-0.7.4/tests/test_data/20210305/
--rw-rw-rw-   0 root         (0) root         (0)    10244 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210305/.DS_Store
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.535151 quantify-core-0.7.4/tests/test_data/20210305/20210305-152943-497-ad8670-Resonator_id2_4.483GHz/
--rw-rw-rw-   0 root         (0) root         (0)    12464 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210305/20210305-152943-497-ad8670-Resonator_id2_4.483GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.535151 quantify-core-0.7.4/tests/test_data/20210305/20210305-154735-413-142768-Resonator_id2_4.483GHz/
--rw-rw-rw-   0 root         (0) root         (0)    27568 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210305/20210305-154735-413-142768-Resonator_id2_4.483GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.535151 quantify-core-0.7.4/tests/test_data/20210305/20210305-160157-184-3c17e9-Resonator_id4_4.541GHz/
--rw-rw-rw-   0 root         (0) root         (0)    27568 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210305/20210305-160157-184-3c17e9-Resonator_id4_4.541GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.536151 quantify-core-0.7.4/tests/test_data/20210305/20210305-161550-671-982c6d-Resonator_id5_4.577GHz/
--rw-rw-rw-   0 root         (0) root         (0)    27568 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210305/20210305-161550-671-982c6d-Resonator_id5_4.577GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.487152 quantify-core-0.7.4/tests/test_data/20210319/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.536151 quantify-core-0.7.4/tests/test_data/20210319/20210319-094728-327-69b211-load_settings_test/
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210319/20210319-094728-327-69b211-load_settings_test/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.488152 quantify-core-0.7.4/tests/test_data/20210322/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.536151 quantify-core-0.7.4/tests/test_data/20210322/20210322-205253-758-6689ca-T1 at 4.715GHz/
--rw-rw-rw-   0 root         (0) root         (0)    11464 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210322/20210322-205253-758-6689ca-T1 at 4.715GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.488152 quantify-core-0.7.4/tests/test_data/20210331/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.537151 quantify-core-0.7.4/tests/test_data/20210331/20210331-133734-718-aa9c83 AllXY q0/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210331/20210331-133734-718-aa9c83 AllXY q0/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.489152 quantify-core-0.7.4/tests/test_data/20210419/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.537151 quantify-core-0.7.4/tests/test_data/20210419/20210419-153127-883-fa4508-Rabi oscillation at 4.515GHz/
--rw-rw-rw-   0 root         (0) root         (0)    11464 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210419/20210419-153127-883-fa4508-Rabi oscillation at 4.515GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.537151 quantify-core-0.7.4/tests/test_data/20210419/20210419-170747-902-9c5a05-Offset_calibration/
--rw-rw-rw-   0 root         (0) root         (0)    13176 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210419/20210419-170747-902-9c5a05-Offset_calibration/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.538151 quantify-core-0.7.4/tests/test_data/20210419/20210419-173649-456-23c5f3-AllXY q0/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210419/20210419-173649-456-23c5f3-AllXY q0/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.489152 quantify-core-0.7.4/tests/test_data/20210420/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.538151 quantify-core-0.7.4/tests/test_data/20210420/20210420-001339-580-97bdef-Echo at 4.715GHz/
--rw-rw-rw-   0 root         (0) root         (0)    12928 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210420/20210420-001339-580-97bdef-Echo at 4.715GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.490152 quantify-core-0.7.4/tests/test_data/20210422/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.538151 quantify-core-0.7.4/tests/test_data/20210422/20210422-104958-297-7d6034-Ramsey oscillation at 4.715GHz/
--rw-rw-rw-   0 root         (0) root         (0)    11464 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210422/20210422-104958-297-7d6034-Ramsey oscillation at 4.715GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.490152 quantify-core-0.7.4/tests/test_data/20210827/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.539151 quantify-core-0.7.4/tests/test_data/20210827/20210827-174946-357-70a986-T1 experiment q0/
--rw-rw-rw-   0 root         (0) root         (0)    12024 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210827/20210827-174946-357-70a986-T1 experiment q0/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.539151 quantify-core-0.7.4/tests/test_data/20210827/20210827-175004-087-ab1aab-Ramsey oscillation q0 at 4.9969 GHz/
--rw-rw-rw-   0 root         (0) root         (0)    12024 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210827/20210827-175004-087-ab1aab-Ramsey oscillation q0 at 4.9969 GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.540151 quantify-core-0.7.4/tests/test_data/20210827/20210827-175021-521-251f28-Echo experiment q0/
--rw-rw-rw-   0 root         (0) root         (0)    12024 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210827/20210827-175021-521-251f28-Echo experiment q0/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.491152 quantify-core-0.7.4/tests/test_data/20210901/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.540151 quantify-core-0.7.4/tests/test_data/20210901/20210901-132357-561-5c3ef7-Ramsey oscillation q0 at 6.1400 GHz/
--rw-rw-rw-   0 root         (0) root         (0)    13848 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20210901/20210901-132357-561-5c3ef7-Ramsey oscillation q0 at 6.1400 GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.492152 quantify-core-0.7.4/tests/test_data/20211029/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.541151 quantify-core-0.7.4/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.541151 quantify-core-0.7.4/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/
--rw-rw-rw-   0 root         (0) root         (0)    12032 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    14504 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/dataset.hdf5
--rw-rw-rw-   0 root         (0) root         (0)   175606 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.542151 quantify-core-0.7.4/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.542151 quantify-core-0.7.4/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/
--rw-rw-rw-   0 root         (0) root         (0)    12032 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    14504 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/dataset.hdf5
--rw-rw-rw-   0 root         (0) root         (0)   175607 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.543151 quantify-core-0.7.4/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.543151 quantify-core-0.7.4/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/
--rw-rw-rw-   0 root         (0) root         (0)    12032 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    14504 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/dataset.hdf5
--rw-rw-rw-   0 root         (0) root         (0)   175605 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.492152 quantify-core-0.7.4/tests/test_data/20220409/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.544151 quantify-core-0.7.4/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/
--rw-rw-rw-   0 root         (0) root         (0)    13096 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/dataset.hdf5
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.493152 quantify-core-0.7.4/tests/test_data/20220509/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.544151 quantify-core-0.7.4/tests/test_data/20220509/20220509-204728-327-69b211-load_settings_test_nested/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20220509/20220509-204728-327-69b211-load_settings_test_nested/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.494152 quantify-core-0.7.4/tests/test_data/20220930/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.545151 quantify-core-0.7.4/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.545151 quantify-core-0.7.4/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/analysis_QubitSpectroscopyAnalysis/
--rw-rw-rw-   0 root         (0) root         (0)    12032 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    16000 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.545151 quantify-core-0.7.4/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.546151 quantify-core-0.7.4/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/analysis_QubitSpectroscopyAnalysis/
--rw-rw-rw-   0 root         (0) root         (0)    12032 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    16000 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.546151 quantify-core-0.7.4/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.547151 quantify-core-0.7.4/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/analysis_QubitSpectroscopyAnalysis/
--rw-rw-rw-   0 root         (0) root         (0)    12032 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    16000 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.495152 quantify-core-0.7.4/tests/test_data/20230508/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.547151 quantify-core-0.7.4/tests/test_data/20230508/20230508-122129-027-38881c-QubitSpectroscopy_q3/
--rw-rw-rw-   0 root         (0) root         (0)    17536 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20230508/20230508-122129-027-38881c-QubitSpectroscopy_q3/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.495152 quantify-core-0.7.4/tests/test_data/20230523/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.547151 quantify-core-0.7.4/tests/test_data/20230523/20230523-114322-399-dacb68-QubitSpectroscopy_q0/
--rw-rw-rw-   0 root         (0) root         (0)    15040 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20230523/20230523-114322-399-dacb68-QubitSpectroscopy_q0/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.547151 quantify-core-0.7.4/tests/test_data/20230523/20230523-175716-868-8746ad-QubitSpectroscopy_q2/
--rw-rw-rw-   0 root         (0) root         (0)    15040 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20230523/20230523-175716-868-8746ad-QubitSpectroscopy_q2/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.496152 quantify-core-0.7.4/tests/test_data/20230927/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.548151 quantify-core-0.7.4/tests/test_data/20230927/20230927-143514-589-e1a20e-time_of_light_calibration_fit_fail/
--rw-rw-rw-   0 root         (0) root         (0)    24288 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20230927/20230927-143514-589-e1a20e-time_of_light_calibration_fit_fail/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.548151 quantify-core-0.7.4/tests/test_data/20230927/20230927-143533-006-fe2167-time_of_light_calibration/
--rw-rw-rw-   0 root         (0) root         (0)    24288 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/20230927/20230927-143533-006-fe2167-time_of_light_calibration/dataset.hdf5
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.548151 quantify-core-0.7.4/tests/test_data/empty/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/empty/nothing
--rw-rw-rw-   0 root         (0) root         (0)     1538 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_data/transmon_test_config.json
--rw-rw-rw-   0 root         (0) root         (0)     2221 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/test_headers_and_copyright.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.550151 quantify-core-0.7.4/tests/utilities/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4330 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/utilities/test_deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)    12811 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/utilities/test_experiment_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2788 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/utilities/test_general.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/utilities/test_inspect_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 16:23:50.551151 quantify-core-0.7.4/tests/visualization/
--rw-rw-rw-   0 root         (0) root         (0)     9657 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/visualization/test_SI_utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     7151 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/visualization/test_instrument_monitor.py
--rw-rw-rw-   0 root         (0) root         (0)     4860 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/visualization/test_mpl_plotting.py
--rw-rw-rw-   0 root         (0) root         (0)     8018 2023-12-15 16:23:37.000000 quantify-core-0.7.4/tests/visualization/test_pyqt_plotmon.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.880898 quantify-core-0.7.5/
+-rw-rw-rw-   0        0        0     1973 2024-04-11 11:20:17.000000 quantify-core-0.7.5/AUTHORS.md
+-rw-rw-rw-   0        0        0    27990 2024-04-12 08:54:49.000000 quantify-core-0.7.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0    14826 2024-04-10 13:20:05.000000 quantify-core-0.7.5/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1516 2024-04-10 13:20:05.000000 quantify-core-0.7.5/LICENSE
+-rw-rw-rw-   0        0        0      278 2024-04-10 13:20:05.000000 quantify-core-0.7.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6556 2024-04-12 08:57:01.880898 quantify-core-0.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3217 2024-04-10 13:20:05.000000 quantify-core-0.7.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.694532 quantify-core-0.7.5/docs/
+-rw-rw-rw-   0        0        0      788 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/Makefile
+-rwxrwxrwx   0        0        0     1162 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/make.bat
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.695531 quantify-core-0.7.5/docs/source/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.698476 quantify-core-0.7.5/docs/source/api/
+-rw-rw-rw-   0        0        0     1567 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/api/analysis.md
+-rw-rw-rw-   0        0        0      508 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/api/data.md
+-rw-rw-rw-   0        0        0      147 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/api/index.md
+-rw-rw-rw-   0        0        0      296 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/api/measurement.md
+-rw-rw-rw-   0        0        0      473 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/api/utilities.md
+-rw-rw-rw-   0        0        0      794 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/api/visualization.md
+-rw-rw-rw-   0        0        0    14253 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/conf.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.698476 quantify-core-0.7.5/docs/source/dev/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.703485 quantify-core-0.7.5/docs/source/dev/design/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.703485 quantify-core-0.7.5/docs/source/dev/design/dataset/
+-rw-rw-rw-   0        0        0      543 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/dev/design/dataset/index.md
+-rw-rw-rw-   0        0        0      153 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/dev/design/index.md
+-rw-rw-rw-   0        0        0       43 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/dev/guide.md
+-rw-rw-rw-   0        0        0       69 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/dev/index.md
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.703485 quantify-core-0.7.5/docs/source/howto/
+-rw-rw-rw-   0        0        0      480 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/howto/index.md
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.703485 quantify-core-0.7.5/docs/source/images/
+-rw-rw-rw-   0        0        0     2254 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/images/QUANTIFY-FAVICON_16.png
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.703485 quantify-core-0.7.5/docs/source/images/install/
+-rw-rw-rw-   0        0        0  2452484 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/images/install/conda_activate.gif
+-rw-rw-rw-   0        0        0   858347 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/images/install/conda_install.gif
+-rw-rw-rw-   0        0        0  1669689 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/images/install/conda_source_installed_all_users.gif
+-rw-rw-rw-   0        0        0    27025 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/images/surface-7-sched.png
+-rw-rw-rw-   0        0        0     1850 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/index.md
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.715451 quantify-core-0.7.5/docs/source/tutorials/
+-rw-rw-rw-   0        0        0      298 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/tutorials/index.md
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.720450 quantify-core-0.7.5/docs/source/user/
+-rw-rw-rw-   0        0        0     1851 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/user/about.md
+-rw-rw-rw-   0        0        0       37 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/user/authors.md
+-rw-rw-rw-   0        0        0       52 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/user/bibliography.md
+-rw-rw-rw-   0        0        0       39 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/user/changelog.md
+-rw-rw-rw-   0        0        0      250 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/user/index.md
+-rw-rw-rw-   0        0        0    13399 2024-04-10 13:20:05.000000 quantify-core-0.7.5/docs/source/user/installation.md
+-rw-rw-rw-   0        0        0    12799 2024-04-10 13:20:05.000000 quantify-core-0.7.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.880898 quantify-core-0.7.5/quantify_core/
+-rw-rw-rw-   0        0        0      123 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/__init__.py
+-rw-rw-rw-   0        0        0       62 2024-04-12 08:57:01.880898 quantify-core-0.7.5/quantify_core/_static_version.py
+-rw-rw-rw-   0        0        0     5795 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/_version.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.761952 quantify-core-0.7.5/quantify_core/analysis/
+-rw-rw-rw-   0        0        0      693 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/analysis/__init__.py
+-rw-rw-rw-   0        0        0    35476 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/analysis/base_analysis.py
+-rw-rw-rw-   0        0        0     5079 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/analysis/calibration.py
+-rw-rw-rw-   0        0        0    10209 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/analysis/conditional_oscillation_analysis.py
+-rw-rw-rw-   0        0        0     3413 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/analysis/cosine_analysis.py
+-rw-rw-rw-   0        0        0    22433 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/analysis/fitting_models.py
+-rw-rw-rw-   0        0        0     2573 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/analysis/interpolation_analysis.py
+-rw-rw-rw-   0        0        0     4341 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/analysis/optimization_analysis.py
+-rw-rw-rw-   0        0        0     9659 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/analysis/readout_calibration_analysis.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.765105 quantify-core-0.7.5/quantify_core/analysis/schemas/
+-rw-rw-rw-   0        0        0     1152 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/analysis/schemas/AnalysisSettings.json
+-rw-rw-rw-   0        0        0        0 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/analysis/schemas/__init__.py
+-rw-rw-rw-   0        0        0    26738 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/analysis/single_qubit_timedomain.py
+-rw-rw-rw-   0        0        0    28269 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/analysis/spectroscopy_analysis.py
+-rw-rw-rw-   0        0        0     5762 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/analysis/time_of_flight_analysis.py
+-rw-rw-rw-   0        0        0     1297 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/analysis/types.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.765105 quantify-core-0.7.5/quantify_core/data/
+-rw-rw-rw-   0        0        0        0 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/data/__init__.py
+-rw-rw-rw-   0        0        0     5853 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/data/dataset_adapters.py
+-rw-rw-rw-   0        0        0    12630 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/data/dataset_attrs.py
+-rw-rw-rw-   0        0        0     6887 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/data/experiment.py
+-rw-rw-rw-   0        0        0    45524 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/data/handling.py
+-rw-rw-rw-   0        0        0     2961 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/data/types.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.765105 quantify-core-0.7.5/quantify_core/measurement/
+-rw-rw-rw-   0        0        0      725 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/measurement/__init__.py
+-rw-rw-rw-   0        0        0    40055 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/measurement/control.py
+-rw-rw-rw-   0        0        0      946 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/measurement/gettables.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.765105 quantify-core-0.7.5/quantify_core/measurement/schemas/
+-rw-rw-rw-   0        0        0     2516 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/measurement/schemas/Gettable.json
+-rw-rw-rw-   0        0        0     1646 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/measurement/schemas/Settable.json
+-rw-rw-rw-   0        0        0        0 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/measurement/schemas/__init__.py
+-rw-rw-rw-   0        0        0     3133 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/measurement/types.py
+-rw-rw-rw-   0        0        0        0 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.785097 quantify-core-0.7.5/quantify_core/utilities/
+-rw-rw-rw-   0        0        0       62 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1849 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/utilities/_docs_helpers.py
+-rw-rw-rw-   0        0        0     1209 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/utilities/_tests_helpers.py
+-rw-rw-rw-   0        0        0    19534 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/utilities/dataset_examples.py
+-rw-rw-rw-   0        0        0     5005 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/utilities/deprecation.py
+-rw-rw-rw-   0        0        0    11089 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/utilities/examples_support.py
+-rw-rw-rw-   0        0        0     9674 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/utilities/experiment_helpers.py
+-rw-rw-rw-   0        0        0     5882 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/utilities/general.py
+-rw-rw-rw-   0        0        0     2883 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/utilities/inspect_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.792102 quantify-core-0.7.5/quantify_core/visualization/
+-rw-rw-rw-   0        0        0    17471 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/visualization/SI_utilities.py
+-rw-rw-rw-   0        0        0      624 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/visualization/__init__.py
+-rw-rw-rw-   0        0        0      932 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/visualization/_appnope.py
+-rw-rw-rw-   0        0        0     1979 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/visualization/color_utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.794102 quantify-core-0.7.5/quantify_core/visualization/ins_mon_widget/
+-rw-rw-rw-   0        0        0        0 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/visualization/ins_mon_widget/__init__.py
+-rw-rw-rw-   0        0        0     9725 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/visualization/ins_mon_widget/qc_snapshot_widget.py
+-rw-rw-rw-   0        0        0     8121 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/visualization/instrument_monitor.py
+-rw-rw-rw-   0        0        0    19888 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/visualization/mpl_plotting.py
+-rw-rw-rw-   0        0        0     4369 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/visualization/plot_interpolation.py
+-rw-rw-rw-   0        0        0    10576 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/visualization/pyqt_plotmon.py
+-rw-rw-rw-   0        0        0    28755 2024-04-10 13:20:05.000000 quantify-core-0.7.5/quantify_core/visualization/pyqt_plotmon_remote.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.880898 quantify-core-0.7.5/quantify_core.egg-info/
+-rw-rw-rw-   0        0        0     6556 2024-04-12 08:57:01.000000 quantify-core-0.7.5/quantify_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11145 2024-04-12 08:57:01.000000 quantify-core-0.7.5/quantify_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 08:57:01.000000 quantify-core-0.7.5/quantify_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 08:22:04.000000 quantify-core-0.7.5/quantify_core.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      608 2024-04-12 08:57:01.000000 quantify-core-0.7.5/quantify_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-12 08:57:01.000000 quantify-core-0.7.5/quantify_core.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 08:57:01.880898 quantify-core-0.7.5/setup.cfg
+-rw-rw-rw-   0        0        0      667 2024-04-10 13:20:05.000000 quantify-core-0.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.796124 quantify-core-0.7.5/tests/
+-rw-rw-rw-   0        0        0       38 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.803525 quantify-core-0.7.5/tests/analysis/
+-rw-rw-rw-   0        0        0     9901 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/analysis/test_base_analysis.py
+-rw-rw-rw-   0        0        0     3385 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/analysis/test_calibration.py
+-rw-rw-rw-   0        0        0     3461 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/analysis/test_conditional_oscillation.py
+-rw-rw-rw-   0        0        0     3177 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/analysis/test_fitting_models.py
+-rw-rw-rw-   0        0        0     1134 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/analysis/test_interpolation_analysis.py
+-rw-rw-rw-   0        0        0     2563 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/analysis/test_optimization_analysis.py
+-rw-rw-rw-   0        0        0     2635 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/analysis/test_qubit_flux_spectroscopy.py
+-rw-rw-rw-   0        0        0     2192 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/analysis/test_qubit_spectroscopy.py
+-rw-rw-rw-   0        0        0     2699 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/analysis/test_readout_calibration.py
+-rw-rw-rw-   0        0        0     2850 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/analysis/test_resonator_flux_spectroscopy.py
+-rw-rw-rw-   0        0        0    18050 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/analysis/test_single_qubit_timedomain.py
+-rw-rw-rw-   0        0        0     3621 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/analysis/test_spectroscopy_analysis.py
+-rw-rw-rw-   0        0        0     2499 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/analysis/test_time_of_flight_analysis.py
+-rw-rw-rw-   0        0        0     1415 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/analysis/test_types.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.803525 quantify-core-0.7.5/tests/data/
+-rw-rw-rw-   0        0        0        0 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/data/__init__.py
+-rw-rw-rw-   0        0        0    31972 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/data/test_data_handling.py
+-rw-rw-rw-   0        0        0     3534 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/data/test_experiment.py
+-rw-rw-rw-   0        0        0     1849 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/data/test_types.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.814595 quantify-core-0.7.5/tests/measurement/
+-rw-rw-rw-   0        0        0        0 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/measurement/__init__.py
+-rw-rw-rw-   0        0        0    52061 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/measurement/test_measurement_control.py
+-rw-rw-rw-   0        0        0     1973 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/measurement/test_types.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.816595 quantify-core-0.7.5/tests/test_data/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.654528 quantify-core-0.7.5/tests/test_data/20200430/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.817594 quantify-core-0.7.5/tests/test_data/20200430/20200430-170837-001-315f36-Cosine test/
+-rw-rw-rw-   0        0        0     1268 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20200430/20200430-170837-001-315f36-Cosine test/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.655526 quantify-core-0.7.5/tests/test_data/20200504/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.818595 quantify-core-0.7.5/tests/test_data/20200504/20200504-191556-002-4209ee-2D Cosine test/
+-rw-rw-rw-   0        0        0    13868 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20200504/20200504-191556-002-4209ee-2D Cosine test/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.656528 quantify-core-0.7.5/tests/test_data/20200814/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.818595 quantify-core-0.7.5/tests/test_data/20200814/20200814-134652-492-fbf254-save/
+-rw-rw-rw-   0        0        0     4037 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20200814/20200814-134652-492-fbf254-save/snapshot.json
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.658527 quantify-core-0.7.5/tests/test_data/20201124/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.819594 quantify-core-0.7.5/tests/test_data/20201124/20201124-184709-137-8a5112-(0) Spec IF=0.000 MHz/
+-rw-rw-rw-   0        0        0      916 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20201124/20201124-184709-137-8a5112-(0) Spec IF=0.000 MHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.820594 quantify-core-0.7.5/tests/test_data/20201124/20201124-184716-237-918bee-(1) Spec IF=20.000 MHz/
+-rw-rw-rw-   0        0        0      916 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20201124/20201124-184716-237-918bee-(1) Spec IF=20.000 MHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.821593 quantify-core-0.7.5/tests/test_data/20201124/20201124-184722-988-0463d4-(2) Spec IF=-20.000 MHz/
+-rw-rw-rw-   0        0        0      916 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20201124/20201124-184722-988-0463d4-(2) Spec IF=-20.000 MHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.821593 quantify-core-0.7.5/tests/test_data/20201124/20201124-184729-618-85970f-(3) Spec IF=40.000 MHz/
+-rw-rw-rw-   0        0        0      916 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20201124/20201124-184729-618-85970f-(3) Spec IF=40.000 MHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.822593 quantify-core-0.7.5/tests/test_data/20201124/20201124-184736-341-3628d4-(4) Spec IF=-40.000 MHz/
+-rw-rw-rw-   0        0        0      916 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20201124/20201124-184736-341-3628d4-(4) Spec IF=-40.000 MHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.659526 quantify-core-0.7.5/tests/test_data/20210118/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.824595 quantify-core-0.7.5/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/
+-rw-rw-rw-   0        0        0   240636 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/dataset.hdf5
+-rw-rw-rw-   0        0        0    36780 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/snapshot.json
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.660529 quantify-core-0.7.5/tests/test_data/20210126/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.826596 quantify-core-0.7.5/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/
+-rw-rw-rw-   0        0        0   244060 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/dataset.hdf5
+-rw-rw-rw-   0        0        0    30350 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/snapshot.json
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.661527 quantify-core-0.7.5/tests/test_data/20210227/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.827595 quantify-core-0.7.5/tests/test_data/20210227/20210227-172939-723-53d82c-Resonator_power_id6_4.612GHz/
+-rw-rw-rw-   0        0        0    73496 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210227/20210227-172939-723-53d82c-Resonator_power_id6_4.612GHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.828595 quantify-core-0.7.5/tests/test_data/20210227/20210227-174714-680-31df85-Resonator_id7_4.660GHz/
+-rw-rw-rw-   0        0        0    13616 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210227/20210227-174714-680-31df85-Resonator_id7_4.660GHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.829595 quantify-core-0.7.5/tests/test_data/20210305/
+-rw-rw-rw-   0        0        0    10244 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210305/.DS_Store
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.830595 quantify-core-0.7.5/tests/test_data/20210305/20210305-152943-497-ad8670-Resonator_id2_4.483GHz/
+-rw-rw-rw-   0        0        0    12464 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210305/20210305-152943-497-ad8670-Resonator_id2_4.483GHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.831595 quantify-core-0.7.5/tests/test_data/20210305/20210305-154735-413-142768-Resonator_id2_4.483GHz/
+-rw-rw-rw-   0        0        0    27568 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210305/20210305-154735-413-142768-Resonator_id2_4.483GHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.831595 quantify-core-0.7.5/tests/test_data/20210305/20210305-160157-184-3c17e9-Resonator_id4_4.541GHz/
+-rw-rw-rw-   0        0        0    27568 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210305/20210305-160157-184-3c17e9-Resonator_id4_4.541GHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.832594 quantify-core-0.7.5/tests/test_data/20210305/20210305-161550-671-982c6d-Resonator_id5_4.577GHz/
+-rw-rw-rw-   0        0        0    27568 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210305/20210305-161550-671-982c6d-Resonator_id5_4.577GHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.664527 quantify-core-0.7.5/tests/test_data/20210319/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.833595 quantify-core-0.7.5/tests/test_data/20210319/20210319-094728-327-69b211-load_settings_test/
+-rw-rw-rw-   0        0        0     2760 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210319/20210319-094728-327-69b211-load_settings_test/snapshot.json
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.665526 quantify-core-0.7.5/tests/test_data/20210322/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.834595 quantify-core-0.7.5/tests/test_data/20210322/20210322-205253-758-6689ca-T1 at 4.715GHz/
+-rw-rw-rw-   0        0        0    11464 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210322/20210322-205253-758-6689ca-T1 at 4.715GHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.665526 quantify-core-0.7.5/tests/test_data/20210331/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.835596 quantify-core-0.7.5/tests/test_data/20210331/20210331-133734-718-aa9c83 AllXY q0/
+-rw-rw-rw-   0        0        0    11344 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210331/20210331-133734-718-aa9c83 AllXY q0/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.667526 quantify-core-0.7.5/tests/test_data/20210419/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.835596 quantify-core-0.7.5/tests/test_data/20210419/20210419-153127-883-fa4508-Rabi oscillation at 4.515GHz/
+-rw-rw-rw-   0        0        0    11464 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210419/20210419-153127-883-fa4508-Rabi oscillation at 4.515GHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.836596 quantify-core-0.7.5/tests/test_data/20210419/20210419-170747-902-9c5a05-Offset_calibration/
+-rw-rw-rw-   0        0        0    13176 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210419/20210419-170747-902-9c5a05-Offset_calibration/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.837598 quantify-core-0.7.5/tests/test_data/20210419/20210419-173649-456-23c5f3-AllXY q0/
+-rw-rw-rw-   0        0        0    11344 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210419/20210419-173649-456-23c5f3-AllXY q0/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.667526 quantify-core-0.7.5/tests/test_data/20210420/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.838596 quantify-core-0.7.5/tests/test_data/20210420/20210420-001339-580-97bdef-Echo at 4.715GHz/
+-rw-rw-rw-   0        0        0    12928 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210420/20210420-001339-580-97bdef-Echo at 4.715GHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.668528 quantify-core-0.7.5/tests/test_data/20210422/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.839596 quantify-core-0.7.5/tests/test_data/20210422/20210422-104958-297-7d6034-Ramsey oscillation at 4.715GHz/
+-rw-rw-rw-   0        0        0    11464 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210422/20210422-104958-297-7d6034-Ramsey oscillation at 4.715GHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.670526 quantify-core-0.7.5/tests/test_data/20210827/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.840597 quantify-core-0.7.5/tests/test_data/20210827/20210827-174946-357-70a986-T1 experiment q0/
+-rw-rw-rw-   0        0        0    12024 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210827/20210827-174946-357-70a986-T1 experiment q0/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.841596 quantify-core-0.7.5/tests/test_data/20210827/20210827-175004-087-ab1aab-Ramsey oscillation q0 at 4.9969 GHz/
+-rw-rw-rw-   0        0        0    12024 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210827/20210827-175004-087-ab1aab-Ramsey oscillation q0 at 4.9969 GHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.841596 quantify-core-0.7.5/tests/test_data/20210827/20210827-175021-521-251f28-Echo experiment q0/
+-rw-rw-rw-   0        0        0    12024 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210827/20210827-175021-521-251f28-Echo experiment q0/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.671526 quantify-core-0.7.5/tests/test_data/20210901/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.842596 quantify-core-0.7.5/tests/test_data/20210901/20210901-132357-561-5c3ef7-Ramsey oscillation q0 at 6.1400 GHz/
+-rw-rw-rw-   0        0        0    13848 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20210901/20210901-132357-561-5c3ef7-Ramsey oscillation q0 at 6.1400 GHz/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.673526 quantify-core-0.7.5/tests/test_data/20211029/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.844596 quantify-core-0.7.5/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.845595 quantify-core-0.7.5/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/
+-rw-rw-rw-   0        0        0    12032 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
+-rw-rw-rw-   0        0        0    14504 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/dataset.hdf5
+-rw-rw-rw-   0        0        0   175606 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/snapshot.json
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.848595 quantify-core-0.7.5/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.849596 quantify-core-0.7.5/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/
+-rw-rw-rw-   0        0        0    12032 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
+-rw-rw-rw-   0        0        0    14504 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/dataset.hdf5
+-rw-rw-rw-   0        0        0   175607 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/snapshot.json
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.849596 quantify-core-0.7.5/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.849596 quantify-core-0.7.5/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/
+-rw-rw-rw-   0        0        0    12032 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
+-rw-rw-rw-   0        0        0    14504 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/dataset.hdf5
+-rw-rw-rw-   0        0        0   175605 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/snapshot.json
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.674527 quantify-core-0.7.5/tests/test_data/20220409/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.849596 quantify-core-0.7.5/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/
+-rw-rw-rw-   0        0        0    13096 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/dataset.hdf5
+-rw-rw-rw-   0        0        0     3047 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/snapshot.json
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.675527 quantify-core-0.7.5/tests/test_data/20220509/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.849596 quantify-core-0.7.5/tests/test_data/20220509/20220509-204728-327-69b211-load_settings_test_nested/
+-rw-rw-rw-   0        0        0     1893 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20220509/20220509-204728-327-69b211-load_settings_test_nested/snapshot.json
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.677527 quantify-core-0.7.5/tests/test_data/20220930/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.849596 quantify-core-0.7.5/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.849596 quantify-core-0.7.5/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/analysis_QubitSpectroscopyAnalysis/
+-rw-rw-rw-   0        0        0    12032 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
+-rw-rw-rw-   0        0        0    16000 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.849596 quantify-core-0.7.5/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.849596 quantify-core-0.7.5/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/analysis_QubitSpectroscopyAnalysis/
+-rw-rw-rw-   0        0        0    12032 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
+-rw-rw-rw-   0        0        0    16000 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.849596 quantify-core-0.7.5/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.849596 quantify-core-0.7.5/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/analysis_QubitSpectroscopyAnalysis/
+-rw-rw-rw-   0        0        0    12032 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
+-rw-rw-rw-   0        0        0    16000 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.677527 quantify-core-0.7.5/tests/test_data/20230308/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.849596 quantify-core-0.7.5/tests/test_data/20230308/20230308-235659-059-cf471e-ResonatorFluxSpectroscopy/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.678526 quantify-core-0.7.5/tests/test_data/20230308/20230308-235659-059-cf471e-ResonatorFluxSpectroscopy/analysis_ResonatorFluxSpectroscopyAnalysis/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.849596 quantify-core-0.7.5/tests/test_data/20230308/20230308-235659-059-cf471e-ResonatorFluxSpectroscopy/analysis_ResonatorFluxSpectroscopyAnalysis/fit_results/
+-rw-rw-rw-   0        0        0     7562 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230308/20230308-235659-059-cf471e-ResonatorFluxSpectroscopy/analysis_ResonatorFluxSpectroscopyAnalysis/fit_results/sin.txt
+-rw-rw-rw-   0        0        0   333312 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230308/20230308-235659-059-cf471e-ResonatorFluxSpectroscopy/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.679526 quantify-core-0.7.5/tests/test_data/20230309/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.849596 quantify-core-0.7.5/tests/test_data/20230309/20230309-235228-129-1a58f5-ResonatorFluxSpectroscopy/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.679526 quantify-core-0.7.5/tests/test_data/20230309/20230309-235228-129-1a58f5-ResonatorFluxSpectroscopy/analysis_ResonatorFluxSpectroscopyAnalysis/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.849596 quantify-core-0.7.5/tests/test_data/20230309/20230309-235228-129-1a58f5-ResonatorFluxSpectroscopy/analysis_ResonatorFluxSpectroscopyAnalysis/fit_results/
+-rw-rw-rw-   0        0        0     7579 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230309/20230309-235228-129-1a58f5-ResonatorFluxSpectroscopy/analysis_ResonatorFluxSpectroscopyAnalysis/fit_results/sin.txt
+-rw-rw-rw-   0        0        0   333312 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230309/20230309-235228-129-1a58f5-ResonatorFluxSpectroscopy/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230309/20230309-235354-353-9c94c5-QubitSpectroscopy/
+-rw-rw-rw-   0        0        0   333312 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230309/20230309-235354-353-9c94c5-QubitSpectroscopy/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.680528 quantify-core-0.7.5/tests/test_data/20230508/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230508/20230508-122129-027-38881c-QubitSpectroscopy_q3/
+-rw-rw-rw-   0        0        0    17536 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230508/20230508-122129-027-38881c-QubitSpectroscopy_q3/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.684526 quantify-core-0.7.5/tests/test_data/20230509/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230509/20230509-135911-755-9471f2-ReadoutCalibration/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.681527 quantify-core-0.7.5/tests/test_data/20230509/20230509-135911-755-9471f2-ReadoutCalibration/analysis_ReadoutCalibrationAnalysis/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230509/20230509-135911-755-9471f2-ReadoutCalibration/analysis_ReadoutCalibrationAnalysis/fit_results/
+-rw-rw-rw-   0        0        0     3895 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230509/20230509-135911-755-9471f2-ReadoutCalibration/analysis_ReadoutCalibrationAnalysis/fit_results/linear_discriminator.txt
+-rw-rw-rw-   0        0        0    32417 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230509/20230509-135911-755-9471f2-ReadoutCalibration/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230509/20230509-135927-693-0977e0-ReadoutCalibration/
+-rw-rw-rw-   0        0        0    32417 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230509/20230509-135927-693-0977e0-ReadoutCalibration/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230509/20230509-152441-841-faef49-ReadoutCalibration/
+-rw-rw-rw-   0        0        0    32417 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230509/20230509-152441-841-faef49-ReadoutCalibration/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230509/20230509-165523-132-dcfea7-ConditionalOscillation/
+-rw-rw-rw-   0        0        0    32362 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230509/20230509-165523-132-dcfea7-ConditionalOscillation/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230509/20230509-165651-504-cabfd0-ConditionalOscillation/
+-rw-rw-rw-   0        0        0    32362 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230509/20230509-165651-504-cabfd0-ConditionalOscillation/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230509/20230509-165733-096-5016ba-ConditionalOscillation/
+-rw-rw-rw-   0        0        0    32362 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230509/20230509-165733-096-5016ba-ConditionalOscillation/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230509/20230509-165820-224-324d99-ConditionalOscillation/
+-rw-rw-rw-   0        0        0    32362 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230509/20230509-165820-224-324d99-ConditionalOscillation/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230509/20230509-165850-578-8a48c2-ConditionalOscillation/
+-rw-rw-rw-   0        0        0    34650 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230509/20230509-165850-578-8a48c2-ConditionalOscillation/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.685526 quantify-core-0.7.5/tests/test_data/20230523/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230523/20230523-110858-666-7a7dbb-QubitFluxSpectroscopy_q2/
+-rw-rw-rw-   0        0        0    72640 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230523/20230523-110858-666-7a7dbb-QubitFluxSpectroscopy_q2/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230523/20230523-114322-399-dacb68-QubitSpectroscopy_q0/
+-rw-rw-rw-   0        0        0    15040 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230523/20230523-114322-399-dacb68-QubitSpectroscopy_q0/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230523/20230523-175716-868-8746ad-QubitSpectroscopy_q2/
+-rw-rw-rw-   0        0        0    15040 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230523/20230523-175716-868-8746ad-QubitSpectroscopy_q2/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.686525 quantify-core-0.7.5/tests/test_data/20230927/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230927/20230927-143514-589-e1a20e-time_of_light_calibration_fit_fail/
+-rw-rw-rw-   0        0        0    24288 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230927/20230927-143514-589-e1a20e-time_of_light_calibration_fit_fail/dataset.hdf5
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/20230927/20230927-143533-006-fe2167-time_of_light_calibration/
+-rw-rw-rw-   0        0        0    24288 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/20230927/20230927-143533-006-fe2167-time_of_light_calibration/dataset.hdf5
+-rw-rw-rw-   0        0        0        0 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.865273 quantify-core-0.7.5/tests/test_data/empty/
+-rw-rw-rw-   0        0        0        0 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/empty/nothing
+-rw-rw-rw-   0        0        0     1538 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_data/transmon_test_config.json
+-rw-rw-rw-   0        0        0     2221 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/test_headers_and_copyright.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.880898 quantify-core-0.7.5/tests/utilities/
+-rw-rw-rw-   0        0        0        0 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/utilities/__init__.py
+-rw-rw-rw-   0        0        0     4330 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/utilities/test_deprecation.py
+-rw-rw-rw-   0        0        0    12811 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/utilities/test_experiment_helpers.py
+-rw-rw-rw-   0        0        0     2788 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/utilities/test_general.py
+-rw-rw-rw-   0        0        0      889 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/utilities/test_inspect_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:57:01.880898 quantify-core-0.7.5/tests/visualization/
+-rw-rw-rw-   0        0        0    10608 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/visualization/test_SI_utilities.py
+-rw-rw-rw-   0        0        0     7158 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/visualization/test_instrument_monitor.py
+-rw-rw-rw-   0        0        0     4860 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/visualization/test_mpl_plotting.py
+-rw-rw-rw-   0        0        0     8018 2024-04-10 13:20:05.000000 quantify-core-0.7.5/tests/visualization/test_pyqt_plotmon.py
```

### Comparing `quantify-core-0.7.4/AUTHORS.md` & `quantify-core-0.7.5/AUTHORS.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Contributors
 
 - Adam Lawrence ([GitLab](https://gitlab.com/adamorangeqs))
 - Adilet Tuleuov ([GitLab](https://gitlab.com/adilnaut))
 - Adriaan Rol ([GitLab](https://gitlab.com/AdriaanRol))
+- Amirtha Varshiny Arumugam ([GitLab](https://gitlab.com/avarshiny))
 - Axel Andersson ([GitLab](https://gitlab.com/axean))
 - Callum Attryde ([GitLab](https://gitlab.com/CallumAttryde))
 - Damien Crielaard ([GitLab](https://gitlab.com/dcrielaard))
 - Daniel Jonathan Weigand ([GitLab](https://gitlab.com/djweigand))
 - Diogo Valada ([GitLab](https://gitlab.com/Astlan))
 - Edgar Reehuis ([GitLab](https://gitlab.com/ereehuis))
 - Gabor Oszkar Denes ([GitLab](https://gitlab.com/gdenes))
@@ -22,11 +23,12 @@
 - Nicolas Piot ([GitLab](https://gitlab.com/npiot))
 - Pieter Eendebak ([GitLab](https://gitlab.com/peendebak))
 - Robert Sokolewicz ([GitLab](https://gitlab.com/rsokolewicz))
 - Sander de Snoo ([GitLab](https://gitlab.com/sldesnoo-Delft))
 - Thomas Middelburg ([GitLab](https://gitlab.com/ThomasMiddelburg))
 - Thomas Reynders ([GitLab](https://gitlab.com/treynders))
 - Tim Vroomans ([GitLab](https://gitlab.com/TimVroomans))
+- Timo Van Abswoude ([GitLab](https://gitlab.com/Timo_van_Abswoude)) 
 - Tobias Bonsen ([GitLab](https://gitlab.com/tobiasbonsen))
 - Victor Gervilla Palomar ([GitLab](https://gitlab.com/v_palomar))
 - Viacheslav Ostroukh ([GitLab](https://gitlab.com/slavoutich))
 - Victor Negirneac ([GitLab](https://gitlab.com/caenrigen))
```

### Comparing `quantify-core-0.7.4/CHANGELOG.md` & `quantify-core-0.7.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,44 @@
 # Changelog
 
+## 0.7.5 (2024-04-11)
+
+### Merged branches and closed issues
+
+- SI utilities 
+  - Cast large values for seconds to minutes or hours (!501)
+  - Add option `auto_scale` to `set_xlabel` and `set_ylabel` (!512)
+
+- Documentation
+  - Update copyright notice to 2024. (!506)
+
+- Analysis 
+  - Added analysis class for resonator flux spectroscopy. (!493)
+  - Add analysis class for qubit flux spectroscopy. (!473)
+  - Add analysis class for readout calibration. (!474)
+  - Add analysis class for the CZ conditional oscillation experiment. (!472)
+  - Fix units of Rabi analysis amplitudes. (!511)
+  - Remove an `xarray` `FutureWarning` in `to_gridded_dataset` when retrieving the dataset dimension names. (!510)
+  - Remove an `xarray` `DeprecationWarning` about `argmin` and `argmax` in the `RabiAnalysis`. (!513)
+  - Remove a `matplotlib` `MatplotlibDeprecationWarning` in `Basic2DAnalysis` when plotting a heatmap. (!510)
+
+- GitLab
+  - Make general Merge Request template the default. (!507)
+  - Add documentation redirect instructions to Release merge request template. (!507)
+
+- Tests
+  - Small refactor of tests to get rid of `PytestRemovedIn8Warning`s. (!508)
+
+- MeasurementControl
+  - Fix overflow warning when running `MeasurementControl.run_adaptive`. (!515)
+  - `grid_setpoints` now returns a list of M ndarrays, where M is the number of settables. Note that this is the transpose of the previous return type. The data type of the input setpoints is now preserved. (!505) 
+  
+- Linting
+  - replaced deprecated numpy definitions with numpy2.0 compatible alternatives. (!517)
+
 ## 0.7.4 (2023-12-15)
 
 ### Merged branches and closed issues
 
 - Documentation
   - Improve documentation build time and enable `sphinx-autobuild`. (!471)
   - Fix missing images in Jupyter cell outputs in documentation deployed using Gitlab Pages. (!480)
```

### Comparing `quantify-core-0.7.4/CONTRIBUTING.md` & `quantify-core-0.7.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/LICENSE` & `quantify-core-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/PKG-INFO` & `quantify-core-0.7.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,116 +1,117 @@
-Metadata-Version: 2.1
-Name: quantify-core
-Version: 0.7.4
-Summary: Quantify-core is a unified quantum computing, solid-state and pulse sequencing physical experimentation framework.
-Maintainer-email: Edgar Reehuis <ereehuis@qblox.com>, Robert Sokolewicz <rsokolewicz@qblox.com>, Tobias Bonsen <tobias@orangeqs.com>, Viacheslav Ostroukh <viacheslav@orangeqs.com>
-License: BSD-3-Clause
-Project-URL: Documentation, https://quantify-os.org/docs/quantify-core
-Project-URL: Source, https://gitlab.com/quantify-os/quantify-core
-Project-URL: Issue tracker, https://gitlab.com/quantify-os/quantify-core/-/issues
-Project-URL: Changelog, https://gitlab.com/quantify-os/quantify-core/-/blob/main/CHANGELOG.md
-Project-URL: Slack, https://join.slack.com/t/quantify-hq/shared_invite/zt-1nd78r4e9-rbWdna53cW4DO_YbtMhVuA
-Project-URL: Authors, https://gitlab.com/quantify-os/quantify-core/-/blob/main/AUTHORS.md
-Keywords: quantum,quantify
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.md
-Requires-Dist: numpy!=1.19.4
-Requires-Dist: qcodes>=0.37.0
-Requires-Dist: qcodes-loop
-Requires-Dist: scipy!=1.6.0,>=1.5.0
-Requires-Dist: h5netcdf
-Requires-Dist: xarray>=0.19.0
-Requires-Dist: matplotlib!=3.5.0
-Requires-Dist: lmfit>=1.0.3
-Requires-Dist: pyqt5>5.15.2
-Requires-Dist: pyqtgraph
-Requires-Dist: jsonschema
-Requires-Dist: adaptive
-Requires-Dist: filelock
-Requires-Dist: appnope
-Requires-Dist: uncertainties
-Requires-Dist: dataclasses_json
-Requires-Dist: dill
-Requires-Dist: methodtools
-Requires-Dist: deepdiff
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-mock; extra == "test"
-Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: pydata-sphinx-theme; extra == "docs"
-Requires-Dist: myst-nb; extra == "docs"
-Requires-Dist: rich[jupyter]; extra == "docs"
-Requires-Dist: scanpydoc; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
-Requires-Dist: sphinx-jsonschema>=1.15; extra == "docs"
-Requires-Dist: sphinx-togglebutton; extra == "docs"
-Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
-Requires-Dist: sphinx-design; extra == "docs"
-Provides-Extra: dev
-Requires-Dist: quantify-core[docs,test]; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: pytest-xdist; extra == "dev"
-Requires-Dist: nbstripout; extra == "dev"
-Requires-Dist: scikit-optimize; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pre-commit-hooks; extra == "dev"
-Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pyright; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: sphinx-autobuild; extra == "dev"
-
-# quantify-core
-
-[![Slack](https://img.shields.io/badge/slack-chat-green.svg)](https://quantify-os.org/slack.html#sec-slack)
-[![Pipelines](https://gitlab.com/quantify-os/quantify-core/badges/main/pipeline.svg)](https://gitlab.com/quantify-os/quantify-core/-/pipelines/)
-[![PyPi](https://img.shields.io/pypi/v/quantify-core.svg)](https://pypi.org/pypi/quantify-core)
-[![Code Quality](https://app.codacy.com/project/badge/Grade/32265e1e7d3f491fa028528aaf8bfa69)](https://app.codacy.com/gl/quantify-os/quantify-core/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-core&amp;utm_campaign=Badge_Grade)
-[![Coverage](https://app.codacy.com/project/badge/Coverage/32265e1e7d3f491fa028528aaf8bfa69)](https://app.codacy.com/gl/quantify-os/quantify-core/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-core&amp;utm_campaign=Badge_Coverage)
-[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://gitlab.com/quantify-os/quantify-core/-/blob/main/LICENSE)
-[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=flat)](https://unitary.fund)
-[![Documentation](https://img.shields.io/badge/documentation-grey)](https://quantify-os.org/docs/quantify-core)
-
-![Quantify logo](https://gitlab.com/quantify-os/quantify-core/-/raw/main/docs/source/images/QUANTIFY_LANDSCAPE.svg)
-
-Quantify is a Python-based data acquisition framework focused on Quantum Computing and
-solid-state physics experiments.
-The framework consists of [quantify-core](https://pypi.org/project/quantify-core/) ([git](https://gitlab.com/quantify-os/quantify-core/) | [docs](https://quantify-os.org/docs/quantify-core))
-and [quantify-scheduler](https://pypi.org/project/quantify-scheduler/) ([git](https://gitlab.com/quantify-os/quantify-scheduler/) | [docs](https://quantify-os.org/docs/quantify-scheduler)).
-It is built on top of [QCoDeS](https://qcodes.github.io/Qcodes/)
-and is a spiritual successor of [PycQED](https://github.com/DiCarloLab-Delft/PycQED_py3).
-`quantify-core` is the core module that contains all basic functionality to control experiments. This includes:
-
-- A framework to control instruments.
-- A data-acquisition loop.
-- Data storage and analysis.
-- Parameter monitoring and live visualization of experiments.
-
-## Overview and Community
-
-For a general overview of Quantify and connecting to its open-source community, see [quantify-os.org](https://quantify-os.org/).
-Quantify is maintained by the Quantify Consortium consisting of Qblox and Orange Quantum Systems.
-
-[<img src="https://gitlab.com/quantify-os/quantify-core/-/raw/main/docs/source/images/Qblox_logo.svg" alt="Qblox logo" width=200px/>](https://qblox.com)
-&nbsp;
-&nbsp;
-&nbsp;
-&nbsp;
-[<img src="https://gitlab.com/quantify-os/quantify-core/-/raw/main/docs/source/images/OQS_logo_with_text.svg" alt="Orange Quantum Systems logo" width=200px/>](https://orangeqs.com)
-
-&nbsp;
-
-The software is free to use under the conditions specified in the [license](https://gitlab.com/quantify-os/quantify-core/-/raw/main/LICENSE).
+Metadata-Version: 2.1
+Name: quantify-core
+Version: 0.7.5
+Summary: Quantify-core is a unified quantum computing, solid-state and pulse sequencing physical experimentation framework.
+Maintainer-email: Edgar Reehuis <ereehuis@qblox.com>, Robert Sokolewicz <rsokolewicz@qblox.com>, Tobias Bonsen <tobias@orangeqs.com>, Viacheslav Ostroukh <viacheslav@orangeqs.com>
+License: BSD-3-Clause
+Project-URL: Documentation, https://quantify-os.org/docs/quantify-core
+Project-URL: Source, https://gitlab.com/quantify-os/quantify-core
+Project-URL: Issue tracker, https://gitlab.com/quantify-os/quantify-core/-/issues
+Project-URL: Changelog, https://gitlab.com/quantify-os/quantify-core/-/blob/main/CHANGELOG.md
+Project-URL: Slack, https://join.slack.com/t/quantify-hq/shared_invite/zt-1nd78r4e9-rbWdna53cW4DO_YbtMhVuA
+Project-URL: Authors, https://gitlab.com/quantify-os/quantify-core/-/blob/main/AUTHORS.md
+Keywords: quantum,quantify
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: numpy!=1.19.4
+Requires-Dist: qcodes>=0.37.0
+Requires-Dist: qcodes-loop
+Requires-Dist: scipy!=1.6.0,>=1.5.0
+Requires-Dist: h5netcdf
+Requires-Dist: xarray>=0.19.0
+Requires-Dist: matplotlib!=3.5.0
+Requires-Dist: lmfit>=1.0.3
+Requires-Dist: pyqt5>5.15.2
+Requires-Dist: pyqtgraph
+Requires-Dist: jsonschema
+Requires-Dist: adaptive
+Requires-Dist: filelock
+Requires-Dist: appnope
+Requires-Dist: uncertainties
+Requires-Dist: dataclasses_json
+Requires-Dist: dill
+Requires-Dist: methodtools
+Requires-Dist: deepdiff
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: pydata-sphinx-theme; extra == "docs"
+Requires-Dist: myst-nb; extra == "docs"
+Requires-Dist: rich[jupyter]; extra == "docs"
+Requires-Dist: scanpydoc; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
+Requires-Dist: sphinx-jsonschema>=1.15; extra == "docs"
+Requires-Dist: sphinx-togglebutton; extra == "docs"
+Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
+Requires-Dist: sphinx-design; extra == "docs"
+Requires-Dist: jupyter_sphinx>=0.4.0; extra == "docs"
+Provides-Extra: dev
+Requires-Dist: quantify-core[docs,test]; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: nbstripout; extra == "dev"
+Requires-Dist: scikit-optimize; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pre-commit-hooks; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pyright; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: sphinx-autobuild; extra == "dev"
+
+# quantify-core
+
+[![Slack](https://img.shields.io/badge/slack-chat-green.svg)](https://quantify-os.org/slack.html#sec-slack)
+[![Pipelines](https://gitlab.com/quantify-os/quantify-core/badges/main/pipeline.svg)](https://gitlab.com/quantify-os/quantify-core/-/pipelines/)
+[![PyPi](https://img.shields.io/pypi/v/quantify-core.svg)](https://pypi.org/pypi/quantify-core)
+[![Code Quality](https://app.codacy.com/project/badge/Grade/32265e1e7d3f491fa028528aaf8bfa69)](https://app.codacy.com/gl/quantify-os/quantify-core/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-core&amp;utm_campaign=Badge_Grade)
+[![Coverage](https://app.codacy.com/project/badge/Coverage/32265e1e7d3f491fa028528aaf8bfa69)](https://app.codacy.com/gl/quantify-os/quantify-core/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-core&amp;utm_campaign=Badge_Coverage)
+[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://gitlab.com/quantify-os/quantify-core/-/blob/main/LICENSE)
+[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=flat)](https://unitary.fund)
+[![Documentation](https://img.shields.io/badge/documentation-grey)](https://quantify-os.org/docs/quantify-core)
+
+![Quantify logo](https://gitlab.com/quantify-os/quantify-core/-/raw/main/docs/source/images/QUANTIFY_LANDSCAPE.svg)
+
+Quantify is a Python-based data acquisition framework focused on Quantum Computing and
+solid-state physics experiments.
+The framework consists of [quantify-core](https://pypi.org/project/quantify-core/) ([git](https://gitlab.com/quantify-os/quantify-core/) | [docs](https://quantify-os.org/docs/quantify-core))
+and [quantify-scheduler](https://pypi.org/project/quantify-scheduler/) ([git](https://gitlab.com/quantify-os/quantify-scheduler/) | [docs](https://quantify-os.org/docs/quantify-scheduler)).
+It is built on top of [QCoDeS](https://qcodes.github.io/Qcodes/)
+and is a spiritual successor of [PycQED](https://github.com/DiCarloLab-Delft/PycQED_py3).
+`quantify-core` is the core module that contains all basic functionality to control experiments. This includes:
+
+- A framework to control instruments.
+- A data-acquisition loop.
+- Data storage and analysis.
+- Parameter monitoring and live visualization of experiments.
+
+## Overview and Community
+
+For a general overview of Quantify and connecting to its open-source community, see [quantify-os.org](https://quantify-os.org/).
+Quantify is maintained by the Quantify Consortium consisting of Qblox and Orange Quantum Systems.
+
+[<img src="https://gitlab.com/quantify-os/quantify-core/-/raw/main/docs/source/images/Qblox_logo.svg" alt="Qblox logo" width=200px/>](https://qblox.com)
+&nbsp;
+&nbsp;
+&nbsp;
+&nbsp;
+[<img src="https://gitlab.com/quantify-os/quantify-core/-/raw/main/docs/source/images/OQS_logo_with_text.svg" alt="Orange Quantum Systems logo" width=200px/>](https://orangeqs.com)
+
+&nbsp;
+
+The software is free to use under the conditions specified in the [license](https://gitlab.com/quantify-os/quantify-core/-/raw/main/LICENSE).
```

### Comparing `quantify-core-0.7.4/README.md` & `quantify-core-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/docs/Makefile` & `quantify-core-0.7.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/docs/make.bat` & `quantify-core-0.7.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/docs/source/api/analysis.md` & `quantify-core-0.7.5/docs/source/api/analysis.md`

 * *Files 10% similar despite different names*

```diff
@@ -66,7 +66,23 @@
 ## `calibration`
 
 ```{eval-rst}
 .. automodule:: quantify_core.analysis.calibration
     :members:
     :show-inheritance:
 ```
+
+## `readout_calibration_analysis`
+
+```{eval-rst}
+.. automodule:: quantify_core.analysis.readout_calibration_analysis
+    :members:
+    :show-inheritance:
+```
+
+## `conditional_oscillation_analysis`
+
+```{eval-rst}
+.. automodule:: quantify_core.analysis.conditional_oscillation_analysis
+    :members:
+    :show-inheritance:
+```
```

### Comparing `quantify-core-0.7.4/docs/source/api/visualization.md` & `quantify-core-0.7.5/docs/source/api/visualization.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/docs/source/conf.py` & `quantify-core-0.7.5/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     "sphinx_autodoc_typehints",
     "sphinx.ext.viewcode",
     "sphinx.ext.intersphinx",
     "sphinx.ext.autosectionlabel",
     "sphinx-jsonschema",
     "sphinx.ext.mathjax",
     "sphinx_togglebutton",
+    "jupyter_sphinx",
     # fancy type hints in docs and
     # solves the same issue as "sphinx_automodapi.smart_resolver"
     # however the smart_resolver seems to fail for external packages like `zhinst`
     "scanpydoc.elegant_typehints",
     "sphinxcontrib.bibtex",
     # documents parameters that are defined in the __init__ of `Instrument`s as
     # instance attributes
@@ -79,15 +80,15 @@
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # See https://stackoverflow.com/a/42513684 for a common list and instructions to find new
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
-    "qcodes": ("https://qcodes.github.io/Qcodes/", None),
+    "qcodes": ("https://microsoft.github.io/Qcodes/", None),
     "xarray": ("https://docs.xarray.dev/en/stable/", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
     "matplotlib": ("https://matplotlib.org/stable/", None),
     "lmfit": ("https://lmfit.github.io/lmfit-py/", None),
     "dateutil": ("https://dateutil.readthedocs.io/en/stable/", None),
     # uncertainties has limited docs, but we can still use something like
     # :doc:`uncertainties <uncertainties:index>`
@@ -108,15 +109,15 @@
 source_suffix = [".rst", ".md"]
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "quantify-core"
-copyright = "2020-2023, Qblox & Orange Quantum Systems"
+copyright = "2020-2024, Qblox & Orange Quantum Systems"
 author = "Quantify Consortium"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
```

### Comparing `quantify-core-0.7.4/docs/source/dev/design/dataset/index.md` & `quantify-core-0.7.5/docs/source/dev/design/dataset/index.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/docs/source/images/QUANTIFY-FAVICON_16.png` & `quantify-core-0.7.5/docs/source/images/QUANTIFY-FAVICON_16.png`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/docs/source/images/install/conda_activate.gif` & `quantify-core-0.7.5/docs/source/images/install/conda_activate.gif`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/docs/source/images/install/conda_install.gif` & `quantify-core-0.7.5/docs/source/images/install/conda_install.gif`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/docs/source/images/install/conda_source_installed_all_users.gif` & `quantify-core-0.7.5/docs/source/images/install/conda_source_installed_all_users.gif`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/docs/source/images/surface-7-sched.png` & `quantify-core-0.7.5/docs/source/images/surface-7-sched.png`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/docs/source/index.md` & `quantify-core-0.7.5/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/docs/source/user/about.md` & `quantify-core-0.7.5/docs/source/user/about.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/docs/source/user/installation.md` & `quantify-core-0.7.5/docs/source/user/installation.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/_version.py` & `quantify-core-0.7.5/quantify_core/_version.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/analysis/__init__.py` & `quantify-core-0.7.5/quantify_core/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/analysis/base_analysis.py` & `quantify-core-0.7.5/quantify_core/analysis/base_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -790,15 +790,15 @@
             fig_id = f"Linecuts x0x1-{yi}"
 
             lines = yvals.plot.line(x="x0", hue="x1", ax=ax)
             # Change the color and labels of the line as we want to tweak this with
             # respect to xarray default.
             for line, z_value in zip(lines, np.array(gridded_dataset["x1"])):
                 # use the default colormap specified
-                cmap = matplotlib.cm.get_cmap()
+                cmap = matplotlib.cm._get_cmap()
                 norm = matplotlib.colors.Normalize(
                     vmin=np.min(gridded_dataset["x1"]),
                     vmax=np.max(gridded_dataset["x1"]),
                 )
                 line.set_color(cmap(norm(z_value)))
                 line.set_label(f"{z_value:.3g}")
```

### Comparing `quantify-core-0.7.4/quantify_core/analysis/calibration.py` & `quantify-core-0.7.5/quantify_core/analysis/calibration.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/analysis/cosine_analysis.py` & `quantify-core-0.7.5/quantify_core/analysis/cosine_analysis.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/analysis/fitting_models.py` & `quantify-core-0.7.5/quantify_core/analysis/fitting_models.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/analysis/interpolation_analysis.py` & `quantify-core-0.7.5/quantify_core/analysis/interpolation_analysis.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/analysis/optimization_analysis.py` & `quantify-core-0.7.5/quantify_core/analysis/optimization_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,17 +59,17 @@
         for x_variable in self.dataset.coords:
             optimum = float(
                 self.dataset[x_variable][
                     arg_optimum_function(self.dataset[y_variable].values)
                 ].values
             )
 
-            self.quantities_of_interest[
-                self.dataset[x_variable].attrs["name"]
-            ] = optimum
+            self.quantities_of_interest[self.dataset[x_variable].attrs["name"]] = (
+                optimum
+            )
 
             text_msg += format_value_string(
                 self.dataset[x_variable].attrs["long_name"],
                 optimum,
                 end_char="\n",
                 unit=self.dataset[x_variable].units,
             )
```

### Comparing `quantify-core-0.7.4/quantify_core/analysis/schemas/AnalysisSettings.json` & `quantify-core-0.7.5/quantify_core/analysis/schemas/AnalysisSettings.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/analysis/single_qubit_timedomain.py` & `quantify-core-0.7.5/quantify_core/analysis/single_qubit_timedomain.py`

 * *Files 1% similar despite different names*

```diff
@@ -619,31 +619,31 @@
         If calibration points are True, automatically determine the point farthest
         from the 0 point to use as a reference to rotate the data.
 
         This will ensure the data lies along the axis with the best SNR.
         """
 
         # index closest to rabi-pulse amplitude = 0
-        min_idx = abs(self.dataset_processed.x0.values).argmin()
+        min_idx = np.argmin(abs(self.dataset_processed.x0.values))
         # transmission measured for Rabi-pulse amplitude closest to 0
-        min_val = self.dataset_processed.S21[min_idx]
+        min_val = self.dataset_processed.S21.values[min_idx]
 
         # find index with max absolute difference (distance in IQ space) to the S21_0
-        max_idx = abs(self.dataset_processed.S21 - min_val).argmax()
-        max_val = self.dataset_processed.S21[max_idx]
+        max_idx = np.argmax(abs(self.dataset_processed.S21.values - min_val))
+        max_val = self.dataset_processed.S21.values[max_idx]
 
         rotation_angle = np.angle(max_val - min_val)
         rot_data = self.dataset_processed.S21 * np.exp(-1j * rotation_angle)
 
         self.dataset_processed["S21_rot"] = rot_data
         self.dataset_processed.S21_rot.attrs["name"] = "S21_rot"
         self.dataset_processed.S21_rot.attrs["units"] = self.dataset.y0.units
-        self.dataset_processed.S21_rot.attrs[
-            "long_name"
-        ] = "Rotated transmission $S_{21}^R$"
+        self.dataset_processed.S21_rot.attrs["long_name"] = (
+            "Rotated transmission $S_{21}^R$"
+        )
 
     def _choose_data_for_fit(self):
         if self.calibration_points:
             y_data = self.dataset_processed.S21_rot.real.values
             x_data = self.dataset_processed.x0.values
         else:
             # if the data is not rotated,fit the magnitude of the signal
@@ -676,15 +676,15 @@
         if fit_warning is None:
             self.quantities_of_interest["fit_success"] = True
 
             text_msg = "Summary\n"
             text_msg += format_value_string(
                 "Pi-pulse amplitude",
                 fit_result.params["amp180"],
-                unit="V",
+                unit="a.u.",
                 end_char="\n",
             )
             text_msg += format_value_string(
                 "Oscillation amplitude",
                 fit_result.params["amplitude"],
                 unit="V",
                 end_char="\n",
```

### Comparing `quantify-core-0.7.4/quantify_core/analysis/time_of_flight_analysis.py` & `quantify-core-0.7.5/quantify_core/analysis/time_of_flight_analysis.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/analysis/types.py` & `quantify-core-0.7.5/quantify_core/analysis/types.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/data/dataset_adapters.py` & `quantify-core-0.7.5/quantify_core/data/dataset_adapters.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/data/dataset_attrs.py` & `quantify-core-0.7.5/quantify_core/data/dataset_attrs.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/data/experiment.py` & `quantify-core-0.7.5/quantify_core/data/experiment.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/data/handling.py` & `quantify-core-0.7.5/quantify_core/data/handling.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,25 +499,25 @@
     os.makedirs(exp_folder, exist_ok=True)
     return exp_folder
 
 
 # pylint: disable=too-many-locals
 def initialize_dataset(
     settable_pars: Iterable,
-    setpoints: np.ndarray,
+    setpoints: list[np.ndarray],
     gettable_pars: Iterable,
 ) -> xr.Dataset:
     """Initialize an empty dataset based on settable_pars, setpoints and gettable_pars.
 
     Parameters
     ----------
     settable_pars
         A list of M settables.
     setpoints
-        An (N*M) array.
+        An (M*N) array.
     gettable_pars
         A list of gettables.
 
 
     Returns
     -------
     :
@@ -531,17 +531,17 @@
             "long_name": _generate_long_name(setpar),
             "units": setpar.unit,
             "batched": _is_batched(setpar),
         }
         if attrs["batched"] and hasattr(setpar, "batch_size"):
             attrs["batch_size"] = setpar.batch_size
         coords.append(f"x{i}")
-        darrs.append(xr.DataArray(data=setpoints[:, i], name=coords[-1], attrs=attrs))
+        darrs.append(xr.DataArray(data=setpoints[i], name=coords[-1], attrs=attrs))
 
-    numpoints = len(setpoints[:, 0])
+    numpoints = len(setpoints[0])
     j = 0
     for getpar in gettable_pars:
         # it's possible for one Gettable to return multiple axes. to handle this, zip
         # the axis info together
         # so we can iterate through when defining the axis in the dataset
         if not isinstance(getpar.name, list):
             itrbl = zip([getpar.name], [getpar.label], [getpar.unit])
@@ -963,16 +963,15 @@
         is independent: :code:`to_gridded_dataset(dset, coords_names=["x0"])`.
 
     Returns
     -------
     :
         The new dataset.
     """
-    if dimension not in quantify_dataset.dims:
-        dims = tuple(quantify_dataset.dims.keys())
+    if dimension not in (dims := tuple(quantify_dataset.dims)):
         raise ValueError(f"Dimension {dimension} not in dims {dims}.")
 
     if coords_names is None:
         # for compatibility with older datasets we use `variables` instead of `coords`
         coords_names = sorted(
             v for v in quantify_dataset.variables if v.startswith("x")
         )
```

### Comparing `quantify-core-0.7.4/quantify_core/data/types.py` & `quantify-core-0.7.5/quantify_core/data/types.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/measurement/__init__.py` & `quantify-core-0.7.5/quantify_core/measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/measurement/control.py` & `quantify-core-0.7.5/quantify_core/measurement/control.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 import math
 import signal
 import tempfile
 import threading
 import time
 import types
 from collections.abc import Iterable
+from functools import reduce
 from itertools import chain
 from pathlib import Path
-from typing import Any, Dict, Optional
-from tqdm.auto import tqdm
+from typing import TYPE_CHECKING, Any, Dict, Optional, Protocol, Sequence, TypeVar
 
 import adaptive
 import numpy as np
-import xarray as xr
 from filelock import FileLock
 from qcodes import validators as vals
 from qcodes.instrument import Instrument, InstrumentChannel
 from qcodes.parameters import InstrumentRefParameter, ManualParameter
+from tqdm.auto import tqdm
 
 from quantify_core import __version__ as _quantify_version
 from quantify_core.data.experiment import QuantifyExperiment
 from quantify_core.data.handling import (
     DATASET_NAME,
     _is_uniformly_spaced_array,
     create_exp_folder,
@@ -34,14 +34,17 @@
     initialize_dataset,
     snapshot,
     trim_dataset,
 )
 from quantify_core.measurement.types import Gettable, Settable, is_batched
 from quantify_core.utilities.general import call_if_has_method
 
+if TYPE_CHECKING:
+    import xarray as xr
+
 # Intended for plotting monitors that run in separate processes
 _DATASET_LOCKS_DIR = Path(tempfile.gettempdir())
 
 
 class MeasurementControl(Instrument):  # pylint: disable=too-many-instance-attributes
     """
     Instrument responsible for controlling the data acquisition loop.
@@ -135,18 +138,22 @@
         # Add experiment_data submodule to allow user to save custom metadata
         experiment_data = InstrumentChannel(self, "experiment_data")
         self.add_submodule("experiment_data", experiment_data)
 
         self._soft_avg_validator = vals.Ints(1, int(1e8)).validate
 
         # variables that are set before the start of any experiment.
-        self._settable_pars = []
-        self._setpoints = []
-        self._setpoints_input = []
-        self._gettable_pars = []
+        self._settable_pars: list[Settable] = []
+        """Parameter(s) to be set during the acquisition loop."""
+        self._setpoints: list[np.ndarray] = []
+        """An (M, N) matrix of N setpoints for M settables."""
+        self._setpoints_input: Iterable[np.ndarray] = []
+        """The values to loop over in the experiment."""
+        self._gettable_pars: list[Gettable] = []
+        """Parameter(s) to be get during the acquisition loop."""
 
         # variables used for book keeping during acquisition loop.
         self._soft_avg = 1
         self._nr_acquired_values = 0
         self._loop_count = 0
         self._begintime = time.time()
         self._last_upd = time.time()
@@ -185,15 +192,17 @@
         if hasattr(self, "_setpoints_input") and self._setpoints_input is not None:
             input_shapes = [
                 np.asarray(points).shape for points in self._setpoints_input
             ]
             str_out += f"    setpoints_grid input shapes: {input_shapes}\n"
 
         if hasattr(self, "_setpoints") and self._setpoints is not None:
-            str_out += f"    setpoints shape: {np.asarray(self._setpoints).shape}\n"
+            str_out += (
+                f"    setpoints shape: {np.asarray(self._setpoints).shape[::-1]}\n"
+            )
 
         return str_out
 
     def __repr__(self):
         """
         Returns a string containing a summary of this object regarding settables,
         gettables and setpoints.
@@ -461,15 +470,15 @@
                 unused_pars = ["adaptive_function"]
                 for unused_par in unused_pars:
                     af_pars_copy.pop(unused_par, None)
                 adaptive_function(measure, **af_pars_copy)
 
         self._reset()
         self.setpoints(
-            np.empty((64, len(self._settable_pars)))
+            np.zeros((64, len(self._settable_pars)))
         )  # block out some space in the dataset
         self._init(name)
 
         try:
             print("Running adaptively...")
             subroutine()
         except KeyboardInterrupt:
@@ -484,16 +493,20 @@
         return self._dataset
 
     def _run_iterative(self, lazy_set: bool = False):
         while self._get_fracdone() < 1.0:
             self._prepare_gettables()
 
             self._dataarray_cache = {}
-            for row in self._setpoints:
-                self._iterative_set_and_get(row, self._curr_setpoint_idx(), lazy_set)
+            for idx in range(len(self._setpoints[0])):
+                self._iterative_set_and_get(
+                    [spt[idx] for spt in self._setpoints],
+                    self._curr_setpoint_idx(),
+                    lazy_set,
+                )
                 self._nr_acquired_values += 1
                 self._update()
                 self._check_interrupt()
             self._dataarray_cache = None
             self._loop_count += 1
 
     def _run_batched(self):  # pylint: disable=too-many-locals
@@ -516,24 +529,24 @@
             self._batch_size_last = batch_size
             slice_len = setpoint_idx + self._batch_size_last
             for i, spar in enumerate(iterative_settables):
                 # Here ensure that all setpoints of each iterative settable are the same
                 # within each batch
                 val, iterator = next(
                     itertools.groupby(
-                        self._setpoints[setpoint_idx:slice_len, where_iterative[i]]
+                        self._setpoints[where_iterative[i]][setpoint_idx:slice_len]
                     )
                 )
                 spar.set(val)
                 # We also determine the size of each next batch
                 self._batch_size_last = min(self._batch_size_last, len(tuple(iterator)))
 
             slice_len = setpoint_idx + self._batch_size_last
             for i, spar in enumerate(batched_settables):
-                pnts = self._setpoints[setpoint_idx:slice_len, where_batched[i]]
+                pnts = self._setpoints[where_batched[i]][setpoint_idx:slice_len]
                 spar.set(pnts)
             # Update for `print_progress`
             self._batch_size_last = min(self._batch_size_last, len(pnts))
 
             self._prepare_gettables()
 
             y_off = 0
@@ -543,20 +556,20 @@
                 if len(np.shape(new_data)) == 1:
                     new_data = new_data.reshape(1, (len(new_data)))
 
                 for row in new_data:
                     yi_name = f"y{y_off}"
                     slice_len = setpoint_idx + len(row)  # the slice we will be updating
                     old_vals = self._dataset[yi_name].values[setpoint_idx:slice_len]
-                    old_vals[
-                        np.isnan(old_vals)
-                    ] = 0  # will be full of NaNs on the first iteration, change to 0
-                    self._dataset[yi_name].values[
-                        setpoint_idx:slice_len
-                    ] = self._build_data(row, old_vals)
+                    old_vals[np.isnan(old_vals)] = (
+                        0  # will be full of NaNs on the first iteration, change to 0
+                    )
+                    self._dataset[yi_name].values[setpoint_idx:slice_len] = (
+                        self._build_data(row, old_vals)
+                    )
                     y_off += 1
 
             self._nr_acquired_values += np.shape(new_data)[1]
             self._update()
             self._check_interrupt()
 
     def _build_data(self, new_data, old_data):
@@ -720,15 +733,15 @@
 
     def _get_batch_size(self):
         # np.inf is not supported by the JSON schema, but we keep the code robust
         min_with_inf = min(
             getattr(par, "batch_size", np.inf)
             for par in chain.from_iterable((self._settable_pars, self._gettable_pars))
         )
-        return min(min_with_inf, len(self._setpoints))
+        return min(min_with_inf, len(self._setpoints[0]))
 
     def _get_is_batched(self) -> bool:
         if any(
             is_batched(gpar) for gpar in chain(self._gettable_pars, self._settable_pars)
         ):
             if not all(is_batched(gpar) for gpar in self._gettable_pars):
                 raise RuntimeError(
@@ -744,28 +757,31 @@
 
         return False
 
     def _get_max_setpoints(self) -> int:
         """
         The total number of setpoints to examine
         """
-        return len(self._setpoints) * self._soft_avg
+        try:
+            return len(self._setpoints[0]) * self._soft_avg
+        except IndexError:
+            return 0
 
     def _curr_setpoint_idx(self) -> int:
         """
         Current position through the sweep
 
         Returns
         -------
         int
             setpoint_idx
         """
         acquired = self._nr_acquired_values
-        setpoint_idx = acquired % len(self._setpoints)
-        self._loop_count = acquired // len(self._setpoints)
+        setpoint_idx = acquired % len(self._setpoints[0])
+        self._loop_count = acquired // len(self._setpoints[0])
         return setpoint_idx
 
     def _get_fracdone(self) -> float:
         """
         Returns the fraction of the experiment that is completed.
         """
         return self._nr_acquired_values / self._get_max_setpoints()
@@ -876,15 +892,16 @@
         elif len(np.shape(setpoints)) == 2:
             # used in plotmon to detect need for interpolation in 2d plot
             is_uniform = all(
                 _is_uniformly_spaced_array(setpoints_i) for setpoints_i in setpoints.T
             )
             self._plot_info["1d_2_settables_uniformly_spaced"] = is_uniform
 
-        self._setpoints = setpoints
+        # UI is to provide an (N, M) array, but internally we store an (M, N) array
+        self._setpoints = setpoints.T
         # `.setpoints()` and `.setpoints_grid()` cannot be used at the same time
         self._setpoints_input = None
 
     def setpoints_grid(self, setpoints: Iterable[np.ndarray]):
         """
         Makes a grid from the provided `setpoints` assuming each array element
         corresponds to an orthogonal dimension.
@@ -952,74 +969,87 @@
         experiment_description["setpoints_shape"] = self._setpoints.shape
         experiment_description["soft_avg"] = self._soft_avg
         experiment_description["acquired_dataset"] = {"tuid": self._dataset.tuid}
 
         return experiment_description
 
 
-def grid_setpoints(setpoints: Iterable, settables: Iterable = None) -> np.ndarray:
+def grid_setpoints(
+    setpoints: Sequence[Sequence],
+    settables: Iterable | None = None,
+) -> list[np.ndarray]:
     """
-    Makes gridded setpoints. If `settables` is provided, the gridding is such that the
-    inner most loop corresponds to the batched settable with the smallest `.batch_size`.
-
-    .. warning ::
+    Make gridded setpoints.
 
-        Using this method typecasts all values into the same type.
-        This may lead to validator errors when setting
-        e.g., a `float` instead of an `int`.
+    If ``settables`` is provided, the gridding is such that the inner most loop
+    corresponds to the batched settable with the smallest ``.batch_size``.
 
     Parameters
     ----------
     setpoints
         A list of arrays that defines the values to loop over in the experiment for each
         orthogonal dimension. The grid is reshaped in the same order.
     settables
         A list of settable objects to which the elements in the `setpoints` correspond
         to. Used to correctly grid data when mixing batched and iterative settables.
 
     Returns
     -------
-    :class:`~numpy.ndarray`
-        An array where the first numpy axis correspond to individual setpoints.
+    list[np.ndarray]
+        A 2D array where the first axis corresponds to the settables, and the second
+        axis to individual setpoints.
     """
 
     if settables is None:
         settables = [None] * len(setpoints)
 
-    coordinates_names = [f"x{i}" for i, pnts in enumerate(setpoints)]
-    dataset_coordinates = xr.Dataset(coords=dict(zip(coordinates_names, setpoints)))
-    coordinates_batched = [
-        name for name, spar in zip(coordinates_names, settables) if is_batched(spar)
-    ]
-    coordinates_iterative = sorted(
-        (
-            name
-            for name, spar in zip(coordinates_names, settables)
-            if not is_batched(spar)
-        ),
-        reverse=True,
-    )
+    coordinates_batched = [i for i, spar in enumerate(settables) if is_batched(spar)]
+    coordinates_iterative = [
+        i for i, spar in enumerate(settables) if not is_batched(spar)
+    ][::-1]
 
+    stack_order = coordinates_iterative
     if len(coordinates_batched):
         batch_sizes = [
             getattr(spar, "batch_size", np.inf)
             for spar in settables
             if is_batched(spar)
         ]
-        coordinates_batched_set = set(coordinates_batched)
-        inner_coord_name = coordinates_batched[np.argmin(batch_sizes)]
-        coordinates_batched_set.remove(inner_coord_name)
+        inner_coord = coordinates_batched[np.argmin(batch_sizes)]
+        coordinates_batched.remove(inner_coord)
         # The inner most coordinate must correspond to the batched settable with
         # min `.batch_size`
-        stack_order = (
-            coordinates_iterative
-            + sorted(coordinates_batched_set, reverse=True)
-            + [inner_coord_name]
-        )
-    else:
-        stack_order = coordinates_iterative + sorted(coordinates_batched, reverse=True)
+        stack_order += coordinates_batched[::-1] + [inner_coord]
+
+    order_of_order = np.argsort(stack_order)
+
+    stacked_dset = _cartesian_product_transposed(*(setpoints[i] for i in stack_order))
+    stacked_dset = [stacked_dset[i] for i in order_of_order]
+    return stacked_dset
+
+
+class _SupportsMul(Protocol):
+    """A type that supports multiplication (*)."""
+
+    def __mul__(self, other): ...
+
+    def __rmul__(self, other): ...
+
+
+T = TypeVar("T", bound=_SupportsMul)
+
+
+def _prod(iter_: Iterable[T]) -> T:
+    return reduce(lambda x, y: x * y, iter_)
 
-    # Internally the xarray's stack mechanism is used to achieve the desired grid
-    stacked_dset = dataset_coordinates.stack(dim_0=stack_order)
 
-    # Return numpy array in the original order
-    return np.column_stack([stacked_dset[name].values for name in coordinates_names])
+def _cartesian_product_transposed(*setpoints: Sequence) -> list[np.ndarray]:
+    lengths = [len(arr) for arr in setpoints]
+    out = []
+    for i, arr in enumerate(setpoints):
+        row = np.array(arr)
+        if i < len(setpoints) - 1:
+            row = np.repeat(row, _prod(lengths[i + 1 :]))
+        if i > 0:
+            row = np.tile(row, _prod(lengths[:i]))
+        out.append(row)
+    return out
```

### Comparing `quantify-core-0.7.4/quantify_core/measurement/gettables.py` & `quantify-core-0.7.5/quantify_core/measurement/gettables.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/measurement/schemas/Gettable.json` & `quantify-core-0.7.5/quantify_core/measurement/schemas/Gettable.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/measurement/schemas/Settable.json` & `quantify-core-0.7.5/quantify_core/measurement/schemas/Settable.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/measurement/types.py` & `quantify-core-0.7.5/quantify_core/measurement/types.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/utilities/_docs_helpers.py` & `quantify-core-0.7.5/quantify_core/utilities/_docs_helpers.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/utilities/_tests_helpers.py` & `quantify-core-0.7.5/quantify_core/utilities/_tests_helpers.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/utilities/dataset_examples.py` & `quantify-core-0.7.5/quantify_core/utilities/dataset_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     ----------
     num_amps
         Number of x points.
     num_times
         Number of y points.
     """
     amps, times = np.linspace(-1, 1, num_amps), np.linspace(0, 10, num_times)
-    amps, times = grid_setpoints([amps, times]).T
+    amps, times = grid_setpoints([amps, times])
     sig = amps * np.cos(times)
 
     attrs = dict(
         tuid=dh.gen_tuid(),
         name="my experiment",
         grid_2d=True,
         grid_2d_uniformly_spaced=True,
@@ -89,15 +89,15 @@
     """
 
     rng = np.random.default_rng(seed=seed)  # random number generator
 
     amp_values = np.linspace(0.45, 0.55, 30)
     time_values = np.linspace(0, 100e-9, 40)
 
-    amp_values, time_values = mc.grid_setpoints([amp_values, time_values]).T
+    amp_values, time_values = mc.grid_setpoints([amp_values, time_values])
     amp_values_norm = np.abs(
         (amp_values - amp_values.mean()) / (amp_values - amp_values.mean()).max()
     )
     pop_q0 = (1 - amp_values_norm) * np.sin(
         2 * np.pi * time_values * 1 / 30e-9 * (amp_values_norm + 0.5)
     )
     pop_q1 = -pop_q0  # mock inverted population for q1
```

### Comparing `quantify-core-0.7.4/quantify_core/utilities/deprecation.py` & `quantify-core-0.7.5/quantify_core/utilities/deprecation.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/utilities/examples_support.py` & `quantify-core-0.7.5/quantify_core/utilities/examples_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,17 +86,17 @@
 # ######################################################################################
 # IQ-related data manipulation and plotting
 # ######################################################################################
 
 
 def mk_iq_shots(
     num_shots: int = 128,
-    sigmas: Union[Tuple[float], NDArray[np.float_]] = (0.1, 0.1),
-    centers: Union[Tuple[complex], NDArray[np.complex_]] = (-0.2 + 0.65j, 0.7 + 4j),
-    probabilities: Union[Tuple[float], NDArray[np.float_]] = (0.4, 0.6),
+    sigmas: Union[Tuple[float], NDArray[np.float64]] = (0.1, 0.1),
+    centers: Union[Tuple[complex], NDArray[np.complex128]] = (-0.2 + 0.65j, 0.7 + 4j),
+    probabilities: Union[Tuple[float], NDArray[np.float64]] = (0.4, 0.6),
     seed: Union[int, None] = 112233,
 ) -> NDArray:
     """
     Generate clusters of (I + 1j*Q) points with a Gaussian distribution.
 
     Utility to mock the data coming from qubit readout experiments.
     Clusters are centered around ``centers`` and data points are distributed between
```

### Comparing `quantify-core-0.7.4/quantify_core/utilities/experiment_helpers.py` & `quantify-core-0.7.5/quantify_core/utilities/experiment_helpers.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/utilities/general.py` & `quantify-core-0.7.5/quantify_core/utilities/general.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/utilities/inspect_utils.py` & `quantify-core-0.7.5/quantify_core/utilities/inspect_utils.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/visualization/SI_utilities.py` & `quantify-core-0.7.5/quantify_core/visualization/SI_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,25 +88,31 @@
     """
     offset_scale, offset_unit = SI_prefix_and_scale_factor(offset, unit)
     disp_offset = offset * offset_scale
     formatter.set_offset_string(f"{disp_offset:+g} {offset_unit}")
 
 
 def set_xlabel(
-    label: str | plt.Axes, unit: str | None = None, axis: plt.Axes | None = None, **kw
+    label: str | plt.Axes,
+    unit: str | None = None,
+    axis: plt.Axes | None = None,
+    auto_scale: bool = True,
+    **kw,
 ) -> plt.Axes:
     """
     Add a unit aware x-label to an axis object.
 
     Parameters
     ----------
     label
         the desired label
     unit
         the unit
+    auto_scale
+        If True, then automatically scale the units
     axis
         matplotlib axis object to set label on
     **kw
         keyword argument to be passed to matplotlib.set_xlabel
     """
     if isinstance(label, plt.Axes):
         warnings.warn(
@@ -117,15 +123,15 @@
             stacklevel=2,
         )
         axis, label, unit = label, unit, axis
 
     if axis is None:
         axis = plt.gca()
 
-    if unit:
+    if unit and auto_scale:
         xticks = axis.get_xticks()
         precision = 4
         scale_factor, offset, unit = _get_scale_factor_and_offset_and_prefix(
             xticks, unit, precision
         )
 
         formatter = matplotlib.ticker.FuncFormatter(
@@ -133,33 +139,41 @@
         )
 
         if offset != 0:
             _set_offset_string(formatter, offset, unit)
 
         axis.xaxis.set_major_formatter(formatter)
         axis.set_xlabel(label + f" [{unit}]", **kw)
+    elif unit:
+        axis.set_xlabel(label + f" [{unit}]", **kw)
     else:
         axis.set_xlabel(label, **kw)
     return axis
 
 
 def set_ylabel(
-    label: str | plt.Axes, unit: str | None = None, axis: plt.Axes | None = None, **kw
+    label: str | plt.Axes,
+    unit: str | None = None,
+    axis: plt.Axes | None = None,
+    auto_scale: bool = True,
+    **kw,
 ) -> plt.Axes | None:
     """
     Add a unit aware y-label to an axis object.
 
     Parameters
     ----------
     label
         the desired label
     unit
         the unit
     axis
         matplotlib axis object to set label on
+    auto_scale
+        If True, then automatically scale the units
     **kw
         keyword argument to be passed to matplotlib.set_ylabel
     """
     if isinstance(label, plt.Axes):
         warnings.warn(
             "Passing axis as a first argument is deprecated and will be removed"
             " in quantify-core >= 0.10.0. Please use the new syntax"
@@ -168,15 +182,15 @@
             stacklevel=2,
         )
         axis, label, unit = label, unit, axis  # type: ignore
 
     if axis is None:
         axis = plt.gca()
 
-    if unit:
+    if unit and auto_scale:
         yticks = axis.get_yticks()
         precision = 6
         scale_factor, offset, unit = _get_scale_factor_and_offset_and_prefix(
             yticks, unit, precision=precision
         )
 
         formatter = matplotlib.ticker.FuncFormatter(
@@ -185,14 +199,16 @@
 
         if offset != 0:
             _set_offset_string(formatter, offset, unit)
 
         axis.yaxis.set_major_formatter(formatter)
 
         axis.set_ylabel(label + f" [{unit}]", **kw)
+    elif unit:
+        axis.set_ylabel(label + f" [{unit}]", **kw)
     else:
         axis.set_ylabel(label, **kw)
     return axis
 
 
 def set_cbarlabel(
     cbar: matplotlib.colorbar.Colorbar, label: str, unit: str | None = None, **kw
@@ -320,14 +336,19 @@
                 prefix_power = np.log10(abs(val)) // 3 * 3
                 prefix = SI_PREFIXES[prefix_power]
                 # Greek symbols not supported in tex
                 if plt.rcParams["text.usetex"] and prefix == "μ":
                     prefix = r"$\mu$"
             if unit == "SI_PREFIX_ONLY":
                 scale_factor, scaled_unit = 10**-prefix_power, prefix
+            elif unit == "s" and val > 2 * 60:
+                if val > 2 * 3600:  # Convert to hours if larger than 2 hours
+                    scale_factor, scaled_unit = 1 / 3600, "hrs"
+                else:  # Convert to minutes if between 2 minutes and 2 hours
+                    scale_factor, scaled_unit = 1 / 60, "min"
             else:
                 scale_factor, scaled_unit = 10**-prefix_power, prefix + unit
         # this exception can be triggered in the pyqtgraph multi processing
         except (KeyError, TypeError):
             scale_factor, scaled_unit = 1, unit
 
     elif unit is None:
```

### Comparing `quantify-core-0.7.4/quantify_core/visualization/__init__.py` & `quantify-core-0.7.5/quantify_core/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/visualization/_appnope.py` & `quantify-core-0.7.5/quantify_core/visualization/_appnope.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/visualization/color_utilities.py` & `quantify-core-0.7.5/quantify_core/visualization/color_utilities.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/visualization/ins_mon_widget/qc_snapshot_widget.py` & `quantify-core-0.7.5/quantify_core/visualization/ins_mon_widget/qc_snapshot_widget.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/visualization/instrument_monitor.py` & `quantify-core-0.7.5/quantify_core/visualization/instrument_monitor.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/visualization/mpl_plotting.py` & `quantify-core-0.7.5/quantify_core/visualization/mpl_plotting.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/visualization/plot_interpolation.py` & `quantify-core-0.7.5/quantify_core/visualization/plot_interpolation.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/visualization/pyqt_plotmon.py` & `quantify-core-0.7.5/quantify_core/visualization/pyqt_plotmon.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core/visualization/pyqt_plotmon_remote.py` & `quantify-core-0.7.5/quantify_core/visualization/pyqt_plotmon_remote.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/quantify_core.egg-info/PKG-INFO` & `quantify-core-0.7.5/quantify_core.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,116 +1,117 @@
-Metadata-Version: 2.1
-Name: quantify-core
-Version: 0.7.4
-Summary: Quantify-core is a unified quantum computing, solid-state and pulse sequencing physical experimentation framework.
-Maintainer-email: Edgar Reehuis <ereehuis@qblox.com>, Robert Sokolewicz <rsokolewicz@qblox.com>, Tobias Bonsen <tobias@orangeqs.com>, Viacheslav Ostroukh <viacheslav@orangeqs.com>
-License: BSD-3-Clause
-Project-URL: Documentation, https://quantify-os.org/docs/quantify-core
-Project-URL: Source, https://gitlab.com/quantify-os/quantify-core
-Project-URL: Issue tracker, https://gitlab.com/quantify-os/quantify-core/-/issues
-Project-URL: Changelog, https://gitlab.com/quantify-os/quantify-core/-/blob/main/CHANGELOG.md
-Project-URL: Slack, https://join.slack.com/t/quantify-hq/shared_invite/zt-1nd78r4e9-rbWdna53cW4DO_YbtMhVuA
-Project-URL: Authors, https://gitlab.com/quantify-os/quantify-core/-/blob/main/AUTHORS.md
-Keywords: quantum,quantify
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.md
-Requires-Dist: numpy!=1.19.4
-Requires-Dist: qcodes>=0.37.0
-Requires-Dist: qcodes-loop
-Requires-Dist: scipy!=1.6.0,>=1.5.0
-Requires-Dist: h5netcdf
-Requires-Dist: xarray>=0.19.0
-Requires-Dist: matplotlib!=3.5.0
-Requires-Dist: lmfit>=1.0.3
-Requires-Dist: pyqt5>5.15.2
-Requires-Dist: pyqtgraph
-Requires-Dist: jsonschema
-Requires-Dist: adaptive
-Requires-Dist: filelock
-Requires-Dist: appnope
-Requires-Dist: uncertainties
-Requires-Dist: dataclasses_json
-Requires-Dist: dill
-Requires-Dist: methodtools
-Requires-Dist: deepdiff
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-mock; extra == "test"
-Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: pydata-sphinx-theme; extra == "docs"
-Requires-Dist: myst-nb; extra == "docs"
-Requires-Dist: rich[jupyter]; extra == "docs"
-Requires-Dist: scanpydoc; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
-Requires-Dist: sphinx-jsonschema>=1.15; extra == "docs"
-Requires-Dist: sphinx-togglebutton; extra == "docs"
-Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
-Requires-Dist: sphinx-design; extra == "docs"
-Provides-Extra: dev
-Requires-Dist: quantify-core[docs,test]; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: pytest-xdist; extra == "dev"
-Requires-Dist: nbstripout; extra == "dev"
-Requires-Dist: scikit-optimize; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pre-commit-hooks; extra == "dev"
-Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pyright; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: sphinx-autobuild; extra == "dev"
-
-# quantify-core
-
-[![Slack](https://img.shields.io/badge/slack-chat-green.svg)](https://quantify-os.org/slack.html#sec-slack)
-[![Pipelines](https://gitlab.com/quantify-os/quantify-core/badges/main/pipeline.svg)](https://gitlab.com/quantify-os/quantify-core/-/pipelines/)
-[![PyPi](https://img.shields.io/pypi/v/quantify-core.svg)](https://pypi.org/pypi/quantify-core)
-[![Code Quality](https://app.codacy.com/project/badge/Grade/32265e1e7d3f491fa028528aaf8bfa69)](https://app.codacy.com/gl/quantify-os/quantify-core/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-core&amp;utm_campaign=Badge_Grade)
-[![Coverage](https://app.codacy.com/project/badge/Coverage/32265e1e7d3f491fa028528aaf8bfa69)](https://app.codacy.com/gl/quantify-os/quantify-core/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-core&amp;utm_campaign=Badge_Coverage)
-[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://gitlab.com/quantify-os/quantify-core/-/blob/main/LICENSE)
-[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=flat)](https://unitary.fund)
-[![Documentation](https://img.shields.io/badge/documentation-grey)](https://quantify-os.org/docs/quantify-core)
-
-![Quantify logo](https://gitlab.com/quantify-os/quantify-core/-/raw/main/docs/source/images/QUANTIFY_LANDSCAPE.svg)
-
-Quantify is a Python-based data acquisition framework focused on Quantum Computing and
-solid-state physics experiments.
-The framework consists of [quantify-core](https://pypi.org/project/quantify-core/) ([git](https://gitlab.com/quantify-os/quantify-core/) | [docs](https://quantify-os.org/docs/quantify-core))
-and [quantify-scheduler](https://pypi.org/project/quantify-scheduler/) ([git](https://gitlab.com/quantify-os/quantify-scheduler/) | [docs](https://quantify-os.org/docs/quantify-scheduler)).
-It is built on top of [QCoDeS](https://qcodes.github.io/Qcodes/)
-and is a spiritual successor of [PycQED](https://github.com/DiCarloLab-Delft/PycQED_py3).
-`quantify-core` is the core module that contains all basic functionality to control experiments. This includes:
-
-- A framework to control instruments.
-- A data-acquisition loop.
-- Data storage and analysis.
-- Parameter monitoring and live visualization of experiments.
-
-## Overview and Community
-
-For a general overview of Quantify and connecting to its open-source community, see [quantify-os.org](https://quantify-os.org/).
-Quantify is maintained by the Quantify Consortium consisting of Qblox and Orange Quantum Systems.
-
-[<img src="https://gitlab.com/quantify-os/quantify-core/-/raw/main/docs/source/images/Qblox_logo.svg" alt="Qblox logo" width=200px/>](https://qblox.com)
-&nbsp;
-&nbsp;
-&nbsp;
-&nbsp;
-[<img src="https://gitlab.com/quantify-os/quantify-core/-/raw/main/docs/source/images/OQS_logo_with_text.svg" alt="Orange Quantum Systems logo" width=200px/>](https://orangeqs.com)
-
-&nbsp;
-
-The software is free to use under the conditions specified in the [license](https://gitlab.com/quantify-os/quantify-core/-/raw/main/LICENSE).
+Metadata-Version: 2.1
+Name: quantify-core
+Version: 0.7.5
+Summary: Quantify-core is a unified quantum computing, solid-state and pulse sequencing physical experimentation framework.
+Maintainer-email: Edgar Reehuis <ereehuis@qblox.com>, Robert Sokolewicz <rsokolewicz@qblox.com>, Tobias Bonsen <tobias@orangeqs.com>, Viacheslav Ostroukh <viacheslav@orangeqs.com>
+License: BSD-3-Clause
+Project-URL: Documentation, https://quantify-os.org/docs/quantify-core
+Project-URL: Source, https://gitlab.com/quantify-os/quantify-core
+Project-URL: Issue tracker, https://gitlab.com/quantify-os/quantify-core/-/issues
+Project-URL: Changelog, https://gitlab.com/quantify-os/quantify-core/-/blob/main/CHANGELOG.md
+Project-URL: Slack, https://join.slack.com/t/quantify-hq/shared_invite/zt-1nd78r4e9-rbWdna53cW4DO_YbtMhVuA
+Project-URL: Authors, https://gitlab.com/quantify-os/quantify-core/-/blob/main/AUTHORS.md
+Keywords: quantum,quantify
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: numpy!=1.19.4
+Requires-Dist: qcodes>=0.37.0
+Requires-Dist: qcodes-loop
+Requires-Dist: scipy!=1.6.0,>=1.5.0
+Requires-Dist: h5netcdf
+Requires-Dist: xarray>=0.19.0
+Requires-Dist: matplotlib!=3.5.0
+Requires-Dist: lmfit>=1.0.3
+Requires-Dist: pyqt5>5.15.2
+Requires-Dist: pyqtgraph
+Requires-Dist: jsonschema
+Requires-Dist: adaptive
+Requires-Dist: filelock
+Requires-Dist: appnope
+Requires-Dist: uncertainties
+Requires-Dist: dataclasses_json
+Requires-Dist: dill
+Requires-Dist: methodtools
+Requires-Dist: deepdiff
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: pydata-sphinx-theme; extra == "docs"
+Requires-Dist: myst-nb; extra == "docs"
+Requires-Dist: rich[jupyter]; extra == "docs"
+Requires-Dist: scanpydoc; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
+Requires-Dist: sphinx-jsonschema>=1.15; extra == "docs"
+Requires-Dist: sphinx-togglebutton; extra == "docs"
+Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
+Requires-Dist: sphinx-design; extra == "docs"
+Requires-Dist: jupyter_sphinx>=0.4.0; extra == "docs"
+Provides-Extra: dev
+Requires-Dist: quantify-core[docs,test]; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: nbstripout; extra == "dev"
+Requires-Dist: scikit-optimize; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pre-commit-hooks; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pyright; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: sphinx-autobuild; extra == "dev"
+
+# quantify-core
+
+[![Slack](https://img.shields.io/badge/slack-chat-green.svg)](https://quantify-os.org/slack.html#sec-slack)
+[![Pipelines](https://gitlab.com/quantify-os/quantify-core/badges/main/pipeline.svg)](https://gitlab.com/quantify-os/quantify-core/-/pipelines/)
+[![PyPi](https://img.shields.io/pypi/v/quantify-core.svg)](https://pypi.org/pypi/quantify-core)
+[![Code Quality](https://app.codacy.com/project/badge/Grade/32265e1e7d3f491fa028528aaf8bfa69)](https://app.codacy.com/gl/quantify-os/quantify-core/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-core&amp;utm_campaign=Badge_Grade)
+[![Coverage](https://app.codacy.com/project/badge/Coverage/32265e1e7d3f491fa028528aaf8bfa69)](https://app.codacy.com/gl/quantify-os/quantify-core/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-core&amp;utm_campaign=Badge_Coverage)
+[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://gitlab.com/quantify-os/quantify-core/-/blob/main/LICENSE)
+[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=flat)](https://unitary.fund)
+[![Documentation](https://img.shields.io/badge/documentation-grey)](https://quantify-os.org/docs/quantify-core)
+
+![Quantify logo](https://gitlab.com/quantify-os/quantify-core/-/raw/main/docs/source/images/QUANTIFY_LANDSCAPE.svg)
+
+Quantify is a Python-based data acquisition framework focused on Quantum Computing and
+solid-state physics experiments.
+The framework consists of [quantify-core](https://pypi.org/project/quantify-core/) ([git](https://gitlab.com/quantify-os/quantify-core/) | [docs](https://quantify-os.org/docs/quantify-core))
+and [quantify-scheduler](https://pypi.org/project/quantify-scheduler/) ([git](https://gitlab.com/quantify-os/quantify-scheduler/) | [docs](https://quantify-os.org/docs/quantify-scheduler)).
+It is built on top of [QCoDeS](https://qcodes.github.io/Qcodes/)
+and is a spiritual successor of [PycQED](https://github.com/DiCarloLab-Delft/PycQED_py3).
+`quantify-core` is the core module that contains all basic functionality to control experiments. This includes:
+
+- A framework to control instruments.
+- A data-acquisition loop.
+- Data storage and analysis.
+- Parameter monitoring and live visualization of experiments.
+
+## Overview and Community
+
+For a general overview of Quantify and connecting to its open-source community, see [quantify-os.org](https://quantify-os.org/).
+Quantify is maintained by the Quantify Consortium consisting of Qblox and Orange Quantum Systems.
+
+[<img src="https://gitlab.com/quantify-os/quantify-core/-/raw/main/docs/source/images/Qblox_logo.svg" alt="Qblox logo" width=200px/>](https://qblox.com)
+&nbsp;
+&nbsp;
+&nbsp;
+&nbsp;
+[<img src="https://gitlab.com/quantify-os/quantify-core/-/raw/main/docs/source/images/OQS_logo_with_text.svg" alt="Orange Quantum Systems logo" width=200px/>](https://orangeqs.com)
+
+&nbsp;
+
+The software is free to use under the conditions specified in the [license](https://gitlab.com/quantify-os/quantify-core/-/raw/main/LICENSE).
```

### Comparing `quantify-core-0.7.4/quantify_core.egg-info/SOURCES.txt` & `quantify-core-0.7.5/quantify_core.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -42,18 +42,20 @@
 quantify_core.egg-info/dependency_links.txt
 quantify_core.egg-info/not-zip-safe
 quantify_core.egg-info/requires.txt
 quantify_core.egg-info/top_level.txt
 quantify_core/analysis/__init__.py
 quantify_core/analysis/base_analysis.py
 quantify_core/analysis/calibration.py
+quantify_core/analysis/conditional_oscillation_analysis.py
 quantify_core/analysis/cosine_analysis.py
 quantify_core/analysis/fitting_models.py
 quantify_core/analysis/interpolation_analysis.py
 quantify_core/analysis/optimization_analysis.py
+quantify_core/analysis/readout_calibration_analysis.py
 quantify_core/analysis/single_qubit_timedomain.py
 quantify_core/analysis/spectroscopy_analysis.py
 quantify_core/analysis/time_of_flight_analysis.py
 quantify_core/analysis/types.py
 quantify_core/analysis/schemas/AnalysisSettings.json
 quantify_core/analysis/schemas/__init__.py
 quantify_core/data/__init__.py
@@ -89,18 +91,22 @@
 quantify_core/visualization/pyqt_plotmon_remote.py
 quantify_core/visualization/ins_mon_widget/__init__.py
 quantify_core/visualization/ins_mon_widget/qc_snapshot_widget.py
 tests/__init__.py
 tests/test_headers_and_copyright.py
 tests/analysis/test_base_analysis.py
 tests/analysis/test_calibration.py
+tests/analysis/test_conditional_oscillation.py
 tests/analysis/test_fitting_models.py
 tests/analysis/test_interpolation_analysis.py
 tests/analysis/test_optimization_analysis.py
+tests/analysis/test_qubit_flux_spectroscopy.py
 tests/analysis/test_qubit_spectroscopy.py
+tests/analysis/test_readout_calibration.py
+tests/analysis/test_resonator_flux_spectroscopy.py
 tests/analysis/test_single_qubit_timedomain.py
 tests/analysis/test_spectroscopy_analysis.py
 tests/analysis/test_time_of_flight_analysis.py
 tests/analysis/test_types.py
 tests/data/__init__.py
 tests/data/test_data_handling.py
 tests/data/test_experiment.py
@@ -155,15 +161,30 @@
 tests/test_data/20220509/20220509-204728-327-69b211-load_settings_test_nested/snapshot.json
 tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/dataset.hdf5
 tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
 tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/dataset.hdf5
 tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
 tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/dataset.hdf5
 tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
+tests/test_data/20230308/20230308-235659-059-cf471e-ResonatorFluxSpectroscopy/dataset.hdf5
+tests/test_data/20230308/20230308-235659-059-cf471e-ResonatorFluxSpectroscopy/analysis_ResonatorFluxSpectroscopyAnalysis/fit_results/sin.txt
+tests/test_data/20230309/20230309-235228-129-1a58f5-ResonatorFluxSpectroscopy/dataset.hdf5
+tests/test_data/20230309/20230309-235228-129-1a58f5-ResonatorFluxSpectroscopy/analysis_ResonatorFluxSpectroscopyAnalysis/fit_results/sin.txt
+tests/test_data/20230309/20230309-235354-353-9c94c5-QubitSpectroscopy/dataset.hdf5
 tests/test_data/20230508/20230508-122129-027-38881c-QubitSpectroscopy_q3/dataset.hdf5
+tests/test_data/20230509/20230509-135911-755-9471f2-ReadoutCalibration/dataset.hdf5
+tests/test_data/20230509/20230509-135911-755-9471f2-ReadoutCalibration/analysis_ReadoutCalibrationAnalysis/fit_results/linear_discriminator.txt
+tests/test_data/20230509/20230509-135927-693-0977e0-ReadoutCalibration/dataset.hdf5
+tests/test_data/20230509/20230509-152441-841-faef49-ReadoutCalibration/dataset.hdf5
+tests/test_data/20230509/20230509-165523-132-dcfea7-ConditionalOscillation/dataset.hdf5
+tests/test_data/20230509/20230509-165651-504-cabfd0-ConditionalOscillation/dataset.hdf5
+tests/test_data/20230509/20230509-165733-096-5016ba-ConditionalOscillation/dataset.hdf5
+tests/test_data/20230509/20230509-165820-224-324d99-ConditionalOscillation/dataset.hdf5
+tests/test_data/20230509/20230509-165850-578-8a48c2-ConditionalOscillation/dataset.hdf5
+tests/test_data/20230523/20230523-110858-666-7a7dbb-QubitFluxSpectroscopy_q2/dataset.hdf5
 tests/test_data/20230523/20230523-114322-399-dacb68-QubitSpectroscopy_q0/dataset.hdf5
 tests/test_data/20230523/20230523-175716-868-8746ad-QubitSpectroscopy_q2/dataset.hdf5
 tests/test_data/20230927/20230927-143514-589-e1a20e-time_of_light_calibration_fit_fail/dataset.hdf5
 tests/test_data/20230927/20230927-143533-006-fe2167-time_of_light_calibration/dataset.hdf5
 tests/test_data/empty/nothing
 tests/utilities/__init__.py
 tests/utilities/test_deprecation.py
```

### Comparing `quantify-core-0.7.4/quantify_core.egg-info/requires.txt` & `quantify-core-0.7.5/quantify_core.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -39,11 +39,12 @@
 rich[jupyter]
 scanpydoc
 sphinx-autodoc-typehints
 sphinx-jsonschema>=1.15
 sphinx-togglebutton
 sphinxcontrib-bibtex
 sphinx-design
+jupyter_sphinx>=0.4.0
 
 [test]
 pytest
 pytest-mock
```

### Comparing `quantify-core-0.7.4/setup.py` & `quantify-core-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/analysis/test_base_analysis.py` & `quantify-core-0.7.5/tests/analysis/test_base_analysis.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/analysis/test_calibration.py` & `quantify-core-0.7.5/tests/analysis/test_calibration.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/analysis/test_fitting_models.py` & `quantify-core-0.7.5/tests/analysis/test_fitting_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for analysis fitting models"""
+
 import numpy as np
 import pytest
 
 import quantify_core.data.handling as dh
 from quantify_core.analysis import fitting_models as fm
```

### Comparing `quantify-core-0.7.4/tests/analysis/test_interpolation_analysis.py` & `quantify-core-0.7.5/tests/analysis/test_interpolation_analysis.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/analysis/test_optimization_analysis.py` & `quantify-core-0.7.5/tests/analysis/test_optimization_analysis.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/analysis/test_qubit_spectroscopy.py` & `quantify-core-0.7.5/tests/analysis/test_qubit_spectroscopy.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/analysis/test_single_qubit_timedomain.py` & `quantify-core-0.7.5/tests/analysis/test_single_qubit_timedomain.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/analysis/test_spectroscopy_analysis.py` & `quantify-core-0.7.5/tests/analysis/test_spectroscopy_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     container = Path(dh.locate_experiment_container(analysis.tuid))
     file_path = (
         container / "analysis_ResonatorSpectroscopyAnalysis" / "dataset_processed.hdf5"
     )
     dataset_processed = dh.load_dataset_from_path(file_path)
 
-    assert "x0" in dataset_processed.dims.keys()
+    assert "x0" in dataset_processed.dims
     assert "x0" in dataset_processed.coords.keys()
     assert "y0" not in dataset_processed.data_vars.keys()
     assert "y1" not in dataset_processed.data_vars.keys()
     assert "S21" in dataset_processed.data_vars.keys()
 
 
 def test_figures_generated(analysis_and_ref):
```

### Comparing `quantify-core-0.7.4/tests/analysis/test_time_of_flight_analysis.py` & `quantify-core-0.7.5/tests/analysis/test_time_of_flight_analysis.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/analysis/test_types.py` & `quantify-core-0.7.5/tests/analysis/test_types.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/data/test_data_handling.py` & `quantify-core-0.7.5/tests/data/test_data_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     y0 = dataset["y0"]
     assert isinstance(y0, xr.DataArray)
     assert y0.attrs["units"] == "V"
     assert y0.attrs["name"] == "y"
     assert y0.attrs["long_name"] == "Signal amplitude"
 
     assert set(dataset.coords.keys()) == {"x0"}
-    assert set(dataset.dims.keys()) == {"dim_0"}
+    assert set(dataset.dims) == {"dim_0"}
 
 
 def test_initialize_dataset_2d():
     xpar = ManualParameter("x", unit="m", label="X position")
     ypar = ManualParameter("y", unit="m", label="Y position")
     getpar = ManualParameter("z", unit="V", label="Signal amplitude")
     setable_pars = [xpar, ypar]
@@ -471,15 +471,15 @@
 
 def test_dynamic_dataset():
     x = ManualParameter("x", unit="m", label="X position")
     y = ManualParameter("y", unit="m", label="Y position")
     z = ManualParameter("z", unit="V", label="Signal amplitude")
     settables = [x, y]
     gettables = [z]
-    dset = dh.initialize_dataset(settables, np.empty((8, len(settables))), gettables)
+    dset = dh.initialize_dataset(settables, np.empty((len(settables), 8)), gettables)
 
     x0_vals = np.random.random(8)
     x1_vals = np.random.random(8)
     y0_vals = np.random.random(8)
     dset["x0"].values[:] = x0_vals
     dset["x1"].values[:] = x1_vals
     dset["y0"].values[:] = y0_vals
@@ -527,17 +527,17 @@
 def test_to_gridded_dataset(tmp_test_data_dir):
     dh.set_datadir(tmp_test_data_dir)
     tuid = "20200504-191556-002-4209ee"
     dset_orig = dh.load_dataset(tuid)
     dset_gridded = dh.to_gridded_dataset(dset_orig)
 
     assert dset_gridded.attrs["tuid"] == tuid
-    assert tuple(dset_gridded.dims.keys()) == ("x0", "x1")
+    assert tuple(dset_gridded.dims) == ("x0", "x1")
     assert tuple(dset_gridded.coords.keys()) == ("x0", "x1")
-    assert tuple(dset_gridded.dims.values()) == (50, 11)
+    assert tuple(dset_gridded.sizes.values()) == (50, 11)
     assert dset_gridded["y0"].dims == ("x0", "x1")
     assert len(dset_gridded["x0"].values) == len(np.unique(dset_orig["x0"]))
 
     for var in ("x0", "x1", "y0"):
         assert dset_orig[var].attrs == dset_gridded[var].attrs
 
     y0 = dset_gridded["y0"].values
```

### Comparing `quantify-core-0.7.4/tests/data/test_experiment.py` & `quantify-core-0.7.5/tests/data/test_experiment.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/data/test_types.py` & `quantify-core-0.7.5/tests/data/test_types.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/measurement/test_measurement_control.py` & `quantify-core-0.7.5/tests/measurement/test_measurement_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,23 +286,23 @@
     )
     assert repr2 == expected
 
 
 def test_setpoints(meas_ctrl):
     x = np.linspace(0, 10, 11)
     meas_ctrl.setpoints(x)
-    assert np.array_equal(meas_ctrl._setpoints[:, 0], x)
+    assert np.array_equal(meas_ctrl._setpoints[0], x)
 
     x = np.random.rand(15, 2)
     meas_ctrl.setpoints(x)
-    assert np.array_equal(meas_ctrl._setpoints, x)
+    assert np.array_equal(meas_ctrl._setpoints, x.T)
 
     x = np.random.rand(15, 4)
     meas_ctrl.setpoints(x)
-    assert np.array_equal(meas_ctrl._setpoints, x)
+    assert np.array_equal(meas_ctrl._setpoints, x.T)
 
 
 def test_iterative_1d(meas_ctrl, parameters):
     xvals = np.linspace(0, 2 * np.pi, 31)
 
     meas_ctrl.settables(parameters.t)
     meas_ctrl.setpoints(xvals)
@@ -483,19 +483,19 @@
     dset = meas_ctrl.run()
 
     assert np.array_equal(meas_ctrl._setpoints, exp_sp)
 
     assert TUID.is_valid(dset.attrs["tuid"])
 
     expected_vals = cosine_function(
-        t=exp_sp[:, 0], amplitude=exp_sp[:, 1], frequency=1, phase=0
+        t=exp_sp[0], amplitude=exp_sp[1], frequency=1, phase=0
     )
 
-    assert np.array_equal(dset["x0"].values, exp_sp[:, 0])
-    assert np.array_equal(dset["x1"].values, exp_sp[:, 1])
+    assert np.array_equal(dset["x0"].values, exp_sp[0])
+    assert np.array_equal(dset["x1"].values, exp_sp[1])
     assert np.array_equal(dset["y0"].values, expected_vals)
 
     # Test properties of the dataset
     assert isinstance(dset, xr.Dataset)
     assert set(dset.variables.keys()) == {"x0", "x1", "y0"}
 
     assert all(e in dset["x0"].values for e in times)
@@ -561,19 +561,19 @@
         assert parameters.amp.set.call_count == 20 * 5
 
     assert np.array_equal(meas_ctrl._setpoints, exp_sp)
 
     assert TUID.is_valid(dset.attrs["tuid"])
 
     expected_vals = cosine_function(
-        t=exp_sp[:, 0], amplitude=exp_sp[:, 1], frequency=1, phase=0
+        t=exp_sp[0], amplitude=exp_sp[1], frequency=1, phase=0
     )
 
-    assert np.array_equal(dset["x0"].values, exp_sp[:, 0])
-    assert np.array_equal(dset["x1"].values, exp_sp[:, 1])
+    assert np.array_equal(dset["x0"].values, exp_sp[0])
+    assert np.array_equal(dset["x1"].values, exp_sp[1])
     assert np.array_equal(dset["y0"].values, expected_vals)
 
     # Test properties of the dataset
     assert set(dset.variables.keys()) == {"x0", "x1", "y0"}
 
     assert all(e in dset["x0"].values for e in times)
     assert all(e in dset["x1"].values for e in amps)
@@ -660,16 +660,16 @@
     meas_ctrl.settables(settables)
     meas_ctrl.setpoints_grid([times, amps])
     meas_ctrl.gettables(gettable)
     dset = meas_ctrl.run("2D batched", save_data=False)
 
     exp_sp = grid_setpoints([times, amps])
     assert np.array_equal(exp_sp, meas_ctrl._setpoints)
-    assert np.array_equal(dset["x0"].values, exp_sp[:, 0])
-    assert np.array_equal(dset["x1"].values, exp_sp[:, 1])
+    assert np.array_equal(dset["x0"].values, exp_sp[0])
+    assert np.array_equal(dset["x1"].values, exp_sp[1])
 
     expected_vals = batched_mock_values(dset["x0"].values)
     assert np.array_equal(dset["y0"].values, expected_vals)
 
     # Test properties of the dataset
     assert isinstance(dset, xr.Dataset)
 
@@ -711,17 +711,18 @@
 
     # Must be specified otherwise all setpoints will be passed to the settable
     parameters.sig.batch_size = len(times)
     parameters.sig.batched = True
 
     dset = meas_ctrl.run("iterative-outer-loop-with-inner-batched-2D")
 
+    np_array_setpoints = meas_ctrl._setpoints
     expected_vals = cosine_function(
-        t=meas_ctrl._setpoints[:, 0],
-        frequency=meas_ctrl._setpoints[:, 1],
+        t=np_array_setpoints[0],
+        frequency=np_array_setpoints[1],
         amplitude=1,
         phase=0,
     )
     assert np.array_equal(dset["y0"].values, expected_vals)
 
 
 def test_batched_2d_grid_multi_return(meas_ctrl):
@@ -735,16 +736,16 @@
     meas_ctrl.settables(settables)
     meas_ctrl.setpoints_grid([times, amps])
     meas_ctrl.gettables(gettable)
     dset = meas_ctrl.run("2D batched multi return")
 
     exp_sp = grid_setpoints([times, amps])
     assert np.array_equal(exp_sp, meas_ctrl._setpoints)
-    assert np.array_equal(dset["x0"].values, exp_sp[:, 0])
-    assert np.array_equal(dset["x1"].values, exp_sp[:, 1])
+    assert np.array_equal(dset["x0"].values, exp_sp[0])
+    assert np.array_equal(dset["x1"].values, exp_sp[1])
 
     expected_vals = batched_mock_values(
         np.stack((dset["x0"].values, dset["x1"].values))
     )
     assert np.array_equal(dset["y0"].values, expected_vals[0])
     assert np.array_equal(dset["y1"].values, expected_vals[1])
 
@@ -879,20 +880,20 @@
     dset = meas_ctrl.run()
 
     assert np.array_equal(meas_ctrl._setpoints, exp_sp)
 
     assert TUID.is_valid(dset.attrs["tuid"])
 
     expected_vals = cosine_function(
-        t=exp_sp[:, 0], amplitude=exp_sp[:, 1], frequency=exp_sp[:, 2], phase=0
+        t=exp_sp[0], amplitude=exp_sp[1], frequency=exp_sp[2], phase=0
     )
 
-    assert np.array_equal(dset["x0"].values, exp_sp[:, 0])
-    assert np.array_equal(dset["x1"].values, exp_sp[:, 1])
-    assert np.array_equal(dset["x2"].values, exp_sp[:, 2])
+    assert np.array_equal(dset["x0"].values, exp_sp[0])
+    assert np.array_equal(dset["x1"].values, exp_sp[1])
+    assert np.array_equal(dset["x2"].values, exp_sp[2])
     assert np.array_equal(dset["y0"].values, expected_vals)
 
     # Test properties of the dataset
     assert isinstance(dset, xr.Dataset)
     assert set(dset.variables.keys()) == {"x0", "x1", "x2", "y0"}
     assert all(e in dset["x0"] for e in times)
     assert all(e in dset["x1"] for e in amps)
@@ -926,18 +927,18 @@
     meas_ctrl.settables([parameters.t, parameters.amp, parameters.freq])
     meas_ctrl.setpoints_grid([times, amps, freqs])
     meas_ctrl.gettables([parameters.DualWave(), parameters.sig, parameters.DualWave()])
     dset = meas_ctrl.run()
 
     exp_sp = grid_setpoints([times, amps, freqs])
     exp_y0 = exp_y3 = sine_function(
-        t=exp_sp[:, 0], amplitude=exp_sp[:, 1], frequency=exp_sp[:, 2], phase=0
+        t=exp_sp[0], amplitude=exp_sp[1], frequency=exp_sp[2], phase=0
     )
     exp_y1 = exp_y2 = exp_y4 = cosine_function(
-        t=exp_sp[:, 0], amplitude=exp_sp[:, 1], frequency=exp_sp[:, 2], phase=0
+        t=exp_sp[0], amplitude=exp_sp[1], frequency=exp_sp[2], phase=0
     )
 
     np.testing.assert_array_equal(dset["y0"], exp_y0)
     np.testing.assert_array_equal(dset["y1"], exp_y1)
     np.testing.assert_array_equal(dset["y2"], exp_y2)
     np.testing.assert_array_equal(dset["y3"], exp_y3)
     np.testing.assert_array_equal(dset["y4"], exp_y4)
@@ -963,20 +964,20 @@
 
     meas_ctrl.settables([batched_settable_t, batched_settable_0, batched_settable_1])
     meas_ctrl.setpoints_grid([times, amps, freqs])
     meas_ctrl.gettables([noisy_gettable, nd_gettable])
     dset = meas_ctrl.run(soft_avg=1000)
 
     exp_sp = grid_setpoints([times, amps, freqs])
-    np.testing.assert_array_almost_equal(dset.y0, exp_sp[:, 0], decimal=2)
+    np.testing.assert_array_almost_equal(dset.y0, exp_sp[0], decimal=2)
     np.testing.assert_array_almost_equal(
-        dset.y1, batched_mock_values(exp_sp[:, 1]), decimal=4
+        dset.y1, batched_mock_values(exp_sp[1]), decimal=4
     )
     np.testing.assert_array_almost_equal(
-        dset.y2, batched_mock_values(exp_sp[:, 2]), decimal=4
+        dset.y2, batched_mock_values(exp_sp[2]), decimal=4
     )
 
 
 def test_batched_attr_raises(meas_ctrl, parameters):
     times = np.linspace(0, 5, 3)
     freqs = np.linspace(41000, 82000, 8)
 
@@ -1025,15 +1026,14 @@
     assert not isinstance(parameters.t(), Iterable)
     assert isinstance(parameters.other_freq(), Iterable)
     assert not isinstance(parameters.amp(), Iterable)
 
     exp_sp = grid_setpoints(setpoints, settables=settables)
     assert np.array_equal(meas_ctrl._setpoints, exp_sp)
 
-    exp_sp = exp_sp.T
     _, _, _, _ = (
         parameters.freq(exp_sp[0]),
         parameters.t(exp_sp[1]),
         parameters.other_freq(exp_sp[2]),
         parameters.amp(exp_sp[3]),
     )
     assert np.array_equal(dset["y0"].values, parameters.sig2())
@@ -1148,18 +1148,21 @@
     dummy_parabola.noise(0)
     meas_ctrl.settables([dummy_parabola.x, dummy_parabola.y])
 
     num_x = 5
     num_y = 20
 
     def _adaptive_function(meas_func, **_):
-        """A dimple adaptive function that executes a 2D sweep and conforms with
+        """A simple adaptive function that executes a 2D sweep and conforms with
         the accepted interface for an adaptive function."""
-        points = grid_setpoints(
-            [np.linspace(-50, 50, num_x), np.linspace(-20, 30, num_y)]
+        points = np.column_stack(
+            [
+                np.tile(np.linspace(-50, 50, num_x), num_y),
+                np.repeat(np.linspace(-20, 30, num_y), num_x),
+            ],
         )
 
         for setpoint in points:
             _ = meas_func(setpoint)
 
         # The meas_ctrl takes care of intercepting the measured values so no return
         # is specified here
@@ -1473,15 +1476,15 @@
     setpoints = [(next(it_b) if m else next(it_i)) for m in batched_mask]
     gridded = grid_setpoints(setpoints, settables=settables)
     expected = np.column_stack(
         [
             np.tile(setpoints_batched[0], len(setpoints_iterative[0])),
             np.repeat(setpoints_iterative[0], len(setpoints_batched[0])),
         ]
-    )
+    ).T
     np.testing.assert_array_equal(gridded, expected)
 
 
 def test_grid_setpoints_mixed_two_batched(setpoints_iterative, setpoints_batched):
     # Several batched settables
     batched_mask = [False, True, True]
     settables = make_settable_set(batched_mask)
@@ -1500,15 +1503,15 @@
                 len(setpoints_iterative[0]) * len(setpoints_batched[1]),
             ),
             np.tile(
                 np.repeat(setpoints_batched[1], len(setpoints_batched[0])),
                 len(setpoints_iterative[0]),
             ),
         ]
-    )
+    ).T
     np.testing.assert_array_equal(gridded, expected)
 
 
 def test_grid_setpoints_mixed_two_batched_two_iterative(
     setpoints_iterative, setpoints_batched
 ):
     # Several batched settables and several iterative settables
@@ -1541,31 +1544,88 @@
             np.tile(
                 setpoints_batched[1],
                 len(setpoints_iterative[0])
                 * len(setpoints_iterative[1])
                 * len(setpoints_batched[0]),
             ),
         ]
-    )
+    ).T
     np.testing.assert_array_equal(gridded, expected)
 
 
 def test_grid_setpoints():
     x = np.arange(5)
     y = np.linspace(-1, 1, 3)
 
     sp = grid_setpoints([x, y])
-    assert sp[:, 0].all() == np.tile(np.arange(5), 3).all()
-    assert sp[:, 1].all() == np.repeat(y, 5).all()
+    assert sp[0].all() == np.tile(np.arange(5), 3).all()
+    assert sp[1].all() == np.repeat(y, 5).all()
 
     z = np.linspace(100, 200, 2)
     sp = grid_setpoints([x, y, z])
-    assert all(e in sp[:, 0] for e in x)
-    assert all(e in sp[:, 1] for e in y)
-    assert all(e in sp[:, 2] for e in z)
+    assert all(e in sp[0] for e in x)
+    assert all(e in sp[1] for e in y)
+    assert all(e in sp[2] for e in z)
+
+
+def test_typed_settables(meas_ctrl, parameters):
+    times = np.linspace(0, 5, 20)
+    atts = list(range(0, 60, 10))
+    att_settable = ManualParameter(
+        "out0_att",
+        label="Output 0 attenuation",
+        unit="dB",
+        vals=vals.Multiples(2, min_value=0, max_value=60),
+        set_parser=int,
+        get_parser=int,
+    )
+
+    meas_ctrl.settables([parameters.t, att_settable])
+    meas_ctrl.setpoints_grid([times, atts])
+
+    meas_ctrl.gettables(parameters.sig)
+    # Should not raise TypeError
+    _ = meas_ctrl.run()
+
+
+def test_typed_settables_batched(meas_ctrl):
+    times = list(range(20))
+    freqs = list(range(1, 11))
+    setpoints = [times, freqs]
+    meas_ctrl.setpoints_grid(setpoints)
+
+    strict_t = ManualParameter(
+        "time",
+        unit="s",
+        vals=vals.Arrays(valid_types=[int]),
+    )
+    strict_freq = ManualParameter(
+        "frequency",
+        unit="Hz",
+        vals=vals.Ints(),
+    )
+    meas_ctrl.settables([strict_t, strict_freq])
+
+    # Using the same gettable for test purposes
+    def cosine_model():
+        return cosine_function(
+            strict_t(), amplitude=1, frequency=strict_freq(), phase=0
+        )
+
+    sig = Parameter(name="sig", label="Signal level", unit="V", get_cmd=cosine_model)
+    meas_ctrl.gettables([sig, sig])
+
+    strict_t.batched = True
+    strict_freq.batched = False
+
+    sig.batch_size = len(times)
+    sig.batched = True
+
+    # Should not raise TypeError
+    _ = meas_ctrl.run("iterative-outer-loop-with-inner-batched-2D")
 
 
 def test_print_progress_no_setpoints(meas_ctrl_empty, mocker):
     mocker.patch(
         "quantify_core.measurement.control.MeasurementControl._get_fracdone",
         side_effect=[0],
     )
```

### Comparing `quantify-core-0.7.4/tests/measurement/test_types.py` & `quantify-core-0.7.5/tests/measurement/test_types.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20200430/20200430-170837-001-315f36-Cosine test/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20200430/20200430-170837-001-315f36-Cosine test/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20200504/20200504-191556-002-4209ee-2D Cosine test/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20200504/20200504-191556-002-4209ee-2D Cosine test/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20200814/20200814-134652-492-fbf254-save/snapshot.json` & `quantify-core-0.7.5/tests/test_data/20200814/20200814-134652-492-fbf254-save/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20201124/20201124-184709-137-8a5112-(0) Spec IF=0.000 MHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20201124/20201124-184709-137-8a5112-(0) Spec IF=0.000 MHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20201124/20201124-184716-237-918bee-(1) Spec IF=20.000 MHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20201124/20201124-184716-237-918bee-(1) Spec IF=20.000 MHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20201124/20201124-184722-988-0463d4-(2) Spec IF=-20.000 MHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20201124/20201124-184722-988-0463d4-(2) Spec IF=-20.000 MHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20201124/20201124-184729-618-85970f-(3) Spec IF=40.000 MHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20201124/20201124-184729-618-85970f-(3) Spec IF=40.000 MHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20201124/20201124-184736-341-3628d4-(4) Spec IF=-40.000 MHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20201124/20201124-184736-341-3628d4-(4) Spec IF=-40.000 MHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/snapshot.json` & `quantify-core-0.7.5/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/snapshot.json` & `quantify-core-0.7.5/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210227/20210227-172939-723-53d82c-Resonator_power_id6_4.612GHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210227/20210227-172939-723-53d82c-Resonator_power_id6_4.612GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210227/20210227-174714-680-31df85-Resonator_id7_4.660GHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210227/20210227-174714-680-31df85-Resonator_id7_4.660GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210305/.DS_Store` & `quantify-core-0.7.5/tests/test_data/20210305/.DS_Store`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210305/20210305-152943-497-ad8670-Resonator_id2_4.483GHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210305/20210305-152943-497-ad8670-Resonator_id2_4.483GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210305/20210305-154735-413-142768-Resonator_id2_4.483GHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210305/20210305-154735-413-142768-Resonator_id2_4.483GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210305/20210305-160157-184-3c17e9-Resonator_id4_4.541GHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210305/20210305-160157-184-3c17e9-Resonator_id4_4.541GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210305/20210305-161550-671-982c6d-Resonator_id5_4.577GHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210305/20210305-161550-671-982c6d-Resonator_id5_4.577GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210319/20210319-094728-327-69b211-load_settings_test/snapshot.json` & `quantify-core-0.7.5/tests/test_data/20210319/20210319-094728-327-69b211-load_settings_test/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210322/20210322-205253-758-6689ca-T1 at 4.715GHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210322/20210322-205253-758-6689ca-T1 at 4.715GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210331/20210331-133734-718-aa9c83 AllXY q0/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210331/20210331-133734-718-aa9c83 AllXY q0/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210419/20210419-153127-883-fa4508-Rabi oscillation at 4.515GHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210419/20210419-153127-883-fa4508-Rabi oscillation at 4.515GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210419/20210419-170747-902-9c5a05-Offset_calibration/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210419/20210419-170747-902-9c5a05-Offset_calibration/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210419/20210419-173649-456-23c5f3-AllXY q0/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210419/20210419-173649-456-23c5f3-AllXY q0/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210420/20210420-001339-580-97bdef-Echo at 4.715GHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210420/20210420-001339-580-97bdef-Echo at 4.715GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210422/20210422-104958-297-7d6034-Ramsey oscillation at 4.715GHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210422/20210422-104958-297-7d6034-Ramsey oscillation at 4.715GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210827/20210827-174946-357-70a986-T1 experiment q0/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210827/20210827-174946-357-70a986-T1 experiment q0/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210827/20210827-175004-087-ab1aab-Ramsey oscillation q0 at 4.9969 GHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210827/20210827-175004-087-ab1aab-Ramsey oscillation q0 at 4.9969 GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210827/20210827-175021-521-251f28-Echo experiment q0/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210827/20210827-175021-521-251f28-Echo experiment q0/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20210901/20210901-132357-561-5c3ef7-Ramsey oscillation q0 at 6.1400 GHz/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20210901/20210901-132357-561-5c3ef7-Ramsey oscillation q0 at 6.1400 GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5` & `quantify-core-0.7.5/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/snapshot.json` & `quantify-core-0.7.5/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5` & `quantify-core-0.7.5/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/snapshot.json` & `quantify-core-0.7.5/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5` & `quantify-core-0.7.5/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/snapshot.json` & `quantify-core-0.7.5/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/snapshot.json` & `quantify-core-0.7.5/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20220509/20220509-204728-327-69b211-load_settings_test_nested/snapshot.json` & `quantify-core-0.7.5/tests/test_data/20220509/20220509-204728-327-69b211-load_settings_test_nested/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5` & `quantify-core-0.7.5/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5` & `quantify-core-0.7.5/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5` & `quantify-core-0.7.5/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20230508/20230508-122129-027-38881c-QubitSpectroscopy_q3/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20230508/20230508-122129-027-38881c-QubitSpectroscopy_q3/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20230523/20230523-114322-399-dacb68-QubitSpectroscopy_q0/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20230523/20230523-114322-399-dacb68-QubitSpectroscopy_q0/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20230523/20230523-175716-868-8746ad-QubitSpectroscopy_q2/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20230523/20230523-175716-868-8746ad-QubitSpectroscopy_q2/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20230927/20230927-143514-589-e1a20e-time_of_light_calibration_fit_fail/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20230927/20230927-143514-589-e1a20e-time_of_light_calibration_fit_fail/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/20230927/20230927-143533-006-fe2167-time_of_light_calibration/dataset.hdf5` & `quantify-core-0.7.5/tests/test_data/20230927/20230927-143533-006-fe2167-time_of_light_calibration/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_data/transmon_test_config.json` & `quantify-core-0.7.5/tests/test_data/transmon_test_config.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/test_headers_and_copyright.py` & `quantify-core-0.7.5/tests/test_headers_and_copyright.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/utilities/test_deprecation.py` & `quantify-core-0.7.5/tests/utilities/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/utilities/test_experiment_helpers.py` & `quantify-core-0.7.5/tests/utilities/test_experiment_helpers.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/utilities/test_general.py` & `quantify-core-0.7.5/tests/utilities/test_general.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/utilities/test_inspect_utils.py` & `quantify-core-0.7.5/tests/utilities/test_inspect_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Unit tests for inspect_utils module."""
+
 # pylint: disable=missing-class-docstring
 # pylint: disable=missing-function-docstring
 from quantify_core.utilities import inspect_utils
 
 
 def test_get_classes() -> None:
     # Arrange
```

### Comparing `quantify-core-0.7.4/tests/visualization/test_SI_utilities.py` & `quantify-core-0.7.5/tests/visualization/test_SI_utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,24 @@
     assert "$\\Phi_0$" == post_unit
 
     unit = None
     scale_factor, post_unit = SI_prefix_and_scale_factor(val=5000.4, unit=unit)
     assert scale_factor == 1
     assert not post_unit
 
+    unit = "s"
+    scale_factor, post_unit = SI_prefix_and_scale_factor(val=150, unit=unit)
+    assert scale_factor == 1 / 60
+    assert post_unit == "min"
+
+    unit = "s"
+    scale_factor, post_unit = SI_prefix_and_scale_factor(val=10000, unit=unit)
+    assert scale_factor == 1 / 3600
+    assert post_unit == "hrs"
+
 
 def test_label_scaling() -> None:
     """
     This test creates a dummy plot and checks if the tick labels are
     rescaled correctly
     """
     _, ax = plt.subplots()
@@ -95,14 +105,34 @@
         "5",
         "7.5",
         "10",
         "12.5",
     ]
 
 
+def test_set_xlabel_auto_scale() -> None:
+    """
+    This test creates a dummy plot and checks if the tick labels are
+    rescaled correctly
+    """
+    _, ax = plt.subplots()
+    x = np.linspace(-6, 6, 101)
+    y = np.cos(x)
+    ax.plot(x * 10_000, y / 1e3)
+    set_xlabel("Distance", unit="m", auto_scale=False)
+    assert ax.get_xlabel() == "Distance [m]"
+    set_xlabel("Distance", unit="m")
+    assert ax.get_xlabel() == "Distance [km]"
+
+    set_ylabel("Amplitude", unit="V", auto_scale=False)
+    assert ax.get_ylabel() == "Amplitude [V]"
+    set_ylabel("Amplitude", unit="V")
+    assert ax.get_ylabel() == "Amplitude [mV]"
+
+
 def test_adjust_adjust_axeslabels_SI() -> None:
     """
     This test creates a dummy plot and checks if the tick labels are
     rescaled correctly
     """
     _, ax = plt.subplots()
     x = np.linspace(-6, 6, 101)
@@ -295,10 +325,10 @@
 
 
 def test_format_value_ufloat() -> None:
     tau = uncertainties.ufloat(2.0, 0.1)
     formatted_string = format_value_string("tau", tau)
     assert formatted_string == r"tau: 2.00$\pm$0.10 "
 
-    tau = uncertainties.ufloat(0.0, np.NaN)
+    tau = uncertainties.ufloat(0.0, np.nan)
     formatted_string = format_value_string("tau", tau)
     assert formatted_string == r"tau: 0 "
```

### Comparing `quantify-core-0.7.4/tests/visualization/test_instrument_monitor.py` & `quantify-core-0.7.5/tests/visualization/test_instrument_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
         # then change it
         self.inst_mon.update_interval(10)
         assert self.inst_mon.update_interval() == 10
 
 
 class TestRepeatTimer:
-    def setup(self):
+    def setup_method(self):
         self.mock_function = Mock()
         self.repeat_timer = RepeatTimer(
             0.1, self.mock_function, args=(1, 2), kwargs={"a": 3}
         )
 
     def test_attributes_created_during_init(self):
         hasattr(self.repeat_timer, "interval")
```

### Comparing `quantify-core-0.7.4/tests/visualization/test_mpl_plotting.py` & `quantify-core-0.7.5/tests/visualization/test_mpl_plotting.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.4/tests/visualization/test_pyqt_plotmon.py` & `quantify-core-0.7.5/tests/visualization/test_pyqt_plotmon.py`

 * *Files identical despite different names*

