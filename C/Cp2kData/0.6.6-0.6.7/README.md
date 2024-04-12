# Comparing `tmp/Cp2kData-0.6.6.tar.gz` & `tmp/Cp2kData-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cp2kData-0.6.6.tar", last modified: Wed Feb 21 10:18:28 2024, max compression
+gzip compressed data, was "Cp2kData-0.6.7.tar", last modified: Fri Apr 12 10:50:58 2024, max compression
```

## Comparing `Cp2kData-0.6.6.tar` & `Cp2kData-0.6.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:28.467276 Cp2kData-0.6.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:28.467276 Cp2kData-0.6.6/Cp2kData.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-02-21 10:18:28.000000 Cp2kData-0.6.6/Cp2kData.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-02-21 10:18:28.000000 Cp2kData-0.6.6/Cp2kData.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 10:18:28.000000 Cp2kData-0.6.6/Cp2kData.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-21 10:18:28.000000 Cp2kData-0.6.6/Cp2kData.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-21 10:18:28.000000 Cp2kData-0.6.6/Cp2kData.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-21 10:18:28.000000 Cp2kData-0.6.6/Cp2kData.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-02-21 10:18:28.467276 Cp2kData-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:28.463276 Cp2kData-0.6.6/cp2kdata/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:28.463276 Cp2kData-0.6.6/cp2kdata/block_parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/atomic_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/converge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/dft_plus_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/dipole.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/energies.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/errors_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/fep.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/geo_opt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/header_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/hirshfeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/md_xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/mulliken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/block_parser/stress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/cell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:28.467276 Cp2kData-0.6.6/cp2kdata/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/cli/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/cli/funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:28.467276 Cp2kData-0.6.6/cp2kdata/cube/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/cube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/cube/cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/dpdata_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:28.467276 Cp2kData-0.6.6/cp2kdata/matplotlibstyle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/matplotlibstyle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/matplotlibstyle/jcp.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)    20354 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:28.467276 Cp2kData-0.6.6/cp2kdata/pdos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/pdos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/pdos/pdos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:28.467276 Cp2kData-0.6.6/cp2kdata/plots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/plots/fep_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/plots/geo_opt_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/plots/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8448 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/test_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/cp2kdata/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 10:18:28.467276 Cp2kData-0.6.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:18:28.467276 Cp2kData-0.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-02-21 10:18:07.000000 Cp2kData-0.6.6/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.611613 Cp2kData-0.6.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.611613 Cp2kData-0.6.7/Cp2kData.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-04-12 10:50:58.000000 Cp2kData-0.6.7/Cp2kData.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-12 10:50:58.000000 Cp2kData-0.6.7/Cp2kData.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:50:58.000000 Cp2kData-0.6.7/Cp2kData.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-12 10:50:58.000000 Cp2kData-0.6.7/Cp2kData.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 10:50:58.000000 Cp2kData-0.6.7/Cp2kData.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 10:50:58.000000 Cp2kData-0.6.7/Cp2kData.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-04-12 10:50:58.611613 Cp2kData-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.603613 Cp2kData-0.6.7/cp2kdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.607613 Cp2kData-0.6.7/cp2kdata/block_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/atomic_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/converge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/dft_plus_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/dipole.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/energies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/errors_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/fep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/geo_opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/header_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/hirshfeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/md_xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/mulliken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/stress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/cell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.607613 Cp2kData-0.6.7/cp2kdata/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/cli/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/cli/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.607613 Cp2kData-0.6.7/cp2kdata/cube/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/cube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/cube/cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/dpdata_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.607613 Cp2kData-0.6.7/cp2kdata/matplotlibstyle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/matplotlibstyle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/matplotlibstyle/jcp.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.607613 Cp2kData-0.6.7/cp2kdata/pdos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/pdos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/pdos/pdos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.611613 Cp2kData-0.6.7/cp2kdata/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/plots/fep_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/plots/geo_opt_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/plots/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8448 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:50:58.611613 Cp2kData-0.6.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.611613 Cp2kData-0.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/tests/test.py
```

### Comparing `Cp2kData-0.6.6/Cp2kData.egg-info/PKG-INFO` & `Cp2kData-0.6.7/Cp2kData.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Cp2kData
-Version: 0.6.6
+Version: 0.6.7
 Summary: A Small Package to Postprocess Cp2k Output
 Author-email: Yongbin Zhuang <robinzhuang@outlook.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `Cp2kData-0.6.6/Cp2kData.egg-info/SOURCES.txt` & `Cp2kData-0.6.7/Cp2kData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/LICENSE` & `Cp2kData-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/PKG-INFO` & `Cp2kData-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Cp2kData
-Version: 0.6.6
+Version: 0.6.7
 Summary: A Small Package to Postprocess Cp2k Output
 Author-email: Yongbin Zhuang <robinzhuang@outlook.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `Cp2kData-0.6.6/README.md` & `Cp2kData-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/block_parser/atomic_kind.py` & `Cp2kData-0.6.7/cp2kdata/block_parser/atomic_kind.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/block_parser/cells.py` & `Cp2kData-0.6.7/cp2kdata/block_parser/cells.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                        init_cell_info=None):
     # init_cell_info are used for npt_I parse.
     # because npt_I doesn't include angle info in MD| block
 
     # notice that the cell of step 0 is excluded from MD| block
 
     # choose parser according to cp2k_info.version
