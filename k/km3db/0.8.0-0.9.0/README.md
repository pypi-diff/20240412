# Comparing `tmp/km3db-0.8.0.tar.gz` & `tmp/km3db-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/km3db-0.8.0.tar", last modified: Mon Sep 26 11:39:03 2022, max compression
+gzip compressed data, was "dist/km3db-0.9.0.tar", last modified: Thu Oct  6 22:26:35 2022, max compression
```

## Comparing `km3db-0.8.0.tar` & `km3db-0.9.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:39:03.433260 km3db-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)      284 2022-09-01 11:46:28.000000 km3db-0.8.0/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      422 2022-09-01 11:46:28.000000 km3db-0.8.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2980 2022-09-01 11:46:28.000000 km3db-0.8.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     2201 2022-09-26 11:30:17.000000 km3db-0.8.0/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     1077 2022-09-01 11:46:28.000000 km3db-0.8.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-09-01 11:46:28.000000 km3db-0.8.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      764 2022-09-01 11:46:28.000000 km3db-0.8.0/Makefile
--rw-r--r--   0 root         (0) root         (0)     8538 2022-09-26 11:39:03.433260 km3db-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6492 2022-09-01 11:46:28.000000 km3db-0.8.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:39:03.425260 km3db-0.8.0/benchmarks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:39:03.429260 km3db-0.8.0/benchmarks/cli/
--rwxrwxrwx   0 root         (0) root         (0)      210 2022-09-14 11:56:11.000000 km3db-0.8.0/benchmarks/cli/detx.sh
--rwxrwxrwx   0 root         (0) root         (0)       69 2022-09-01 11:46:28.000000 km3db-0.8.0/benchmarks/cli/runinfo.sh
--rwxrwxrwx   0 root         (0) root         (0)      117 2022-09-01 11:46:28.000000 km3db-0.8.0/benchmarks/cli/streamds.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:39:03.429260 km3db-0.8.0/benchmarks/general/
--rwxrwxrwx   0 root         (0) root         (0)      392 2022-09-01 11:46:28.000000 km3db-0.8.0/benchmarks/general/compass.py
--rwxrwxrwx   0 root         (0) root         (0)       61 2022-09-01 11:46:28.000000 km3db-0.8.0/benchmarks/general/database_api.py
--rwxrwxrwx   0 root         (0) root         (0)      145 2022-09-01 11:46:28.000000 km3db-0.8.0/benchmarks/general/runtable.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:39:03.429260 km3db-0.8.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)      634 2022-09-01 11:46:28.000000 km3db-0.8.0/doc/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:39:03.429260 km3db-0.8.0/doc/_static/
--rw-rw-rw-   0 root         (0) root         (0)       55 2022-09-01 11:46:28.000000 km3db-0.8.0/doc/_static/default.css
--rw-rw-rw-   0 root         (0) root         (0)    24268 2022-09-01 11:46:28.000000 km3db-0.8.0/doc/_static/default_gallery_thumbnail.png
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-09-01 11:46:28.000000 km3db-0.8.0/doc/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2842 2022-09-01 11:46:28.000000 km3db-0.8.0/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       65 2022-09-01 11:46:28.000000 km3db-0.8.0/doc/examples.rst
--rw-rw-rw-   0 root         (0) root         (0)      336 2022-09-01 11:46:28.000000 km3db-0.8.0/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2022-09-01 11:46:28.000000 km3db-0.8.0/doc/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:39:03.425260 km3db-0.8.0/doc/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:39:03.429260 km3db-0.8.0/doc/modules/generated/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-01 11:46:28.000000 km3db-0.8.0/doc/modules/generated/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:39:03.429260 km3db-0.8.0/examples/
--rw-rw-rw-   0 root         (0) root         (0)      126 2022-09-01 11:46:28.000000 km3db-0.8.0/examples/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3577 2022-09-26 11:26:05.000000 km3db-0.8.0/examples/plot_detid_and_run_streams.py
--rw-rw-rw-   0 root         (0) root         (0)     6360 2022-09-26 11:26:05.000000 km3db-0.8.0/examples/plot_run_summary_numbers.py
--rw-rw-rw-   0 root         (0) root         (0)     7688 2022-09-01 11:46:28.000000 km3db-0.8.0/examples/plot_sea_current.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:39:03.429260 km3db-0.8.0/km3db/
--rw-rw-rw-   0 root         (0) root         (0)      198 2022-09-01 11:46:28.000000 km3db-0.8.0/km3db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:39:03.433260 km3db-0.8.0/km3db/cli/
--rw-rw-rw-   0 root         (0) root         (0)     1465 2022-09-26 11:26:05.000000 km3db-0.8.0/km3db/cli/detx.py
--rw-rw-rw-   0 root         (0) root         (0)      525 2022-09-01 11:46:28.000000 km3db-0.8.0/km3db/cli/km3db.py
--rw-rw-rw-   0 root         (0) root         (0)     1916 2022-09-01 11:46:28.000000 km3db-0.8.0/km3db/cli/runinfo.py
--rw-rw-rw-   0 root         (0) root         (0)     2751 2022-09-01 11:46:28.000000 km3db-0.8.0/km3db/cli/runtable.py
--rw-rw-rw-   0 root         (0) root         (0)     7029 2022-09-26 11:26:05.000000 km3db-0.8.0/km3db/cli/streamds.py
--rw-rw-rw-   0 root         (0) root         (0)     1059 2022-09-01 11:46:28.000000 km3db-0.8.0/km3db/cli/wtd.py
--rw-rw-rw-   0 root         (0) root         (0)     1444 2022-09-01 11:46:28.000000 km3db-0.8.0/km3db/compat.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2022-09-26 11:26:05.000000 km3db-0.8.0/km3db/core.py
--rw-rw-rw-   0 root         (0) root         (0)      359 2022-09-01 11:46:28.000000 km3db-0.8.0/km3db/extras.py
--rw-rw-rw-   0 root         (0) root         (0)     5812 2022-09-01 11:46:28.000000 km3db-0.8.0/km3db/logger.py
--rw-rw-rw-   0 root         (0) root         (0)    12846 2022-09-26 11:26:05.000000 km3db-0.8.0/km3db/tools.py
--rw-r--r--   0 root         (0) root         (0)      176 2022-09-26 11:39:03.000000 km3db-0.8.0/km3db/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:39:03.433260 km3db-0.8.0/km3db.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8538 2022-09-26 11:39:03.000000 km3db-0.8.0/km3db.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1171 2022-09-26 11:39:03.000000 km3db-0.8.0/km3db.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-26 11:39:03.000000 km3db-0.8.0/km3db.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      203 2022-09-26 11:39:03.000000 km3db-0.8.0/km3db.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      260 2022-09-26 11:39:03.000000 km3db-0.8.0/km3db.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-09-26 11:39:03.000000 km3db-0.8.0/km3db.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      136 2022-09-01 11:46:28.000000 km3db-0.8.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-09-01 11:46:28.000000 km3db-0.8.0/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:39:03.433260 km3db-0.8.0/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      200 2022-09-01 11:46:28.000000 km3db-0.8.0/requirements/dev.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-09-01 11:46:28.000000 km3db-0.8.0/requirements/extras.txt
--rw-rw-rw-   0 root         (0) root         (0)       36 2022-09-01 11:46:28.000000 km3db-0.8.0/requirements/install.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:39:03.433260 km3db-0.8.0/scripts/
--rwxrwxrwx   0 root         (0) root         (0)    18359 2022-09-01 11:46:28.000000 km3db-0.8.0/scripts/run_benchmarks.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-26 11:39:03.433260 km3db-0.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1699 2022-09-01 11:46:28.000000 km3db-0.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 11:39:03.433260 km3db-0.8.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2248 2022-09-01 11:46:28.000000 km3db-0.8.0/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2022-09-01 11:46:28.000000 km3db-0.8.0/tests/test_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     6479 2022-09-01 11:46:28.000000 km3db-0.8.0/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-06 22:26:35.434614 km3db-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)      284 2022-09-01 11:46:28.000000 km3db-0.9.0/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      422 2022-09-01 11:46:28.000000 km3db-0.9.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2980 2022-09-01 11:46:28.000000 km3db-0.9.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2367 2022-10-06 22:10:51.000000 km3db-0.9.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2022-09-01 11:46:28.000000 km3db-0.9.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       60 2022-09-01 11:46:28.000000 km3db-0.9.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      764 2022-09-01 11:46:28.000000 km3db-0.9.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)     9621 2022-10-06 22:26:35.434614 km3db-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7447 2022-10-06 22:10:51.000000 km3db-0.9.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-06 22:26:35.426614 km3db-0.9.0/benchmarks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-06 22:26:35.430614 km3db-0.9.0/benchmarks/cli/
+-rwxrwxrwx   0 root         (0) root         (0)      210 2022-09-14 11:56:11.000000 km3db-0.9.0/benchmarks/cli/detx.sh
+-rwxrwxrwx   0 root         (0) root         (0)       69 2022-09-01 11:46:28.000000 km3db-0.9.0/benchmarks/cli/runinfo.sh
+-rwxrwxrwx   0 root         (0) root         (0)      261 2022-10-06 22:10:51.000000 km3db-0.9.0/benchmarks/cli/streamds.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-06 22:26:35.430614 km3db-0.9.0/benchmarks/general/
+-rwxrwxrwx   0 root         (0) root         (0)      392 2022-09-01 11:46:28.000000 km3db-0.9.0/benchmarks/general/compass.py
+-rwxrwxrwx   0 root         (0) root         (0)       61 2022-09-01 11:46:28.000000 km3db-0.9.0/benchmarks/general/database_api.py
+-rwxrwxrwx   0 root         (0) root         (0)      145 2022-09-01 11:46:28.000000 km3db-0.9.0/benchmarks/general/runtable.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-06 22:26:35.430614 km3db-0.9.0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2022-09-01 11:46:28.000000 km3db-0.9.0/doc/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-06 22:26:35.430614 km3db-0.9.0/doc/_static/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2022-09-01 11:46:28.000000 km3db-0.9.0/doc/_static/default.css
+-rw-rw-rw-   0 root         (0) root         (0)    24268 2022-09-01 11:46:28.000000 km3db-0.9.0/doc/_static/default_gallery_thumbnail.png
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-09-01 11:46:28.000000 km3db-0.9.0/doc/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2842 2022-09-01 11:46:28.000000 km3db-0.9.0/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2022-09-01 11:46:28.000000 km3db-0.9.0/doc/examples.rst
+-rw-rw-rw-   0 root         (0) root         (0)      336 2022-09-01 11:46:28.000000 km3db-0.9.0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2022-09-01 11:46:28.000000 km3db-0.9.0/doc/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-06 22:26:35.430614 km3db-0.9.0/doc/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-06 22:26:35.430614 km3db-0.9.0/doc/modules/generated/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-01 11:46:28.000000 km3db-0.9.0/doc/modules/generated/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-06 22:26:35.430614 km3db-0.9.0/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      126 2022-09-01 11:46:28.000000 km3db-0.9.0/examples/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3562 2022-10-06 12:51:04.000000 km3db-0.9.0/examples/plot_detid_and_run_streams.py
+-rw-rw-rw-   0 root         (0) root         (0)     6328 2022-10-06 12:51:04.000000 km3db-0.9.0/examples/plot_run_summary_numbers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7688 2022-09-01 11:46:28.000000 km3db-0.9.0/examples/plot_sea_current.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-06 22:26:35.434614 km3db-0.9.0/km3db/
+-rw-rw-rw-   0 root         (0) root         (0)      198 2022-09-01 11:46:28.000000 km3db-0.9.0/km3db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-06 22:26:35.434614 km3db-0.9.0/km3db/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2022-10-06 12:51:04.000000 km3db-0.9.0/km3db/cli/detx.py
+-rw-rw-rw-   0 root         (0) root         (0)      525 2022-09-01 11:46:28.000000 km3db-0.9.0/km3db/cli/km3db.py
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2022-09-01 11:46:28.000000 km3db-0.9.0/km3db/cli/runinfo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2022-09-01 11:46:28.000000 km3db-0.9.0/km3db/cli/runtable.py
+-rw-rw-rw-   0 root         (0) root         (0)     8889 2022-10-06 20:41:34.000000 km3db-0.9.0/km3db/cli/streamds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2022-09-01 11:46:28.000000 km3db-0.9.0/km3db/cli/wtd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2022-09-01 11:46:28.000000 km3db-0.9.0/km3db/compat.py
+-rw-rw-rw-   0 root         (0) root         (0)     7191 2022-10-06 12:51:04.000000 km3db-0.9.0/km3db/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2022-10-06 12:51:04.000000 km3db-0.9.0/km3db/extras.py
+-rw-rw-rw-   0 root         (0) root         (0)     5812 2022-09-01 11:46:28.000000 km3db-0.9.0/km3db/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    13702 2022-10-06 22:10:51.000000 km3db-0.9.0/km3db/tools.py
+-rw-r--r--   0 root         (0) root         (0)      176 2022-10-06 22:26:35.000000 km3db-0.9.0/km3db/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-06 22:26:35.434614 km3db-0.9.0/km3db.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9621 2022-10-06 22:26:35.000000 km3db-0.9.0/km3db.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1171 2022-10-06 22:26:35.000000 km3db-0.9.0/km3db.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-10-06 22:26:35.000000 km3db-0.9.0/km3db.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      203 2022-10-06 22:26:35.000000 km3db-0.9.0/km3db.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      265 2022-10-06 22:26:35.000000 km3db-0.9.0/km3db.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2022-10-06 22:26:35.000000 km3db-0.9.0/km3db.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      136 2022-09-01 11:46:28.000000 km3db-0.9.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       29 2022-09-01 11:46:28.000000 km3db-0.9.0/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-06 22:26:35.434614 km3db-0.9.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      200 2022-09-01 11:46:28.000000 km3db-0.9.0/requirements/dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       12 2022-10-06 12:51:04.000000 km3db-0.9.0/requirements/extras.txt
+-rw-rw-rw-   0 root         (0) root         (0)       36 2022-09-01 11:46:28.000000 km3db-0.9.0/requirements/install.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-06 22:26:35.434614 km3db-0.9.0/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)    18359 2022-09-01 11:46:28.000000 km3db-0.9.0/scripts/run_benchmarks.py
+-rw-r--r--   0 root         (0) root         (0)       38 2022-10-06 22:26:35.434614 km3db-0.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2022-09-01 11:46:28.000000 km3db-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-06 22:26:35.434614 km3db-0.9.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2248 2022-09-01 11:46:28.000000 km3db-0.9.0/tests/test_core.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2022-09-01 11:46:28.000000 km3db-0.9.0/tests/test_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     6479 2022-09-01 11:46:28.000000 km3db-0.9.0/tests/test_tools.py
```

### Comparing `km3db-0.8.0/.gitlab-ci.yml` & `km3db-0.9.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/CHANGELOG.rst` & `km3db-0.9.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 Unreleased changes
 ------------------
 
 
 Version 0
 ---------
