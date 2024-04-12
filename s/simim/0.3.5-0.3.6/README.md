# Comparing `tmp/simim-0.3.5.tar.gz` & `tmp/simim-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simim-0.3.5.tar", last modified: Wed Apr 10 04:53:18 2024, max compression
+gzip compressed data, was "simim-0.3.6.tar", last modified: Fri Apr 12 13:06:07 2024, max compression
```

## Comparing `simim-0.3.5.tar` & `simim-0.3.6.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.659098 simim-0.3.5/
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1067 2024-03-15 00:09:14.000000 simim-0.3.5/LICENSE
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     3411 2024-04-10 04:53:18.658861 simim-0.3.5/PKG-INFO
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1339 2024-04-10 04:52:29.000000 simim-0.3.5/README.md
-drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.637712 simim-0.3.5/docs/
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     2467 2024-03-08 22:52:24.000000 simim-0.3.5/docs/conf.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1149 2024-04-10 04:51:51.000000 simim-0.3.5/pyproject.toml
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       38 2024-04-10 04:53:18.659141 simim-0.3.5/setup.cfg
-drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.639182 simim-0.3.5/simim/
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      263 2024-03-07 15:56:24.000000 simim-0.3.5/simim/__init__.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    24509 2024-03-15 23:47:46.000000 simim-0.3.5/simim/_handlers.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     9754 2024-03-15 23:47:34.000000 simim-0.3.5/simim/_paths.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      651 2024-03-07 15:56:24.000000 simim-0.3.5/simim/_pltsetup.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1767 2024-04-09 16:09:24.000000 simim-0.3.5/simim/constants.py
-drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.642485 simim-0.3.5/simim/galprops/
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       87 2024-02-28 23:24:15.000000 simim-0.3.5/simim/galprops/__init__.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    10173 2024-03-07 15:56:24.000000 simim-0.3.5/simim/galprops/galprops.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    31442 2024-03-15 00:09:14.000000 simim-0.3.5/simim/galprops/galprops_am.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     2581 2024-02-28 23:39:58.000000 simim-0.3.5/simim/galprops/galprops_builtin.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    10949 2024-02-28 22:12:47.000000 simim-0.3.5/simim/galprops/line_co.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1252 2024-02-28 21:12:40.000000 simim-0.3.5/simim/galprops/line_co_dutycycle.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     2926 2024-02-28 21:39:26.000000 simim-0.3.5/simim/galprops/line_densegas.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    14272 2024-02-28 22:19:50.000000 simim-0.3.5/simim/galprops/line_fir.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    13740 2024-02-28 22:12:23.000000 simim-0.3.5/simim/galprops/line_fir_yang.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1054 2024-02-28 21:43:51.000000 simim-0.3.5/simim/galprops/log10normal.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    10201 2024-03-01 20:03:27.000000 simim-0.3.5/simim/galprops/sfr_behroozi13.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    14797 2024-03-15 00:09:14.000000 simim-0.3.5/simim/galprops/sfr_bethermin17.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     7816 2024-03-15 00:09:14.000000 simim-0.3.5/simim/galprops/sfr_ir.py
-drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.647513 simim-0.3.5/simim/instrument/
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      140 2024-03-07 15:56:24.000000 simim-0.3.5/simim/instrument/__init__.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     4630 2024-03-07 15:56:24.000000 simim-0.3.5/simim/instrument/_helpers.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    54001 2024-03-07 15:56:24.000000 simim-0.3.5/simim/instrument/instrument.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1765 2024-03-07 15:56:24.000000 simim-0.3.5/simim/instrument/noise_functions.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     2491 2024-03-07 15:56:24.000000 simim-0.3.5/simim/instrument/spatial_response.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      590 2024-03-07 15:56:24.000000 simim-0.3.5/simim/instrument/spectral_response.py
-drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.648185 simim-0.3.5/simim/lightcone/
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       80 2024-03-01 20:03:27.000000 simim-0.3.5/simim/lightcone/__init__.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    20117 2024-03-15 23:47:46.000000 simim-0.3.5/simim/lightcone/lchandler.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    35373 2024-03-07 15:56:24.000000 simim-0.3.5/simim/lightcone/lcmaker.py
-drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.650167 simim-0.3.5/simim/map/
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      259 2024-03-01 20:03:27.000000 simim-0.3.5/simim/map/__init__.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)   108750 2024-03-20 23:56:41.000000 simim-0.3.5/simim/map/gridder.py
-drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.650543 simim-0.3.5/simim/resources/
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)   645911 2013-04-08 17:19:38.000000 simim-0.3.5/simim/resources/behroozi13_release.dat
-drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.653856 simim-0.3.5/simim/siminterface/
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      160 2024-03-21 15:01:42.000000 simim-0.3.5/simim/siminterface/__init__.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     5393 2024-02-26 13:49:27.000000 simim-0.3.5/simim/siminterface/_illustris_datahandling.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    27068 2024-02-28 19:23:15.000000 simim-0.3.5/simim/siminterface/_rawsiminterface.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      879 2024-03-21 14:33:27.000000 simim-0.3.5/simim/siminterface/_sims.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    26058 2024-03-21 14:32:20.000000 simim-0.3.5/simim/siminterface/illustris.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    26736 2024-03-15 23:47:46.000000 simim-0.3.5/simim/siminterface/simhandler.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    18073 2024-03-21 23:03:50.000000 simim-0.3.5/simim/siminterface/universemachine.py
-drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.658596 simim-0.3.5/simim.egg-info/
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     3411 2024-04-10 04:53:18.000000 simim-0.3.5/simim.egg-info/PKG-INFO
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1741 2024-04-10 04:53:18.000000 simim-0.3.5/simim.egg-info/SOURCES.txt
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)        1 2024-04-10 04:53:18.000000 simim-0.3.5/simim.egg-info/dependency_links.txt
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       48 2024-04-10 04:53:18.000000 simim-0.3.5/simim.egg-info/entry_points.txt
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       65 2024-04-10 04:53:18.000000 simim-0.3.5/simim.egg-info/requires.txt
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       38 2024-04-10 04:53:18.000000 simim-0.3.5/simim.egg-info/top_level.txt
-drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.655173 simim-0.3.5/simim_dev/
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    12877 2024-03-15 00:09:14.000000 simim-0.3.5/simim_dev/dev_features.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     8200 2024-03-24 18:32:20.000000 simim-0.3.5/simim_dev/dev_lim_stats.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     4021 2024-03-24 14:06:11.000000 simim-0.3.5/simim_dev/dev_spectral_functions.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     3270 2024-03-15 00:09:14.000000 simim-0.3.5/simim_dev/old_obs_noise.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    52131 2024-03-15 00:09:14.000000 simim-0.3.5/simim_dev/old_obs_radio.py
-drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.657660 simim-0.3.5/tests/
-drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.657975 simim-0.3.5/tests/by_eye_checks/
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1550 2024-03-14 23:47:34.000000 simim-0.3.5/tests/by_eye_checks/e2e_sfr.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1848 2024-03-21 23:11:46.000000 simim-0.3.5/tests/make_testbox_resource.py
-drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-10 04:53:18.658217 simim-0.3.5/tests/old_test_code/
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    12155 2024-02-28 21:12:40.000000 simim-0.3.5/tests/old_test_code/lightcone.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    11512 2024-03-20 23:23:48.000000 simim-0.3.5/tests/test_gridder.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1799 2024-03-07 15:56:24.000000 simim-0.3.5/tests/test_imports.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    24778 2024-03-07 15:56:24.000000 simim-0.3.5/tests/test_instrument.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     3187 2024-02-28 21:05:15.000000 simim-0.3.5/tests/test_rawsiminterface.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     3153 2024-03-21 23:16:14.000000 simim-0.3.5/tests/test_rawsiminterface2.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      431 2024-03-07 15:56:24.000000 simim-0.3.5/tests/test_siminterface.py
--rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    11485 2024-03-20 23:58:31.000000 simim-0.3.5/tests/test_spec_gridder.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-12 13:06:07.179008 simim-0.3.6/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1067 2024-03-15 00:09:14.000000 simim-0.3.6/LICENSE
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     3506 2024-04-12 13:06:07.178732 simim-0.3.6/PKG-INFO
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1434 2024-04-12 13:05:30.000000 simim-0.3.6/README.md
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-12 13:06:07.163100 simim-0.3.6/docs/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     2467 2024-03-08 22:52:24.000000 simim-0.3.6/docs/conf.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1149 2024-04-12 13:05:36.000000 simim-0.3.6/pyproject.toml
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       38 2024-04-12 13:06:07.179054 simim-0.3.6/setup.cfg
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-12 13:06:07.163856 simim-0.3.6/simim/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      263 2024-03-07 15:56:24.000000 simim-0.3.6/simim/__init__.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    24509 2024-03-15 23:47:46.000000 simim-0.3.6/simim/_handlers.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     9754 2024-03-15 23:47:34.000000 simim-0.3.6/simim/_paths.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      651 2024-03-07 15:56:24.000000 simim-0.3.6/simim/_pltsetup.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1767 2024-04-09 16:09:24.000000 simim-0.3.6/simim/constants.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-12 13:06:07.166780 simim-0.3.6/simim/galprops/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       87 2024-02-28 23:24:15.000000 simim-0.3.6/simim/galprops/__init__.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    10173 2024-03-07 15:56:24.000000 simim-0.3.6/simim/galprops/galprops.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    31442 2024-03-15 00:09:14.000000 simim-0.3.6/simim/galprops/galprops_am.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     2581 2024-02-28 23:39:58.000000 simim-0.3.6/simim/galprops/galprops_builtin.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    10949 2024-02-28 22:12:47.000000 simim-0.3.6/simim/galprops/line_co.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1252 2024-02-28 21:12:40.000000 simim-0.3.6/simim/galprops/line_co_dutycycle.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     2926 2024-02-28 21:39:26.000000 simim-0.3.6/simim/galprops/line_densegas.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    14272 2024-02-28 22:19:50.000000 simim-0.3.6/simim/galprops/line_fir.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    13740 2024-02-28 22:12:23.000000 simim-0.3.6/simim/galprops/line_fir_yang.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1054 2024-02-28 21:43:51.000000 simim-0.3.6/simim/galprops/log10normal.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    10201 2024-03-01 20:03:27.000000 simim-0.3.6/simim/galprops/sfr_behroozi13.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    14797 2024-03-15 00:09:14.000000 simim-0.3.6/simim/galprops/sfr_bethermin17.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     7816 2024-03-15 00:09:14.000000 simim-0.3.6/simim/galprops/sfr_ir.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-12 13:06:07.167589 simim-0.3.6/simim/instrument/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      140 2024-03-07 15:56:24.000000 simim-0.3.6/simim/instrument/__init__.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     4630 2024-03-07 15:56:24.000000 simim-0.3.6/simim/instrument/_helpers.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    54001 2024-03-07 15:56:24.000000 simim-0.3.6/simim/instrument/instrument.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1765 2024-03-07 15:56:24.000000 simim-0.3.6/simim/instrument/noise_functions.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     2491 2024-03-07 15:56:24.000000 simim-0.3.6/simim/instrument/spatial_response.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      590 2024-03-07 15:56:24.000000 simim-0.3.6/simim/instrument/spectral_response.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-12 13:06:07.168002 simim-0.3.6/simim/lightcone/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       80 2024-03-01 20:03:27.000000 simim-0.3.6/simim/lightcone/__init__.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    20117 2024-03-15 23:47:46.000000 simim-0.3.6/simim/lightcone/lchandler.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    35373 2024-03-07 15:56:24.000000 simim-0.3.6/simim/lightcone/lcmaker.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-12 13:06:07.168298 simim-0.3.6/simim/map/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      259 2024-03-01 20:03:27.000000 simim-0.3.6/simim/map/__init__.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)   108750 2024-03-20 23:56:41.000000 simim-0.3.6/simim/map/gridder.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-12 13:06:07.168477 simim-0.3.6/simim/resources/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)   645911 2013-04-08 17:19:38.000000 simim-0.3.6/simim/resources/behroozi13_release.dat
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-12 13:06:07.171552 simim-0.3.6/simim/siminterface/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      160 2024-03-21 15:01:42.000000 simim-0.3.6/simim/siminterface/__init__.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     5393 2024-02-26 13:49:27.000000 simim-0.3.6/simim/siminterface/_illustris_datahandling.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    27068 2024-02-28 19:23:15.000000 simim-0.3.6/simim/siminterface/_rawsiminterface.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      879 2024-03-21 14:33:27.000000 simim-0.3.6/simim/siminterface/_sims.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    26058 2024-04-12 13:03:59.000000 simim-0.3.6/simim/siminterface/illustris.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    26736 2024-03-15 23:47:46.000000 simim-0.3.6/simim/siminterface/simhandler.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    18073 2024-03-21 23:03:50.000000 simim-0.3.6/simim/siminterface/universemachine.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-12 13:06:07.178434 simim-0.3.6/simim.egg-info/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     3506 2024-04-12 13:06:07.000000 simim-0.3.6/simim.egg-info/PKG-INFO
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1741 2024-04-12 13:06:07.000000 simim-0.3.6/simim.egg-info/SOURCES.txt
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)        1 2024-04-12 13:06:07.000000 simim-0.3.6/simim.egg-info/dependency_links.txt
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       48 2024-04-12 13:06:07.000000 simim-0.3.6/simim.egg-info/entry_points.txt
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       65 2024-04-12 13:06:07.000000 simim-0.3.6/simim.egg-info/requires.txt
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)       38 2024-04-12 13:06:07.000000 simim-0.3.6/simim.egg-info/top_level.txt
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-12 13:06:07.176791 simim-0.3.6/simim_dev/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    12877 2024-03-15 00:09:14.000000 simim-0.3.6/simim_dev/dev_features.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     8200 2024-03-24 18:32:20.000000 simim-0.3.6/simim_dev/dev_lim_stats.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     4021 2024-03-24 14:06:11.000000 simim-0.3.6/simim_dev/dev_spectral_functions.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     3270 2024-03-15 00:09:14.000000 simim-0.3.6/simim_dev/old_obs_noise.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    52131 2024-03-15 00:09:14.000000 simim-0.3.6/simim_dev/old_obs_radio.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-12 13:06:07.177812 simim-0.3.6/tests/
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-12 13:06:07.177966 simim-0.3.6/tests/by_eye_checks/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1550 2024-03-14 23:47:34.000000 simim-0.3.6/tests/by_eye_checks/e2e_sfr.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1848 2024-03-21 23:11:46.000000 simim-0.3.6/tests/make_testbox_resource.py
+drwxr-xr-x   0 keenan   (649963457) MPIA\Domain Users (1357073302)        0 2024-04-12 13:06:07.178092 simim-0.3.6/tests/old_test_code/
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    12155 2024-02-28 21:12:40.000000 simim-0.3.6/tests/old_test_code/lightcone.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    11512 2024-03-20 23:23:48.000000 simim-0.3.6/tests/test_gridder.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     1799 2024-03-07 15:56:24.000000 simim-0.3.6/tests/test_imports.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    24778 2024-03-07 15:56:24.000000 simim-0.3.6/tests/test_instrument.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     3187 2024-02-28 21:05:15.000000 simim-0.3.6/tests/test_rawsiminterface.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)     3153 2024-03-21 23:16:14.000000 simim-0.3.6/tests/test_rawsiminterface2.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)      431 2024-03-07 15:56:24.000000 simim-0.3.6/tests/test_siminterface.py
+-rw-r--r--   0 keenan   (649963457) MPIA\Domain Users (1357073302)    11485 2024-03-20 23:58:31.000000 simim-0.3.6/tests/test_spec_gridder.py
```

### Comparing `simim-0.3.5/LICENSE` & `simim-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/PKG-INFO` & `simim-0.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simim
-Version: 0.3.5
+Version: 0.3.6
 Summary: Code for simulating the radio, sub-mm and FIR sky
 Author: R P Keenan
 License: MIT License
         
         Copyright (c) 2024 R P Keenan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -66,10 +66,14 @@
 4. tests directory - unit tests; these cover more recent additions to the SimIM source code
 but are relatively sparse for the galprops, lightcone, and siminterface modules.
 5. pyproject.toml, .readthedocs.yaml, .gitignore - config files for pip,
    readthedocs, and git
 
 Change Log
 ----------