-    if cp2k_info.version in ['2022.2', '2023.1']:
+    if cp2k_info.version in ['2022.2', '2023.1', '2023.2', '2024.1']:
         ALL_MD_CELL_RE = ALL_MD_CELL_RE_V2023
     elif cp2k_info.version in ['7.1']:
         ALL_MD_CELL_RE = ALL_MD_CELL_RE_V7
     else:
         WARNING = f"cp2k version={cp2k_info.version} is not supported yet \
                     for parsing MD cell from cp2k log files."
         raise NotImplementedError(WARNING)
@@ -111,14 +111,15 @@
             # print(match)
             cell = [match["a"], match["b"], match["c"],
                     match["alpha"], match["beta"], match["gamma"]]
             cell = np.array(cell, dtype=float)
             # convert bohr to angstrom
             cell[:3] = cell[:3] * au2A
             # make sure cell length are in angstrom and cell angles are in degree before sent to cellpar_to_cell
+            #TODO: replace this cellpar_to_cell with more accurate functions in the future
             cell = cellpar_to_cell(cell)
             all_md_cells.append(cell)
     else:
         # for NPT_I parser, cell angle info is lost in MD| block
         init_cell_param = cell_to_cellpar(init_cell_info)
         init_cell_angles = init_cell_param[3:]
         for match in ALL_MD_CELL_RE.finditer(output_file):
@@ -126,14 +127,15 @@
             cell = [match["a"], match["b"], match["c"],
                     match["alpha"], match["beta"], match["gamma"]]
             cell = np.array(cell, dtype=float)
             cell[3:] = init_cell_angles
             # convert bohr to angstrom
             cell[:3] = cell[:3] * au2A
             # make sure cell length are in angstrom and cell angles are in degree before sent to cellpar_to_cell
+            #TODO: replace this cellpar_to_cell with more accurate functions in the future
             cell = cellpar_to_cell(cell)
             all_md_cells.append(cell)
 
     if all_md_cells:
         return np.array(all_md_cells, dtype=float)
     else:
         return None
```

### Comparing `Cp2kData-0.6.6/cp2kdata/block_parser/converge.py` & `Cp2kData-0.6.7/cp2kdata/block_parser/converge.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/block_parser/coordinates.py` & `Cp2kData-0.6.7/cp2kdata/block_parser/coordinates.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/block_parser/dft_plus_u.py` & `Cp2kData-0.6.7/cp2kdata/block_parser/dft_plus_u.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/block_parser/dipole.py` & `Cp2kData-0.6.7/cp2kdata/block_parser/dipole.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/block_parser/forces.py` & `Cp2kData-0.6.7/cp2kdata/block_parser/forces.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/block_parser/geo_opt.py` & `Cp2kData-0.6.7/cp2kdata/block_parser/geo_opt.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/block_parser/header_info.py` & `Cp2kData-0.6.7/cp2kdata/block_parser/header_info.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,33 +3,51 @@
 # use monty.re because it can terminate on match
 from monty.re import regrep
 
 
 @dataclass
 class Cp2kInfo:
     version: str = None