+0.9.0 / 2022-10-07
+~~~~~~~~~~~~~~~~~~
+* Added support for direct HDF5 and CSV output: no shell-piping needed anymore:
+  ``streamds get detectors -o detectors.csv``.
+
 0.8.0 / 2022-09-26
 ~~~~~~~~~~~~~~~~~~
 * Allow option for ``detx`` to choose the format version with ``-v``
 
 0.7.5 / 2022-09-01
 ~~~~~~~~~~~~~~~~~~
 * Added the updated KM3NeT DB cookie for the new GitLab CI runners
```

### Comparing `km3db-0.8.0/LICENSE` & `km3db-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/Makefile` & `km3db-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/PKG-INFO` & `km3db-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: km3db
-Version: 0.8.0
+Version: 0.9.0
 Summary: KM3NeT database library
 Home-page: https://git.km3net.de/km3py/km3db
 Author: Tamas Gal
 Author-email: tgal@km3net.de
 License: UNKNOWN
 Description: KM3NeT database library
         =======================
@@ -154,22 +154,27 @@
           $ streamds -h
           Access the KM3NeT StreamDS DataBase service.
         
           Usage:
               streamds
               streamds list
               streamds info STREAM
-              streamds get [-f FORMAT] STREAM [PARAMETERS...]
+              streamds get [-f FORMAT -o OUTFILE -g GROUPBY] STREAM [PARAMETERS...]
+              streamds upload [-q -x] CSV_FILE
               streamds (-h | --help)
               streamds --version
         
           Options:
               STREAM      Name of the stream.
               PARAMETERS  List of parameters separated by space (e.g. detid=29).
