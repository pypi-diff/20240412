# Comparing `tmp/lisaanalysistools-1.0.4.tar.gz` & `tmp/lisaanalysistools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lisaanalysistools-1.0.4.tar", last modified: Sat Apr  6 01:31:17 2024, max compression
+gzip compressed data, was "lisaanalysistools-1.0.5.tar", last modified: Fri Apr 12 02:06:27 2024, max compression
```

## Comparing `lisaanalysistools-1.0.4.tar` & `lisaanalysistools-1.0.5.tar`

### file list

```diff
@@ -1,71 +1,57 @@
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.627090 lisaanalysistools-1.0.4/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.4/CHANGELOG
--rw-r--r--   0 mlkatz1    (502) staff       (20)    11357 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.4/LICENSE
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.625256 lisaanalysistools-1.0.4/LISAanalysistools.egg-info/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     3380 2024-04-06 01:31:17.000000 lisaanalysistools-1.0.4/LISAanalysistools.egg-info/PKG-INFO
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1802 2024-04-06 01:31:17.000000 lisaanalysistools-1.0.4/LISAanalysistools.egg-info/SOURCES.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2024-04-06 01:31:17.000000 lisaanalysistools-1.0.4/LISAanalysistools.egg-info/dependency_links.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2024-03-13 23:07:52.000000 lisaanalysistools-1.0.4/LISAanalysistools.egg-info/not-zip-safe
--rw-r--r--   0 mlkatz1    (502) staff       (20)       14 2024-04-06 01:31:17.000000 lisaanalysistools-1.0.4/LISAanalysistools.egg-info/top_level.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)      451 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.4/MANIFEST.in
--rw-r--r--   0 mlkatz1    (502) staff       (20)     4756 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.4/Makefile
--rw-r--r--   0 mlkatz1    (502) staff       (20)     3380 2024-04-06 01:31:17.626357 lisaanalysistools-1.0.4/PKG-INFO
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2783 2024-04-06 01:10:31.000000 lisaanalysistools-1.0.4/README.md
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.570677 lisaanalysistools-1.0.4/include/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1694 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/include/Detector.hpp
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.581110 lisaanalysistools-1.0.4/lisatools/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.4/lisatools/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)      123 2024-04-06 01:31:17.000000 lisaanalysistools-1.0.4/lisatools/_version.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    15321 2024-04-06 01:04:36.000000 lisaanalysistools-1.0.4/lisatools/analysiscontainer.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     9187 2024-04-06 01:14:58.000000 lisaanalysistools-1.0.4/lisatools/datacontainer.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    13852 2024-04-02 17:24:55.000000 lisaanalysistools-1.0.4/lisatools/detector.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    34174 2024-04-06 01:05:28.000000 lisaanalysistools-1.0.4/lisatools/diagnostic.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     5154 2024-02-20 21:17:07.000000 lisaanalysistools-1.0.4/lisatools/glitch.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.585071 lisaanalysistools-1.0.4/lisatools/sampling/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.4/lisatools/sampling/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    29585 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/lisatools/sampling/likelihood.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.598911 lisaanalysistools-1.0.4/lisatools/sampling/moves/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1220 2023-06-08 00:14:36.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/gbgroupstretch.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    51802 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/gbmultipletryrj.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    31152 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/gbspecialgroupstretch.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    90189 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/gbspecialstretch.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    14163 2023-10-25 21:01:10.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/mbhspecialmove.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)      469 2023-06-08 00:14:36.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/placeholder.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     3348 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/skymodehop.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    25092 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/specialforegroundmove.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    21407 2024-04-06 01:06:43.000000 lisaanalysistools-1.0.4/lisatools/sampling/prior.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     9682 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/lisatools/sampling/stopping.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    14340 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/lisatools/sampling/utility.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    27263 2024-04-06 01:17:33.000000 lisaanalysistools-1.0.4/lisatools/sensitivity.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.600301 lisaanalysistools-1.0.4/lisatools/sources/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2024-03-01 22:45:54.000000 lisaanalysistools-1.0.4/lisatools/sources/__init__.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.602710 lisaanalysistools-1.0.4/lisatools/sources/emri/
--rw-r--r--   0 mlkatz1    (502) staff       (20)       41 2024-03-01 23:04:25.000000 lisaanalysistools-1.0.4/lisatools/sources/emri/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2297 2024-03-05 21:50:21.000000 lisaanalysistools-1.0.4/lisatools/sources/emri/tdiwaveform.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     9421 2024-04-06 01:09:31.000000 lisaanalysistools-1.0.4/lisatools/stochastic.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.609850 lisaanalysistools-1.0.4/lisatools/utils/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.4/lisatools/utils/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1354 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/lisatools/utils/constants.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    33765 2023-10-25 21:01:10.000000 lisaanalysistools-1.0.4/lisatools/utils/multigpudataholder.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2995 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/lisatools/utils/pointeradjust.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     6831 2024-04-06 00:53:22.000000 lisaanalysistools-1.0.4/lisatools/utils/utility.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)      667 2024-04-06 01:10:06.000000 lisaanalysistools-1.0.4/pyproject.toml
--rw-r--r--   0 mlkatz1    (502) staff       (20)       30 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/requirements-data.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)       15 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/requirements-demo.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)      263 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/requirements-dev.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)       33 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/requirements-release.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)      143 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/requirements.txt
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.616210 lisaanalysistools-1.0.4/scripts/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1578 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/scripts/data_download.py
--rwxr-xr-x   0 mlkatz1    (502) staff       (20)      819 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/scripts/generate-changelog.bash
--rwxr-xr-x   0 mlkatz1    (502) staff       (20)      279 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/scripts/install-hooks.bash
--rwxr-xr-x   0 mlkatz1    (502) staff       (20)       55 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/scripts/post-commit.bash
--rwxr-xr-x   0 mlkatz1    (502) staff       (20)     1253 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/scripts/run-tests.bash
--rwxr-xr-x   0 mlkatz1    (502) staff       (20)     1242 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/scripts/to_conda.bash
--rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2024-04-06 01:31:17.627241 lisaanalysistools-1.0.4/setup.cfg
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2756 2024-03-27 20:31:21.000000 lisaanalysistools-1.0.4/setup.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.623636 lisaanalysistools-1.0.4/src/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     3857 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/src/Detector.cpp
--rw-r--r--   0 mlkatz1    (502) staff       (20)   636410 2024-04-06 01:29:48.000000 lisaanalysistools-1.0.4/src/pycppdetector.cpp
--rw-r--r--   0 mlkatz1    (502) staff       (20)     5100 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/src/pycppdetector.pyx
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-12 02:06:27.759797 lisaanalysistools-1.0.5/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.5/CHANGELOG
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    11357 2024-04-11 21:28:07.000000 lisaanalysistools-1.0.5/LICENSE
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-12 02:06:27.758685 lisaanalysistools-1.0.5/LISAanalysistools.egg-info/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3380 2024-04-12 02:06:27.000000 lisaanalysistools-1.0.5/LISAanalysistools.egg-info/PKG-INFO
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1322 2024-04-12 02:06:27.000000 lisaanalysistools-1.0.5/LISAanalysistools.egg-info/SOURCES.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2024-04-12 02:06:27.000000 lisaanalysistools-1.0.5/LISAanalysistools.egg-info/dependency_links.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2024-04-11 21:58:02.000000 lisaanalysistools-1.0.5/LISAanalysistools.egg-info/not-zip-safe
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       14 2024-04-12 02:06:27.000000 lisaanalysistools-1.0.5/LISAanalysistools.egg-info/top_level.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      451 2024-04-11 21:28:07.000000 lisaanalysistools-1.0.5/MANIFEST.in
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4756 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.5/Makefile
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3380 2024-04-12 02:06:27.759291 lisaanalysistools-1.0.5/PKG-INFO
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2783 2024-04-11 22:16:20.000000 lisaanalysistools-1.0.5/README.md
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-12 02:06:27.734062 lisaanalysistools-1.0.5/include/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1694 2024-04-11 21:28:07.000000 lisaanalysistools-1.0.5/include/Detector.hpp
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-12 02:06:27.741684 lisaanalysistools-1.0.5/lisatools/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.5/lisatools/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      123 2024-04-12 02:06:27.000000 lisaanalysistools-1.0.5/lisatools/_version.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    15321 2024-04-11 21:28:07.000000 lisaanalysistools-1.0.5/lisatools/analysiscontainer.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     9187 2024-04-11 21:28:07.000000 lisaanalysistools-1.0.5/lisatools/datacontainer.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    13851 2024-04-11 21:55:26.000000 lisaanalysistools-1.0.5/lisatools/detector.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    34174 2024-04-11 21:28:08.000000 lisaanalysistools-1.0.5/lisatools/diagnostic.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-12 02:06:27.745273 lisaanalysistools-1.0.5/lisatools/sampling/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.5/lisatools/sampling/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    29585 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.5/lisatools/sampling/likelihood.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-12 02:06:27.746292 lisaanalysistools-1.0.5/lisatools/sampling/moves/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.5/lisatools/sampling/moves/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3348 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.5/lisatools/sampling/moves/skymodehop.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    21407 2024-04-11 21:28:08.000000 lisaanalysistools-1.0.5/lisatools/sampling/prior.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     9682 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.5/lisatools/sampling/stopping.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    14340 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.5/lisatools/sampling/utility.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    27297 2024-04-11 21:55:49.000000 lisaanalysistools-1.0.5/lisatools/sensitivity.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-12 02:06:27.746855 lisaanalysistools-1.0.5/lisatools/sources/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2024-04-11 21:28:08.000000 lisaanalysistools-1.0.5/lisatools/sources/__init__.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-12 02:06:27.747925 lisaanalysistools-1.0.5/lisatools/sources/emri/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       41 2024-04-11 21:28:08.000000 lisaanalysistools-1.0.5/lisatools/sources/emri/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2297 2024-04-11 21:28:08.000000 lisaanalysistools-1.0.5/lisatools/sources/emri/tdiwaveform.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     9421 2024-04-11 21:28:08.000000 lisaanalysistools-1.0.5/lisatools/stochastic.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-12 02:06:27.750080 lisaanalysistools-1.0.5/lisatools/utils/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.5/lisatools/utils/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1354 2024-04-11 21:28:08.000000 lisaanalysistools-1.0.5/lisatools/utils/constants.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2995 2024-04-11 21:28:08.000000 lisaanalysistools-1.0.5/lisatools/utils/pointeradjust.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     6831 2024-04-11 21:28:08.000000 lisaanalysistools-1.0.5/lisatools/utils/utility.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      667 2024-04-11 22:16:37.000000 lisaanalysistools-1.0.5/pyproject.toml
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-12 02:06:27.753837 lisaanalysistools-1.0.5/scripts/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1578 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.5/scripts/data_download.py
+-rwxr-xr-x   0 mlkatz1    (502) staff       (20)      819 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.5/scripts/generate-changelog.bash
+-rwxr-xr-x   0 mlkatz1    (502) staff       (20)      279 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.5/scripts/install-hooks.bash
+-rwxr-xr-x   0 mlkatz1    (502) staff       (20)       55 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.5/scripts/post-commit.bash
+-rwxr-xr-x   0 mlkatz1    (502) staff       (20)     1253 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.5/scripts/run-tests.bash
+-rwxr-xr-x   0 mlkatz1    (502) staff       (20)     1242 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.5/scripts/to_conda.bash
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2024-04-12 02:06:27.759912 lisaanalysistools-1.0.5/setup.cfg
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2756 2024-04-11 21:28:08.000000 lisaanalysistools-1.0.5/setup.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-12 02:06:27.757992 lisaanalysistools-1.0.5/src/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3857 2024-04-11 21:28:08.000000 lisaanalysistools-1.0.5/src/Detector.cpp
+-rw-r--r--   0 mlkatz1    (502) staff       (20)   636410 2024-04-11 22:17:00.000000 lisaanalysistools-1.0.5/src/pycppdetector.cpp
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     5100 2024-04-11 21:28:08.000000 lisaanalysistools-1.0.5/src/pycppdetector.pyx
```

### Comparing `lisaanalysistools-1.0.4/LICENSE` & `lisaanalysistools-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/LISAanalysistools.egg-info/PKG-INFO` & `lisaanalysistools-1.0.5/LISAanalysistools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lisaanalysistools
-Version: 1.0.4
+Version: 1.0.5
 Home-page: https://github.com/mikekatz04/lisa-on-gpu
 Author: Michael Katz
 Author-email: mikekatz04@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Natural Language :: English