+    restart: bool = None
 
 
 CP2K_INFO_VERSION_PATTERN = \
     r"""(?xm)
     ^\sCP2K\|\sversion\sstring:\s{10,42}
     CP2K\sversion\s(?P<version>\d{1,4}\.\d)(?:\s\(Development\sVersion\))?$
     """
 
+CP2K_INFO_RESTART_PATTERN = \
+    r"""(?xm)
+    ^\s\*\s{28}RESTART\sINFORMATION\s{30}\*$
+    """
 
 def parse_cp2k_info(filename) -> Cp2kInfo:
 
     cp2k_info = regrep(
         filename=filename,
-        patterns={"version": CP2K_INFO_VERSION_PATTERN},
+        patterns={
+            "version": CP2K_INFO_VERSION_PATTERN,
+            "restart": CP2K_INFO_RESTART_PATTERN
+            },
         terminate_on_match=True
     )
 
-    return Cp2kInfo(version=cp2k_info["version"][0][0][0])
-
+    num_match_restart = len(cp2k_info['restart'])
+    if num_match_restart > 1:
+        raise ValueError(f"More than one restart information found in {filename}")
+    elif num_match_restart == 1:
+        cp2k_restart = True
+    elif num_match_restart == 0:
+        cp2k_restart = False
+
+    return Cp2kInfo(
+        version=cp2k_info["version"][0][0][0],
+        restart=cp2k_restart
+        )
 
 @dataclass
 class GlobalInfo:
     run_type: str = None
     print_level: str = None
```

### Comparing `Cp2kData-0.6.6/cp2kdata/block_parser/hirshfeld.py` & `Cp2kData-0.6.7/cp2kdata/block_parser/hirshfeld.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/block_parser/md_xyz.py` & `Cp2kData-0.6.7/cp2kdata/block_parser/md_xyz.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # from monty.io import zopen
 import regex as re
 import numpy as np
+from cp2kdata.utils import format_logger
 ENERGY_RE = re.compile(
     r"""(?x)
     \sE\s=\s+(?P<energy>[\s-]\d+\.\d+)
     """
 )
 
 
+
 def parse_md_ener(ener_file):
-    print(f"Parsing Energies from {ener_file}")
+    format_logger(info="Energies", filename=ener_file)
+    #print(f"Parsing Energies from {ener_file}")
     energies_list = np.loadtxt(ener_file, usecols=4, ndmin=1, dtype=np.float64)
     return energies_list
 
 
 def parse_pos_xyz(posxyz_file):
-    print(f"Parsing Structures from {posxyz_file}")
+    format_logger(info="Structures", filename=posxyz_file)
+    #print(f"Parsing Structures from {posxyz_file}")
     fp = open(posxyz_file, "r")
     lines = fp.readlines()
     energies_list = []
     pos_list = []
     while len(lines) > 0:
         chemical_symbols = []
         positions = []
@@ -35,15 +39,16 @@
         pos_list.append(positions)
     energies_list = np.array(energies_list, dtype=np.float64)
     pos_list = np.array(pos_list, dtype=np.float64)
     return pos_list, energies_list, chemical_symbols
 
 
 def parse_frc_xyz(frcxyz_file):
-    print(f"Parsing Froces from {frcxyz_file}")
+    format_logger(info="Forces", filename=frcxyz_file)
+    #print(f"Parsing Froces from {frcxyz_file}")
     fp = open(frcxyz_file, "r")
     lines = fp.readlines()
     force_list = []
     while len(lines) > 0:
         symbols = []
         positions = []
         natoms = int(lines.pop(0))
@@ -58,15 +63,16 @@
     force_list = np.array(force_list, dtype=np.float64)
     return force_list
 
 # NOTE: incomplete function, do not release!
 
 
 def parse_pos_xyz_from_wannier(wannier_xyz_fiel):
-    print(f"Parsing Structures from {wannier_xyz_fiel}")
+    #
+    #print(f"Parsing Structures from {wannier_xyz_fiel}")
     fp = open(wannier_xyz_fiel, "r")
     lines = fp.readlines()
     force_list = []
     while len(lines) > 0:
         symbols = []
         positions = []
         natoms = int(lines.pop(0))