+              CSV_FILE    Whitespace separated data for the runsummary tables.
               -f FORMAT   Usually 'txt' for ASCII or 'text' for UTF-8 [default: txt].
+              -o OUTFILE  Output file: supported formats '.csv' and '.h5'.
+              -g COLUMN   Group dataset by the name of the given row when writing HDF5.
+              -q          Test run! When uploading, a TEST_ prefix will be added to the data.
               -x          Do not verify the SSL certificate.
               -h --help   Show this screen.
         
         For example, a list of available detectors::
         
           > streamds get detectors
           OID	SERIALNUMBER	LOCATIONID	CITY	FIRSTRUN	LASTRUN
@@ -180,14 +185,25 @@
           D_ARCA001	7	A00073795	Italy	1	2763
           FR_INFRAS	8	A00073796	France	1600	3202
           D_DU003NA	9	A00070003	Napoli	1	242
           D_DU004NA	12	A00070003	Napoli	243	342
           D_DU001MA	13	A00070004	Marseille	1	1922
           D_ARCA003	14	A00073795	Italy	1	6465
         
+        To write the database output to a file, use the ``-o`` option, e.g.
+        ``streamds get detectors -o detectors.csv``. The currently supported
+        filetypes are ``.csv`` and ``.h5``. In case of ``.h5``, the data can
+        be grouped by providing ``-g COLUMN``, which will split up the
+        output and write distinct HDF5 dataset. It's useful to group large
+        datasets by e.g. ``RUN``, however, only numerical datatypes are supported
+        currently::
+        
+          > streamds get toashort detid=D0ORCA010 minrun=13000 maxrun=13005 -g RUN -o KM3NeT_00000100_toashort.h5
+          Database output written to 'KM3NeT_00000100_toashort.h5'.
+        
         
         ``km3db``
         ~~~~~~~~~
         
         The ``km3db`` command gives direct access to database URLs and is mainly a
         debugging tool::
```

### Comparing `km3db-0.8.0/README.rst` & `km3db-0.9.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -146,22 +146,27 @@
   $ streamds -h
   Access the KM3NeT StreamDS DataBase service.
 
   Usage:
       streamds
       streamds list
       streamds info STREAM
-      streamds get [-f FORMAT] STREAM [PARAMETERS...]
+      streamds get [-f FORMAT -o OUTFILE -g GROUPBY] STREAM [PARAMETERS...]
+      streamds upload [-q -x] CSV_FILE
       streamds (-h | --help)
       streamds --version
 
   Options:
       STREAM      Name of the stream.
       PARAMETERS  List of parameters separated by space (e.g. detid=29).
+      CSV_FILE    Whitespace separated data for the runsummary tables.
       -f FORMAT   Usually 'txt' for ASCII or 'text' for UTF-8 [default: txt].
+      -o OUTFILE  Output file: supported formats '.csv' and '.h5'.
+      -g COLUMN   Group dataset by the name of the given row when writing HDF5.
+      -q          Test run! When uploading, a TEST_ prefix will be added to the data.
       -x          Do not verify the SSL certificate.
       -h --help   Show this screen.
 
 For example, a list of available detectors::
 
   > streamds get detectors
   OID	SERIALNUMBER	LOCATIONID	CITY	FIRSTRUN	LASTRUN
