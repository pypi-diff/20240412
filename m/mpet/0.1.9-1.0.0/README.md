# Comparing `tmp/mpet-0.1.9.tar.gz` & `tmp/mpet-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpet-0.1.9.tar", last modified: Fri Jan 27 20:27:10 2023, max compression
+gzip compressed data, was "mpet-1.0.0.tar", last modified: Fri Apr 12 14:43:45 2024, max compression
```

## Comparing `mpet-0.1.9.tar` & `mpet-1.0.0.tar`

### file list

```diff
@@ -1,89 +1,106 @@
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-01-27 20:27:10.775100 mpet-0.1.9/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     2662 2022-02-21 14:49:31.000000 mpet-0.1.9/LICENSE
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     2951 2023-01-27 20:27:10.775100 mpet-0.1.9/PKG-INFO
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     2569 2023-01-27 20:04:19.000000 mpet-0.1.9/README.md
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-01-27 20:27:10.763100 mpet-0.1.9/bin/
--rwxrwxr-x   0 cogswell  (1001) cogswell  (1001)     3579 2023-01-13 16:18:34.000000 mpet-0.1.9/bin/mpetplot.py
--rwxrwxr-x   0 cogswell  (1001) cogswell  (1001)     1061 2022-02-21 14:49:31.000000 mpet-0.1.9/bin/mpetrun.py
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-01-27 20:27:10.767100 mpet-0.1.9/mpet/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       78 2022-02-21 14:49:31.000000 mpet-0.1.9/mpet/__init__.py
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-01-27 20:27:10.767100 mpet-0.1.9/mpet/config/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       96 2022-02-21 14:49:31.000000 mpet-0.1.9/mpet/config/__init__.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    35020 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/config/configuration.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1268 2023-01-13 16:18:31.000000 mpet-0.1.9/mpet/config/constants.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     8473 2022-11-17 21:22:40.000000 mpet-0.1.9/mpet/config/derived_values.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     4107 2022-08-03 20:32:18.000000 mpet-0.1.9/mpet/config/parameterset.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     7987 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/config/schemas.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      525 2022-08-03 20:32:18.000000 mpet-0.1.9/mpet/daeVariableTypes.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    12047 2022-02-21 14:49:31.000000 mpet-0.1.9/mpet/data_reporting.py
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-01-27 20:27:10.767100 mpet-0.1.9/mpet/electrode/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)        0 2022-02-21 14:49:31.000000 mpet-0.1.9/mpet/electrode/__init__.py
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-01-27 20:27:10.767100 mpet-0.1.9/mpet/electrode/diffusion/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      582 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/diffusion/__init__.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       31 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/diffusion/constant.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       35 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/diffusion/lattice.py
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-01-27 20:27:10.771100 mpet-0.1.9/mpet/electrode/materials/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      629 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/LiC6.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      379 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/LiC6_1param.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      779 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/LiC6_2step_ss.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1048 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/LiC6_LIONSIMBA.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      241 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/LiC6_coke_ss.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      272 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/LiC6_coke_ss2.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      420 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/LiC6_ss.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      458 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/LiC6_ss2.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      864 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/LiCoO2_LIONSIMBA.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      357 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/LiFePO4.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      422 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/LiMn2O4_ss.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      418 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/LiMn2O4_ss2.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      116 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/materials/Li_ss.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      330 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/NCA_ss1.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      618 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/NCA_ss2.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      191 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/materials/__init__.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      227 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/testIS_ss.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      215 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrode/materials/testRS.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      340 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/materials/testRS_ps.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      565 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/materials/testRS_ss.py
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-01-27 20:27:10.771100 mpet-0.1.9/mpet/electrode/reactions/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      386 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/reactions/BV.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      408 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/reactions/BV_gMod01.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      328 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/reactions/BV_mod01.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      328 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/reactions/BV_mod02.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      247 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/reactions/BV_raw.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      754 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/reactions/CIET.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      925 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/reactions/MHC.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      438 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/reactions/MHC_kfunc.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      846 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/reactions/Marcus.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       82 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrode/reactions/__init__.py
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-01-27 20:27:10.775100 mpet-0.1.9/mpet/electrolyte/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      775 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrolyte/Doyle96_EC_DMC_1_2.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      774 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/electrolyte/Doyle96_EC_DMC_2_1.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      788 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrolyte/LIONSIMBA_isothermal.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1286 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrolyte/LIONSIMBA_nonisothermal.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1036 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrolyte/LiClO4_PC.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      616 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrolyte/__init__.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1035 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrolyte/valoen_bernardi.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1217 2022-09-13 21:08:24.000000 mpet-0.1.9/mpet/electrolyte/valoen_reimers.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       49 2022-02-21 14:49:31.000000 mpet-0.1.9/mpet/exceptions.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1385 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/extern_funcs.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     3053 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/geometry.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     7081 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/main.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    25607 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/mod_cell.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    24736 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/mod_electrodes.py
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-01-27 20:27:10.775100 mpet-0.1.9/mpet/plot/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)        0 2022-02-21 14:49:31.000000 mpet-0.1.9/mpet/plot/__init__.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    13860 2022-02-21 14:49:31.000000 mpet-0.1.9/mpet/plot/colormaps_custom.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    11580 2023-01-13 16:18:34.000000 mpet-0.1.9/mpet/plot/outmat2txt.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    37094 2023-01-13 16:18:34.000000 mpet-0.1.9/mpet/plot/plot_data.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      907 2022-08-03 20:32:18.000000 mpet-0.1.9/mpet/ports.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     8193 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/props_am.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    10939 2023-01-13 16:18:34.000000 mpet-0.1.9/mpet/sim.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     6215 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/utils.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       22 2023-01-27 20:04:19.000000 mpet-0.1.9/mpet/version.py
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-01-27 20:27:10.767100 mpet-0.1.9/mpet.egg-info/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     2951 2023-01-27 20:27:10.000000 mpet-0.1.9/mpet.egg-info/PKG-INFO
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     2251 2023-01-27 20:27:10.000000 mpet-0.1.9/mpet.egg-info/SOURCES.txt
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)        1 2023-01-27 20:27:10.000000 mpet-0.1.9/mpet.egg-info/dependency_links.txt
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      126 2023-01-27 20:27:10.000000 mpet-0.1.9/mpet.egg-info/requires.txt
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)        5 2023-01-27 20:27:10.000000 mpet-0.1.9/mpet.egg-info/top_level.txt
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       38 2023-01-27 20:27:10.775100 mpet-0.1.9/setup.cfg
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1160 2022-09-13 21:08:24.000000 mpet-0.1.9/setup.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-12 14:43:45.595993 mpet-1.0.0/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     2662 2024-04-12 14:40:07.000000 mpet-1.0.0/LICENSE
+-rw-r--r--   0 cogswell  (1001) cogswell  (1001)     3611 2024-04-12 14:43:45.595993 mpet-1.0.0/PKG-INFO
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     2569 2024-04-12 14:40:07.000000 mpet-1.0.0/README.md
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-12 14:43:45.579992 mpet-1.0.0/bin/
+-rwxrwxr-x   0 cogswell  (1001) cogswell  (1001)     1504 2024-04-12 14:40:07.000000 mpet-1.0.0/bin/create_ensemble.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     3976 2024-04-12 14:40:07.000000 mpet-1.0.0/bin/mpet_create_runjobs_dashboard.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    27523 2024-04-12 14:40:07.000000 mpet-1.0.0/bin/mpet_plot_app.py
+-rwxrwxr-x   0 cogswell  (1001) cogswell  (1001)     4768 2024-04-12 14:40:07.000000 mpet-1.0.0/bin/mpetplot.py
+-rwxrwxr-x   0 cogswell  (1001) cogswell  (1001)     1061 2024-04-12 14:40:07.000000 mpet-1.0.0/bin/mpetrun.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     5165 2024-04-12 14:40:07.000000 mpet-1.0.0/bin/run_jobs.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-12 14:43:45.579992 mpet-1.0.0/mpet/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       78 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/__init__.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-12 14:43:45.583992 mpet-1.0.0/mpet/config/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       96 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/config/__init__.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    40526 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/config/configuration.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1344 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/config/constants.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     9035 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/config/derived_values.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     4092 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/config/parameterset.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    10007 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/config/schemas.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      525 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/daeVariableTypes.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    12047 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/data_reporting.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-12 14:43:45.575992 mpet-1.0.0/mpet/electrode/
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-12 14:43:45.583992 mpet-1.0.0/mpet/electrode/diffusion/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      232 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/diffusion/NMC532_Colclasure20.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      581 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/diffusion/__init__.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       31 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/diffusion/constant.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       35 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/diffusion/lattice.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-12 14:43:45.587993 mpet-1.0.0/mpet/electrode/materials/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      368 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/LTO.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      629 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/LiC6.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      379 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/LiC6_1param.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      779 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/LiC6_2step_ss.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1704 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/LiC6_Colclasure_1506T.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1048 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/LiC6_LIONSIMBA.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      241 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/LiC6_coke_ss.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      272 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/LiC6_coke_ss2.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      420 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/LiC6_ss.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      458 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/LiC6_ss2.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      864 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/LiCoO2_LIONSIMBA.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      357 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/LiFePO4.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      422 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/LiMn2O4_ss.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      418 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/LiMn2O4_ss2.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      116 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/Li_ss.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      330 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/NCA_ss1.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      618 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/NCA_ss2.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      826 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/NMC532_Colclasure20.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      191 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/__init__.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      227 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/testIS_ss.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      215 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/testRS.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      340 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/testRS_ps.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      565 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/materials/testRS_ss.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-12 14:43:45.587993 mpet-1.0.0/mpet/electrode/reactions/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      386 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/reactions/BV.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      465 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/reactions/BV_Colclasure20.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      376 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/reactions/BV_NMC_Park2021.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      408 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/reactions/BV_gMod01.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      328 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/reactions/BV_mod01.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      328 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/reactions/BV_mod02.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      247 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/reactions/BV_raw.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      754 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/reactions/CIET.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      925 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/reactions/MHC.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      438 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/reactions/MHC_kfunc.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      846 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/reactions/Marcus.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       82 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrode/reactions/__init__.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-12 14:43:45.591992 mpet-1.0.0/mpet/electrolyte/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     2057 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrolyte/Colclasure20.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      775 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrolyte/Doyle96_EC_DMC_1_2.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      774 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrolyte/Doyle96_EC_DMC_2_1.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      788 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrolyte/LIONSIMBA_isothermal.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1286 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrolyte/LIONSIMBA_nonisothermal.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1036 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrolyte/LiClO4_PC.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      617 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrolyte/__init__.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      369 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrolyte/solid_elyte.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1035 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrolyte/valoen_bernardi.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1217 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/electrolyte/valoen_reimers.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       49 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/exceptions.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1385 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/extern_funcs.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     3721 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/geometry.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     7731 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/main.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    27924 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/mod_CCCVCPcycle.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    31663 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/mod_cell.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    30708 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/mod_electrodes.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     9996 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/mod_interface.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-12 14:43:45.591992 mpet-1.0.0/mpet/plot/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)        0 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/plot/__init__.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    13860 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/plot/colormaps_custom.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    15038 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/plot/outmat2txt.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    48002 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/plot/plot_data.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    23787 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/plot/plot_data_db.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1631 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/ports.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     9281 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/props_am.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)    13676 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/sim.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     7883 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/utils.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       22 2024-04-12 14:40:07.000000 mpet-1.0.0/mpet/version.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-12 14:43:45.591992 mpet-1.0.0/mpet.egg-info/
+-rw-r--r--   0 cogswell  (1001) cogswell  (1001)     3611 2024-04-12 14:43:45.000000 mpet-1.0.0/mpet.egg-info/PKG-INFO
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     2763 2024-04-12 14:43:45.000000 mpet-1.0.0/mpet.egg-info/SOURCES.txt
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)        1 2024-04-12 14:43:45.000000 mpet-1.0.0/mpet.egg-info/dependency_links.txt
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      206 2024-04-12 14:43:45.000000 mpet-1.0.0/mpet.egg-info/requires.txt
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)        5 2024-04-12 14:43:45.000000 mpet-1.0.0/mpet.egg-info/top_level.txt
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       38 2024-04-12 14:43:45.595993 mpet-1.0.0/setup.cfg
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1411 2024-04-12 14:40:07.000000 mpet-1.0.0/setup.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2024-04-12 14:43:45.591992 mpet-1.0.0/tests/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     4186 2024-04-12 14:40:07.000000 mpet-1.0.0/tests/test_defs.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     8351 2024-04-12 14:40:07.000000 mpet-1.0.0/tests/test_suite.py
```

### Comparing `mpet-0.1.9/LICENSE` & `mpet-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/PKG-INFO` & `mpet-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: mpet
-Version: 0.1.9
-Summary: Multiphase porous electrode theory
-Home-page: https://bitbucket.org/bazantgroup/mpet
-Author: Dan Cogswell
-Author-email: cogswell@mit.edu
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: doc
-License-File: LICENSE
-
 [![Build](https://img.shields.io/github/actions/workflow/status/TRI-AMDD/mpet/mpet-regression-test.yml?branch=development)](https://github.com/TRI-AMDD/mpet/actions/workflows/mpet-regression-test.yml)
 [![Coverage Status](https://coveralls.io/repos/github/TRI-AMDD/mpet/badge.svg?branch=development)](https://coveralls.io/github/TRI-AMDD/mpet?branch=development)
 [![readthedocs](https://readthedocs.org/projects/mpet/badge/?version=latest)](https://mpet.readthedocs.io)
 [![release](https://img.shields.io/github/v/release/TRI-AMDD/mpet)](https://github.com/TRI-AMDD/mpet/releases)
 
 # MPET -- Multiphase Porous Electrode Theory
```

### Comparing `mpet-0.1.9/bin/mpetrun.py` & `mpet-1.0.0/bin/mpetrun.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/config/configuration.py` & `mpet-1.0.0/mpet/config/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,18 +136,14 @@
         # load system parameters file
         self.D_s = ParameterSet(paramfile, 'system', self.path)
         # the anode and separator are optional: only if there are volumes to simulate
         trodes = ['c']
         if self.D_s['Nvol_a'] > 0:
             trodes.append('a')
         self['trodes'] = trodes
-        # to check for separator, directly access underlying dict of system config;
-        # self['Nvol']['s'] would not work because that requires have_separator to
-        # be defined already
-        self['have_separator'] = self.D_s['Nvol_s'] > 0
 
         # load electrode parameter file(s)
         self.paramfiles = {}
 
         cathode_paramfile = self.D_s['cathode']
         if not os.path.isabs(cathode_paramfile):
             cathode_paramfile = os.path.join(self.path, cathode_paramfile)
@@ -413,14 +409,15 @@
         second time results in an error. The processing consists of several steps:
 
         #. Set numpy random seed (if enabled in config)
         #. Set default values
         #. Scale to non-dimensional values
         #. Parse current/voltage segments
         #. Either generate particle distributions or load from previous run
+        #. Create simulation times
 
         :param bool prevDir: if True, load particle distributions from previous run,
             otherwise generate them
         """
         if self.config_processed:
             raise Exception('The config can be processed only once as values are scaled in-place')
         self.config_processed = True
@@ -436,14 +433,18 @@
         limtrode = self['limtrode']
         theoretical_1C_current = self[limtrode, 'cap'] / 3600.  # A/m^2
         param = '1C_current_density'
         if self[param] is None:
             # set to theoretical value
             self[param] = theoretical_1C_current
 
+        # use custom concentration when using solid electrolyte model
+        if self['elyteModelType'] == 'solid':
+            self['c0'] = self['c0']
+
         # apply scalings
         self._scale_system_parameters(theoretical_1C_current)
         self._scale_electrode_parameters()  # includes separator
         # reference voltage, should only be calculated after scaling of system and trode parameters
         Vref = self['c', 'phiRef']
         if 'a' in self['trodes']:
             Vref -= self['a', 'phiRef']
@@ -459,14 +460,24 @@
             # particle distributions
             self._distr_part()
             # Gibss free energy, must be done after distr_part
             self._G()
             # Electrode parameters that depend on invidividual particle
             self._indvPart()
 
+        self._create_times()
+
+    def _create_times(self):
+        """
+
+        """
+        # The list of reporting times excludes the first index (zero, which is implied)
+        if not self["times"]:
+            self["times"] = list(np.linspace(0, self["tend"], self["tsteps"] + 1))[1:]
+
     def _scale_system_parameters(self, theoretical_1C_current):
         """
         Scale system parameters to non-dimensional values. This method should be called only once,
         from :meth:`_process_config`.
         """
         # non-dimensional scalings
         self['T'] = self['T'] / constants.T_ref
@@ -479,17 +490,27 @@
         self['phi_cathode'] = 0.  # TODO: why is this defined if always 0?
         self['currset'] = self['currset'] / (theoretical_1C_current * self['curr_ref'])
         if self['power'] is not None:
             self['power'] = self['power'] / (self['power_ref'])
         self['k0_foil'] = self['k0_foil'] / (self['1C_current_density'] * self['curr_ref'])
         self['Rfilm_foil'] = self['Rfilm_foil'] / self['Rser_ref']
 
+        if self['elyteModelType'] == 'solid':
+            self['cmax'] = self['cmax'] / constants.c_ref
+
+        if self['simInterface_a'] or self['simInterface_c']:
+            self['Dp_i'] = self['Dp_i'] / self['D_ref']
+            if self['interfaceModelType'] != 'solid':
+                self['Dm_i'] = self['Dm_i'] / self['D_ref']
+            self['c0_int'] = self['c0_int'] / constants.c_ref
+            self['cmax_i'] = self['cmax_i'] / constants.c_ref
+
     def _scale_electrode_parameters(self):
         """
-        Scale electrode and separator parameters to non-dimensional values.
+        Scale electrode, separator, and interface region parameters to non-dimensional values.
         This method should be called only once, from :meth:`_process_config`.
         """
         kT = constants.k * constants.T_ref
 
         # scalings per electrode
         self['beta'] = {}
         for trode in self['trodes']:
@@ -502,17 +523,21 @@
                 self[trode, 'B'] = self[trode, 'B'] / (kT * constants.N_A * self[trode, 'cs_ref'])
             for param in ['Omega_a', 'Omega_b', 'Omega_c', 'EvdW']:
                 value = self[trode, param]
                 if value is not None:
                     self[trode, param] = value / kT
 
         # scalings on separator
-        if self['have_separator']:
+        if self['Nvol']['s']:
             self['L']['s'] /= self['L_ref']
 
+        # scaling related to interface region (if present)
+        if self['simInterface_a'] or self['simInterface_c']:
+            self['L_i'] /= self['L_ref']
+
     def _scale_macroscopic_parameters(self, Vref):
         """
         Scale macroscopic input parameters to non-dimensional values and add
         reference values.
         This method should be called only once, from :meth:`_process_config`.
         """
 
@@ -537,35 +562,90 @@
                 segments.append((self["segments"][i][0]*self["1C_current_density"]
                                 / theoretical_1C_current/self['curr_ref'],
                                 self["segments"][i][1]*60/self['t_ref']))
         elif self['profileType'] == 'CVsegments':
             for i in range(len(self['segments'])):
                 segments.append((-((constants.e/kT)*self['segments'][i][0]+Vref),
                                 self['segments'][i][1]*60/self['t_ref']))
+        elif self['profileType'] == 'CCCVCPcycle':
+            # just a simple cycler
+            for i in range(len(self["segments"])):
+
+                # find hard capfrac cutoff (0.99 for charge, 0.01 for discharge)
+                hard_cut = self["capFrac"] if self["segments"][i][5] <= 2 else 1 - \
+                    self["capFrac"]
+                # if input is None, stores as None for cutoffs only. otherwise
+                # nondimensionalizes cutoffs & setpoints
+                volt_cut = None if self["segments"][i][1] is None else - \
+                    ((constants.e/kT)*(self["segments"][i][1])+Vref)
+                # we set capfrac cutoff to be 0.99 if it is not set to prevent overfilling
+                # capfrac_cut = 0.99 if dD_s["segments"][i][2] == None else
+                # dD_s["segments"][i][2]
+                capfrac_cut = hard_cut if self["segments"][i][2] is None \
+                    else self["segments"][i][2]
+                crate_cut = None if self["segments"][i][3] is None else \
+                    self['segments'][i][3] * self["1C_current_density"] / \
+                    theoretical_1C_current / self['curr_ref']
+                time_cut = None if self["segments"][i][4] is None else \
+                    self["segments"][i][4]*60/self['t_ref']
+                if not (volt_cut or capfrac_cut or crate_cut or time_cut):
+                    print(
+                        "Warning: in segment "
+                        + str(i)
+                        + " of the cycle no cutoff is specified.")
+                if self["segments"][i][5] == 1 or self["segments"][i][5] == 4:
+                    # stores Crate, voltage cutoff, capfrac cutoff, C-rate cutoff(none),  time
+                    # cutoff, type
+                    segments.append(
+                        (self["segments"][i][0]
+                         * self["1C_current_density"]
+                         / theoretical_1C_current
+                         / self['curr_ref'],
+                         volt_cut,
+                         capfrac_cut,
+                         None,
+                         time_cut,
+                         self["segments"][i][5]))
+                elif self["segments"][i][5] == 2 or self["segments"][i][5] == 5:
+                    # stores voltage, voltage cutoff (none), capfrac cutoff, C-rate cutoff,
+                    # time cutoff, type
+                    segments.append((-((constants.e/kT)*(
+                        self["segments"][i][0])+Vref), None, capfrac_cut, crate_cut, time_cut,
+                        self["segments"][i][5]))
+                # elif CP segments
+                elif self["segments"][i][5] == 3 or self["segments"][i][5] == 6:
+                    segments.append((-(constants.e/(kT*self['curr_ref']
+                                                    * theoretical_1C_current))
+                                     * self["segments"][i][0], volt_cut, capfrac_cut,
+                                     crate_cut, time_cut, self["segments"][i][5]))
+                # elif just incrementing step
+                elif self["segments"][i][5] == 0:
+                    segments.append((0, None, None, None, None, 0))
 
         # Current or voltage segments profiles
         segments_tvec = np.zeros(2 * self['numsegments'] + 1)
         segments_setvec = np.zeros(2 * self['numsegments'] + 1)
         if self['profileType'] == 'CCsegments':
             segments_setvec[0] = 0.
         elif self['profileType'] == 'CVsegments':
             segments_setvec[0] = -(kT / constants.e) * Vref
         tPrev = 0.
-        for segIndx in range(self['numsegments']):
-            tNext = tPrev + self['tramp']
-            segments_tvec[2*segIndx+1] = tNext
-            tPrev = tNext
-            # Factor of 60 here to convert to s
-            tNext = tPrev + (self['segments'][segIndx][1] * 60 - self["tramp"])
-            segments_tvec[2*segIndx+2] = tNext
-            tPrev = tNext
-            setNext = self['segments'][segIndx][0]
-            segments_setvec[2*segIndx+1] = setNext
-            segments_setvec[2*segIndx+2] = setNext
-        segments_tvec /= self['t_ref']
+        if self['profileType'] == 'CCsegments' or self['profileType'] == 'CVsegments':
+            for segIndx in range(self['numsegments']):
+                tNext = tPrev + self['tramp']
+                segments_tvec[2*segIndx+1] = tNext
+                tPrev = tNext
+                # Factor of 60 here to convert to s
+                tNext = tPrev + (self['segments'][segIndx][1] * 60 - self["tramp"])
+                segments_tvec[2*segIndx+2] = tNext
+                tPrev = tNext
+                setNext = self['segments'][segIndx][0]
+                segments_setvec[2*segIndx+1] = setNext
+                segments_setvec[2*segIndx+2] = setNext
+            segments_tvec /= self['t_ref']
         if self['profileType'] == 'CCsegments':
             segments_setvec *= self["1C_current_density"]/theoretical_1C_current/self['curr_ref']
         elif self['profileType'] == 'CVsegments':
             segments_setvec = -((constants.e/kT)*segments_setvec + Vref)
         if 'segments' in self['profileType']:
             self['tend'] = segments_tvec[-1]
             # Pad the last segment so no extrapolation occurs
@@ -602,14 +682,16 @@
         # intialize dicts in config
         self['psd_num'] = {}
         self['psd_len'] = {}
         self['psd_area'] = {}
         self['psd_vol'] = {}
         self['psd_vol_FracVol'] = {}
 
+        self['gamma_contact'] = {}
+
         for trode in self['trodes']:
             solidType = self[trode, 'type']
             Nvol = self['Nvol'][trode]
             Npart = self['Npart'][trode]
 
             # check if PSD is specified. If so, it is an ndarray so use np.all
             if not np.all(self['specified_psd'][trode]):
@@ -627,18 +709,35 @@
             else:
                 # use user-defined PSD
                 raw = self['specified_psd'][trode]
                 if raw.shape != (Nvol, Npart):
                     raise ValueError('Specified particle size distribution discretization '
                                      'of volumes inequal to the one specified in the config file')
 
+            stddev_c = self['stand_dev_contact']
+            mean_c = self['fraction_of_contact']
+
+            if 0 < mean_c < 1:
+                # Contact penalty for BV
+                mean_c = 1 - mean_c  # to make distribution start at 1 if gamma is 1
+                var_c = stddev_c**2
+                mu_c = np.log((mean_c**2) / np.sqrt(var_c + mean_c**2))
+                sigma_c = np.sqrt(np.log(var_c/(mean_c**2) + 1))
+                raw_c = 1 - np.random.lognormal(mu_c, sigma_c, size=(Nvol, Npart))
+                raw_c[raw_c <= 0.0001] = 0.0001
+                gamma_contact = raw_c
+            elif mean_c == 1:
+                gamma_contact = np.ones((Nvol, Npart))
+            else:
+                raise NotImplementedError('Contact error should be between 0 and 1')
+
             # For particles with internal profiles, convert psd to
             # integers -- number of steps
             solidDisc = self[trode, 'discretization']
-            if solidType in ['ACR']:
+            if solidType in ['ACR','ACR_Diff','ACR2']:
                 psd_num = np.ceil(raw / solidDisc).astype(int)
                 psd_len = solidDisc * psd_num
             elif solidType in ['CHR', 'diffn', 'CHR2', 'diffn2']:
                 psd_num = np.ceil(raw / solidDisc).astype(int) + 1
                 psd_len = solidDisc * (psd_num - 1)
             # For homogeneous particles (only one 'volume' per particle)
             elif solidType in ['homog', 'homog_sdn', 'homog2', 'homog2_sdn']:
@@ -670,14 +769,15 @@
 
             # store values to config
             self['psd_num'][trode] = psd_num
             self['psd_len'][trode] = psd_len
             self['psd_area'][trode] = psd_area
             self['psd_vol'][trode] = psd_vol
             self['psd_vol_FracVol'][trode] = psd_frac_vol
+            self['gamma_contact'][trode] = gamma_contact
 
     def _G(self):
         """
         Generate Gibbs free energy distribution and store in config.
         """
         self['G'] = {}
         for trode in self['trodes']:
@@ -717,14 +817,15 @@
             for i in range(Nvol):
                 for j in range(Npart):
                     # This specific particle dimensions
                     self[trode, 'indvPart']['N'][i, j] = self['psd_num'][trode][i,j]
                     plen = self['psd_len'][trode][i,j]
                     parea = self['psd_area'][trode][i,j]
                     pvol = self['psd_vol'][trode][i,j]
+                    gamma_cont = self['gamma_contact'][trode][i,j]
                     # Define a few reference scales
                     F_s_ref = plen * cs_ref_part / self['t_ref']  # part/(m^2 s)
                     i_s_ref = constants.e * F_s_ref  # A/m^2
                     kappa_ref = constants.k * constants.T_ref * cs_ref_part * plen**2  # J/m
                     gamma_S_ref = kappa_ref / plen  # J/m^2
                     # non-dimensional quantities
                     if self[trode, 'kappa'] is not None:
@@ -734,14 +835,18 @@
                         self[trode, 'indvPart']['beta_s'][i, j] = nd_dgammadc \
                             / self[trode, 'indvPart']['kappa'][i, j]
                     self[trode, 'indvPart']['D'][i, j] = self[trode, 'D'] * self['t_ref'] / plen**2
                     self[trode, 'indvPart']['E_D'][i, j] = self[trode, 'E_D'] \
                         / (constants.k * constants.N_A * constants.T_ref)
                     self[trode, 'indvPart']['k0'][i, j] = self[trode, 'k0'] \
                         / (constants.e * F_s_ref)
+                    self[trode, 'indvPart']['gamma_con'][i, j] = gamma_cont
+                    if self['fraction_of_contact'] != 1.0 and not self['localized_losses']:
+                        self[trode, 'indvPart']['k0'][i, j] = self[trode, 'k0'] \
+                            / (constants.e * F_s_ref)*gamma_cont
                     self[trode, 'indvPart']['E_A'][i, j] = self[trode, 'E_A'] \
                         / (constants.k * constants.N_A * constants.T_ref)
                     self[trode, 'indvPart']['Rfilm'][i, j] = self[trode, 'Rfilm'] \
                         / (constants.k * constants.T_ref / (constants.e * i_s_ref))
                     self[trode, 'indvPart']['delta_L'][i, j] = (parea * plen) / pvol
                     # If we're using the model that varies Omg_a with particle size,
                     # overwrite its value for each particle
@@ -759,16 +864,16 @@
         """
         Verify configuration parameters.
         """
         # solid type
         for trode in self['trodes']:
             solidShape = self[trode, 'shape']
             solidType = self[trode, 'type']
-            if solidType in ["ACR", "homog_sdn"] and solidShape != "C3":
-                raise Exception("ACR and homog_sdn req. C3 shape")
+            if solidType in ["ACR", "ACR_Diff", "homog_sdn", "ACR2"] and solidShape != "C3":
+                raise Exception("ACR, ACR_Diff, ACR2 and homog_sdn req. C3 shape")
             if (solidType in ["CHR", "diffn"] and solidShape not in ["sphere", "cylinder"]):
                 raise NotImplementedError("CHR and diffn req. sphere or cylinder")
 
     @staticmethod
     def size2regsln(size):
         """
         This function returns the non-dimensional regular solution
```

### Comparing `mpet-0.1.9/mpet/config/constants.py` & `mpet-1.0.0/mpet/config/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 #: Electron charge, C
 e = 1.602e-19
 #: Avogadro constant, particle / mol
 N_A = 6.022e23
 #: Reference flux, C/mol
 F = e * N_A
 #: General particle classification (1 var)
-two_var_types = ["diffn2", "CHR2", "homog2", "homog2_sdn"]
+two_var_types = ["diffn2", "CHR2", "homog2", "homog2_sdn", "ACR2"]
 #: General particle classification (2 var)
-one_var_types = ["ACR", "diffn", "CHR", "homog", "homog_sdn"]
+one_var_types = ["ACR","ACR_Diff", "diffn", "CHR", "homog", "homog_sdn"]
 #: Reference concentration, mol/m^3 = 1M
 c_ref = 1000.
 #: Reaction rate epsilon for values close to zero
 reactions_epsilon = 1e-12
 
 #: parameter that are defined per electrode with a ``_{electrode}`` suffix
 PARAMS_PER_TRODE = ['Nvol', 'Npart', 'mean', 'stddev', 'cs0', 'simBulkCond', 'sigma_s',
                     'simPartCond', 'G_mean', 'G_stddev', 'L', 'P_L', 'poros', 'BruggExp',
-                    'specified_psd']
+                    'specified_psd','specified_poros']
 #: subset of ``PARAMS_PER_TRODE``` that is defined for the separator as well
-PARAMS_SEPARATOR = ['Nvol', 'L', 'poros', 'BruggExp']
+PARAMS_SEPARATOR = ['Nvol', 'L', 'poros', 'BruggExp', 'specified_poros']
 #: parameters that are defined for each particle, and their type
 PARAMS_PARTICLE = {'N': int, 'kappa': float, 'beta_s': float, 'D': float, 'k0': float,
                    'Rfilm': float, 'delta_L': float, 'Omega_a': float, 'E_D': float,
-                   'E_A': float}
+                   'E_A': float, 'gamma_con': float}
```

### Comparing `mpet-0.1.9/mpet/config/derived_values.py` & `mpet-1.0.0/mpet/config/derived_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,16 +169,24 @@
         """Maximum concentration for given electrode
         """
         return self.config[trode, 'rho_s'] / constants.N_A
 
     def cap(self, trode):
         """Theoretical capacity of given electrode
         """
-        return constants.e * self.config['L'][trode] * (1 - self.config['poros'][trode]) \
+        capacity = constants.e * self.config['L'][trode] * (1 - self.config['poros'][trode]) \
             * self.config['P_L'][trode] * self.config[trode, 'rho_s']
+        if np.all(self.config['specified_poros'][trode]):
+            sum_porosity = 0
+            for i in self.config['specified_poros'][trode]:
+                sum_porosity = sum_porosity + i
+            avg_porosity = sum_porosity/np.size(self.config['specified_poros'][trode])
+            capacity = constants.e * self.config['L'][trode] * (1 - avg_porosity) \
+                * self.config['P_L'][trode] * self.config[trode, 'rho_s']
+        return capacity
 
     def numsegments(self):
         """Number of segments in voltage/current profile
         """
         return len(self.config['segments'])
 
     def L_ref(self):
@@ -187,14 +195,16 @@
         return self.config['L']['c']
 
     def D_ref(self):
         """Reference diffusivity
         """
         if self.config['elyteModelType'] == 'dilute':
             return self.config['Damb']
+        elif self.config['elyteModelType'] == 'solid':
+            return self.config['Damb']
         else:
             SMset = self.config["SMset"]
             elyte_function = import_function(self.config["SMset_filename"], SMset,
                                              mpet_module=f"mpet.electrolyte.{SMset}")
             return elyte_function()[-1]
 
     def z(self):
```

### Comparing `mpet-0.1.9/mpet/config/parameterset.py` & `mpet-1.0.0/mpet/config/parameterset.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         Create config from file.
 
         :param str fname: full path to .cfg file
         """
         if not os.path.isfile(fname):
             raise Exception(f'Missing config file: {fname}')
         # create config parser
-        parser = configparser.ConfigParser()
+        parser = configparser.ConfigParser(strict=False)
         parser.optionxform = str
         parser.read(fname)
 
         # get schemas for all potential sections
         section_schemas = getattr(schemas, self.config_type)
 
         # load each potential section and validate schema
@@ -83,15 +83,15 @@
         elif item in PARAMS_PER_TRODE:
             # this is only valid for electrode config
             assert self.config_type == 'system', 'Requested electrode parameter from system config'
             # create a new dict containg the value per electrode
             d = {}
             # some parameters are also defined for the separator
             trodes = self['trodes'][:]  # make a copy here to avoid adding values to the original
-            if item in PARAMS_SEPARATOR and self['have_separator']:
+            if item in PARAMS_SEPARATOR:
                 trodes.append('s')
             for trode in trodes:
                 # get the value for this electrode/separator and store it
                 key = f'{item}_{trode}'
                 d[trode] = self[key]
                 del self.params[key]
             self.params[item] = d
```

### Comparing `mpet-0.1.9/mpet/config/schemas.py` & `mpet-1.0.0/mpet/config/schemas.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     :param str key: The raw key from the config file
     :return: segments (tuple)
     """
     segments = ast.literal_eval(key)
     assert isinstance(segments, list), "segments must be a list"
     assert len(segments) > 0, "There must be at least one segment"
     for item in segments:
-        assert (isinstance(item, tuple)) and (len(item) == 2), \
+        assert (len(item) == 6) or (len(item) == 2), \
             "Each segment must be a tuple of (setpoint, time)"
     return segments
 
 
 def check_allowed_values(value, allowed_values):
     """
     Check if value was chosen from a set of allowed values
@@ -47,49 +47,60 @@
     :return: Boolean representation of value
     """
     assert isinstance(value, str), f"{value} must be a string"
     # strtobool returns 0 or 1, use bool() to convert to actual boolean type
     return bool(strtobool(value))
 
 
+#: Defaults for config sections that are optional
+DEFAULT_SECTIONS = {'Interface': {'simInterface_a': False, 'simInterface_c': False}}
+
+
 #: System parameters, per section
 system = {'Sim Params': {'profileType': lambda x:
-                         check_allowed_values(x, ["CC", "CV", "CP", "CCsegments", "CVsegments"]),
+                         check_allowed_values(x, ["CC", "CV", "CP", "CCsegments", "CVsegments",
+                                                  "CCCVCPcycle"]),
                          'Crate': Use(float),
                          Optional('power', default=None): Use(float),
                          Optional('1C_current_density', default=None): Use(float),
                          Optional('tramp', default=0.): Use(float),
                          'Vmax': Use(float),
                          'Vmin': Use(float),
                          Optional('Vset', default=None): Use(float),
                          Optional('capFrac', default=1.0): Use(float),
                          Optional('segments', default=[]): Use(parse_segments),
                          Optional('prevDir', default=''): str,
                          'tend': And(Use(float), lambda x: x > 0),
                          'tsteps': And(Use(int), lambda x: x > 0),
+                         Optional('times', default=[]): Use(ast.literal_eval),
                          'relTol': And(Use(float), lambda x: x > 0),
                          'absTol': And(Use(float), lambda x: x > 0),
                          'T': Use(float),
                          'randomSeed': Use(tobool),
                          Optional('seed'): And(Use(int), lambda x: x >= 0),
                          Optional('dataReporter', default='mat'): str,
                          'Rser': Use(float),
                          'Nvol_c': And(Use(int), lambda x: x > 0),
                          'Nvol_s': And(Use(int), lambda x: x >= 0),
                          'Nvol_a': And(Use(int), lambda x: x >= 0),
                          'Npart_c': And(Use(int), lambda x: x >= 0),
-                         'Npart_a': And(Use(int), lambda x: x >= 0)},
+                         'Npart_a': And(Use(int), lambda x: x >= 0),
+                         Optional('totalCycle', default=1): And(Use(int), lambda x: x >= 0)},
           'Electrodes': {'cathode': str,
                          'anode': str,
                          'k0_foil': Use(float),
                          'Rfilm_foil': Use(float)},
           'Particles': {'mean_c': Use(float),
                         'stddev_c': Use(float),
                         'mean_a': Use(float),
                         'stddev_a': Use(float),
+                        Optional('fraction_of_contact',default=1.0): Use(float),
+                        Optional('stand_dev_contact',default=0): Use(float),
+                        Optional('localized_losses', default=False):
+                            Or(Use(tobool), Use(lambda x: np.array(ast.literal_eval(x)))),
                         'cs0_c': Use(float),
                         'cs0_a': Use(float),
                         Optional('specified_psd_c', default=False):
                             Or(Use(tobool), Use(lambda x: np.array(ast.literal_eval(x)))),
                         Optional('specified_psd_a', default=False):
                             Or(Use(tobool), Use(lambda x: np.array(ast.literal_eval(x))))},
           'Conductivity': {'simBulkCond_c': Use(tobool),
@@ -106,29 +117,49 @@
                        'L_a': Use(float),
                        'L_s': Use(float),
                        'P_L_c': Use(float),
                        'P_L_a': Use(float),
                        'poros_c': Use(float),
                        'poros_a': Use(float),
                        'poros_s': Use(float),
+                       Optional('specified_poros_c', default=False):
+                            Or(Use(tobool), Use(lambda x: np.array(ast.literal_eval(x)))),
+                       Optional('specified_poros_a', default=False):
+                            Or(Use(tobool), Use(lambda x: np.array(ast.literal_eval(x)))),
+                       Optional('specified_poros_s', default=False):
+                            Or(Use(tobool), Use(lambda x: np.array(ast.literal_eval(x)))),
                        'BruggExp_c': Use(float),
                        'BruggExp_a': Use(float),
                        'BruggExp_s': Use(float)},
           'Electrolyte': {'c0': Use(float),
                           'zp': Use(int),
                           'zm': And(Use(int), lambda x: x < 0),
                           'nup': Use(int),
                           'num': Use(int),
                           'elyteModelType': str,
                           Optional('SMset_filename', default=None): str,
                           'SMset': str,
                           'n': Use(int),
                           'sp': Use(int),
                           Optional('Dp', default=None): Use(float),
-                          Optional('Dm', default=None): Use(float)}}
+                          Optional('Dm', default=None): Use(float),
+                          Optional('cmax'): Use(float),
+                          Optional('a_slyte'): Use(float)},
+          'Interface': {Optional('simInterface_a',default=False): Use(tobool),
+                        Optional('simInterface_c',default=False): Use(tobool),
+                        Optional('Nvol_i'): And(Use(int), lambda x: x > 0),
+                        Optional('L_i'): Use(float),
+                        Optional('BruggExp_i'): Use(float),
+                        Optional('poros_i'): Use(float),
+                        Optional('interfaceModelType'): str,
+                        Optional('interfaceSMset'): str,
+                        Optional('c0_int'): Use(float),
+                        Optional('cmax_i'): Use(float),
+                        Optional('Dp_i'): Use(float),
+                        Optional('Dm_i'): Use(float)}}
 
 #: Electrode parameters, per section
 electrode = {'Particles': {'type': lambda x: check_allowed_values(x,
                                                                   constants.one_var_types
                                                                   + constants.two_var_types),
                            'discretization': Use(float),
                            'shape': lambda x:
```

### Comparing `mpet-0.1.9/mpet/daeVariableTypes.py` & `mpet-1.0.0/mpet/daeVariableTypes.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/data_reporting.py` & `mpet-1.0.0/mpet/data_reporting.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrode/diffusion/__init__.py` & `mpet-1.0.0/mpet/electrode/diffusion/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """This folder contains diffusion functions that return
- the filling-fraction dependent variation of
+the filling-fraction dependent variation of
 the transport coefficient, D(y), such that
 Flux = -D_ref*D(y)*grad(y) for solid solution transport or
 Flux = -D_ref*D(y)*grad(mu) for thermo-based transport
 where y here is the filling fraction, D_ref has dimensions of
 length^2/time, D(y) is dimensionless, and mu, the chemical
 potential, has been scaled to the thermal energy, k*Tref. For more
 details on the two forms, see muRfuncs which defines both solid
```

### Comparing `mpet-0.1.9/mpet/electrode/materials/LiC6.py` & `mpet-1.0.0/mpet/electrode/materials/LiC6.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrode/materials/LiC6_2step_ss.py` & `mpet-1.0.0/mpet/electrode/materials/LiC6_2step_ss.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrode/materials/LiC6_LIONSIMBA.py` & `mpet-1.0.0/mpet/electrode/materials/LiC6_LIONSIMBA.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrode/materials/LiCoO2_LIONSIMBA.py` & `mpet-1.0.0/mpet/electrode/materials/LiCoO2_LIONSIMBA.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrode/materials/NCA_ss2.py` & `mpet-1.0.0/mpet/electrode/materials/NCA_ss2.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrode/materials/testRS_ss.py` & `mpet-1.0.0/mpet/electrode/materials/testRS_ss.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrode/reactions/CIET.py` & `mpet-1.0.0/mpet/electrode/reactions/CIET.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrode/reactions/MHC.py` & `mpet-1.0.0/mpet/electrode/reactions/MHC.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrode/reactions/Marcus.py` & `mpet-1.0.0/mpet/electrode/reactions/Marcus.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrolyte/Doyle96_EC_DMC_1_2.py` & `mpet-1.0.0/mpet/electrolyte/Doyle96_EC_DMC_1_2.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrolyte/Doyle96_EC_DMC_2_1.py` & `mpet-1.0.0/mpet/electrolyte/Doyle96_EC_DMC_2_1.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrolyte/LIONSIMBA_isothermal.py` & `mpet-1.0.0/mpet/electrolyte/LIONSIMBA_isothermal.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrolyte/LIONSIMBA_nonisothermal.py` & `mpet-1.0.0/mpet/electrolyte/LIONSIMBA_nonisothermal.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrolyte/LiClO4_PC.py` & `mpet-1.0.0/mpet/electrolyte/LiClO4_PC.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrolyte/__init__.py` & `mpet-1.0.0/mpet/electrolyte/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,13 +2,15 @@
 This module provides functions defining properties of the ion-conducting
 phase -- the electrolyte Manage functions for the parameters involved in
 Stefan-Maxwell based concentrated electrolyte transport theory for
 binary electrolytes.
 
 Each electrolyte set must output functions for the following as a
 function of c (electrolyte concentration, M)
+
  - Dchem [m^2/s] = the prefactor for grad(c) in species conservation
  - sigma [S/m] = the conductivity
- - (1 + dln(f_\pm)/dln(c)) = the "thermodynamic factor"
+ - (1 + dln(f_pm)/dln(c)) = the "thermodynamic factor"
  - t_+^0 = the transference number of the cations
+
 T in these equations is nondimensionalized wrt 298K
 """
```

### Comparing `mpet-0.1.9/mpet/electrolyte/valoen_bernardi.py` & `mpet-1.0.0/mpet/electrolyte/valoen_bernardi.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/electrolyte/valoen_reimers.py` & `mpet-1.0.0/mpet/electrolyte/valoen_reimers.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/extern_funcs.py` & `mpet-1.0.0/mpet/extern_funcs.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/geometry.py` & `mpet-1.0.0/mpet/geometry.py`

 * *Files 20% similar despite different names*

```diff
@@ -87,7 +87,29 @@
     # Vector of Bruggeman exponents
     Brugg_pad = utils.pad_vec(utils.get_asc_vec(BruggExp, Nvol))
 
     # Vector of posority/tortuosity (assuming Bruggeman)
     out["eps_o_tau"] = porosvec_pad/porosvec_pad**(Brugg_pad)
 
     return out
+
+
+def get_interface_disc(Nvol, L, poros, BruggExp):
+    out = {}
+    # Width of each cell
+    out["dxvec"] = utils.get_const_vec(L/Nvol, Nvol)
+
+    # Distance between cell centers
+    dxtmp = np.hstack((out["dxvec"][0], out["dxvec"], out["dxvec"][-1]))
+    out["dxd1"] = utils.mean_linear(dxtmp)
+
+    # The porosity vector
+    out["porosvec"] = utils.get_const_vec(poros, Nvol)
+    porosvec_pad = utils.pad_vec(out["porosvec"])
+
+    # Vector of Bruggeman exponents
+    Brugg_pad = utils.pad_vec(utils.get_const_vec(BruggExp, Nvol))
+
+    # Vector of posority/tortuosity (assuming Bruggeman)
+    out["eps_o_tau"] = porosvec_pad/porosvec_pad**(Brugg_pad)
+
+    return out
```

### Comparing `mpet-0.1.9/mpet/main.py` & `mpet-1.0.0/mpet/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import subprocess as subp
 import sys
 import time
 from shutil import copyfile
 
 import daetools.pyDAE as dae
 from daetools.solvers.superlu import pySuperLU
-import numpy as np
 
 import mpet
 import mpet.data_reporting as data_reporting
 from mpet.config import Config
 import mpet.sim as sim
 import mpet.utils as utils
 
@@ -33,47 +32,54 @@
 
     # Enable reporting of all variables
     simulation.m.SetReportingOn(True)
 
     # Turn off reporting of some variables
     simulation.m.endCondition.ReportingOn = False
 
-    # Turn off reporting of particle ports
+    # Turn off reporting of particle and interface ports
     for trode in simulation.m.trodes:
         for particle in simulation.m.particles[trode]:
             pModel = particle[0]
             for port in pModel.Ports:
                 for var in port.Variables:
                     var.ReportingOn = False
+        if config[f"simInterface_{trode}"]:
+            for interfaces in simulation.m.interfaces[trode]:
+                for iModel in interfaces:
+                    for port in iModel.Ports:
+                        for var in port.Variables:
+                            var.ReportingOn = False
 
     # Turn off reporting of cell ports
     for port in simulation.m.Ports:
         for var in port.Variables:
             var.ReportingOn = False
 
     # Set relative tolerances
     daesolver.RelativeTolerance = config["relTol"]
 
     # Set the time horizon and the reporting interval
     simulation.TimeHorizon = config["tend"]
     # The list of reporting times excludes the first index (zero, which is implied)
-    simulation.ReportingTimes = list(np.linspace(0, config["tend"], config["tsteps"] + 1))[1:]
+    simulation.ReportingTimes = config["times"]
 
     # Connect data reporter
     simName = simulation.m.Name + time.strftime(
         " [%d.%m.%Y %H:%M:%S]", time.localtime())
     if not datareporter.Connect("", simName):
         sys.exit()
 
     # Initialize the simulation
     simulation.Initialize(daesolver, datareporter, log)
 
     # Solve at time=0 (initialization)
     # Increase the number of Newton iterations for more robust initialization
-    dae.daeGetConfig().SetString("daetools.IDAS.MaxNumItersIC","100")
+    dae.daeGetConfig().SetString("daetools.IDAS.MaxNumItersIC","1000")
+    dae.daeGetConfig().SetString("daetools.IDAS.MaxNumSteps","100000")
     simulation.SolveInitial()
 
     # Run
     try:
         simulation.Run()
     except Exception as e:
         print(str(e))
@@ -82,22 +88,24 @@
     except KeyboardInterrupt:
         print("\nphi_applied at ctrl-C:",
               simulation.m.phi_applied.GetValue(), "\n")
         simulation.ReportData(simulation.CurrentTime)
     simulation.Finalize()
 
 
-def main(paramfile, keepArchive=True):
+def main(paramfile, keepArchive=True, keepFullRun=False):
     timeStart = time.time()
     # Get the parameters dictionary (and the config instance) from the
     # parameter file
     config = Config(paramfile)
 
     # Directories we'll store output in.
-    outdir_name = time.strftime("%Y%m%d_%H%M%S", time.localtime())
+    config_file = os.path.basename(paramfile)
+    config_base = os.path.splitext(config_file)[0]
+    outdir_name = "_".join((time.strftime("%Y%m%d_%H%M%S", time.localtime()), config_base))
     outdir_path = os.path.join(os.getcwd(), "history")
     outdir = os.path.join(outdir_path, outdir_name)
     # Make sure there's a place to store the output
     try:
         os.makedirs(outdir)
     except OSError as exception:
         if exception.errno == errno.EEXIST:
@@ -190,14 +198,20 @@
     print("Total time:", tTot, "s")
     try:
         with open(os.path.join(outdir, 'run_info.txt'), 'a') as fo:
             print("\nTotal run time:", tTot, "s", file=fo)
     except Exception:
         pass
 
-    # Copy or move simulation output to current directory
+    # Copy or move simulation output to current directory. If running multiple jobs,
+    # make sure to keep all sim_output
     tmpDir = os.path.join(os.getcwd(), "sim_output")
-    shutil.rmtree(tmpDir, ignore_errors=True)
+    if not keepFullRun:
+        shutil.rmtree(tmpDir, ignore_errors=True)
+        tmpsubDir = tmpDir
+    else:
+        tmpsubDir = os.path.join(tmpDir, outdir_name)
+
     if keepArchive:
-        shutil.copytree(outdir, tmpDir)
+        shutil.copytree(outdir, tmpsubDir)
     else:
-        shutil.move(outdir, tmpDir)
+        shutil.move(outdir, tmpsubDir)
```

### Comparing `mpet-0.1.9/mpet/mod_cell.py` & `mpet-1.0.0/mpet/mod_cell.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,24 +10,27 @@
 import daetools.pyDAE as dae
 from pyUnits import s
 
 import numpy as np
 
 import mpet.extern_funcs as extern_funcs
 import mpet.geometry as geom
+import mpet.mod_CCCVCPcycle as mod_CCCVCPcycle
 import mpet.mod_electrodes as mod_electrodes
+from mpet.mod_interface import InterfaceRegion
 import mpet.ports as ports
 import mpet.utils as utils
 from mpet.config import constants
 from mpet.daeVariableTypes import mole_frac_t, elec_pot_t, conc_t
 
 # Dictionary of end conditions
 endConditions = {
     1:"Vmax reached",
-    2:"Vmin reached"}
+    2:"Vmin reached",
+    3:"End condition for CCCVCPcycle reached"}
 
 
 class ModCell(dae.daeModel):
     def __init__(self, config, Name, Parent=None, Description=""):
         dae.daeModel.__init__(self, Name, Parent, Description)
 
         self.config = config
@@ -35,15 +38,15 @@
         Nvol = config["Nvol"]
         Npart = config["Npart"]
         self.trodes = trodes = config["trodes"]
 
         # Domains where variables are distributed
         self.DmnCell = {}  # domains over full cell dimensions
         self.DmnPart = {}  # domains over particles in each cell volume
-        if config['have_separator']:  # If we have a separator
+        if config['Nvol']['s']:  # If we have a separator
             self.DmnCell["s"] = dae.daeDomain(
                 "DmnCell_s", self, dae.unit(),
                 "Simulated volumes in the separator")
         for trode in trodes:
             self.DmnCell[trode] = dae.daeDomain(
                 "DmnCell_{trode}".format(trode=trode), self, dae.unit(),
                 "Simulated volumes in electrode {trode}".format(trode=trode))
@@ -54,14 +57,15 @@
 
         # Variables
         self.c_lyte = {}
         self.phi_lyte = {}
         self.phi_bulk = {}
         self.phi_part = {}
         self.R_Vp = {}
+        self.R_Vi = {}
         self.ffrac = {}
         for trode in trodes:
             # Concentration/potential in electrode regions of elyte
             self.c_lyte[trode] = dae.daeVariable(
                 "c_lyte_{trode}".format(trode=trode), conc_t, self,
                 "Concentration in the elyte in electrode {trode}".format(trode=trode),
                 [self.DmnCell[trode]])
@@ -77,30 +81,35 @@
                 "phi_part_{trode}".format(trode=trode), elec_pot_t, self,
                 "Electrostatic potential at each particle",
                 [self.DmnCell[trode], self.DmnPart[trode]])
             self.R_Vp[trode] = dae.daeVariable(
                 "R_Vp_{trode}".format(trode=trode), dae.no_t, self,
                 "Rate of reaction of positives per electrode volume",
                 [self.DmnCell[trode]])
+            if self.config[f'simInterface_{trode}']:
+                self.R_Vi[trode] = dae.daeVariable(
+                    "R_Vi_{trode}".format(trode=trode), dae.no_t, self,
+                    "Rate of reaction of positives per electrode volume with interface region",
+                    [self.DmnCell[trode]])
             self.ffrac[trode] = dae.daeVariable(
                 "ffrac_{trode}".format(trode=trode), mole_frac_t, self,
                 "Overall filling fraction of solids in electrodes")
-        if config['have_separator']:  # If we have a separator
+        if config['Nvol']['s']:  # If we have a separator
             self.c_lyte["s"] = dae.daeVariable(
                 "c_lyte_s", conc_t, self,
                 "Concentration in the electrolyte in the separator",
                 [self.DmnCell["s"]])
             self.phi_lyte["s"] = dae.daeVariable(
                 "phi_lyte_s", elec_pot_t, self,
                 "Electrostatic potential in electrolyte in separator",
                 [self.DmnCell["s"]])
         # Note if we're doing a single electrode volume simulation
         # It will be in a perfect bath of electrolyte at the applied
         # potential.
-        if ('a' not in config['trodes']) and (not config['have_separator']) and Nvol["c"] == 1:
+        if ('a' not in config['trodes']) and (not config['Nvol']['s']) and Nvol["c"] == 1:
             self.SVsim = True
         else:
             self.SVsim = False
             # Ghost points (GP) to aid in boundary condition (BC) implemenation
             self.c_lyteGP_L = dae.daeVariable("c_lyteGP_L", conc_t, self, "c_lyte left BC GP")
             self.phi_lyteGP_L = dae.daeVariable(
                 "phi_lyteGP_L", elec_pot_t, self, "phi_lyte left BC GP")
@@ -115,21 +124,25 @@
         self.endCondition = dae.daeVariable(
             "endCondition", dae.no_t, self, "A nonzero value halts the simulation")
 
         # Create models for representative particles within electrode
         # volumes and ports with which to talk to them.
         self.portsOutLyte = {}
         self.portsOutBulk = {}
+        self.portsInInterface = {}
         self.particles = {}
+        self.interfaces = {}
         for trode in trodes:
             Nv = Nvol[trode]
             Np = Npart[trode]
             self.portsOutLyte[trode] = np.empty(Nv, dtype=object)
             self.portsOutBulk[trode] = np.empty((Nv, Np), dtype=object)
+            self.portsInInterface[trode] = np.empty((Nv, Np), dtype=object)
             self.particles[trode] = np.empty((Nv, Np), dtype=object)
+            self.interfaces[trode] = np.empty((Nv, Np), dtype=object)
             for vInd in range(Nv):
                 self.portsOutLyte[trode][vInd] = ports.portFromElyte(
                     "portTrode{trode}vol{vInd}".format(trode=trode, vInd=vInd), dae.eOutletPort,
                     self, "Electrolyte port to particles")
                 for pInd in range(Np):
                     self.portsOutBulk[trode][vInd,pInd] = ports.portFromBulk(
                         "portTrode{trode}vol{vInd}part{pInd}".format(
@@ -144,19 +157,58 @@
                     else:
                         raise NotImplementedError("unknown solid type")
                     self.particles[trode][vInd,pInd] = pMod(
                         config, trode, vInd, pInd,
                         Name="partTrode{trode}vol{vInd}part{pInd}".format(
                             trode=trode, vInd=vInd, pInd=pInd),
                         Parent=self)
-                    self.ConnectPorts(self.portsOutLyte[trode][vInd],
-                                      self.particles[trode][vInd,pInd].portInLyte)
+
+                    if config[f"simInterface_{trode}"]:
+                        # instantiate interfaces between particle and electrolyte per particle
+                        self.interfaces[trode][vInd,pInd] = InterfaceRegion(
+                            Name="interfaceTrode{trode}vol{vInd}part{pInd}".format(
+                                trode=trode, vInd=vInd, pInd=pInd),
+                            Parent=self, config=config, cell=self,
+                            particle=self.particles[trode][vInd,pInd],
+                            vInd=vInd,pInd=pInd,trode=trode)
+
+                        self.portsInInterface[trode][vInd,pInd] = ports.portFromInterface(
+                            "portIface{trode}vol{vInd}part{pInd}".format(
+                                trode=trode, vInd=vInd, pInd=pInd),
+                            dae.eInletPort, self,
+                            "Interface region port to elyte")
+
+                        # connect elyte to interface, then interface to particle
+                        self.ConnectPorts(self.portsOutLyte[trode][vInd],
+                                          self.interfaces[trode][vInd,pInd].portInLyte)
+
+                        self.ConnectPorts(
+                            self.interfaces[trode][vInd,pInd].portOutInterfaceParticle,
+                            self.particles[trode][vInd,pInd].portInLyte)
+
+                        # connect interface to elyte
+                        self.ConnectPorts(self.interfaces[trode][vInd,pInd].portOutInterfaceElyte,
+                                          self.portsInInterface[trode][vInd,pInd])
+
+                        # connect particle to interface
+                        self.ConnectPorts(self.particles[trode][vInd,pInd].portOutParticle,
+                                          self.interfaces[trode][vInd,pInd].portInParticle)
+                    else:
+                        # connect elyte to particle
+                        self.ConnectPorts(self.portsOutLyte[trode][vInd],
+                                          self.particles[trode][vInd,pInd].portInLyte)
+
                     self.ConnectPorts(self.portsOutBulk[trode][vInd,pInd],
                                       self.particles[trode][vInd,pInd].portInBulk)
 
+        # if cycling, set current port to cycling module
+        if self.profileType == "CCCVCPcycle":
+            pCycle = mod_CCCVCPcycle.CCCVCPcycle
+            self.cycle = pCycle(config, Name="CCCVCPcycle", Parent=self)
+
     def DeclareEquations(self):
         dae.daeModel.DeclareEquations(self)
 
         # Some values of domain lengths
         trodes = self.trodes
         config = self.config
         Nvol = config["Nvol"]
@@ -182,22 +234,34 @@
         for trode in trodes:
             for vInd in range(Nvol[trode]):
                 eq = self.CreateEquation(
                     "R_Vp_trode{trode}vol{vInd}".format(vInd=vInd, trode=trode))
                 # Start with no reaction, then add reactions for each
                 # particle in the volume.
                 RHS = 0
+                # interface region has separate reaction rate
+                if config[f"simInterface_{trode}"]:
+                    eq_i = self.CreateEquation(
+                        "R_Vi_trode{trode}vol{vInd}".format(vInd=vInd, trode=trode))
+                    RHS_i = 0
                 # sum over particle volumes in given electrode volume
                 for pInd in range(Npart[trode]):
                     # The volume of this particular particle
                     Vj = config["psd_vol_FracVol"][trode][vInd,pInd]
                     RHS += -(config["beta"][trode] * (1-config["poros"][trode])
                              * config["P_L"][trode] * Vj
                              * self.particles[trode][vInd,pInd].dcbardt())
+                    if config[f"simInterface_{trode}"]:
+                        # Nm0 = self.portsInInterface[trode][vInd,pInd].Nm0()
+                        i0 = self.portsInInterface[trode][vInd,pInd].i0()
+                        # TODO: what is the reaction rate?
+                        RHS_i += -i0
                 eq.Residual = self.R_Vp[trode](vInd) - RHS
+                if config[f"simInterface_{trode}"]:
+                    eq_i.Residual = self.R_Vi[trode](vInd) - RHS_i
 
         # Define output port variables
         for trode in trodes:
             for vInd in range(Nvol[trode]):
                 eq = self.CreateEquation(
                     "portout_c_trode{trode}vol{vInd}".format(vInd=vInd, trode=trode))
                 eq.Residual = (self.c_lyte[trode](vInd)
@@ -217,14 +281,20 @@
             # solid phase
             simBulkCond = config['simBulkCond'][trode]
             if simBulkCond:
                 # Calculate the RHS for electrode conductivity
                 phi_tmp = utils.add_gp_to_vec(utils.get_var_vec(self.phi_bulk[trode], Nvol[trode]))
                 porosvec = utils.pad_vec(utils.get_const_vec(
                     (1-self.config["poros"][trode])**(1-config["BruggExp"][trode]), Nvol[trode]))
+                if np.all(self.config['specified_poros'][trode]):
+                    specified_por = self.config['specified_poros'][trode]
+                    porosvec = (
+                        (np.ones(Nvol[trode]) - specified_por))**(
+                            (1 - self.config["BruggExp"][trode]))
+                    porosvec = utils.pad_vec(porosvec)
                 poros_walls = utils.mean_harmonic(porosvec)
                 if trode == "a":  # anode
                     # Potential at the current collector is from
                     # simulation
                     phi_tmp[0] = self.phi_cell()
                     # No current passes into the electrolyte
                     phi_tmp[-1] = phi_tmp[-2]
@@ -232,20 +302,26 @@
                     phi_tmp[0] = phi_tmp[1]
                     # Potential at current at current collector is
                     # reference (set)
                     phi_tmp[-1] = config["phi_cathode"]
                 dx = config["L"][trode]/Nvol[trode]
                 dvg_curr_dens = np.diff(-poros_walls*config["sigma_s"][trode]
                                         * np.diff(phi_tmp)/dx)/dx
+
             # Actually set up the equations for bulk solid phi
             for vInd in range(Nvol[trode]):
                 eq = self.CreateEquation(
                     "phi_ac_trode{trode}vol{vInd}".format(vInd=vInd, trode=trode))
                 if simBulkCond:
-                    eq.Residual = -dvg_curr_dens[vInd] - self.R_Vp[trode](vInd)
+                    # select reaction rate with interface region or particle
+                    if config[f"simInterface_{trode}"]:
+                        R_V = self.R_Vi
+                    else:
+                        R_V = self.R_Vp
+                    eq.Residual = -dvg_curr_dens[vInd] - R_V[trode](vInd)
                 else:
                     if trode == "a":  # anode
                         eq.Residual = self.phi_bulk[trode](vInd) - self.phi_cell()
                     else:  # cathode
                         eq.Residual = self.phi_bulk[trode](vInd) - config["phi_cathode"]
 
             # Simulate the potential drop along the connected
@@ -283,19 +359,26 @@
         # electrolyte equations are simple
         if self.SVsim:
             eq = self.CreateEquation("c_lyte")
             eq.Residual = self.c_lyte["c"].dt(0) - 0
             eq = self.CreateEquation("phi_lyte")
             eq.Residual = self.phi_lyte["c"](0) - self.phi_cell()
         else:
-            disc = geom.get_elyte_disc(Nvol, config["L"], config["poros"], config["BruggExp"])
+            if np.all(config["specified_poros"]["c"]):
+                config_poros = config["specified_poros"]
+            else:
+                config_poros = config["poros"]
+            disc = geom.get_elyte_disc(Nvol, config["L"], config_poros, config["BruggExp"])
             cvec = utils.get_asc_vec(self.c_lyte, Nvol)
             dcdtvec = utils.get_asc_vec(self.c_lyte, Nvol, dt=True)
             phivec = utils.get_asc_vec(self.phi_lyte, Nvol)
-            Rvvec = utils.get_asc_vec(self.R_Vp, Nvol)
+            if config[f"simInterface_{trode}"]:
+                Rvvec = utils.get_asc_vec(self.R_Vi, Nvol)
+            else:
+                Rvvec = utils.get_asc_vec(self.R_Vp, Nvol)
             # Apply concentration and potential boundary conditions
             # Ghost points on the left and no-gradients on the right
             ctmp = np.hstack((self.c_lyteGP_L(), cvec, cvec[-1]))
             phitmp = np.hstack((self.phi_lyteGP_L(), phivec, phivec[-1]))
 
             Nm_edges, i_edges = get_lyte_internal_fluxes(ctmp, phitmp, disc, config)
 
@@ -309,26 +392,24 @@
                 eqC.Residual = Nm_edges[0]
 
                 # Phi BC from BV at the foil
                 # We assume BV kinetics with alpha = 0.5,
                 # exchange current density, ecd = k0_foil * c_lyte**(0.5)
                 cWall = .5*(ctmp[0] + ctmp[1])
                 ecd = config["k0_foil"]*cWall**0.5
+                # Concentration is fixed for solid
+                if config["elyteModelType"] == 'solid':
+                    ecd = config["k0_foil"]*1**0.5
                 # note negative current because positive current is
                 # oxidation here
-                BVfunc = -self.current() / ecd
-                eta_eff = 2*np.arcsinh(-BVfunc/2.)
-                eta = eta_eff + self.current()*config["Rfilm_foil"]
-                # eta = mu_R - mu_O = -mu_O (evaluated at interface)
-                # mu_O = [T*ln(c) +] phiWall - phi_cell = -eta
-                # phiWall = -eta + phi_cell [- T*ln(c)]
-                phiWall = -eta + self.phi_cell()
+                eta = self.phi_cell() - self.current()*config["Rfilm_foil"] \
+                    - .5*(phitmp[0] + phitmp[1])
                 if config["elyteModelType"] == "dilute":
-                    phiWall -= config["T"]*np.log(cWall)
-                eqP.Residual = phiWall - .5*(phitmp[0] + phitmp[1])
+                    eta -= config["T"]*np.log(cWall)
+                eqP.Residual = self.current() - ecd*2*np.sinh(eta/2)
 
             # We have a porous anode -- no flux of charge or anions through current collector
             else:
                 eqC.Residual = ctmp[0] - ctmp[1]
                 eqP.Residual = phitmp[0] - phitmp[1]
 
             dvgNm = np.diff(Nm_edges)/disc["dxvec"]
@@ -351,14 +432,15 @@
         rxn_scl = config["beta"][limtrode] * (1-config["poros"][limtrode]) \
             * config["P_L"][limtrode]
         for vInd in range(Nvol[limtrode]):
             if limtrode == "a":
                 eq.Residual -= dx * self.R_Vp[limtrode](vInd)/rxn_scl
             else:
                 eq.Residual += dx * self.R_Vp[limtrode](vInd)/rxn_scl
+
         # Define the measured voltage, offset by the "applied" voltage
         # by any series resistance.
         # phi_cell = phi_applied - I*R
         eq = self.CreateEquation("Measured_Voltage")
         eq.Residual = self.phi_cell() - (
             self.phi_applied() - config["Rser"]*self.current())
 
@@ -457,35 +539,42 @@
                 eq.Residual = self.phi_applied() - config["segments"][-1][0]
                 self.END_IF()
 
         for eq in self.Equations:
             eq.CheckUnitsConsistency = False
 
         # Ending conditions for the simulation
-        if self.profileType in ["CC", "CCsegments"]:
+        if self.profileType in ["CC", "CCsegments", "CV", "CVsegments", "CCCVCPcycle"]:
             # Vmax reached
             self.ON_CONDITION((self.phi_applied() <= config["phimin"])
                               & (self.endCondition() < 1),
                               setVariableValues=[(self.endCondition, 1)])
 
             # Vmin reached
             self.ON_CONDITION((self.phi_applied() >= config["phimax"])
                               & (self.endCondition() < 1),
                               setVariableValues=[(self.endCondition, 2)])
 
+            if self.profileType == "CCCVCPcycle":
+                # we need to set the end condition outside for some reason
+                self.ON_CONDITION((self.cycle.cycle_number() >= config["totalCycle"]+1)
+                                  & (self.endCondition() < 1),
+                                  setVariableValues=[(self.endCondition, 3)])
+
 
 def get_lyte_internal_fluxes(c_lyte, phi_lyte, disc, config):
     zp, zm, nup, num = config["zp"], config["zm"], config["nup"], config["num"]
     nu = nup + num
     T = config["T"]
     dxd1 = disc["dxd1"]
     eps_o_tau = disc["eps_o_tau"]
 
     # Get concentration at cell edges using weighted mean
     wt = utils.pad_vec(disc["dxvec"])
+
     c_edges_int = utils.weighted_linear_mean(c_lyte, wt)
 
     if config["elyteModelType"] == "dilute":
         # Get porosity at cell edges using weighted harmonic mean
         eps_o_tau_edges = utils.weighted_linear_mean(eps_o_tau, wt)
         Dp = eps_o_tau_edges * config["Dp"]
         Dm = eps_o_tau_edges * config["Dm"]
@@ -510,8 +599,30 @@
             np.diff(phi_lyte)/dxd1
             + nu*T*(sp/(n*nup)+tp0(c_edges_int, T)/(zp*nup))
             * thermFac(c_edges_int, T)
             * np.diff(np.log(c_lyte))/dxd1
             )
         Nm_edges_int = num*(-D_edges*np.diff(c_lyte)/dxd1
                             + (1./(num*zm)*(1-tp0(c_edges_int, T))*i_edges_int))
+    elif config["elyteModelType"] == "solid":
+        SMset = config["SMset"]
+        elyte_function = utils.import_function(config["SMset_filename"], SMset,
+                                               mpet_module=f"mpet.electrolyte.{SMset}")
+        D_fs, sigma_fs, thermFac, tp0 = elyte_function()[:-1]
+        # sigma_fs and thermFac not used bc the solid system is considered linear
+        a_slyte = config["a_slyte"]
+        c_edges_int_norm = c_edges_int / config["cmax"]
+
+        # Get diffusivity at cell edges using weighted harmonic mean
+        eps_o_tau_edges = utils.weighted_linear_mean(eps_o_tau, wt)
+        Dp = eps_o_tau_edges * config["Dp"]
+        Dm = (zp * Dp - zp * Dp * tp0) / (tp0 * zm)
+        Dp0 = Dp / (1-c_edges_int_norm)  # should be c0/cmax
+        Dchemp = Dp0 * (1 - 2 * a_slyte * c_edges_int_norm + 2 * a_slyte * c_edges_int_norm**2)
+        Dchemm = Dm
+        Damb = (zp * Dp * Dchemm + zm * Dm * Dchemp) / (zp * Dp - zm * Dm)
+        i_edges_int = (-((nup*zp*Dchemp + num*zm*Dchemm)*np.diff(c_lyte)/dxd1)
+                       - (nup * zp ** 2 * Dp0 * (1 - c_edges_int_norm) + num * zm ** 2 * Dm) / T
+                       * c_edges_int * np.diff(phi_lyte) / dxd1)
+        Nm_edges_int = num * (-Damb * np.diff(c_lyte) / dxd1
+                              + (1. / (num * zm) * (1 - tp0) * i_edges_int))
     return Nm_edges_int, i_edges_int
```

### Comparing `mpet-0.1.9/mpet/mod_electrodes.py` & `mpet-1.0.0/mpet/mod_electrodes.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,18 +4,22 @@
  - mass conservation (concentration evolution)
  - reaction rate at the surface of the particles
 In each model class it has options for different types of particles:
  - homogeneous
  - Fick-like diffusion
  - Cahn-Hilliard (with reaction boundary condition)
  - Allen-Cahn (with reaction throughout the particle)
+
 These models can be instantiated from the mod_cell module to simulate various types of active
 materials within a battery electrode.
 """
+
+
 import daetools.pyDAE as dae
+
 import numpy as np
 import scipy.sparse as sprs
 import scipy.interpolate as sintrp
 
 import mpet.geometry as geo
 import mpet.ports as ports
 import mpet.props_am as props_am
@@ -71,14 +75,18 @@
             "portInLyte", dae.eInletPort, self, "Inlet port from electrolyte")
         self.portInBulk = ports.portFromBulk(
             "portInBulk", dae.eInletPort, self,
             "Inlet port from e- conducting phase")
         self.phi_lyte = self.portInLyte.phi_lyte
         self.c_lyte = self.portInLyte.c_lyte
         self.phi_m = self.portInBulk.phi_m
+        if self.config[f"simInterface_{trode}"]:
+            self.portOutParticle = ports.portFromParticle(
+                "portOutParticle", dae.eOutletPort, self,
+                "Outlet port from particle")
 
     def get_trode_param(self, item):
         """
         Shorthand to retrieve electrode-specific value
         """
         value = self.config[self.trode, item]
         # check if it is a particle-specific parameter
@@ -105,47 +113,52 @@
             self.noise2 = sintrp.interp1d(tvec, noise_data2, axis=0,
                                           bounds_error=False, fill_value=0.)
         noises = (self.noise1, self.noise2)
 
         # Figure out mu_O, mu of the oxidized state
         mu_O, act_lyte = calc_mu_O(
             self.c_lyte(), self.phi_lyte(), self.phi_m(), T,
-            self.config["elyteModelType"])
+            self.config, self.trode)
 
         # Define average filling fractions in particle
         eq1 = self.CreateEquation("c1bar")
         eq2 = self.CreateEquation("c2bar")
         eq1.Residual = self.c1bar()
         eq2.Residual = self.c2bar()
         for k in range(N):
             eq1.Residual -= self.c1(k) * volfrac_vec[k]
             eq2.Residual -= self.c2(k) * volfrac_vec[k]
         eq = self.CreateEquation("cbar")
-        eq.Residual = self.cbar() - .5*(self.c1bar() + self.c2bar())
+        eq.Residual = self.cbar() - (0.5*self.c1bar() + 0.5*self.c2bar())
 
         # Define average rate of filling of particle
         eq = self.CreateEquation("dcbardt")
         eq.Residual = self.dcbardt()
         for k in range(N):
-            eq.Residual -= .5*(self.c1.dt(k) + self.c2.dt(k)) * volfrac_vec[k]
+            eq.Residual -= (0.5*self.c1.dt(k) + 0.5*self.c2.dt(k)) * volfrac_vec[k]
 
         c1 = np.empty(N, dtype=object)
         c2 = np.empty(N, dtype=object)
         c1[:] = [self.c1(k) for k in range(N)]
         c2[:] = [self.c2(k) for k in range(N)]
-        if self.get_trode_param("type") in ["diffn2", "CHR2"]:
-            # Equations for 1D particles of 1 field varible
+        if self.get_trode_param("type") in ["diffn2", "CHR2", "ACR2"]:
+            # Equations for 1D particles of 2 field variables
             self.sld_dynamics_1D2var(c1, c2, mu_O, act_lyte, noises)
         elif self.get_trode_param("type") in ["homog2", "homog2_sdn"]:
-            # Equations for 0D particles of 1 field variables
+            # Equations for 0D particles of 2 field variables
             self.sld_dynamics_0D2var(c1, c2, mu_O, act_lyte, noises)
 
         for eq in self.Equations:
             eq.CheckUnitsConsistency = False
 
+        if self.config[f"simInterface_{self.trode}"]:
+            # Output dcbardt to interface region
+            eq = self.CreateEquation("particle_to_interface_dcbardt")
+            eq.Residual = self.portOutParticle.dcbardt() - self.dcbardt()
+
     def sld_dynamics_0D2var(self, c1, c2, muO, act_lyte, noises):
         T = self.config["T"]
         c1_surf = c1
         c2_surf = c2
         (mu1R_surf, mu2R_surf), (act1R_surf, act2R_surf) = calc_muR(
             (c1_surf, c2_surf), (self.c1bar(), self.c2bar()), self.config,
             self.trode, self.ind)
@@ -187,17 +200,25 @@
         if self.get_trode_param("type") in ["diffn2", "CHR2"]:
             (mu1R, mu2R), (act1R, act2R) = calc_muR(
                 (c1, c2), (self.c1bar(), self.c2bar()), self.config, self.trode, self.ind)
             c1_surf = c1[-1]
             c2_surf = c2[-1]
             mu1R_surf, act1R_surf = mu1R[-1], act1R[-1]
             mu2R_surf, act2R_surf = mu2R[-1], act2R[-1]
-        eta1 = calc_eta(mu1R_surf, muO)
-        eta2 = calc_eta(mu2R_surf, muO)
+            eta1 = calc_eta(mu1R_surf, muO)
+            eta2 = calc_eta(mu2R_surf, muO)
         if self.get_trode_param("type") in ["ACR2"]:
+            c1_surf = c1
+            c2_surf = c2
+            (mu1R, mu2R), (act1R, act2R) = calc_muR(
+                (c1, c2), (self.c1bar(), self.c2bar()), self.config, self.trode, self.ind)
+            mu1R_surf, act1R_surf = mu1R, act1R
+            mu2R_surf, act2R_surf = mu2R, act2R
+            eta1 = calc_eta(mu1R, muO)
+            eta2 = calc_eta(mu2R, muO)
             eta1_eff = np.array([eta1[i]
                                  + self.Rxn1(i)*self.get_trode_param("Rfilm") for i in range(N)])
             eta2_eff = np.array([eta2[i]
                                  + self.Rxn2(i)*self.get_trode_param("Rfilm") for i in range(N)])
         else:
             eta1_eff = eta1 + self.Rxn1()*self.get_trode_param("Rfilm")
             eta2_eff = eta2 + self.Rxn2()*self.get_trode_param("Rfilm")
@@ -218,15 +239,18 @@
         else:
             eq1 = self.CreateEquation("Rxn1")
             eq2 = self.CreateEquation("Rxn2")
             eq1.Residual = self.Rxn1() - Rxn1
             eq2.Residual = self.Rxn2() - Rxn2
 
         # Get solid particle fluxes (if any) and RHS
-        if self.get_trode_param("type") in ["diffn2", "CHR2"]:
+        if self.get_trode_param("type") in ["ACR2"]:
+            RHS1 = 0.5*np.array([self.get_trode_param("delta_L")*self.Rxn1(i) for i in range(N)])
+            RHS2 = 0.5*np.array([self.get_trode_param("delta_L")*self.Rxn2(i) for i in range(N)])
+        elif self.get_trode_param("type") in ["diffn2", "CHR2"]:
             # Positive reaction (reduction, intercalation) is negative
             # flux of Li at the surface.
             Flux1_bc = -0.5 * self.Rxn1()
             Flux2_bc = -0.5 * self.Rxn2()
             Dfunc_name = self.get_trode_param("Dfunc")
             Dfunc = utils.import_function(self.get_trode_param("Dfunc_filename"),
                                           Dfunc_name,
@@ -272,24 +296,32 @@
         self.config = config
         self.trode = trode
         self.ind = (vInd, pInd)
 
         # Domain
         self.Dmn = dae.daeDomain("discretizationDomain", self, dae.unit(),
                                  "discretization domain")
-
         # Variables
         self.c = dae.daeVariable("c", mole_frac_t, self,
                                  "Concentration in active particle",
                                  [self.Dmn])
+
+        # Creation of the ghost points to assit BC
+
+        if self.get_trode_param("type") in ["ACR_Diff"]:
+            self.c_left_GP = dae.daeVariable("c_left", mole_frac_t, self,
+                                             "Concentration on the left side of the particle")
+            self.c_right_GP = dae.daeVariable("c_right", mole_frac_t, self,
+                                              "Concentration on the right side of the particle")
+
         self.cbar = dae.daeVariable(
             "cbar", mole_frac_t, self,
             "Average concentration in active particle")
         self.dcbardt = dae.daeVariable("dcbardt", dae.no_t, self, "Rate of particle filling")
-        if config[trode, "type"] not in ["ACR"]:
+        if config[trode, "type"] not in ["ACR", "ACR_Diff"]:
             self.Rxn = dae.daeVariable("Rxn", dae.no_t, self, "Rate of reaction")
         else:
             self.Rxn = dae.daeVariable("Rxn", dae.no_t, self, "Rate of reaction", [self.Dmn])
 
         # Get reaction rate function
         rxnType = config[trode, "rxnType"]
         self.calc_rxn_rate = utils.import_function(config[trode, "rxnType_filename"],
@@ -302,14 +334,18 @@
             "Inlet port from electrolyte")
         self.portInBulk = ports.portFromBulk(
             "portInBulk", dae.eInletPort, self,
             "Inlet port from e- conducting phase")
         self.phi_lyte = self.portInLyte.phi_lyte
         self.c_lyte = self.portInLyte.c_lyte
         self.phi_m = self.portInBulk.phi_m
+        if config[f"simInterface_{trode}"]:
+            self.portOutParticle = ports.portFromParticle(
+                "portOutParticle", dae.eOutletPort, self,
+                "Outlet port from particle")
 
     def get_trode_param(self, item):
         """
         Shorthand to retrieve electrode-specific value
         """
         value = self.config[self.trode, item]
         # check if it is a particle-specific parameter
@@ -331,49 +367,58 @@
             tvec = np.linspace(0., 1.05*self.config["tend"], numnoise)
             noise_data = noise_prefac*np.random.randn(numnoise, N)
             self.noise = sintrp.interp1d(tvec, noise_data, axis=0,
                                          bounds_error=False, fill_value=0.)
 
         # Figure out mu_O, mu of the oxidized state
         mu_O, act_lyte = calc_mu_O(self.c_lyte(), self.phi_lyte(), self.phi_m(), T,
-                                   self.config["elyteModelType"])
+                                   self.config, self.trode)
 
         # Define average filling fraction in particle
         eq = self.CreateEquation("cbar")
         eq.Residual = self.cbar()
         for k in range(N):
             eq.Residual -= self.c(k) * volfrac_vec[k]
 
         # Define average rate of filling of particle
         eq = self.CreateEquation("dcbardt")
         eq.Residual = self.dcbardt()
         for k in range(N):
             eq.Residual -= self.c.dt(k) * volfrac_vec[k]
 
         c = np.empty(N, dtype=object)
-        c[:] = [self.c(k) for k in range(N)]
-        if self.get_trode_param("type") in ["ACR", "diffn", "CHR"]:
+        if self.get_trode_param("type") in ["ACR_Diff"]:
+            ctmp = utils.get_var_vec(self.c,N)
+            c = np.hstack((self.c_left_GP(),ctmp,self.c_right_GP()))
+        else:
+            c[:] = [self.c(k) for k in range(N)]
+        if self.get_trode_param("type") in ["ACR", "ACR_Diff", "diffn", "CHR"]:
             # Equations for 1D particles of 1 field varible
             self.sld_dynamics_1D1var(c, mu_O, act_lyte, self.noise)
         elif self.get_trode_param("type") in ["homog", "homog_sdn"]:
             # Equations for 0D particles of 1 field variables
             self.sld_dynamics_0D1var(c, mu_O, act_lyte, self.noise)
 
         for eq in self.Equations:
             eq.CheckUnitsConsistency = False
 
+        if self.config[f"simInterface_{self.trode}"]:
+            # Output dcbardt to interface region
+            eq = self.CreateEquation("particle_to_interface_dcbardt")
+            eq.Residual = self.portOutParticle.dcbardt() - self.dcbardt()
+
     def sld_dynamics_0D1var(self, c, muO, act_lyte, noise):
         T = self.config["T"]
         c_surf = c
         muR_surf, actR_surf = calc_muR(c_surf, self.cbar(), self.config,
                                        self.trode, self.ind)
         eta = calc_eta(muR_surf, muO)
         eta_eff = eta + self.Rxn()*self.get_trode_param("Rfilm")
         if self.get_trode_param("noise"):
-            eta_eff += noise[0]()
+            eta_eff += noise(dae.Time().Value)
         Rxn = self.calc_rxn_rate(
             eta_eff, c_surf, self.c_lyte(), self.get_trode_param("k0"),
             self.get_trode_param("E_A"), T, actR_surf, act_lyte,
             self.get_trode_param("lambda"), self.get_trode_param("alpha"))
         eq = self.CreateEquation("Rxn")
         eq.Residual = self.Rxn() - Rxn[0]
 
@@ -385,47 +430,95 @@
         T = self.config["T"]
         # Equations for concentration evolution
         # Mass matrix, M, where M*dcdt = RHS, where c and RHS are vectors
         Mmat = get_Mmat(self.get_trode_param('shape'), N)
         dr, edges = geo.get_dr_edges(self.get_trode_param('shape'), N)
 
         # Get solid particle chemical potential, overpotential, reaction rate
-        if self.get_trode_param("type") in ["ACR"]:
+        if self.get_trode_param("type") in ["ACR", "ACR_Diff"]:
             c_surf = c
+            # surface diffusion in the ACR C3 model
+            if self.get_trode_param("type") in ["ACR_Diff"]:
+                dx = 1/np.size(c)
+                beta_s = self.get_trode_param("beta_s")
+                eqL = self.CreateEquation("leftBC")
+                eqL.Residual = (c_surf[0] - c_surf[1] +
+                                - dx*beta_s*(c_surf[1]+0.008)*(1-c_surf[1]-0.008))
+                eqR = self.CreateEquation("rightBC")
+                eqR.Residual = (c_surf[-1] - c_surf[-2] +
+                                - dx*beta_s*(c_surf[-2]+0.008)*(1-c_surf[-2]-0.008))
+
+        if self.get_trode_param("type") in ["ACR", "ACR_Diff"]:
             muR_surf, actR_surf = calc_muR(
                 c_surf, self.cbar(), self.config, self.trode, self.ind)
         elif self.get_trode_param("type") in ["diffn", "CHR"]:
             muR, actR = calc_muR(c, self.cbar(), self.config, self.trode, self.ind)
             c_surf = c[-1]
             muR_surf = muR[-1]
             if actR is None:
                 actR_surf = None
             else:
                 actR_surf = actR[-1]
-        eta = calc_eta(muR_surf, muO)
-        if self.get_trode_param("type") in ["ACR"]:
+        # surface diffusion in the ACR C3 model
+        if self.get_trode_param("type") in ["ACR_Diff"]:
+            eta = calc_eta(muR_surf[1:-1], muO)
+        else:
+            eta = calc_eta(muR_surf, muO)
+        if self.get_trode_param("type") in ["ACR", "ACR_Diff"]:
             eta_eff = np.array([eta[i] + self.Rxn(i)*self.get_trode_param("Rfilm")
                                 for i in range(N)])
         else:
             eta_eff = eta + self.Rxn()*self.get_trode_param("Rfilm")
-        Rxn = self.calc_rxn_rate(
-            eta_eff, c_surf, self.c_lyte(), self.get_trode_param("k0"),
-            self.get_trode_param("E_A"), T, actR_surf, act_lyte,
-            self.get_trode_param("lambda"), self.get_trode_param("alpha"))
-        if self.get_trode_param("type") in ["ACR"]:
+        if self.get_trode_param("type") in ["ACR_Diff"]:
+            Rxn = self.calc_rxn_rate(
+                eta_eff, c_surf[1:-1], self.c_lyte(), self.get_trode_param("k0"),
+                self.get_trode_param("E_A"), T, actR_surf[1:-1], act_lyte,
+                self.get_trode_param("lambda"), self.get_trode_param("alpha"))
+        else:
+            Rxn = self.calc_rxn_rate(
+                eta_eff, c_surf, self.c_lyte(), self.get_trode_param("k0"),
+                self.get_trode_param("E_A"), T, actR_surf, act_lyte,
+                self.get_trode_param("lambda"), self.get_trode_param("alpha"))
+        if self.get_trode_param("type") in ["ACR", "ACR_Diff"]:
             for i in range(N):
                 eq = self.CreateEquation("Rxn_{i}".format(i=i))
                 eq.Residual = self.Rxn(i) - Rxn[i]
         else:
             eq = self.CreateEquation("Rxn")
             eq.Residual = self.Rxn() - Rxn
 
         # Get solid particle fluxes (if any) and RHS
-        if self.get_trode_param("type") in ["ACR"]:
-            RHS = np.array([self.get_trode_param("delta_L")*self.Rxn(i) for i in range(N)])
+        if self.get_trode_param("type") in ["ACR", "ACR_Diff"]:
+            # For ACR model localized contact loss.
+            if self.config['localized_losses']:
+                gamma_con = self.get_trode_param('gamma_con')
+                if gamma_con == 1:
+                    RHS = np.array([self.get_trode_param("delta_L")*self.Rxn(i) for i in range(N)])
+                else:
+                    N_cont = int((gamma_con)*N)-12
+                    RHS = np.zeros(N, dtype=object)
+                    position = int(np.random.uniform()*N)
+                    # random position of contact + 6 points on the sides to facilitate wetting
+                    if 6+position+N_cont < N-6:
+                        for i in range(0,6):
+                            RHS[i] = self.get_trode_param("delta_L")*self.Rxn(i)
+                        for i in range(N-6,N):
+                            RHS[i] = self.get_trode_param("delta_L")*self.Rxn(i)
+                        for i in range(position+6,position+N_cont,1):
+                            RHS[i] = self.get_trode_param("delta_L")*self.Rxn(i)
+                    else:
+                        for i in range(0,6):
+                            RHS[i] = self.get_trode_param("delta_L")*self.Rxn(i)
+                        for i in range(position, N):
+                            RHS[i] = self.get_trode_param("delta_L")*self.Rxn(i)
+                        for i in range(6,N_cont-(N-position)):
+                            RHS[i] = self.get_trode_param("delta_L")*self.Rxn(i)
+            else:
+                RHS = np.array([self.get_trode_param("delta_L")*self.Rxn(i) for i in range(N)])
+
         elif self.get_trode_param("type") in ["diffn", "CHR"]:
             # Positive reaction (reduction, intercalation) is negative
             # flux of Li at the surface.
             Flux_bc = -self.Rxn()
             Dfunc_name = self.get_trode_param("Dfunc")
             Dfunc = utils.import_function(self.get_trode_param("Dfunc_filename"),
                                           Dfunc_name,
@@ -441,17 +534,33 @@
             elif self.get_trode_param("shape") == "cylinder":
                 area_vec = 2*np.pi*edges  # per unit height
             RHS = -np.diff(Flux_vec * area_vec)
 
         dcdt_vec = np.empty(N, dtype=object)
         dcdt_vec[0:N] = [self.c.dt(k) for k in range(N)]
         LHS_vec = MX(Mmat, dcdt_vec)
+        if self.get_trode_param("type") in ["ACR_Diff"]:
+            # surface diffusion in the ACR C3 model
+            surf_diff_vec = calc_surf_diff(c_surf, muR_surf, self.get_trode_param("D"))
         for k in range(N):
             eq = self.CreateEquation("dcsdt_discr{k}".format(k=k))
-            eq.Residual = LHS_vec[k] - RHS[k]
+            if self.get_trode_param("type") in ["ACR_Diff"]:
+                eq.Residual = LHS_vec[k] - RHS[k] - surf_diff_vec[k]
+            else:
+                eq.Residual = LHS_vec[k] - RHS[k]
+
+
+# surface diffusion in the ACR C3 model
+def calc_surf_diff(c_surf, muR_surf, D):
+    N_2 = np.size(c_surf)
+    dxs = 1./N_2
+    c_surf_long = c_surf
+    c_surf_short = (c_surf_long[0:-1] + c_surf_long[1:])/2
+    surf_diff = D*(np.diff(c_surf_short*(1-c_surf_short)*np.diff(muR_surf)))/(dxs**2)
+    return surf_diff
 
 
 def calc_eta(muR, muO):
     return muR - muO
 
 
 def get_Mmat(shape, N):
@@ -520,21 +629,31 @@
         Flux1_vec[1:N] = -D/T * Dfunc(c1_edges) * np.exp(-E_D/T + E_D/1) * \
             np.diff(mu1_R+noise1(dae.Time().Value))/dr
         Flux2_vec[1:N] = -D/T * Dfunc(c2_edges) * np.exp(-E_D/T + E_D/1) * \
             np.diff(mu2_R+noise2(dae.Time().Value))/dr
     return Flux1_vec, Flux2_vec
 
 
-def calc_mu_O(c_lyte, phi_lyte, phi_sld, T, elyteModelType):
+def calc_mu_O(c_lyte, phi_lyte, phi_sld, T, config, trode):
+    elyteModelType = config["elyteModelType"]
+
+    if config[f"simInterface_{trode}"]:
+        elyteModelType = config["interfaceModelType"]
+
     if elyteModelType == "SM":
         mu_lyte = phi_lyte
         act_lyte = c_lyte
     elif elyteModelType == "dilute":
         act_lyte = c_lyte
         mu_lyte = T*np.log(act_lyte) + phi_lyte
+    elif elyteModelType == "solid":
+        a_slyte = config['a_slyte']
+        cmax = config['cmax']
+        act_lyte = (c_lyte / cmax) / (1 - c_lyte / cmax)*np.exp(a_slyte*(1 - 2*c_lyte))
+        mu_lyte = phi_lyte
     mu_O = mu_lyte - phi_sld
     return mu_O, act_lyte
 
 
 def calc_muR(c, cbar, config, trode, ind):
     muRfunc = props_am.muRfuncs(config, trode, ind).muRfunc
     muR_ref = config[trode, "muR_ref"]
```

### Comparing `mpet-0.1.9/mpet/plot/colormaps_custom.py` & `mpet-1.0.0/mpet/plot/colormaps_custom.py`

 * *Files identical despite different names*

### Comparing `mpet-0.1.9/mpet/plot/outmat2txt.py` & `mpet-1.0.0/mpet/plot/outmat2txt.py`

 * *Files 19% similar despite different names*

```diff
@@ -70,67 +70,84 @@
 
 bulkpHdrP2 = """Columns correspond to this electrode's cell center
 positions (see discData.txt).
 """
 bulkpHdr = ("Bulk electrode electric potential [V]\n" + RowsStr + bulkpHdrP2)
 fnameBulkpBase = "bulkPot{l}Data.txt"
 
+RowStrHdr1 = "First column corresponds to the cycle number.\n"
+RowStrHdr2 = """Second, third and fourth columns respond to gravimetric charge capacity of limiting
+electrode in mAh/g, gravimetric discharge capacity of limiting electrode in mAh/g, cycle
+capacity fraction relative to original capacity, and cycle efficiency (discharge
+capacity/charge capacity).\n"""
+cyclerHdr = ("Cycling Data\n" + RowStrHdr1 + RowStrHdr2)
+fnameCycleBase = "cycleData.txt"
+
+RowStrHdr1Q = """Each (2*i,2*i+1) row represents the (V(t), Q(t)) in cycle i in units of
+(V, Ah/m^2).\n"""
+vQCyclerHdr = ("Voltage/Capacity Cycling Data\n" + RowStrHdr1Q)
+
+RowStrHdr2Q = """Each (2*i,2*i+1) row represents the (V(t), dQ(t)dV) in cycle i in units of
+(V, Ah/m^2).\n"""
+vdQCyclerHdr = ("Voltage/dQ Cycling Data\n" + RowStrHdr2Q)
+
 
 def main(indir, genData=True, discData=True, elyteData=True,
          csldData=True, cbarData=True, bulkpData=True):
     config = plot_data.show_data(
         indir, plot_type="params", print_flag=False, save_flag=False,
-        data_only=True)
+        data_only=True, color_changes=None, smooth_type=None)
     trodes = config["trodes"]
     CrateCurr = config["1C_current_density"]  # A/m^2
     psd_len_c = config["psd_len"]["c"]
+    totalCycle = config["totalCycle"]
     Nv_c, Np_c = psd_len_c.shape
     dlm = ","
 
     def get_trode_str(tr):
         return ("Anode" if tr == "a" else "Cathode")
     if "a" in trodes:
         psd_len_a = config["psd_len"]["a"]
         Nv_a, Np_a = psd_len_a.shape
     tVec, vVec = plot_data.show_data(
         indir, plot_type="vt", print_flag=False, save_flag=False,
-        data_only=True)
+        data_only=True, color_changes=None, smooth_type=None)
     ntimes = len(tVec)
 
     if genData:
         ffVec_c = plot_data.show_data(
             indir, plot_type="soc_c", print_flag=False,
-            save_flag=False, data_only=True)[1]
+            save_flag=False, data_only=True, color_changes=None, smooth_type=None)[1]
         if "a" in trodes:
             ffVec_a = plot_data.show_data(
                 indir, plot_type="soc_a", print_flag=False,
-                save_flag=False, data_only=True)[1]
+                save_flag=False, data_only=True, color_changes=None, smooth_type=None)[1]
         else:
             ffVec_a = np.ones(len(tVec))
         currVec = plot_data.show_data(
             indir, plot_type="curr", print_flag=False,
-            save_flag=False, data_only=True)[1]
+            save_flag=False, data_only=True, color_changes=None, smooth_type=None)[1]
         powerVec = plot_data.show_data(
             indir, plot_type="power", print_flag=False,
-            save_flag=False, data_only=True)[1]
+            save_flag=False, data_only=True, color_changes=None, smooth_type=None)[1]
         genMat = np.zeros((ntimes, 7))
         genMat[:,0] = tVec
         genMat[:,1] = ffVec_a
         genMat[:,2] = ffVec_c
         genMat[:,3] = vVec
         genMat[:,4] = currVec
         genMat[:,5] = currVec * CrateCurr
         genMat[:,6] = powerVec
         np.savetxt(os.path.join(indir, "generalData.txt"),
                    genMat, delimiter=dlm, header=genDataHdr)
 
     if discData:
         cellCentersVec, facesVec = plot_data.show_data(
             indir, plot_type="discData", print_flag=False,
-            save_flag=False, data_only=True)
+            save_flag=False, data_only=True, color_changes=None, smooth_type=None)
         with open(os.path.join(indir, "discData.txt"), "w") as fo:
             print(discCCbattery, file=fo)
             print(",".join(map(str, cellCentersVec)), file=fo)
             offset = 0
             if "a" in trodes:
                 print(file=fo)
                 print(discCCanode, file=fo)
@@ -160,34 +177,35 @@
 
     if elyteData:
         valid_current = True
         # If there wasn't an electrolyte, then a ghost point variable wouldn't have been created,
         # so we'll get a KeyError in attempting to "plot" the electrolyte current density.
         try:
             plot_data.show_data(
-                indir, plot_type="elytei", print_flag=False, save_flag=False, data_only=True)
+                indir, plot_type="elytei", print_flag=False, save_flag=False, data_only=True,
+                color_changes=None, smooth_type=None)
         except KeyError:
             valid_current = False
         elytecMat = plot_data.show_data(
             indir, plot_type="elytec", print_flag=False,
-            save_flag=False, data_only=True)[1]
+            save_flag=False, data_only=True, color_changes=None, smooth_type=None)[1]
         elytepMat = plot_data.show_data(
             indir, plot_type="elytep", print_flag=False,
-            save_flag=False, data_only=True)[1]
+            save_flag=False, data_only=True, color_changes=None, smooth_type=None)[1]
         np.savetxt(os.path.join(indir, "elyteConcData.txt"),
                    elytecMat, delimiter=dlm, header=elytecHdr)
         np.savetxt(os.path.join(indir, "elytePotData.txt"),
                    elytepMat, delimiter=dlm, header=elytepHdr)
         if valid_current:
             elyteiMat = plot_data.show_data(
                 indir, plot_type="elytei", print_flag=False,
-                save_flag=False, data_only=True)[1]
+                save_flag=False, data_only=True, color_changes=None, smooth_type=None)[1]
             elytediviMat = plot_data.show_data(
                 indir, plot_type="elytedivi", print_flag=False,
-                save_flag=False, data_only=True)[1]
+                save_flag=False, data_only=True, color_changes=None, smooth_type=None)[1]
             np.savetxt(os.path.join(indir, "elyteCurrDensData.txt"),
                        elyteiMat, delimiter=dlm, header=elyteiHdr)
             np.savetxt(os.path.join(indir, "elyteDivCurrDensData.txt"),
                        elytediviMat, delimiter=dlm, header=elytediviHdr)
 
     if csldData:
         dataFileName = "output_data"
@@ -225,15 +243,15 @@
         # close file if it is a h5py file
         if isinstance(data, h5py._hl.files.File):
             data.close()
 
     if cbarData:
         cbarDict = plot_data.show_data(
             indir, plot_type="cbar_full", print_flag=False,
-            save_flag=False, data_only=True)
+            save_flag=False, data_only=True, color_changes='discrete', smooth_type=None)
         for tr in trodes:
             Trode = get_trode_str(tr)
             fname = "cbar{l}Data.txt".format(l=Trode)
             Nv, Np = config["Nvol"][tr], config["Npart"][tr]
             NpartTot = Nv*Np
             cbarMat = np.zeros((ntimes, NpartTot))
             cbarHdr = cbarHdrBase
@@ -246,19 +264,64 @@
             np.savetxt(os.path.join(indir, fname), cbarMat,
                        delimiter=dlm, header=cbarHdr.rstrip(','))
 
     if bulkpData:
         if "a" in trodes:
             bulkp_aData = plot_data.show_data(
                 indir, plot_type="bulkp_a", print_flag=False,
-                save_flag=False, data_only=True)[1]
+                save_flag=False, data_only=True, color_changes=None, smooth_type=None)[1]
             fname = fnameBulkpBase.format(l="Anode")
             np.savetxt(os.path.join(indir, fname), bulkp_aData,
                        delimiter=dlm, header=bulkpHdr)
         bulkp_cData = plot_data.show_data(
             indir, plot_type="bulkp_c", print_flag=False,
-            save_flag=False, data_only=True)[1]
+            save_flag=False, data_only=True, color_changes=None, smooth_type=None)[1]
         fname = fnameBulkpBase.format(l="Cathode")
         np.savetxt(os.path.join(indir, fname), bulkp_cData,
                    delimiter=dlm, header=bulkpHdr)
 
+    if totalCycle > 1:
+        # save general cycle data
+        cycNum, cycleCapacityCh, cycleCapacityDisch = plot_data.show_data(
+            indir, plot_type="cycle_capacity", print_flag=False, save_flag=False,
+            data_only=True)
+        cycleCapFrac = plot_data.show_data(
+            indir, plot_type="cycle_cap_frac", print_flag=False,
+            save_flag=False, data_only=True)[1]
+        cycleEfficiency = plot_data.show_data(
+            indir, plot_type="cycle_efficiency", print_flag=False,
+            save_flag=False, data_only=True)[1]
+        genMat = np.zeros((len(cycNum), 5))
+        genMat[:,0] = cycNum
+        genMat[:,1] = cycleCapacityCh
+        genMat[:,2] = cycleCapacityDisch
+        genMat[:,3] = cycleCapFrac
+        genMat[:,4] = cycleEfficiency
+        np.savetxt(os.path.join(indir, fnameCycleBase), genMat, delimiter=dlm,
+                   header=cyclerHdr)
+
+        # save QV and dQdV data
+        voltCycle, capCycle = plot_data.show_data(
+            indir, plot_type="cycle_Q_V", print_flag=False, save_flag=False,
+            data_only=True)
+        fname = "QVCycle.txt"
+        genMat = np.zeros((voltCycle.shape[0]*2, voltCycle.shape[1]))
+        genMat[:voltCycle.shape[0],:] = voltCycle
+        genMat[voltCycle.shape[0]:voltCycle.shape[0]*2,:] = capCycle
+        np.savetxt(os.path.join(indir, fname), genMat, delimiter=dlm,
+                   header=vQCyclerHdr)
+
+        voltCycle, dQdVCycle = plot_data.show_data(
+            indir, plot_type="cycle_dQ_dV", print_flag=False, save_flag=False,
+            data_only=True)
+        fname = "dQdVCycle.txt"
+        genMat = np.zeros((voltCycle.shape[0]*2, voltCycle.shape[1]))
+        genMat[:voltCycle.shape[0],:] = voltCycle
+        genMat[voltCycle.shape[0]:voltCycle.shape[0]*2,:] = dQdVCycle
+        np.savetxt(os.path.join(indir, fname), genMat, delimiter=dlm,
+                   header=vdQCyclerHdr)
+
+        # close file if it is a h5py file
+        if isinstance(data, h5py._hl.files.File):
+            data.close()
+
     return
```

### Comparing `mpet-0.1.9/mpet/plot/plot_data.py` & `mpet-1.0.0/mpet/plot/plot_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 
 import matplotlib as mpl
 import matplotlib.animation as manim
 import matplotlib.collections as mcollect
 import matplotlib.pyplot as plt
 import numpy as np
+import scipy.integrate as integrate
+from scipy.interpolate import interp1d
 
 import mpet.geometry as geom
 import mpet.mod_cell as mod_cell
 import mpet.utils as utils
 from mpet.config import Config, constants
 
 """Set list of matplotlib rc parameters to make more readable plots."""
@@ -21,15 +23,16 @@
 # mpl.rcParams['legend.fontsize'] = labelfsize - 2
 # mpl.rcParams['lines.linewidth'] = 3
 # mpl.rcParams['lines.markersize'] = 10
 # mpl.rcParams['lines.markeredgewidth'] = 0.1
 # mpl.rcParams['text.usetex'] = True
 
 
-def show_data(indir, plot_type, print_flag, save_flag, data_only, vOut=None, pOut=None, tOut=None):
+def show_data(indir, plot_type, print_flag, save_flag, data_only, color_changes, smooth_type,
+              vOut=None, pOut=None, tOut=None):
     pfx = 'mpet.'
     sStr = "_"
     ttl_fmt = "% = {perc:2.1f}"
     # Read in the simulation results and calcuations data
     dataFileName = "output_data"
     dataFile = os.path.join(indir, dataFileName)
     data = utils.open_data_file(dataFile)
@@ -43,14 +46,15 @@
         sStr = "."
     # Read in the parameters used to define the simulation
     config = Config.from_dicts(indir)
     # simulated (porous) electrodes
     trodes = config["trodes"]
     # Pick out some useful calculated values
     limtrode = config["limtrode"]
+    tot_cycle = config["totalCycle"]
     k = constants.k                      # Boltzmann constant, J/(K Li)
     Tref = constants.T_ref               # Temp, K
     e = constants.e                      # Charge of proton, C
     F = constants.F                      # C/mol
     c_ref = constants.c_ref
     td = config["t_ref"]
     Etheta = {"a": 0.}
@@ -65,15 +69,15 @@
     # Discretization (and associated porosity)
     Lfac = 1e6
     Lunit = r"$\mu$m"
     dxc = config["L"]["c"]/Nvol["c"]
     dxvec = np.array(Nvol["c"] * [dxc])
     porosvec = np.array(Nvol["c"] * [config["poros"]["c"]])
     cellsvec = dxc*np.arange(Nvol["c"]) + dxc/2.
-    if config["have_separator"]:
+    if config["Nvol"]["s"]:
         dxs = config["L"]["s"]/Nvol["s"]
         dxvec_s = np.array(Nvol["s"] * [dxs])
         dxvec = np.hstack((dxvec_s, dxvec))
         poros_s = np.array(Nvol["s"] * [config["poros"]["s"]])
         porosvec = np.hstack((poros_s, porosvec))
         cellsvec += config["L"]["s"] / config["L"]["c"]
         cellsvec_s = dxs*np.arange(Nvol["s"]) + dxs/2.
@@ -109,38 +113,38 @@
 #        for i in trodes:
 #            print "PSD_{l}:".format(l=l)
 #            print psd_len[l].transpose()
 #            print "Actual psd_mean [nm]:", np.mean(psd_len[l])
 #            print "Actual psd_stddev [nm]:", np.std(psd_len[l])
         print("Cell structure:")
         print(("porous anode | " if "a" in config["trodes"] else "flat anode | ")
-              + ("sep | " if config["have_separator"] else "") + "porous cathode")
+              + ("sep | " if config["Nvol"]["s"] else "") + "porous cathode")
         if "a" in config["trodes"]:
             print("capacity ratio cathode:anode, 'z':", config["z"])
         for trode in trodes:
             print("solidType_{t}:".format(t=trode), config[trode, 'type'])
             print("solidShape_{t}".format(t=trode), config[trode, 'shape'])
             print("rxnType_{t}:".format(t=trode), config[trode, 'rxnType'])
         if profileType == "CC":
             print("C_rate:", config['Crate'])
             theoretical_1C_current = config[config['limtrode'], 'cap'] / 3600.
             currset_dim = config['currset'] * theoretical_1C_current * config['curr_ref']
             print("current:", currset_dim, "A/m^2")
-        else:  # CV
+        elif profileType == "CV":  # CV
             Vref = config['c', 'phiRef']
             if 'a' in config["trodes"]:
                 Vref -= config['a', 'phiRef']
             Vset_dim = -(config['Vset'] * k * Tref / e - Vref)
             print("Vset:", Vset_dim)
         print("Specified psd_mean, c [{unit}]:".format(unit=Lunit),
               np.array(config['mean']["c"])*Lfac)
         print("Specified psd_stddev, c [{unit}]:".format(unit=Lunit),
               np.array(config['stddev']["c"])*Lfac)
         print("ndim B_c:", config["c", "B"])
-        if config["have_separator"]:
+        if config["Nvol"]["s"]:
             print("Nvol_s:", Nvol["s"])
         print("Nvol_c:", Nvol["c"])
         if 'a' in config["trodes"]:
             print("Nvol_a:", Nvol["a"])
         print("Npart_c:", Npart["c"])
         if 'a' in config["trodes"]:
             print("Npart_a:", Npart["a"])
@@ -232,14 +236,16 @@
         for pInd in range(Npart[trode]):
             for vInd in range(Nvol[trode]):
                 sol_str = str_base.format(pInd=pInd, vInd=vInd)
                 # Remove axis ticks
                 ax[pInd,vInd].xaxis.set_major_locator(plt.NullLocator())
                 datay = utils.get_dict_key(data, sol_str, squeeze=False)[:,-1]
                 line, = ax[pInd,vInd].plot(times, datay)
+        if save_flag:
+            fig.savefig("mpet_surf.pdf", bbox_inches="tight")
         return fig, ax
 
     # Plot SoC profile
     if plot_type[:-2] in ["soc"]:
         trode = plot_type[-1]
         ffvec = utils.get_dict_key(data, pfx + 'ffrac_{trode}'.format(trode=trode))
         if data_only:
@@ -276,14 +282,16 @@
             cvec = np.hstack((cvec_a, cvec))
         cavg = np.sum(porosvec*dxvec*cvec, axis=1)/np.sum(porosvec*dxvec)
         if data_only:
             plt.close(fig)
             return times*td, cavg
         np.set_printoptions(precision=8)
         ax.plot(times*td, cavg)
+        if save_flag:
+            fig.savefig("mpet_elytecons.pdf", bbox_inches="tight")
         return fig, ax
 
     # Plot current profile
     if plot_type == "curr":
         theoretical_1C_current = config[config['limtrode'], "cap"] / 3600.  # A/m^2
         current = (utils.get_dict_key(data, pfx + 'current')
                    * theoretical_1C_current / config['1C_current_density'] * config['curr_ref'])
@@ -296,15 +304,15 @@
         xmax = np.max(ffvec)
         ax.set_xlabel("Time [s]")
         ax.set_ylabel("Current [C-rate]")
         if save_flag:
             fig.savefig("mpet_current.png", bbox_inches="tight")
         return fig, ax
 
-    if plot_type == "power":
+    elif plot_type == "power":
         current = utils.get_dict_key(data, pfx + 'current') * (3600/td) * (cap/3600)  # in A/m^2
         voltage = (Vstd - (k*Tref/e)*utils.get_dict_key(data, pfx + 'phi_applied'))  # in V
         power = np.multiply(current, voltage)
         if data_only:
             return times*td, power
         fig, ax = plt.subplots(figsize=figsize)
         ax.plot(times*td, power)
@@ -323,15 +331,15 @@
         c_sep, p_sep = pfx + 'c_lyte_s', pfx + 'phi_lyte_s'
         c_anode, p_anode = pfx + 'c_lyte_a', pfx + 'phi_lyte_a'
         c_cath, p_cath = pfx + 'c_lyte_c', pfx + 'phi_lyte_c'
         datay_c = utils.get_dict_key(data, c_cath, squeeze=False)
         datay_p = utils.get_dict_key(data, p_cath, squeeze=False)
         L_c = config['L']["c"] * config['L_ref'] * Lfac
         Ltot = L_c
-        if config["have_separator"]:
+        if config["Nvol"]["s"]:
             datay_s_c = utils.get_dict_key(data, c_sep, squeeze=False)
             datay_s_p = utils.get_dict_key(data, p_sep, squeeze=False)
             datay_c = np.hstack((datay_s_c, datay_c))
             datay_p = np.hstack((datay_s_p, datay_p))
             L_s = config['L']["s"] * config['L_ref'] * Lfac
             Ltot += L_s
         else:
@@ -573,15 +581,18 @@
                     numy = len(datay)
                     datax = np.linspace(0, lens[pInd,vInd] * Lfac, numy)
                     line, = ax[pInd,vInd].plot(datax, datay)
                     lines[pInd,vInd] = line
                 ax[pInd,vInd].set_ylim(ylim)
                 ax[pInd,vInd].set_xlim((0, lens[pInd,vInd] * Lfac))
                 if plt_axlabels:
-                    ax[pInd, vInd].set_xlabel(r"$r$ [{Lunit}]".format(Lunit=Lunit))
+                    if config[trode, "type"] in ["ACR", "ACr_diff", "ACR2"]:
+                        ax[pInd, vInd].set_xlabel(r"$x$ [{Lunit}]".format(Lunit=Lunit))
+                    else:
+                        ax[pInd, vInd].set_xlabel(r"$r$ [{Lunit}]".format(Lunit=Lunit))
                     if plot_type[0] == "c":
                         ax[pInd, vInd].set_ylabel(r"$\widetilde{{c}}$")
                     elif plot_type[:2] == "mu":
                         ax[pInd, vInd].set_ylabel(r"$\mu/k_\mathrm{B}T$")
                 if timettl:
                     ttl = ax[pInd, vInd].text(
                         0.5, 1.04, "t = {tval:3.3f} {ttlu}".format(
@@ -661,20 +672,19 @@
                                 t=trode, vInd=vInd, pInd=pInd)
                             + sStr + "cbar")
                         dataCbar[trode][tInd,vInd,pInd] = (
                             np.squeeze(utils.get_dict_key(data, dataStr))[tInd])
         if data_only:
             return dataCbar
         # Set up colors.
-        # Define if you want smooth or discrete color changes
-        # Option: "smooth" or "discrete"
-        color_changes = "discrete"
-#        color_changes = "smooth"
+        # Uses either discrete or smooth colors
+        # Define if you want smooth or discrete color changes in plot settings (-c)
+        # Option: "discrete" or "smooth"
         # Discrete color changes:
-        if color_changes == "discrete":
+        if color_changes == 'discrete':
             # Make a discrete colormap that goes from green to yellow
             # to red instantaneously
             cdict = {
                 "red": [(0.0, 0.0, 0.0),
                         (to_yellow, 0.0, 1.0),
                         (1.0, 1.0, 1.0)],
                 "green": [(0.0, 0.502, 0.502),
@@ -683,18 +693,19 @@
                           (1.0, 0.0, 0.0)],
                 "blue": [(0.0, 0.0, 0.0),
                          (1.0, 0.0, 0.0)]
                 }
             cmap = mpl.colors.LinearSegmentedColormap(
                 "discrete", cdict)
         # Smooth colormap changes:
-        if color_changes == "smooth":
+        if color_changes == 'smooth':
             # generated with colormap.org
-            cmaps = np.load("colormaps_custom.npz")
-            cmap_data = cmaps["GnYlRd_3"]
+            cmap_location = os.path.dirname(os.path.abspath(__file__)) + r'\colormaps_custom.npz'
+            cmaps = np.load(cmap_location)
+            cmap_data = cmaps[smooth_type]
             cmap = mpl.colors.ListedColormap(cmap_data/255.)
 
         size_frac_min = 0.10
         fig, axs = plt.subplots(1, len(trvec), squeeze=False, figsize=figsize)
         ttlx = 0.5 if len(trvec) < 2 else 1.1
         ttl = axs[0,0].text(
             ttlx, 1.05, ttl_fmt.format(perc=0),
@@ -807,14 +818,204 @@
         def animate(tind):
             line1.set_ydata(datay[tind])
             t_current = times[tind]
             tfrac = (t_current - tmin)/(tmax - tmin) * 100
             ttl.set_text(ttl_fmt.format(perc=tfrac))
             return line1, ttl
 
+    # plot cycling plots
+    elif plot_type[0:5] == "cycle":
+        current = utils.get_dict_key(data, pfx + 'current') / td  # gives us C-rates in /s
+        # the capacity we calculate is the apparent capacity from experimental measurement,
+        # not the real capacity of the electrode
+        charge_discharge = utils.get_dict_key(data, pfx + "CCCVCPcycle_charge_discharge")
+        ind_start_disch, ind_end_disch, ind_start_ch, ind_end_ch = \
+            utils.get_negative_sign_change_arrays(charge_discharge)
+        # get segments that indicate 1s for the charge/discharge segments, one for each
+        # charge/discharge in the y axis
+        cycle_numbers = np.arange(1, tot_cycle + 1)  # get cycle numbers on x axis
+        # first figure out the number of cycles
+        # find mass of limiting electrode
+        # get the currents (are multiplied by 0 if it is not the segment we want)
+        currents = cap * current  # A/m^2
+        voltage = (Vstd - (k*Tref/e)*utils.get_dict_key(data, pfx + 'phi_applied'))  # in V
+        # Q(t) array for the ith cycle for discharge_cap_func[i]
+        discharge_cap_func = np.zeros((tot_cycle, 400))
+        charge_cap_func = np.zeros((tot_cycle, 400))
+        # V(t) array for the ith cycle for discharge_volt[i]
+        discharge_volt = np.zeros((tot_cycle, 400))
+        charge_volt = np.zeros((tot_cycle, 400))
+        # total discharge capacity
+        discharge_capacities = np.zeros(tot_cycle)
+        charge_capacities = np.zeros(tot_cycle)
+        discharge_total_cap = np.zeros((tot_cycle, len(times)))
+        charge_total_cap = np.zeros((tot_cycle, len(times)))
+        # only save discharge_cap_func and discharge_volt up to those values
+        for j in range(tot_cycle):
+            print("hi", ind_start_disch[j], ind_end_disch[j])
+            discharge_cap_temp = integrate.cumtrapz(
+                currents[ind_start_disch[j]:ind_end_disch[j]],
+                times[ind_start_disch[j]:ind_end_disch[j]]*td, initial=0)/3600
+            # get the total one padded with zeros so we can sum
+            discharge_total_cap[j,:] = np.append(np.zeros(ind_start_disch[j]),
+                                                 np.append(discharge_cap_temp, np.zeros(
+                                                     len(currents)-ind_end_disch[j])))
+            # integrate Q = int(I)dt, units in A hr/m^2
+            # Ahr. pad w zero because the first number is always 0
+            dis_volt_temp = voltage[ind_start_disch[j]:ind_end_disch[j]]
+            # only fill the interpolated values
+            discharge_volt[j,:] = np.linspace(dis_volt_temp[0], dis_volt_temp[-1], 400)
+            f = interp1d(dis_volt_temp, discharge_cap_temp, fill_value='extrapolate')
+            discharge_cap_func[j,:] = f(np.linspace(dis_volt_temp[0], dis_volt_temp[-1], 400))
+            discharge_capacities[j] = discharge_cap_func[j,-1] * 1000  # mAh/m^2
+
+        for j in range(tot_cycle):
+            charge_cap_temp = integrate.cumtrapz(
+                currents[ind_start_ch[j]:ind_end_ch[j]],
+                times[ind_start_ch[j]:ind_end_ch[j]]*td, initial=0)/3600
+            # get the total one padded with zeros so we can sum
+            charge_total_cap[j,:] = np.append(np.zeros(ind_start_ch[j]),
+                                              np.append(charge_cap_temp, np.zeros(
+                                                  len(currents)-ind_end_ch[j])))
+            # integrate Q = int(I)dt, units in A hr/m^2
+            # Ahr. pad w zero because the first number is always 0
+            ch_volt_temp = voltage[ind_start_ch[j]:ind_end_ch[j]]
+            # only fill the interpolated values
+            charge_volt[j,:] = np.linspace(ch_volt_temp[0], ch_volt_temp[-1], 400)
+            f = interp1d(ch_volt_temp, charge_cap_temp, fill_value='extrapolate')
+            charge_cap_func[j,:] = f(np.linspace(ch_volt_temp[0], ch_volt_temp[-1], 400))
+            charge_capacities[j] = charge_cap_func[j,-1] * 1000  # mAh/m^2
+
+        # units will be in Ahr/m^2*m^2 = Ah
+        # discharge_voltages and Q store each of the V, Q data. cycle i is stored in row i for
+        # both of these arrays
+        gravimetric_caps_disch = -discharge_capacities/(config["P_L"][limtrode] * (
+            1-config["poros"][limtrode]) * (config["L"][limtrode]*config['L_ref']))  # mAh/m^3
+        gravimetric_caps_ch = charge_capacities/(config["P_L"][limtrode] * (
+            1-config["poros"][limtrode]) * (config["L"][limtrode]*config['L_ref']))  # mAh/m^3
+        # discharge_capacities = np.trapz(discharge_currents, times*td) *1000/3600
+        # #mAh/m^2 since int over time
+        # get the total capacites that we output in the data file with padded zeros
+        discharge_total_capacities = np.sum(discharge_total_cap, axis=0)
+        charge_total_capacities = np.sum(charge_total_cap, axis=0)
+
+        # for QV or dQdV plots:
+        # plot all cycles if less than six cycles, otherwise use equal spacing and plot six
+        plot_indexes = 0
+        if tot_cycle > 7:
+            plot_indexes = (np.arange(0, 7)*(tot_cycle-1)/6).astype(int)
+        else:
+            plot_indexes = np.arange(0, tot_cycle)
+
+        if plot_type == "cycle_capacity":  # plots discharge capacity
+            if len(gravimetric_caps_disch) != len(cycle_numbers):
+                # if we weren't able to complete the simulation, we only plot up to the
+                # cycle we were able to calculate
+                cycle_numbers = cycle_numbers[:len(gravimetric_caps_disch)]
+            if data_only:
+                return cycle_numbers, gravimetric_caps_ch, gravimetric_caps_disch
+            fig, ax = plt.subplots(figsize=figsize)
+            ax.plot(cycle_numbers, np.round(gravimetric_caps_ch, decimals=2), 'o', label='Charge')
+            ax.plot(
+                cycle_numbers,
+                np.round(
+                    gravimetric_caps_disch,
+                    decimals=2),
+                'o',
+                label='Discharge')
+            ax.legend()
+            ax.set_xlabel("Cycle Number")
+            ax.set_ylabel(r"Capacity [mAh/$m^3$]")
+            ax.xaxis.set_major_locator(mpl.ticker.MaxNLocator(integer=True))
+            if save_flag:
+                fig.savefig("mpet_cycle_capacity.png", bbox_inches="tight")
+            return fig, ax
+        elif plot_type == "cycle_efficiency":
+            # do we need to change this q because molweight changed? should be okay because Nm
+            # still same efficiency = discharge_cap/charge_cap
+            efficiencies = np.abs(np.divide(discharge_capacities, charge_capacities))
+            if len(efficiencies) != len(cycle_numbers):
+                # if we weren't able to complete the simulation, we only plot up to the
+                # cycle we were able to calculate
+                cycle_numbers = cycle_numbers[:len(efficiencies)]
+            if data_only:
+                return cycle_numbers, efficiencies
+            fig, ax = plt.subplots(figsize=figsize)
+            ax.plot(cycle_numbers, efficiencies, 'o')
+            ax.set_xlabel("Cycle Number")
+            ax.set_ylabel("Cycle Efficiency")
+            ax.set_ylim(0, 1.1)
+            ax.xaxis.set_major_locator(mpl.ticker.MaxNLocator(integer=True))
+            if save_flag:
+                fig.savefig("mpet_cycle_efficiency.png", bbox_inches="tight")
+            return fig, ax
+        elif plot_type == "cycle_cap_frac":
+            discharge_cap_fracs = discharge_capacities/discharge_capacities[0]
+            if len(discharge_cap_fracs) != len(cycle_numbers):
+                # if we weren't able to complete the simulation, we only plot up to the
+                # cycle we were able to calculate
+                cycle_numbers = cycle_numbers[:len(discharge_cap_fracs)]
+            if data_only:
+                return cycle_numbers, discharge_cap_fracs
+            # normalize by the first discharge capacity
+            fig, ax = plt.subplots(figsize=figsize)
+            ax.plot(cycle_numbers, np.round(discharge_cap_fracs, decimals=2), 'o')
+            ax.set_xlabel("Cycle Number")
+            ax.set_ylabel("State of Health")
+            ax.set_ylim(0, 1.1)
+            ax.xaxis.set_major_locator(mpl.ticker.MaxNLocator(integer=True))
+            if save_flag:
+                fig.savefig("mpet_cycle_cap_frac.png", bbox_inches="tight")
+            return fig, ax
+        elif plot_type == "cycle_Q_V":
+
+            if data_only:
+                return discharge_volt, discharge_cap_func
+
+            fig, ax = plt.subplots(figsize=figsize)
+            for i in plot_indexes:
+                ax.plot(discharge_cap_func[i,:], discharge_volt[i,:])
+            ax.legend(plot_indexes+1)
+            ax.set_xlabel(r'Capacity (A hr/m$^2$)')
+            ax.set_ylabel("Voltage (V)")
+            ax.xaxis.set_major_locator(mpl.ticker.MaxNLocator(integer=True))
+            if save_flag:
+                fig.savefig("mpet_Q_V.png", bbox_inches="tight")
+            return fig, ax
+
+        elif plot_type == "cycle_dQ_dV":
+            # nondimensionalize dQ and dV by initial discharge cap
+            max_cap = discharge_capacities[0]/1000  # in Ahr/m^2
+            # calculates dQdV along each curve
+            dQ_dV = np.divide(np.diff(discharge_cap_func/max_cap, axis=1),
+                              np.diff(discharge_volt, axis=1))
+            volt = (discharge_volt[:,1:]+discharge_volt[:,:-1])/2
+
+            if data_only:
+                return volt, dQ_dV
+
+            fig, ax = plt.subplots(figsize=figsize)
+            for i in plot_indexes:
+                ax.plot(discharge_volt[i,:], dQ_dV[i,:])
+            ax.legend(plot_indexes+1)
+            ax.set_xlabel("Voltage (V)")
+            ax.set_ylabel('d%Q/dV (%/V))')
+            ax.xaxis.set_major_locator(mpl.ticker.MaxNLocator(integer=True))
+            if save_flag:
+                fig.savefig("mpet_dQ_dV.png", bbox_inches="tight")
+            return fig, ax
+
+        elif plot_type == "cycle_data":
+            discharge_energies = discharge_total_capacities*voltage
+            charge_energies = charge_total_capacities*voltage
+            if data_only:
+                return discharge_total_capacities, charge_total_capacities, discharge_energies, \
+                    charge_energies
+            return
+
     else:
         raise Exception("Unexpected plot type argument. See README.md.")
 
     ani = manim.FuncAnimation(
         fig, animate, frames=numtimes, interval=50, blit=True, repeat=False, init_func=init)
     if save_flag:
         fig.tight_layout()
```

### Comparing `mpet-0.1.9/mpet/ports.py` & `mpet-1.0.0/mpet/ports.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,7 +17,27 @@
 
 class portFromBulk(dae.daePort):
     def __init__(self, Name, PortType, Model, Description=""):
         dae.daePort.__init__(self, Name, PortType, Model, Description)
         self.phi_m = dae.daeVariable(
             "phi_m", elec_pot_t, self,
             "Electric potential in the e- conducting phase")
+
+
+class portFromParticle(dae.daePort):
+    def __init__(self, Name, PortType, Model, Description=""):
+        dae.daePort.__init__(self, Name, PortType, Model, Description)
+        self.dcbardt = dae.daeVariable(
+            "dcbardt", dae.no_t, self,
+            "Rate of particle filling")
+
+
+class portFromInterface(dae.daePort):
+    def __init__(self, Name, PortType, Model, Description=""):
+        dae.daePort.__init__(self, Name, PortType, Model, Description)
+        self.i0 = dae.daeVariable(
+            "i0", dae.no_t, self,
+            "Current density in first interface region volume")
+
+        self.Nm0 = dae.daeVariable(
+            "Nm0", dae.no_t, self,
+            "Flux in first interface region volume")
```

### Comparing `mpet-0.1.9/mpet/props_am.py` & `mpet-1.0.0/mpet/props_am.py`

 * *Files 26% similar despite different names*

```diff
@@ -150,14 +150,27 @@
         ytmp[0] = ywet
         ytmp[-1] = ywet
         dxs = 1./N
         curv = np.diff(ytmp, 2)/(dxs**2)
         muR_nh = -kappa*curv + B*(y - ybar)
         return muR_nh
 
+    def non_homog_rect_variational(self, y, ybar, B, kappa):
+        """ Helper function """
+        # the taylor expansion at the edges is used
+        N_2 = len(y)
+        ytmp = np.empty(N_2+2, dtype=object)
+        dxs = 1./N_2
+        ytmp[1:-1] = y
+        ytmp[0] = y[0] + np.diff(y)[0]*dxs + 0.5*np.diff(y,2)[0]*dxs**2
+        ytmp[-1] = y[-1] + np.diff(y)[-1]*dxs + 0.5*np.diff(y,2)[-1]*dxs**2
+        curv = np.diff(ytmp, 2)/(dxs**2)
+        muR_nh = -kappa*curv + B*(y - ybar)
+        return muR_nh
+
     def non_homog_round_wetting(self, y, ybar, B, kappa, beta_s, shape, r_vec):
         """ Helper function """
         dr = r_vec[1] - r_vec[0]
         Rs = 1.
         curv = geo.calc_curv(y, dr, r_vec, Rs, beta_s, shape)
         muR_nh = B*(y - ybar) - kappa*curv
         return muR_nh
@@ -173,24 +186,34 @@
                 and isinstance(y[0], np.ndarray)):
             mod2var = True
             N = len(y[0])
         else:
             raise Exception("Unknown input type")
         if ("homog" not in ptype) and (N > 1):
             shape = self.get_trode_param("shape")
-            kappa = self.get_trode_param("kappa")
-            B = self.get_trode_param("B")
             if shape == "C3":
                 if mod1var:
+                    kappa = self.get_trode_param("kappa")
+                    B = self.get_trode_param("B")
+                    if self.get_trode_param("type") in ["ACR"]:
+                        cwet = self.get_trode_param("cwet")
+                        muR_nh = self.non_homog_rect_fixed_csurf(
+                            y, ybar, B, kappa, cwet)
+                    elif self.get_trode_param("type") in ["ACR_Diff"]:
+                        muR_nh = self.non_homog_rect_variational(
+                            y, ybar, B, kappa)
+                elif mod2var:
+                    kappa = self.get_trode_param("kappa")
+                    B = self.get_trode_param("B")
                     cwet = self.get_trode_param("cwet")
                     muR_nh = self.non_homog_rect_fixed_csurf(
                         y, ybar, B, kappa, cwet)
-                elif mod2var:
-                    raise NotImplementedError("no 2param C3 model known")
             elif shape in ["cylinder", "sphere"]:
+                kappa = self.get_trode_param("kappa")
+                B = self.get_trode_param("B")
                 beta_s = self.get_trode_param("beta_s")
                 r_vec = geo.get_unit_solid_discr(shape, N)[0]
                 if mod1var:
                     muR_nh = self.non_homog_round_wetting(
                         y, ybar, B, kappa, beta_s, shape, r_vec)
                 elif mod2var:
                     muR1_nh = self.non_homog_round_wetting(
```

### Comparing `mpet-0.1.9/mpet/sim.py` & `mpet-1.0.0/mpet/sim.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,23 +42,26 @@
 
         # Define the model we're going to simulate
         self.m = mod_cell.ModCell(config, "mpet")
 
     def SetUpParametersAndDomains(self):
         # Domains
         config = self.config
-        if config["have_separator"]:
+        if config["Nvol"]["s"]:
             self.m.DmnCell["s"].CreateArray(config["Nvol"]["s"])
         for tr in config["trodes"]:
             self.m.DmnCell[tr].CreateArray(config["Nvol"][tr])
             self.m.DmnPart[tr].CreateArray(config["Npart"][tr])
             for i in range(config["Nvol"][tr]):
                 for j in range(config["Npart"][tr]):
                     self.m.particles[tr][i, j].Dmn.CreateArray(
                         int(config["psd_num"][tr][i,j]))
+                    if config[f"simInterface_{tr}"]:
+                        self.m.interfaces[tr][i, j].Dmn.CreateArray(
+                            int(config["Nvol_i"]))
 
     def SetUpVariables(self):
         config = self.config
         Nvol = config["Nvol"]
         Npart = config["Npart"]
         phi_cathode = config["phi_cathode"]
         if not config["prevDir"] or config["prevDir"] == "false":
@@ -83,14 +86,17 @@
                         # concentrations and set initial value for
                         # solid concentrations
                         solidType = self.config[tr, "type"]
                         if solidType in constants.one_var_types:
                             part.cbar.SetInitialGuess(cs0)
                             for k in range(Nij):
                                 part.c.SetInitialCondition(k, cs0)
+                                if self.config["c","type"] in ["ACR_Diff"]:
+                                    part.c_left_GP.SetInitialGuess(cs0)
+                                    part.c_right_GP.SetInitialGuess(cs0)
                         elif solidType in constants.two_var_types:
                             part.c1bar.SetInitialGuess(cs0)
                             part.c2bar.SetInitialGuess(cs0)
                             part.cbar.SetInitialGuess(cs0)
                             epsrnd = 0.0001
                             rnd1 = epsrnd*(np.random.rand(Nij) - 0.5)
                             rnd2 = epsrnd*(np.random.rand(Nij) - 0.5)
@@ -114,28 +120,46 @@
 
             # Initialize the ghost points used for boundary conditions
             if not self.m.SVsim:
                 self.m.c_lyteGP_L.SetInitialGuess(config["c0"])
                 self.m.phi_lyteGP_L.SetInitialGuess(0)
 
             # Separator electrolyte initialization
-            if config["have_separator"]:
+            if config["Nvol"]["s"]:
                 for i in range(Nvol["s"]):
                     self.m.c_lyte["s"].SetInitialCondition(i, config['c0'])
                     self.m.phi_lyte["s"].SetInitialGuess(i, 0)
 
             # Anode and cathode electrolyte initialization
             for tr in config["trodes"]:
                 for i in range(Nvol[tr]):
                     self.m.c_lyte[tr].SetInitialCondition(i, config['c0'])
                     self.m.phi_lyte[tr].SetInitialGuess(i, 0)
 
                     # Set electrolyte concentration in each particle
                     for j in range(Npart[tr]):
                         self.m.particles[tr][i,j].c_lyte.SetInitialGuess(config["c0"])
+                        # Set concentration and potential in interface region
+                        if config[f"simInterface_{tr}"]:
+                            for k in range(config["Nvol_i"]):
+                                self.m.interfaces[tr][i,j].c.SetInitialCondition(k,
+                                                                                 config["c0_int"])
+                                self.m.interfaces[tr][i,j].phi.SetInitialGuess(k, 0)
+
+            # set up cycling stuff
+            if config['profileType'] == "CCCVCPcycle":
+                cyc = self.m.cycle
+                cyc.last_current.AssignValue(0)
+                cyc.last_phi_applied.AssignValue(phi_guess)
+                cyc.maccor_cycle_counter.AssignValue(1)
+                cyc.maccor_step_number.SetInitialGuess(1)
+
+                # used to determine new time cutoffs at each section
+                cyc.time_counter.AssignValue(0)
+                cyc.cycle_number.AssignValue(1)
 
         else:
             dPrev = self.dataPrev
             data = utils.open_data_file(dPrev)
             for tr in config["trodes"]:
                 self.m.ffrac[tr].SetInitialGuess(
                     utils.get_dict_key(data, "ffrac_" + tr, final=True))
@@ -170,15 +194,15 @@
                             part.cbar.SetInitialGuess(
                                 utils.get_dict_key(data, partStr + "cbar", final=True))
                             for k in range(Nij):
                                 part.c1.SetInitialCondition(
                                     k, data[partStr + "c1"][-1,k])
                                 part.c2.SetInitialCondition(
                                     k, data[partStr + "c2"][-1,k])
-            if config["have_separator"]:
+            if config["Nvol"]["s"]:
                 for i in range(Nvol["s"]):
                     self.m.c_lyte["s"].SetInitialCondition(
                         i, data["c_lyte_s"][-1,i])
                     self.m.phi_lyte["s"].SetInitialGuess(
                         i, data["phi_lyte_s"][-1,i])
             for tr in config["trodes"]:
                 for i in range(Nvol[tr]):
@@ -194,14 +218,45 @@
                 self.m.phi_lyteGP_L.SetInitialGuess(
                     utils.get_dict_key(data, "phi_lyteGP_L", final=True))
 
             # Guess the initial cell voltage
             self.m.phi_applied.SetInitialGuess(utils.get_dict_key(data, "phi_applied", final=True))
             self.m.phi_cell.SetInitialGuess(utils.get_dict_key(data, "phi_cell", final=True))
 
+            # set up cycling stuff
+            if config['profileType'] == "CCCVCPcycle":
+                cycle_header = "CCCVCPcycle_"
+                cyc = self.m.cycle
+                cyc.last_current.AssignValue(
+                    utils.get_dict_key(
+                        data,
+                        cycle_header
+                        + "last_current",
+                        final=True))
+                cyc.last_phi_applied.AssignValue(utils.get_dict_key(
+                    data, cycle_header + "last_phi_applied", final=True))
+                cyc.maccor_cycle_counter.AssignValue(utils.get_dict_key(
+                    data, cycle_header + "maccor_cycle_counter", final=True))
+                cyc.maccor_step_number.AssignValue(utils.get_dict_key(
+                    data, cycle_header + "maccor_step_number", final=True))
+
+                # used to determine new time cutoffs at each section
+                cyc.time_counter.AssignValue(
+                    utils.get_dict_key(
+                        data,
+                        cycle_header
+                        + "time_counter",
+                        final=True))
+                cyc.cycle_number.AssignValue(
+                    utils.get_dict_key(
+                        data,
+                        cycle_header
+                        + "cycle_number",
+                        final=True))
+
             # close file if it is a h5py file
             if isinstance(data, h5py._hl.files.File):
                 data.close()
 
         # The simulation runs when the endCondition is 0
         self.m.endCondition.AssignValue(0)
```

### Comparing `mpet-0.1.9/mpet/utils.py` & `mpet-1.0.0/mpet/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -66,14 +66,16 @@
     for sectn in ["a", "s", "c"]:
         # If we have information within this battery section
         if sectn in var.keys():
             # If it's an array of dae variable objects
             if isinstance(var[sectn], dae.pyCore.daeVariable):
                 varout[sectn] = get_var_vec(var[sectn], Nvol[sectn], dt)
             # Otherwise, it's a parameter that varies with electrode section
+            elif isinstance(var[sectn], np.ndarray):
+                varout[sectn] = var[sectn]
             else:
                 varout[sectn] = get_const_vec(var[sectn], Nvol[sectn])
         # Otherwise, fill with zeros
         else:
             try:
                 varout[sectn] = np.zeros(Nvol[sectn])
             except KeyError:
@@ -84,15 +86,15 @@
 
 def get_dxvec(L, Nvol):
     """Get a vector of cell widths spanning the full cell."""
     if "a" in Nvol:
         dxa = Nvol["a"] * [L["a"]/Nvol["a"]]
     else:
         dxa = []
-    if "s" in Nvol:
+    if Nvol["s"]:
         dxs = Nvol["s"] * [L["s"]/Nvol["s"]]
     else:
         dxs = []
     dxc = Nvol["c"] * [L["c"]/Nvol["c"]]
     out = np.array(dxa + dxs + dxc)
     return out
 
@@ -135,14 +137,42 @@
         return data[string][...,-1].item()
     elif squeeze:
         return np.squeeze(data[string][...])
     else:  # returns entire array
         return data[string][...]
 
 
+def get_negative_sign_change_arrays(input_array):
+    """This function takes an array of (+1, +1, +1, -1, -1, -1... +1, -1 ...) and splits it
+       into a number of arrays in the y direction which are (0, 0, 0, 1, 1, 1... 0, 0)
+       whenever the array hits a sign change. It should have the number of cycles as rows.
+       Thus it will be size (N*M) for each output, where N is the number of cycles
+       and M is the size of the array. In each ith row there are only 1's for the ith charging
+       cycle.
+       Returns beginning and end discharge and charge segments in order
+       """
+    sign_mults = np.zeros((len(input_array) - 1))  # is +1 if no sign change, -1 if sign change@i+1
+    for i in range(len(input_array)-1):
+        # ends up 0 if no sign change, +1 if sign change
+        sign_mults[i] = (input_array[i] * input_array[i+1] - 1) / (-2)
+    # if we have no outputs with sign change, then end
+    if np.all(sign_mults == 0):
+        print("ERROR: Did not complete a single cycle, cannot plot cycling plots")
+        raise
+    # the odd sign changes indicate the beginning of the discharge cycle
+    indices = np.array(np.nonzero(sign_mults)).flatten()  # get indices of nonzero elements
+    neg_indices_start = indices[::2] + 1
+    neg_indices_end = indices[1::2] + 1
+    pos_indices_start = indices[1::2] + 1
+    pos_indices_start = np.delete(pos_indices_start, -1)
+    pos_indices_start = np.insert(pos_indices_start, 0, 0)
+    pos_indices_end = indices[::2] + 1
+    return neg_indices_start, neg_indices_end, pos_indices_start, pos_indices_end
+
+
 def import_function(filename, function, mpet_module=None):
     """Load a function from a file that is not part of MPET, with a fallback to MPET internal
     functions.
 
     :param Config config: MPET configuration
     :param str filename: .py file containing the function to import. None to load from mpet_module
                          instead
```

### Comparing `mpet-0.1.9/mpet.egg-info/SOURCES.txt` & `mpet-1.0.0/mpet.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 LICENSE
 README.md
 setup.py
+bin/create_ensemble.py
+bin/mpet_create_runjobs_dashboard.py
+bin/mpet_plot_app.py
 bin/mpetplot.py
 bin/mpetrun.py
+bin/run_jobs.py
 mpet/__init__.py
 mpet/daeVariableTypes.py
 mpet/data_reporting.py
 mpet/exceptions.py
 mpet/extern_funcs.py
 mpet/geometry.py
 mpet/main.py
+mpet/mod_CCCVCPcycle.py
 mpet/mod_cell.py
 mpet/mod_electrodes.py
+mpet/mod_interface.py
 mpet/ports.py
 mpet/props_am.py
 mpet/sim.py
 mpet/utils.py
 mpet/version.py
 mpet.egg-info/PKG-INFO
 mpet.egg-info/SOURCES.txt
@@ -24,53 +30,63 @@
 mpet.egg-info/top_level.txt
 mpet/config/__init__.py
 mpet/config/configuration.py
 mpet/config/constants.py
 mpet/config/derived_values.py
 mpet/config/parameterset.py
 mpet/config/schemas.py
-mpet/electrode/__init__.py
+mpet/electrode/diffusion/NMC532_Colclasure20.py
 mpet/electrode/diffusion/__init__.py
 mpet/electrode/diffusion/constant.py
 mpet/electrode/diffusion/lattice.py
+mpet/electrode/materials/LTO.py
 mpet/electrode/materials/LiC6.py
 mpet/electrode/materials/LiC6_1param.py
 mpet/electrode/materials/LiC6_2step_ss.py
+mpet/electrode/materials/LiC6_Colclasure_1506T.py
 mpet/electrode/materials/LiC6_LIONSIMBA.py
 mpet/electrode/materials/LiC6_coke_ss.py
 mpet/electrode/materials/LiC6_coke_ss2.py
 mpet/electrode/materials/LiC6_ss.py
 mpet/electrode/materials/LiC6_ss2.py
 mpet/electrode/materials/LiCoO2_LIONSIMBA.py
 mpet/electrode/materials/LiFePO4.py
 mpet/electrode/materials/LiMn2O4_ss.py
 mpet/electrode/materials/LiMn2O4_ss2.py
 mpet/electrode/materials/Li_ss.py
 mpet/electrode/materials/NCA_ss1.py
 mpet/electrode/materials/NCA_ss2.py
+mpet/electrode/materials/NMC532_Colclasure20.py
 mpet/electrode/materials/__init__.py
 mpet/electrode/materials/testIS_ss.py
 mpet/electrode/materials/testRS.py
 mpet/electrode/materials/testRS_ps.py
 mpet/electrode/materials/testRS_ss.py
 mpet/electrode/reactions/BV.py
+mpet/electrode/reactions/BV_Colclasure20.py
+mpet/electrode/reactions/BV_NMC_Park2021.py
 mpet/electrode/reactions/BV_gMod01.py
 mpet/electrode/reactions/BV_mod01.py
 mpet/electrode/reactions/BV_mod02.py
 mpet/electrode/reactions/BV_raw.py
 mpet/electrode/reactions/CIET.py
 mpet/electrode/reactions/MHC.py
 mpet/electrode/reactions/MHC_kfunc.py
 mpet/electrode/reactions/Marcus.py
 mpet/electrode/reactions/__init__.py
+mpet/electrolyte/Colclasure20.py
 mpet/electrolyte/Doyle96_EC_DMC_1_2.py
 mpet/electrolyte/Doyle96_EC_DMC_2_1.py
 mpet/electrolyte/LIONSIMBA_isothermal.py
 mpet/electrolyte/LIONSIMBA_nonisothermal.py
 mpet/electrolyte/LiClO4_PC.py
 mpet/electrolyte/__init__.py
+mpet/electrolyte/solid_elyte.py
 mpet/electrolyte/valoen_bernardi.py
 mpet/electrolyte/valoen_reimers.py
 mpet/plot/__init__.py
 mpet/plot/colormaps_custom.py
 mpet/plot/outmat2txt.py
-mpet/plot/plot_data.py
+mpet/plot/plot_data.py
+mpet/plot/plot_data_db.py
+tests/test_defs.py
+tests/test_suite.py
```

### Comparing `mpet-0.1.9/setup.py` & `mpet-1.0.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,24 +13,27 @@
     version=__version__,
     description='Multiphase porous electrode theory',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Dan Cogswell',
     author_email='cogswell@mit.edu',
     license='MIT',
-    url='https://bitbucket.org/bazantgroup/mpet',
+    url='https://github.com/TRI-AMDD/mpet',
     packages=[
         'mpet','mpet.plot',
         'mpet.electrode.diffusion',
         'mpet.electrode.materials',
         'mpet.electrode.reactions',
         'mpet.electrolyte','mpet.config'
     ],
     install_requires=['numpy','scipy','matplotlib','pyQt5', 'h5py', 'configparser', 'schema'],
     extras_require={'test':['pytest','coverage', 'coveralls', 'flake8'],
-                    'doc':['sphinx','sphinx_rtd_theme']},
+                    'doc':['sphinx','sphinx_rtd_theme'],
+                    'dashboard': ['dash', 'dash_bootstrap_components'],
+                    'cluster_jobs': ['dask-jobqueue', 'bokeh']},
     python_requires='>=3.6',
-    scripts=['bin/mpetrun.py','bin/mpetplot.py'],
+    scripts=['bin/mpetrun.py','bin/mpetplot.py','bin/run_jobs.py', 'bin/create_ensemble.py',
+             'bin/mpet_create_runjobs_dashboard.py', 'bin/mpet_plot_app.py'],
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
 )
```