@@ -81,29 +87,31 @@
             positions.append([float(x), float(y), float(z)])
         force_list.append(positions)
     force_list = np.array(force_list, dtype=np.float64)
     return force_list
 
 
 def parse_md_stress(stress_file):
-    print(f"Parsing Stresses from {stress_file}")
+    format_logger(info="Stresses", filename=stress_file)
+    #print(f"Parsing Stresses from {stress_file}")
     stresses_list = np.loadtxt(
         stress_file,
         usecols=(2, 3, 4, 5, 6, 7, 8, 9, 10),
         ndmin=2,
         dtype=np.float64
     )
 
     numb_frames = stresses_list.shape[0]
 
     return stresses_list.reshape(numb_frames, 3, 3)
 
 
 def parse_md_cell(cell_file):
-    print(f"Parsing Cells from {cell_file}")
+    format_logger(info="Cells", filename=cell_file)
+    #print(f"Parsing Cells from {cell_file}")
     cells_list = np.loadtxt(
         cell_file,
         usecols=(2, 3, 4, 5, 6, 7, 8, 9, 10),
         ndmin=2,
         dtype=np.float64
     )
     numb_frames = cells_list.shape[0]
```

### Comparing `Cp2kData-0.6.6/cp2kdata/block_parser/mulliken.py` & `Cp2kData-0.6.7/cp2kdata/block_parser/mulliken.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/block_parser/stress.py` & `Cp2kData-0.6.7/cp2kdata/block_parser/stress.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/cell.py` & `Cp2kData-0.6.7/cp2kdata/cell.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/cli/cmd.py` & `Cp2kData-0.6.7/cp2kdata/cli/cmd.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/cube/cube.py` & `Cp2kData-0.6.7/cp2kdata/cube/cube.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/dpdata_plugin.py` & `Cp2kData-0.6.7/cp2kdata/dpdata_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,27 +68,29 @@
         print(WRAPPER)
         return data
 
 
 @Format.register("cp2k/aimd_output")
 @Format.register("cp2kdata/md")
 class CP2KMDFormat(Format):
-    def from_labeled_system(self, file_name, **kwargs):
+    def from_labeled_system(self, file_name, restart: bool=None, **kwargs):
 
         # -- Set Basic Parameters --
         path_prefix = file_name  # in cp2k md, file_name is directory name.
         true_symbols = kwargs.get('true_symbols', False)
         cells = kwargs.get('cells', None)
         cp2k_output_name = kwargs.get('cp2k_output_name', None)
 
         # -- start parsing --
         print(WRAPPER)
 
         cp2kmd = Cp2kOutput(output_file=cp2k_output_name,
-                            run_type="MD", path_prefix=path_prefix)
+                            run_type="MD",
+                            path_prefix=path_prefix,
+                            restart=restart)
 
         num_frames = cp2kmd.get_num_frames()
 
         chemical_symbols = get_chemical_symbols_from_cp2kdata(
             cp2koutput=cp2kmd,
             true_symbols=true_symbols
         )