@@ -172,14 +177,25 @@
   D_ARCA001	7	A00073795	Italy	1	2763
   FR_INFRAS	8	A00073796	France	1600	3202
   D_DU003NA	9	A00070003	Napoli	1	242
   D_DU004NA	12	A00070003	Napoli	243	342
   D_DU001MA	13	A00070004	Marseille	1	1922
   D_ARCA003	14	A00073795	Italy	1	6465
 
+To write the database output to a file, use the ``-o`` option, e.g.
+``streamds get detectors -o detectors.csv``. The currently supported
+filetypes are ``.csv`` and ``.h5``. In case of ``.h5``, the data can
+be grouped by providing ``-g COLUMN``, which will split up the
+output and write distinct HDF5 dataset. It's useful to group large
+datasets by e.g. ``RUN``, however, only numerical datatypes are supported
+currently::
+
+  > streamds get toashort detid=D0ORCA010 minrun=13000 maxrun=13005 -g RUN -o KM3NeT_00000100_toashort.h5
+  Database output written to 'KM3NeT_00000100_toashort.h5'.
+
 
 ``km3db``
 ~~~~~~~~~
 
 The ``km3db`` command gives direct access to database URLs and is mainly a
 debugging tool::
```

### Comparing `km3db-0.8.0/doc/Makefile` & `km3db-0.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/doc/_static/default_gallery_thumbnail.png` & `km3db-0.9.0/doc/_static/default_gallery_thumbnail.png`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/doc/conf.py` & `km3db-0.9.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/doc/make.bat` & `km3db-0.9.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/examples/plot_detid_and_run_streams.py` & `km3db-0.9.0/examples/plot_detid_and_run_streams.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,95 +13,93 @@
 import pandas as pd
 
 #####################################################
 # First, we declare the sds client. This object will take care of the
 # DB connection. ``container`` is set to `pd`, which means the sds
 # will return ``pandas.DataFrame``.
 
-sds = km3db.tools.StreamDS(container="pd") 
+sds = km3db.tools.StreamDS(container="pd")
 
 
 #####################################################
 # Getting the detectors list
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~
 #
 # The detectors list is available in the `detectors` stream.
 
-print (sds.detectors())
+print(sds.detectors())
 
 #####################################################
 # We can see that the list of detectors is quite long, because it
 # includes also testing setup in several laboratories.
 # The actual detectors, ORCA and ARCA, are respectively associated to
 # France and Italy as `CITY`. We can use these selectors to narrow
 # down the selection:
 
-print (sds.detectors(city='France'))
-print (sds.detectors(city='Italy'))
+print(sds.detectors(city="France"))
+print(sds.detectors(city="Italy"))
 
 #####################################################
 # Often, we want to look at a specific detector, for which we have the
 # serial number, e.g. ORCA6 with the serial number 49. It is possible
 # to use that as a selector too:
 
-print (sds.detectors(serialnumber=49))
+print(sds.detectors(serialnumber=49))
 
 #####################################################
 # Getting the run list for a given detector
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 #
 # Now that we have access to the detector list, we can look at the
 # list of runs for a given setup. This is contained in the `runs`
 # stream. We will use the last detector from the ARCA list as an
 # example. Note that `detid` is the `runs` tables is the `OID` from
 # the detector stream.  Let's look at the list of run for this
 # configuration:
 
 # Take the last detector config for ARCA
-det = sds.detectors(city='Italy').iloc[-1]
-print (det)
+det = sds.detectors(city="Italy").iloc[-1]
+print(det)
 
-runs = sds.runs(detid = det['OID'])
-print (runs)
+runs = sds.runs(detid=det["OID"])
+print(runs)
 
 #####################################################
 # This table contains information relative to the job settings:
 
-print (list(runs.columns))
+print(list(runs.columns))
 
 #####################################################
 # We can see that the start/stop time of the run is provide with
 # `UNIXJOBSTART`/`UNIXJOBEND`. Using ``pandas.to_datetime``, we create
 # new variable in datetime format, allowing an easier usage.
 
-runs['datetime_start'] = pd.to_datetime(runs['UNIXJOBSTART'], unit='ms')
-runs['datetime_stop'] = pd.to_datetime(runs['UNIXJOBEND'], unit='ms')
-
-print (runs)
-
+runs["datetime_start"] = pd.to_datetime(runs["UNIXJOBSTART"], unit="ms")
+runs["datetime_stop"] = pd.to_datetime(runs["UNIXJOBEND"], unit="ms")
 
+print(runs)
 
 
 #####################################################
 # Access individual run
 # ~~~~~~~~~~~~~~~~~~~~~
 #
 # It is often necessary to access the information run per run, or for
 # a set of runs. A good option for that is to use the indexing of dataframe.
 # First, we set the `RUN` to be the index:
 
-runs = runs.set_index('RUN')
+runs = runs.set_index("RUN")
 
 #####################################################
 # The first column is now containing the run number, and each row can
 # be accessed with this index, using the `loc` getter:
 
-run_id = runs.sample(1).index[0] # Get a random run number from the frame
-print (f"For this example, we will be using {run_id}.")
+run_id = runs.sample(1).index[0]  # Get a random run number from the frame
+print(f"For this example, we will be using {run_id}.")
 
 #####################################################
 # Now, to access the information for this run:
-print (runs.loc[run_id])
+print(runs.loc[run_id])
 
 #####################################################
 # And accessing a specific information for this run:
-print (f"The run setup name for run {run_id} was: {runs.loc[run_id]['RUNSETUPNAME']}")
+print(f"The run setup name for run {run_id} was: {runs.loc[run_id]['RUNSETUPNAME']}")
```

### Comparing `km3db-0.8.0/examples/plot_run_summary_numbers.py` & `km3db-0.9.0/examples/plot_run_summary_numbers.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,179 +21,183 @@
 import matplotlib.pyplot as plt
 
 #####################################################
 # First, we declare the sds client. This object will take care of the
 # DB connection. ``container`` is set to `pd`, which means the sds
 # will return ``pandas.DataFrame``.
 
-sds = km3db.tools.StreamDS(container="pd") 
+sds = km3db.tools.StreamDS(container="pd")
 
 #####################################################
 # What contains runsummarynumbers stream ?
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 #
 # To explore what contains this Stream, we will first query few runs
 # from ORCA6 and print the resulting dataframe.
 
-df = sds.runsummarynumbers(detid = "D_ORCA006", minrun = 8000, maxrun = 8000)
-print (df)
+df = sds.runsummarynumbers(detid="D_ORCA006", minrun=8000, maxrun=8000)
+print(df)
 
 #####################################################
 # Let's take a look in the `SOURCE_NAME` column :
 
-print(df['SOURCE_NAME'].unique())
+print(df["SOURCE_NAME"].unique())
 
 #####################################################
 # We can already see 2 categories of `SOURCE_NAME':