@@ -56,15 +56,15 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.0.4
+Current Version: 1.0.5
 
 ## Authors/Developers
 
 * **Michael Katz**
 * Lorenzo Speri
 * Christian Chapman-Bird
 * Natalia Korsakova
```

### Comparing `lisaanalysistools-1.0.4/Makefile` & `lisaanalysistools-1.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/PKG-INFO` & `lisaanalysistools-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lisaanalysistools
-Version: 1.0.4
+Version: 1.0.5
 Home-page: https://github.com/mikekatz04/lisa-on-gpu
 Author: Michael Katz
 Author-email: mikekatz04@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Natural Language :: English
@@ -56,15 +56,15 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.0.4
+Current Version: 1.0.5
 
 ## Authors/Developers
 
 * **Michael Katz**
 * Lorenzo Speri
 * Christian Chapman-Bird
 * Natalia Korsakova
```

### Comparing `lisaanalysistools-1.0.4/README.md` & `lisaanalysistools-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.0.4
+Current Version: 1.0.5
 
 ## Authors/Developers
 
 * **Michael Katz**
 * Lorenzo Speri
 * Christian Chapman-Bird
 * Natalia Korsakova
```

### Comparing `lisaanalysistools-1.0.4/include/Detector.hpp` & `lisaanalysistools-1.0.5/include/Detector.hpp`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/lisatools/analysiscontainer.py` & `lisaanalysistools-1.0.5/lisatools/analysiscontainer.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/lisatools/datacontainer.py` & `lisaanalysistools-1.0.5/lisatools/datacontainer.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/lisatools/detector.py` & `lisaanalysistools-1.0.5/lisatools/detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,15 +439,15 @@
         return out
 
 
 # defaults
 scirdv1 = LISAModel((15.0e-12) ** 2, (3.0e-15) ** 2, DefaultOrbits(), "scirdv1")
 proposal = LISAModel((10.0e-12) ** 2, (3.0e-15) ** 2, DefaultOrbits(), "proposal")
 mrdv1 = LISAModel((10.0e-12) ** 2, (2.4e-15) ** 2, DefaultOrbits(), "mrdv1")
-sangria = LISAModel((10.0e-12) ** 2, (2.4e-15) ** 2, DefaultOrbits(), "sangria")
+sangria = LISAModel((7.9e-12) ** 2, (2.4e-15) ** 2, DefaultOrbits(), "sangria")
 
 __stock_list_models__ = [scirdv1, proposal, mrdv1, sangria]
 __stock_list_models_name__ = [tmp.name for tmp in __stock_list_models__]
 
 
 def get_available_default_lisa_models() -> List[LISAModel]:
     """Get list of default LISA models
```