```

### Comparing `Cp2kData-0.6.6/cp2kdata/matplotlibstyle/jcp.mplstyle` & `Cp2kData-0.6.7/cp2kdata/matplotlibstyle/jcp.mplstyle`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/output.py` & `Cp2kData-0.6.7/cp2kdata/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import glob
 import os
 import sys
 from functools import cached_property
 from .plots.geo_opt_plot import geo_opt_info_plot
 from .block_parser.header_info import GlobalInfo, Cp2kInfo, DFTInfo
 
-
+from cp2kdata.utils import format_logger
 from cp2kdata.block_parser.dft_plus_u import parse_dft_plus_u_occ
 from cp2kdata.block_parser.forces import parse_atomic_forces_list
 from cp2kdata.block_parser.geo_opt import parse_geo_opt_info
 from cp2kdata.block_parser.header_info import parse_dft_info, parse_global_info, parse_cp2k_info, parse_md_info
 from cp2kdata.block_parser.hirshfeld import parse_hirshfeld_pop_list
 from cp2kdata.block_parser.mulliken import parse_mulliken_pop_list
 from cp2kdata.block_parser.energies import parse_energies_list
@@ -22,17 +22,25 @@
 from cp2kdata.block_parser.cells import parse_all_cells, parse_all_md_cells
 from cp2kdata.block_parser.md_xyz import parse_md_ener, parse_pos_xyz, parse_frc_xyz, parse_md_stress, parse_md_cell
 
 
 class Cp2kOutput:
     """Class for parsing cp2k output"""
 
-    def __init__(self, output_file=None, run_type: str = None, path_prefix=".", **kwargs):
+    def __init__(
+            self,
+            output_file: str=None,
+            run_type: str=None,
+            path_prefix: str=".",
+            restart: bool=None,
+            **kwargs
+            ):
+
         # --set some basic information
-        self.required_information = kwargs
+        #self.required_information = kwargs
         self.path_prefix = path_prefix
 
         if output_file is None:
             self.filename = None
         elif os.path.isfile(os.path.join(self.path_prefix, output_file)):
             self.filename = os.path.join(self.path_prefix, output_file)
         else:
@@ -80,14 +88,19 @@
             with open(self.filename, 'r') as fp:
                 self.output_file = fp.read()
             self.cp2k_info = parse_cp2k_info(self.filename)
             self.dft_info = parse_dft_info(self.filename)
         else:
             self.cp2k_info = Cp2kInfo(version="Unknown")
 
+        # overwrite the restart if users provide restart information
+        # restart should be true or false
+        if restart is not None:
+            self.cp2k_info.restart = restart
+
         self.check_run_type(run_type=self.global_info.run_type)
 
         run_type_parser_candidates = {
             "ENERGY": self.parse_energy_force,
             "ENERGY_FORCE": self.parse_energy_force,
             "GEO_OPT": self.parse_geo_opt,
             "CELL_OPT": self.parse_cell_opt,
@@ -364,40 +377,42 @@
             os.path.join(self.path_prefix, "*pos*.xyz"))
         if pos_xyz_file_list:
             self.atomic_frames_list, energies_list_from_pos, self.chemical_symbols = parse_pos_xyz(
                 pos_xyz_file_list[0])
 
             if not hasattr(self, "energies_list"):
                 self.energies_list = energies_list_from_pos
+        else:
+            # if no pos file and ener file, parse energies from the output file
+            format_logger(info="Energies", filename=self.filename)
+            self.energies_list = parse_energies_list(self.output_file)
 
         frc_xyz_file_list = glob.glob(
             os.path.join(self.path_prefix, "*frc*.xyz"))
         if frc_xyz_file_list:
             self.atomic_forces_list = parse_frc_xyz(frc_xyz_file_list[0])
         else:
-            print(
-                f"Parsing Forces from the CP2K output/log file: {self.filename}")
+            format_logger(info="Forces", filename=self.filename)
             self.atomic_forces_list = parse_atomic_forces_list(
                 self.output_file)
 
         stress_file_list = glob.glob(
             os.path.join(self.path_prefix, "*.stress"))
         if stress_file_list:
             print(
-                f"cp2kdata found a stress file: {stress_file_list[0]}"
-                "But the parser for stress is not supported yet"
+                f"cp2kdata found a file recording stresses: {stress_file_list[0]}"
+                f"But the parser for {stress_file_list[0]} is not supported yet"
                 )
             #TODO: the unit of stress is bar in -1.stress file, but not GPa in the output file
             #TODO: however, covert bar to GPa is not consistent with the output file!
             #TODO: check this latter
             #self.stress_tensor_list = parse_md_stress(stress_file_list[0])
             self.stress_tensor_list = None
         else:
-            print(
-                f"Parsing Stress from the CP2K output/log file: {self.filename}")
+            format_logger(info="Stresses", filename=self.filename)
             self.stress_tensor_list = parse_stress_tensor_list(
                 self.output_file)
 
         self.num_frames = len(self.energies_list)
 
         # here parse cell information
         WARNING_MSG_PARSE_CELL_FROM_OUTPUT = \
@@ -407,85 +422,88 @@
                 "The raw data of cell information are lengths and angles,\n"
                 "which are later transformed to cell matrices by codes.\n"
                 "However, the a axis of the cell are always assumed to be aligned to "
                 "the x axis of the coordinate.\n"
                 "Make sure the a axis in real cell matrices are always aligned to x axis.\n"
                 "Otherwise, parsing cell information from `-1.cell` file is recommended.\n"
 
-                "CP2K input setting\n"
+                "CP2K input setup for write `-1.cell` file\n"
                 "------------------\n"
                 "&MOTION\n"
                 " &PRINT\n"
                 "   &CELL\n"
                 "     &EACH\n"
                 "       MD 1\n"
                 "     &END EACH\n"
                 "   &END CELL\n"
                 " &END PRINT\n"
                 "&END MOTION\n"
                 "------------------\n"
             )
 
-        WARNING_MSG = "cp2kdata obtains more than one initial cell from the output file, \
-                    please check if your output file has duplicated header information."
 
         cell_file_list = glob.glob(os.path.join(self.path_prefix, "*.cell"))
         if (self.md_info.ensemble_type == "NVT") or \
             (self.md_info.ensemble_type == "NVE") or \
-                (self.md_info.ensemble_type == "REFTRAJ"):
+                (self.md_info.ensemble_type == "REFTRAJ"): # not ture REFTRAJ also contrains different cell?
             if cell_file_list:
                 self.all_cells = parse_md_cell(cell_file_list[0])
             elif self.filename:
-                print(f"Parsing Cells Information from {self.filename}")
+                format_logger(info="Cells", filename=self.filename)
                 print(WARNING_MSG_PARSE_CELL_FROM_OUTPUT)
+
+                #self.organize_md_cell()
                 # parse the first cell
                 first_cell = parse_all_cells(self.output_file)
-                assert first_cell.shape == (1, 3, 3), WARNING_MSG
+                assert first_cell.shape == (1, 3, 3)
                 self.all_cells = first_cell
                 self.all_cells = np.repeat(
                     self.all_cells, repeats=self.num_frames, axis=0)
 
         elif (self.md_info.ensemble_type == "NPT_F"):
             if cell_file_list:
                 # all cells include initial cell
                 self.all_cells = parse_md_cell(cell_file_list[0])
             elif self.filename:
-                print(f"Parsing Cells Information from {self.filename}")
+                format_logger(info="Cells", filename=self.filename)
                 print(WARNING_MSG_PARSE_CELL_FROM_OUTPUT)
-                # only parse the first cell
-                first_cell = parse_all_cells(self.output_file)
-                assert first_cell.shape == (1, 3, 3), WARNING_MSG
-                # parse the rest of the cells
-                self.all_cells = parse_all_md_cells(self.output_file,
-                                                    cp2k_info=self.cp2k_info)
-                # prepend the first cell
-                self.all_cells = np.insert(
-                    self.all_cells, 0, first_cell[0], axis=0)
+
+                self.organize_md_cell()
 
         elif (self.md_info.ensemble_type == "NPT_I"):
             if cell_file_list:
                 self.all_cells = parse_md_cell(cell_file_list[0])
             elif self.filename:
-                print(f"Parsing Cells Information from {self.filename}")
+                format_logger(info="Cells", filename=self.filename)
                 print(WARNING_MSG_PARSE_CELL_FROM_OUTPUT)
-                # only parse the first cell
-                first_cell = parse_all_cells(self.output_file)
-                assert first_cell.shape == (1, 3, 3), WARNING_MSG
-                # parse the rest of the cells
-                self.all_cells = parse_all_md_cells(self.output_file,
-                                                    cp2k_info=self.cp2k_info,
-                                                    init_cell_info=first_cell[0])
-                # prepend the first cell
-                self.all_cells = np.insert(
-                    self.all_cells, 0, first_cell[0], axis=0)
+
+                self.organize_md_cell()
 
         self.init_atomic_coordinates, self.atom_kind_list, self.chemical_symbols = parse_init_atomic_coordinates(
             self.output_file)
         self.atomic_kind = parse_atomic_kinds(self.output_file)
 
+    def organize_md_cell(self):
+        # whether reserve the first cell is determined by the restart
+
+        WARNING_MSG = "cp2kdata obtains more than one initial cell from the output file, \
+                    please check if your output file has duplicated header information."
+
+        # only parse the first cell
+        first_cell = parse_all_cells(self.output_file)
+        assert first_cell.shape == (1, 3, 3), WARNING_MSG
+        # parse the rest of the cells
+        self.all_cells = parse_all_md_cells(self.output_file,
+                                            cp2k_info=self.cp2k_info,
+                                            init_cell_info=first_cell[0])
+        # prepend the first cell
+        if self.cp2k_info.restart is not True:
+            self.all_cells = np.insert(
+                self.all_cells, 0, first_cell[0], axis=0)
+
     @staticmethod
     def get_global_info(run_type=None, filename=None):
         if filename:
             global_info = parse_global_info(filename)
         elif run_type:
             global_info = GlobalInfo(run_type=run_type.upper())
         else:
```