-# 
+#
 # - Some corresponding to DOM module ID. These values are representing
 #   summary information per DOM.
 # - Some corresponding to version numbers. These values are
 #   representing summary information for the whole detector. The
 #   version number correspond to the JPP version used to compute these
 #   meta-variables.
 
 
-
 #####################################################
-# Exploit detector-related summary information 
+# Exploit detector-related summary information
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 #
 # This time we will get a much larger set of runs, but we will only
 # get the information from `SOURCE_NAME == 14.4.1` (last JPP version
 # when this example was wrote).
 
 run_min = 8000
 run_max = 8500
 detid = "D_ORCA006"
 
-df = sds.runsummarynumbers(detid = detid, minrun = run_min, maxrun = run_max, source_name = "14.4.1")
+df = sds.runsummarynumbers(
+    detid=detid, minrun=run_min, maxrun=run_max, source_name="14.4.1"
+)
 
 #####################################################
-# 
+#
 # We will use the `pivot` function to re-arrange the dataframe
 # shape in a more practical way.
 
-df = df.pivot(index = 'RUN', columns = 'PARAMETER_NAME', values = 'DATA_VALUE')
+df = df.pivot(index="RUN", columns="PARAMETER_NAME", values="DATA_VALUE")
 print(df)
 
 #####################################################
 #
 # Now let's look at what is available in the columns :
-print (list(df.columns))
+print(list(df.columns))
 
 #####################################################
 #
 # One can notice two time-related variables: `UTCMin_s` and
 # `UTCMax_s`.  These two variables contains the start and stop time of
 # the run, in seconds. In python, it's often more convenient to
 # convert the time object to datetime-objects. Pandas is having a very
 # convenient function for that: ``pandas.to_datetime``.  In the
 # following lines, we are defining 3 new columns, respectively
 # containing the start, mean and stop time of the run:
 
-df['t_start'] = pd.to_datetime(df['UTCMin_s'], unit = 's')
-df['t_stop'] = pd.to_datetime(df['UTCMax_s'], unit = 's')
-df['t_mean'] = pd.to_datetime(np.mean(df[['UTCMin_s','UTCMax_s']], axis=1), unit = 's')
+df["t_start"] = pd.to_datetime(df["UTCMin_s"], unit="s")
+df["t_stop"] = pd.to_datetime(df["UTCMax_s"], unit="s")
+df["t_mean"] = pd.to_datetime(np.mean(df[["UTCMin_s", "UTCMax_s"]], axis=1), unit="s")
 
-print (df)
+print(df)
 
 #####################################################
 #
 # As a first example, we can look at the evolution of HRV and mean PMT
 # rate in function of time.  For the mean PMT rate, we also represent
 # its +/- standard variation.
 
-fig, axe = plt.subplots(figsize=[12,4])
+fig, axe = plt.subplots(figsize=[12, 4])
 
 axeb = axe.twinx()
 
-axe.plot(df['t_start'], df['MEAN_Rate_Hz'], color = 'C0')
-ymin = df['MEAN_Rate_Hz'] - df['RMS_Rate_Hz']
-ymax = df['MEAN_Rate_Hz'] + df['RMS_Rate_Hz']
-axe.fill_between(df['t_start'], ymin, ymax, color = 'C0', alpha = 0.5)
+axe.plot(df["t_start"], df["MEAN_Rate_Hz"], color="C0")
+ymin = df["MEAN_Rate_Hz"] - df["RMS_Rate_Hz"]
+ymax = df["MEAN_Rate_Hz"] + df["RMS_Rate_Hz"]
+axe.fill_between(df["t_start"], ymin, ymax, color="C0", alpha=0.5)
 
-axeb.plot(df['t_start'], df['HRV'], color = 'C1')
+axeb.plot(df["t_start"], df["HRV"], color="C1")
 
-axe.set_ylabel('PMT rate [kHz]')
-axe.yaxis.label.set_color('C0')
+axe.set_ylabel("PMT rate [kHz]")
+axe.yaxis.label.set_color("C0")
 
-axeb.set_ylabel('High rate veto fraction')
-axeb.yaxis.label.set_color('C1')
+axeb.set_ylabel("High rate veto fraction")
+axeb.yaxis.label.set_color("C1")
 
 #####################################################
 #
 # We can also look at the events rate, with a break down of the
 # different trigger rates
 
-triggers_name = [
-    'JTrigger3DMuon',
-    'JTrigger3DShower',
-    'JTriggerMXShower'
-]
+triggers_name = ["JTrigger3DMuon", "JTrigger3DShower", "JTriggerMXShower"]
 
-fig, axe = plt.subplots(figsize=[12,4])
-axe.set_yscale('log')
+fig, axe = plt.subplots(figsize=[12, 4])
+axe.set_yscale("log")
 
-axe.plot(df['t_start'], df['JDAQEvent']/df['livetime_s'], color = 'gray', label = "DAQ events", zorder=0)
+axe.plot(
+    df["t_start"],
+    df["JDAQEvent"] / df["livetime_s"],
+    color="gray",
+    label="DAQ events",
+    zorder=0,
+)
 
-for name in triggers_name :
-    axe.plot(df['t_start'], df[name]/df['livetime_s'], label=name,zorder=1)
+for name in triggers_name:
+    axe.plot(df["t_start"], df[name] / df["livetime_s"], label=name, zorder=1)
 
-axe.set_ylabel('Rate [kHz]')
+axe.set_ylabel("Rate [kHz]")
 axe.legend()
 
 plt.tight_layout()
 
 
 #####################################################
-# Exploit DOM-related summary information 
+# Exploit DOM-related summary information
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 #
 # First, we will remove the detector-related information from the
 # dataframe. For this, we only keep the `SOURCE_NAME` starting by
 # `80`. As all the `SOURCE_NAME` are now an integer, we convert them
 # to int.
 
-df = sds.runsummarynumbers(detid = "D_ORCA006", minrun = 8000, maxrun = 8050)
-df = df[df['SOURCE_NAME'].str.contains('^80.*')]
-df = df.astype({'SOURCE_NAME':int})
+df = sds.runsummarynumbers(detid="D_ORCA006", minrun=8000, maxrun=8050)
+df = df[df["SOURCE_NAME"].str.contains("^80.*")]
+df = df.astype({"SOURCE_NAME": int})
 
 #####################################################
 # We will use the `pivot` function to re-arrange the dataframe
 # shape in a more practical way.
 # We would like a dataframe with the columns name being
 # `PARAMETER_NAME`, each rows being the showing the `VALUES` for a
 # given module (`SOURCE_NAME`) during a given `RUN`.
 # This is done with the following line :
 