### Comparing `lisaanalysistools-1.0.4/lisatools/diagnostic.py` & `lisaanalysistools-1.0.5/lisatools/diagnostic.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/lisatools/sampling/likelihood.py` & `lisaanalysistools-1.0.5/lisatools/sampling/likelihood.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/lisatools/sampling/moves/skymodehop.py` & `lisaanalysistools-1.0.5/lisatools/sampling/moves/skymodehop.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/lisatools/sampling/prior.py` & `lisaanalysistools-1.0.5/lisatools/sampling/prior.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/lisatools/sampling/stopping.py` & `lisaanalysistools-1.0.5/lisatools/sampling/stopping.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/lisatools/sampling/utility.py` & `lisaanalysistools-1.0.5/lisatools/sampling/utility.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/lisatools/sensitivity.py` & `lisaanalysistools-1.0.5/lisatools/sensitivity.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,24 +113,27 @@
             model: Noise model. Object of type :class:`lisa_models.LISAModel`. It can also be a string corresponding to one of the stock models.
             **kwargs: For interoperability.
 
         Returns:
             PSD values.
 
         """
-        x = 2.0 * np.pi * lisaLT * f
 
         # get noise values
         Spm, Sop = cls.lisanoises(f, model)
 
         # transform as desired for TDI combination
         Sout = cls.transform(f, Spm, Sop, **kwargs)
 
         # will add zero if ignored
-        Sout += cls.get_stochastic_contribution(f, **kwargs)
+        stochastic_contribution = cls.stochastic_transform(
+            f, cls.get_stochastic_contribution(f, **kwargs), **kwargs
+        )
+
+        Sout += stochastic_contribution
         return Sout
 
     @classmethod
     def get_stochastic_contribution(
         cls,
         f: float | np.ndarray,
         stochastic_params: Optional[tuple] = (),
@@ -169,20 +172,17 @@
             (stochastic_params != () and stochastic_params is not None)
             or (stochastic_kwargs != {} and stochastic_kwargs is not None)
             or stochastic_function is not None
         ):
             if stochastic_function is None:
                 stochastic_function = FittedHyperbolicTangentGalacticForeground
 
-            try:
                 check = stochastic_function.get_Sh(
                     f, *stochastic_params, **stochastic_kwargs
                 )
-            except:
-                breakpoint()
             sgal[:] = check
 
         if squeeze:
             sgal = sgal.squeeze()
         return sgal
 
     @staticmethod
@@ -339,23 +339,25 @@
     ) -> float | np.ndarray:
         __doc__ = (
             "Transform from the base sensitivity functions to the A,E TDI PSDs.\n\n"
             + Sensitivity.transform.__doc__.split("PSDs.\n\n")[-1]
         )
 
         x = 2.0 * np.pi * lisaLT * f
-        return (
+        Sa = (
             8.0
             * np.sin(x) ** 2
             * (
                 2.0 * Spm * (3.0 + 2.0 * np.cos(x) + np.cos(2 * x))
                 + Sop * (2.0 + np.cos(x))
             )
         )
 
+        return Sa
+
     @staticmethod
     def stochastic_transform(
         f: float | np.ndarray, Sh: float | np.ndarray, **kwargs: dict
     ) -> float | np.ndarray:
         __doc__ = (
             "Transform from the base stochastic functions to the XYZ stochastic TDI information.\n\n"
             + Sensitivity.stochastic_transform.__doc__.split("PSDs.\n\n")[-1]
```

### Comparing `lisaanalysistools-1.0.4/lisatools/sources/emri/tdiwaveform.py` & `lisaanalysistools-1.0.5/lisatools/sources/emri/tdiwaveform.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/lisatools/stochastic.py` & `lisaanalysistools-1.0.5/lisatools/stochastic.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/lisatools/utils/constants.py` & `lisaanalysistools-1.0.5/lisatools/utils/constants.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/lisatools/utils/pointeradjust.py` & `lisaanalysistools-1.0.5/lisatools/utils/pointeradjust.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/lisatools/utils/utility.py` & `lisaanalysistools-1.0.5/lisatools/utils/utility.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/scripts/data_download.py` & `lisaanalysistools-1.0.5/scripts/data_download.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/scripts/generate-changelog.bash` & `lisaanalysistools-1.0.5/scripts/generate-changelog.bash`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/scripts/run-tests.bash` & `lisaanalysistools-1.0.5/scripts/run-tests.bash`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/scripts/to_conda.bash` & `lisaanalysistools-1.0.5/scripts/to_conda.bash`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/setup.py` & `lisaanalysistools-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/src/Detector.cpp` & `lisaanalysistools-1.0.5/src/Detector.cpp`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.4/src/pycppdetector.cpp` & `lisaanalysistools-1.0.5/src/pycppdetector.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "include/Detector.hpp"
         ],
         "include_dirs": [
             "src",
             "./include",
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/core/include"
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "lisatools.cutils.detector",
         "sources": [
             "src/pycppdetector.pyx",
             "src/Detector.cpp"
         ]
@@ -1553,177 +1553,177 @@
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1753,42 +1753,42 @@
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_9lisatools_6cutils_8detector_pycppDetector;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3506,261 +3506,261 @@
 #define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
 #define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
 #define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
 #define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
 #define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
 /* #### Code section: module_code ### */
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3769,29 +3769,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3802,15 +3802,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3819,29 +3819,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3852,15 +3852,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3869,29 +3869,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3902,15 +3902,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3919,29 +3919,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3952,15 +3952,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3969,29 +3969,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4002,217 +4002,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 970, __pyx_L1_error)
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4228,15 +4228,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4244,68 +4244,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 982, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4313,15 +4313,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4336,15 +4336,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4360,15 +4360,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4376,68 +4376,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 988, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4445,15 +4445,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4468,15 +4468,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4492,15 +4492,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4508,68 +4508,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 994, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4577,15 +4577,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4600,170 +4600,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8957,26 +8957,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-i5sha6z5/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 990, __pyx_L1_error)
```

### Comparing `lisaanalysistools-1.0.4/src/pycppdetector.pyx` & `lisaanalysistools-1.0.5/src/pycppdetector.pyx`

 * *Files identical despite different names*