### Comparing `Cp2kData-0.6.6/cp2kdata/pdos/pdos.py` & `Cp2kData-0.6.7/cp2kdata/pdos/pdos.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/plots/fep_plot.py` & `Cp2kData-0.6.7/cp2kdata/plots/fep_plot.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/plots/geo_opt_plot.py` & `Cp2kData-0.6.7/cp2kdata/plots/geo_opt_plot.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/plots/test_plot.py` & `Cp2kData-0.6.7/cp2kdata/plots/test_plot.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/test_input.py` & `Cp2kData-0.6.7/cp2kdata/test_input.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/units.py` & `Cp2kData-0.6.7/cp2kdata/units.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.6/cp2kdata/utils.py` & `Cp2kData-0.6.7/cp2kdata/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 this script put misc function here.
 """
 from turtle import pos
 from ase.geometry.analysis import Analysis
 from ase.io import read, write
-from cp2kdata import Cp2kOutput
+#from cp2kdata import Cp2kOutput
 import numpy as np
 import os
 import shutil
 
 # frequently used unit convertion
 au2eV = 27.211386245988
 au2A = 0.529177210903
@@ -71,14 +71,16 @@
 def printtbox(arg):
     """
     This function is a print decorated with a few characters so that the
     print function present a characteristic string. Useful for postprocess.
     """
     print("--> CP2KDATA: {0}".format(arg))
 
+def format_logger(info, filename):
+    print(f"Parsing {info:10} from {filename}")
 
 def file_content(file, num):
     # read a specific line of file or return the block
     # file: enter file name
     # num: a integer -> return specific line content
     #      a tuple (num1, num2) -> return the line content
     #                              between num1 and num2-1
@@ -107,14 +109,14 @@
                     if (_idx >= num[0]):
                         content += line
             return content
         else:
             raise ValueError("The length of range is wrong!")
 
 
-def get_opt_cell_stc(output_file, pos_file):
-    op = Cp2kOutput(output_file)
-    opt_cell = op.get_all_cells()[-1]
-    opt_pos = read(pos_file, index="-1")
-    opt_pos.set_cell(opt_cell)
-    opt_pos.set_pbc(True)
-    write("opt_stc.cif", opt_pos, format="cif")
+# def get_opt_cell_stc(output_file, pos_file):
+#     op = Cp2kOutput(output_file)
+#     opt_cell = op.get_all_cells()[-1]
+#     opt_pos = read(pos_file, index="-1")
+#     opt_pos.set_cell(opt_cell)
+#     opt_pos.set_pbc(True)
+#     write("opt_stc.cif", opt_pos, format="cif")
```

### Comparing `Cp2kData-0.6.6/pyproject.toml` & `Cp2kData-0.6.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Cp2kData"
-version = "0.6.6"
+version = "0.6.7"
 description = "A Small Package to Postprocess Cp2k Output"
 authors = [
     {name = "Yongbin Zhuang", email = "robinzhuang@outlook.com"}
     ]
 license = {file = "LICENSE"}
 readme = "README.md"
 classifiers = [
```

### Comparing `Cp2kData-0.6.6/tests/test.py` & `Cp2kData-0.6.7/tests/test.py`

 * *Files identical despite different names*