-df = df.pivot(index = ['SOURCE_NAME','RUN'], columns = 'PARAMETER_NAME', values = 'DATA_VALUE')
-print (df)
+df = df.pivot(
+    index=["SOURCE_NAME", "RUN"], columns="PARAMETER_NAME", values="DATA_VALUE"
+)
+print(df)
 
 #####################################################
 # We can look at the list of available columns :
 
-print (list(df.columns))
+print(list(df.columns))
 
 #####################################################
 # Finally, let's plot the evolution of the rate per PMT for a given
 # module ID. Here, we randomly pick `806451572`.
 
 mID = 806451572
 
-fig, axe = plt.subplots(figsize=[8,4])
-axe.set_yscale('log')
+fig, axe = plt.subplots(figsize=[8, 4])
+axe.set_yscale("log")
 
-cmap = mpl.cm.get_cmap('viridis')
+cmap = mpl.cm.get_cmap("viridis")
 
 for i in range(31):
-    colName = 'pmt_{}_mean_rate'.format(i)
-    color = cmap(i/30.)
+    colName = "pmt_{}_mean_rate".format(i)
+    color = cmap(i / 30.0)
     axe.plot(df.loc[mID].index, df.loc[mID][colName], color=color)
-    
-axe.set_xlabel('Run ID')
-axe.set_ylabel('Mean rate [kHz]')
-plt.tight_layout()
 
+axe.set_xlabel("Run ID")
+axe.set_ylabel("Mean rate [kHz]")
+plt.tight_layout()
 
 
 plt.show()
```

### Comparing `km3db-0.8.0/examples/plot_sea_current.py` & `km3db-0.9.0/examples/plot_sea_current.py`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/km3db/cli/detx.py` & `km3db-0.9.0/km3db/cli/detx.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,18 +34,24 @@
     try:
         det_id = int(args["DET_ID"])
     except ValueError:
         log.error("Please proivde a valid detector ID (e.g. 49).")
         return
 
     if args["RUN"] is not None:
-        detx = km3db.tools.detx_for_run(det_id, int(args["RUN"]), version=int(args["-v"]))
+        detx = km3db.tools.detx_for_run(
+            det_id, int(args["RUN"]), version=int(args["-v"])
+        )
     else:
         detx = km3db.tools.detx(
-            det_id, pcal=args["-p"], rcal=args["-r"], tcal=args["-t"], version=int(args["-v"]) 
+            det_id,
+            pcal=args["-p"],
+            rcal=args["-r"],
+            tcal=args["-t"],
+            version=int(args["-v"]),
         )
 
     if detx is None:
         log.error("No detx found.")
         return
 
     if args["-o"]:
```

### Comparing `km3db-0.8.0/km3db/cli/km3db.py` & `km3db-0.9.0/km3db/cli/km3db.py`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/km3db/cli/runinfo.py` & `km3db-0.9.0/km3db/cli/runinfo.py`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/km3db/cli/runtable.py` & `km3db-0.9.0/km3db/cli/runtable.py`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/km3db/cli/streamds.py` & `km3db-0.9.0/km3db/cli/streamds.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 """
 Access the KM3NeT StreamDS DataBase service.
 
 Usage:
     streamds
     streamds list
     streamds info STREAM
-    streamds get [-f FORMAT] STREAM [PARAMETERS...]
+    streamds get [-f FORMAT -o OUTFILE -g COLUMN] STREAM [PARAMETERS...]
     streamds upload [-q -x] CSV_FILE
     streamds (-h | --help)
     streamds --version
 
 Options:
     STREAM      Name of the stream.
     PARAMETERS  List of parameters separated by space (e.g. detid=29).
     CSV_FILE    Whitespace separated data for the runsummary tables.
     -f FORMAT   Usually 'txt' for ASCII or 'text' for UTF-8 [default: txt].