+Version 0.3.6
+- Correct critical but in downloading TNG simulation data
+
 Version 0.3.5
 - Update ascii loader for UniverseMachine to use less memory and hopefully run faster
+- Gridder for spectra
 - Minor bug fixes and some tests
```

### Comparing `simim-0.3.5/README.md` & `simim-0.3.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -22,10 +22,14 @@
 4. tests directory - unit tests; these cover more recent additions to the SimIM source code
 but are relatively sparse for the galprops, lightcone, and siminterface modules.
 5. pyproject.toml, .readthedocs.yaml, .gitignore - config files for pip,
    readthedocs, and git
 
 Change Log
 ----------
+Version 0.3.6
+- Correct critical but in downloading TNG simulation data
+
 Version 0.3.5
 - Update ascii loader for UniverseMachine to use less memory and hopefully run faster
+- Gridder for spectra
 - Minor bug fixes and some tests
```

### Comparing `simim-0.3.5/docs/conf.py` & `simim-0.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/pyproject.toml` & `simim-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "simim"
 authors = [{name = "R P Keenan"}]
 description = "Code for simulating the radio, sub-mm and FIR sky"
 readme = "README.md"
 license = {file = "LICENSE"}
-version = "0.3.5"
+version = "0.3.6"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Astronomy"
 ]
 keywords = [
     "astronomy", "line intensity mapping", "LIM", "extragalactic",
```

### Comparing `simim-0.3.5/simim/_handlers.py` & `simim-0.3.6/simim/_handlers.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/_paths.py` & `simim-0.3.6/simim/_paths.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/_pltsetup.py` & `simim-0.3.6/simim/_pltsetup.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/constants.py` & `simim-0.3.6/simim/constants.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/galprops/galprops.py` & `simim-0.3.6/simim/galprops/galprops.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/galprops/galprops_am.py` & `simim-0.3.6/simim/galprops/galprops_am.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/galprops/galprops_builtin.py` & `simim-0.3.6/simim/galprops/galprops_builtin.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/galprops/line_co.py` & `simim-0.3.6/simim/galprops/line_co.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/galprops/line_co_dutycycle.py` & `simim-0.3.6/simim/galprops/line_co_dutycycle.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/galprops/line_densegas.py` & `simim-0.3.6/simim/galprops/line_densegas.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/galprops/line_fir.py` & `simim-0.3.6/simim/galprops/line_fir.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/galprops/line_fir_yang.py` & `simim-0.3.6/simim/galprops/line_fir_yang.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/galprops/log10normal.py` & `simim-0.3.6/simim/galprops/log10normal.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/galprops/sfr_behroozi13.py` & `simim-0.3.6/simim/galprops/sfr_behroozi13.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/galprops/sfr_bethermin17.py` & `simim-0.3.6/simim/galprops/sfr_bethermin17.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/galprops/sfr_ir.py` & `simim-0.3.6/simim/galprops/sfr_ir.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/instrument/_helpers.py` & `simim-0.3.6/simim/instrument/_helpers.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/instrument/instrument.py` & `simim-0.3.6/simim/instrument/instrument.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/instrument/noise_functions.py` & `simim-0.3.6/simim/instrument/noise_functions.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/instrument/spatial_response.py` & `simim-0.3.6/simim/instrument/spatial_response.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/instrument/spectral_response.py` & `simim-0.3.6/simim/instrument/spectral_response.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/lightcone/lchandler.py` & `simim-0.3.6/simim/lightcone/lchandler.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/lightcone/lcmaker.py` & `simim-0.3.6/simim/lightcone/lcmaker.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/map/gridder.py` & `simim-0.3.6/simim/map/gridder.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/resources/behroozi13_release.dat` & `simim-0.3.6/simim/resources/behroozi13_release.dat`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/siminterface/_illustris_datahandling.py` & `simim-0.3.6/simim/siminterface/_illustris_datahandling.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/siminterface/_rawsiminterface.py` & `simim-0.3.6/simim/siminterface/_rawsiminterface.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/siminterface/_sims.py` & `simim-0.3.6/simim/siminterface/_sims.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/siminterface/illustris.py` & `simim-0.3.6/simim/siminterface/illustris.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,15 +298,15 @@
                 not_downloaded.append(i)
         if len(not_downloaded) > 0:
             warnings.warn("No data exists for snapshots {} - run .download".format(not_downloaded))
 
         # File naming conventions for the raw simulation downloads:
         if self.sim in _illsims:
             self.raw_fname = 'groups_'
-        if self.sim == _tngsims:
+        if self.sim in _tngsims:
             self.raw_fname = 'fof_subhalo_tab_'
 
     # Function to load the data in a format we want:
     def _loader(self, path, snapshot, fields):
         """Loader to get a field from a snapshot halo catalog
 
         This is promarily meant for internal use by the .format method
```

### Comparing `simim-0.3.5/simim/siminterface/simhandler.py` & `simim-0.3.6/simim/siminterface/simhandler.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim/siminterface/universemachine.py` & `simim-0.3.6/simim/siminterface/universemachine.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim.egg-info/PKG-INFO` & `simim-0.3.6/simim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simim
-Version: 0.3.5
+Version: 0.3.6
 Summary: Code for simulating the radio, sub-mm and FIR sky
 Author: R P Keenan
 License: MIT License
         
         Copyright (c) 2024 R P Keenan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -66,10 +66,14 @@
 4. tests directory - unit tests; these cover more recent additions to the SimIM source code
 but are relatively sparse for the galprops, lightcone, and siminterface modules.
 5. pyproject.toml, .readthedocs.yaml, .gitignore - config files for pip,
    readthedocs, and git
 
 Change Log
 ----------
+Version 0.3.6
+- Correct critical but in downloading TNG simulation data
+
 Version 0.3.5
 - Update ascii loader for UniverseMachine to use less memory and hopefully run faster
+- Gridder for spectra
 - Minor bug fixes and some tests
```

### Comparing `simim-0.3.5/simim.egg-info/SOURCES.txt` & `simim-0.3.6/simim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim_dev/dev_features.py` & `simim-0.3.6/simim_dev/dev_features.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim_dev/dev_lim_stats.py` & `simim-0.3.6/simim_dev/dev_lim_stats.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim_dev/dev_spectral_functions.py` & `simim-0.3.6/simim_dev/dev_spectral_functions.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim_dev/old_obs_noise.py` & `simim-0.3.6/simim_dev/old_obs_noise.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/simim_dev/old_obs_radio.py` & `simim-0.3.6/simim_dev/old_obs_radio.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/tests/by_eye_checks/e2e_sfr.py` & `simim-0.3.6/tests/by_eye_checks/e2e_sfr.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/tests/make_testbox_resource.py` & `simim-0.3.6/tests/make_testbox_resource.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/tests/old_test_code/lightcone.py` & `simim-0.3.6/tests/old_test_code/lightcone.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/tests/test_gridder.py` & `simim-0.3.6/tests/test_gridder.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/tests/test_imports.py` & `simim-0.3.6/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/tests/test_instrument.py` & `simim-0.3.6/tests/test_instrument.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/tests/test_rawsiminterface.py` & `simim-0.3.6/tests/test_rawsiminterface.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/tests/test_rawsiminterface2.py` & `simim-0.3.6/tests/test_rawsiminterface2.py`

 * *Files identical despite different names*

### Comparing `simim-0.3.5/tests/test_spec_gridder.py` & `simim-0.3.6/tests/test_spec_gridder.py`

 * *Files identical despite different names*