+    -o OUTFILE  Output file: supported formats '.csv' and '.h5'.
+    -g COLUMN   Group dataset by the name of the given row when writing HDF5.
     -q          Test run! When uploading, a TEST_ prefix will be added to the data.
     -x          Do not verify the SSL certificate.
     -h --help   Show this screen.
 
 """
 import getpass
 import json
@@ -46,15 +48,15 @@
 
 def print_info(stream):
     """Print the information about a stream"""
     sds = km3db.StreamDS()
     sds.help(stream)
 
 
-def get_data(stream, parameters, fmt):
+def get_data(stream, parameters, fmt, outfile=None, groupby=None):
     """Retrieve data for given stream and parameters, or None if not found"""
     sds = km3db.StreamDS()
     if stream not in sds.streams:
         log.error("Stream '{}' not found in the database.".format(stream))
         return
     params = {}
     if parameters:
@@ -65,22 +67,73 @@
                     "The correct syntax is 'parameter=value'".format(parameter)
                 )
                 continue
             key, value = parameter.split("=")
             params[key] = value
     data = sds.get(stream, fmt, **params)
     if data is not None:
-        try:
-            print(data)
-        except BrokenPipeError:
-            pass
+        if outfile is not None:
+            write_output(outfile, stream, data, groupby)
+        else:
+            try:
+                print(data)
+            except BrokenPipeError:
+                pass
     else:
         sds.help(stream)
 
 
+def write_output(outfile, stream, data, groupby=None):
+    """Writes the DB output to a file (HDF5 or CSV)"""
+    _, ext = os.path.splitext(outfile)
+
+    if ext == ".h5":
+        write_output_hdf5(outfile, stream, data, groupby=groupby)
+        exit(0)
+    if ext == ".csv":
+        write_output_csv(outfile, stream, data)
+        exit(0)
+
+    log.error("Unsupported filetype with '{}'".format(ext))
+    exit(1)
+
+
+def write_output_hdf5(outfile, stream, data, groupby):
+    """Write DB output to HDF5"""
+    h5py = km3db.extras.h5py()
+    df = km3db.tools.topandas(data)
+    with h5py.File(outfile, "a") as h5f:
+        if groupby is not None:
+            for group, _df in df.groupby(groupby):
+                sa = km3db.tools.df_to_sarray(_df)
+                dset_name = stream + "/{}".format(group)
+                if dset_name in h5f:
+                    log.warning(
+                        "Dataset '{}' already exists, skipping...".format(dset_name)
+                    )
+                    continue
+                h5f.create_dataset(
+                    stream + "/{}".format(group),
+                    compression="gzip",
+                    compression_opts=3,
+                    data=sa,
+                )
+        else:
+            sa = km3db.tools.df_to_sarray(df)
+            h5f[stream] = sa
+    print("Database output written to '{}'.".format(outfile))
+
+
+def write_output_csv(outfile, stream, data):
+    """Write DB output to CSV"""
+    with open(outfile, "w") as fobj:
+        fobj.write(data)
+    print("Database output written to '{}'.".format(outfile))
+
+
 def available_streams():
     """Show a short list of available streams."""
     sds = km3db.StreamDS()
     print("Available streams: ")
     print(", ".join(sorted(sds.streams)))
 
 
@@ -99,129 +152,126 @@
         return
 
     cols = set(df.columns)
 
     if not REQUIRED_COLUMNS.issubset(cols):
         log.error(
             "Missing columns: {}.".format(
-                ', '.join(str(c) for c in REQUIRED_COLUMNS - cols)
+                ", ".join(str(c) for c in REQUIRED_COLUMNS - cols)
             )
         )
         return
 
     parameters = cols - REQUIRED_COLUMNS
     if len(parameters) < 1:
         log.error("No parameter columns found.")
         return
 
     if len(df) == 0:
         log.critical("Empty dataset.")
         return
 
     print(
-        "Found data for parameters: {}.".format(
-            ', '.join(str(c) for c in parameters)
-        )
+        "Found data for parameters: {}.".format(", ".join(str(c) for c in parameters))
     )
     print("Converting CSV data into JSON")
     if testrun:
         log.warn("Test run: adding 'TEST_' prefix to parameter names")
         prefix = "TEST_"
     else:
         prefix = ""
 
-    db = km3db.DBManager()    # noqa
+    db = km3db.DBManager()  # noqa
 
-    det_id_zero_mask = df['det_id'] == 0
+    det_id_zero_mask = df["det_id"] == 0
     if sum(det_id_zero_mask) > 0:
         log.warning("Entries with 'det_id=0' found, removing them.")
         df = df[~det_id_zero_mask]
-    df['det_id'] = df['det_id'].apply(km3db.tools.todetoid)
+    df["det_id"] = df["det_id"].apply(km3db.tools.todetoid)
     print(df)
     data = convert_runsummary_to_json(df, prefix=prefix)
     print("We have {:.3f} MB to upload.".format(len(data) / 1024**2))
 
     print("Requesting database session.")
     session_cookie = db.session_cookie
 
     print("Uploading the data to the database.")
     r = requests.post(
         RUNSUMMARY_URL,
         cookies={"sid": session_cookie},
-        files={'datafile': data},
-        verify=verify
+        files={"datafile": data},
+        verify=verify,
     )
 
     if r.status_code == 200:
         log.debug("POST request status code: {}".format(r.status_code))
         print("Database response:")
         db_answer = json.loads(r.text)
         for key, value in db_answer.items():
             print("  -> {}: {}".format(key, value))
-        if db_answer['Result'] == 'OK':
+        if db_answer["Result"] == "OK":
             print("Upload successful.")
         else:
             log.critical("Something went wrong.")
     else:
         log.error("POST request status code: {}".format(r.status_code))
         log.critical("Something went wrong...")
         return
 
 
 def convert_runsummary_to_json(
-    df, comment='Uploaded via km3pipe.StreamDS', prefix='TEST_'
+    df, comment="Uploaded via km3pipe.StreamDS", prefix="TEST_"
 ):
     """Convert a Pandas DataFrame with runsummary to JSON for DB upload"""
     data_field = []
     comment += ", by {}".format(getpass.getuser())
-    for det_id, det_data in df.groupby('det_id'):
+    for det_id, det_data in df.groupby("det_id"):
         runs_field = []
         data_field.append({"DetectorId": det_id, "Runs": runs_field})
 
-        for run, run_data in det_data.groupby('run'):
+        for run, run_data in det_data.groupby("run"):
             parameters_field = []
-            runs_field.append({
-                "Run": int(run),
-                "Parameters": parameters_field
-            })
+            runs_field.append({"Run": int(run), "Parameters": parameters_field})
 
             parameter_dict = {}
             for row in run_data.iterrows():
                 for parameter_name in run_data.columns:
                     if parameter_name in REQUIRED_COLUMNS:
                         continue
 
                     if parameter_name not in parameter_dict:
-                        entry = {'Name': prefix + parameter_name, 'Data': []}
+                        entry = {"Name": prefix + parameter_name, "Data": []}
                         parameter_dict[parameter_name] = entry
                     data_value = getattr(row[1], parameter_name)
                     try:
                         data_value = float(data_value)
                     except ValueError as e:
                         log.critical("Data values has to be floats!")
                         raise ValueError(e)
-                    value = {
-                        'S': str(getattr(row[1], 'source')),
-                        'D': data_value
-                    }
-                    parameter_dict[parameter_name]['Data'].append(value)
+                    value = {"S": str(getattr(row[1], "source")), "D": data_value}
+                    parameter_dict[parameter_name]["Data"].append(value)
             for parameter_data in parameter_dict.values():
                 parameters_field.append(parameter_data)
     data_to_upload = {"Comment": comment, "Data": data_field}
     file_data_to_upload = json.dumps(data_to_upload)
     return file_data_to_upload
 
 
-
 def main():
     args = docopt(__doc__)
 
     if args["info"]:
         print_info(args["STREAM"])
     elif args["list"]:
         print_streams()
-    elif args['upload']:
-        upload_runsummary(args['CSV_FILE'], args['-q'], args['-x'])
+    elif args["upload"]:
+        upload_runsummary(args["CSV_FILE"], args["-q"], args["-x"])
     elif args["get"]:
-        get_data(args["STREAM"], args["PARAMETERS"], fmt=args["-f"])
+        get_data(
+            args["STREAM"],
+            args["PARAMETERS"],
+            fmt=args["-f"],
+            outfile=args["-o"],
+            groupby=args["-g"],
+        )
     else:
         available_streams()
```

### Comparing `km3db-0.8.0/km3db/cli/wtd.py` & `km3db-0.9.0/km3db/cli/wtd.py`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/km3db/compat.py` & `km3db-0.9.0/km3db/compat.py`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/km3db/core.py` & `km3db-0.9.0/km3db/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,16 +50,16 @@
         try:
             f = self.opener.open(target_url)
         except km3db.compat.HTTPError as e:
             if e.code == 403:
                 if retries:
                     log.error(
                         "Access forbidden, your session has expired. "
-                        "Deleting the cookie (%s) and retrying once.", 
-                            COOKIE_FILENAME
+                        "Deleting the cookie (%s) and retrying once.",
+                        COOKIE_FILENAME,
                     )
                     retries -= 1
                 else:
                     log.critical("Access forbidden. Giving up...")
                     return default
                 time.sleep(1)
                 self.reset()
@@ -80,15 +80,19 @@
         except km3db.compat.RemoteDisconnected as e:
             if retries:
                 retries -= 1
                 log.error("RemoteDisconnected '%s', retrying in 30 seconds.", e)
                 time.sleep(30)
                 return self.get(url, default=default, retries=retries)
             else:
-                log.error("Giving up... RemoteDisconnected: %s\n" "Target URL: %s", e, target_url)
+                log.error(
+                    "Giving up... RemoteDisconnected: %s\n" "Target URL: %s",
+                    e,
+                    target_url,
+                )
                 return default
         try:
             content = f.read()
         except km3db.compat.IncompleteRead as icread:
             log.error("Incomplete data received from the DB.")
             content = icread.partial
         log.debug("Got {0} bytes of data.".format(len(content)))
```

### Comparing `km3db-0.8.0/km3db/logger.py` & `km3db-0.9.0/km3db/logger.py`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/km3db/tools.py` & `km3db-0.9.0/km3db/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python3
 from collections import OrderedDict, namedtuple
 import json
 
+import numpy as np
+
 import km3db.compat
 import km3db.core
 import km3db.extras
 from km3db.logger import log
 
 
 try:
@@ -322,14 +324,46 @@
 
 
 def topandas(text):
     """Create a DataFrame from database output"""
     return km3db.extras.pandas().read_csv(km3db.compat.StringIO(text), sep="\t")
 
 
+def df_to_sarray(df):
+    """
+    Convert a pandas DataFrame object to a numpy structured array.
+
+    Parameters
+    ----------
+    df : Pandas.DataFrame
+      the data frame to convert
+
+    Returns
+    -------
+    A numpy structured array representation of df.
+    """
+
+    for dtype in df.dtypes:
+        if dtype is np.dtype("O"):
+            log.critical(
+                "At least one column contains strings, "
+                "which are currently not supported in the HDF5 backend. "
+                "The CSV backend will work fine."
+            )
+            exit(1)
+
+    cols = df.columns
+    types = [(cols[i], df[k].dtype.type) for (i, k) in enumerate(cols)]
+    v = df.values
+    arr = np.zeros(v.shape[0], np.dtype(types))
+    for (idx, field) in enumerate(arr.dtype.names):
+        arr[field] = v[:, idx]
+    return arr
+
+
 def show_compass_calibration(clb_upi, version="3"):
     """Show compass calibration data for given `clb_upi`."""
     db = km3db.core.DBManager()
     compass_upi = clbupi2compassupi(clb_upi)
     compass_model = compass_upi.split("/")[1]
     print("Compass UPI: {}".format(compass_upi))
     print("Compass model: {}".format(compass_model))
@@ -376,28 +410,28 @@
         if run_info.run == run:
             break
     else:
         log.error("Run {} not found for detector {}".format(run, det_id))
         return None
 
     tcal = run_info.t0_calibsetid
-    if tcal == '':
+    if tcal == "":
         log.warning(
             "No time calibration found for run {} (detector {})".format(run, det_id)
         )
         tcal = 0
 
     pcal = run_info.pos_calibsetid
-    if pcal == '':
+    if pcal == "":
         log.warning(
             "No position calibration found for run {} (detector {})".format(run, det_id)
         )
         pcal = 0
 
     rcal = run_info.rot_calibsetid
-    if rcal == '':
+    if rcal == "":
         log.warning(
             "No rotation calibration found for run {} (detector {})".format(run, det_id)
         )
         rcal = 0
 
     return detx(det_id, pcal=pcal, rcal=rcal, tcal=tcal, version=version)
```

### Comparing `km3db-0.8.0/km3db.egg-info/PKG-INFO` & `km3db-0.9.0/km3db.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: km3db
-Version: 0.8.0
+Version: 0.9.0
 Summary: KM3NeT database library
 Home-page: https://git.km3net.de/km3py/km3db
 Author: Tamas Gal
 Author-email: tgal@km3net.de
 License: UNKNOWN
 Description: KM3NeT database library
         =======================
@@ -154,22 +154,27 @@
           $ streamds -h
           Access the KM3NeT StreamDS DataBase service.
         
           Usage:
               streamds
               streamds list
               streamds info STREAM
-              streamds get [-f FORMAT] STREAM [PARAMETERS...]
+              streamds get [-f FORMAT -o OUTFILE -g GROUPBY] STREAM [PARAMETERS...]
+              streamds upload [-q -x] CSV_FILE
               streamds (-h | --help)
               streamds --version
         
           Options:
               STREAM      Name of the stream.
               PARAMETERS  List of parameters separated by space (e.g. detid=29).
+              CSV_FILE    Whitespace separated data for the runsummary tables.
               -f FORMAT   Usually 'txt' for ASCII or 'text' for UTF-8 [default: txt].
+              -o OUTFILE  Output file: supported formats '.csv' and '.h5'.
+              -g COLUMN   Group dataset by the name of the given row when writing HDF5.
+              -q          Test run! When uploading, a TEST_ prefix will be added to the data.
               -x          Do not verify the SSL certificate.
               -h --help   Show this screen.
         
         For example, a list of available detectors::
         
           > streamds get detectors
           OID	SERIALNUMBER	LOCATIONID	CITY	FIRSTRUN	LASTRUN
@@ -180,14 +185,25 @@
           D_ARCA001	7	A00073795	Italy	1	2763
           FR_INFRAS	8	A00073796	France	1600	3202
           D_DU003NA	9	A00070003	Napoli	1	242
           D_DU004NA	12	A00070003	Napoli	243	342
           D_DU001MA	13	A00070004	Marseille	1	1922
           D_ARCA003	14	A00073795	Italy	1	6465
         
+        To write the database output to a file, use the ``-o`` option, e.g.
+        ``streamds get detectors -o detectors.csv``. The currently supported
+        filetypes are ``.csv`` and ``.h5``. In case of ``.h5``, the data can
+        be grouped by providing ``-g COLUMN``, which will split up the
+        output and write distinct HDF5 dataset. It's useful to group large
+        datasets by e.g. ``RUN``, however, only numerical datatypes are supported
+        currently::
+        
+          > streamds get toashort detid=D0ORCA010 minrun=13000 maxrun=13005 -g RUN -o KM3NeT_00000100_toashort.h5
+          Database output written to 'KM3NeT_00000100_toashort.h5'.
+        
         
         ``km3db``
         ~~~~~~~~~
         
         The ``km3db`` command gives direct access to database URLs and is mainly a
         debugging tool::
```

### Comparing `km3db-0.8.0/km3db.egg-info/SOURCES.txt` & `km3db-0.9.0/km3db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/scripts/run_benchmarks.py` & `km3db-0.9.0/scripts/run_benchmarks.py`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/setup.py` & `km3db-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/tests/test_core.py` & `km3db-0.9.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `km3db-0.8.0/tests/test_tools.py` & `km3db-0.9.0/tests/test_tools.py`

 * *Files identical despite different names*

