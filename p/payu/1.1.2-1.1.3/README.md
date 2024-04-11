# Comparing `tmp/payu-1.1.2.tar.gz` & `tmp/payu-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payu-1.1.2.tar", last modified: Tue Jan 23 01:35:54 2024, max compression
+gzip compressed data, was "payu-1.1.3.tar", last modified: Thu Apr 11 23:19:26 2024, max compression
```

## Comparing `payu-1.1.2.tar` & `payu-1.1.3.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 01:35:54.768203 payu-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-23 01:35:47.000000 payu-1.1.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11022 2024-01-23 01:35:47.000000 payu-1.1.2/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-01-23 01:35:47.000000 payu-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-23 01:35:47.000000 payu-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-01-23 01:35:47.000000 payu-1.1.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-23 01:35:54.768203 payu-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-01-23 01:35:47.000000 payu-1.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 01:35:54.756203 payu-1.1.2/payu/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-23 01:35:47.000000 payu-1.1.2/payu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-23 01:35:54.768203 payu-1.1.2/payu/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-01-23 01:35:47.000000 payu-1.1.2/payu/backports.py
--rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-01-23 01:35:47.000000 payu-1.1.2/payu/branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-01-23 01:35:47.000000 payu-1.1.2/payu/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-01-23 01:35:47.000000 payu-1.1.2/payu/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-01-23 01:35:47.000000 payu-1.1.2/payu/envmod.py
--rw-r--r--   0 runner    (1001) docker     (127)    39875 2024-01-23 01:35:47.000000 payu-1.1.2/payu/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-01-23 01:35:47.000000 payu-1.1.2/payu/fsops.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-01-23 01:35:47.000000 payu-1.1.2/payu/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-01-23 01:35:47.000000 payu-1.1.2/payu/laboratory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15861 2024-01-23 01:35:47.000000 payu-1.1.2/payu/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    14154 2024-01-23 01:35:47.000000 payu-1.1.2/payu/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 01:35:54.760203 payu-1.1.2/payu/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/accessom2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/cable.py
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/cesm_cmeps.py
--rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/cice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/cice5.py
--rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/fms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/gold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/matm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11511 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/mitgcm.py
--rw-r--r--   0 runner    (1001) docker     (127)    18061 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/mom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/mom6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/mom_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/nemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/oasis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/qgcm.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/um.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/ww3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-01-23 01:35:47.000000 payu-1.1.2/payu/models/yatm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-01-23 01:35:47.000000 payu-1.1.2/payu/namcouple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 01:35:54.760203 payu-1.1.2/payu/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-23 01:35:47.000000 payu-1.1.2/payu/profilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-01-23 01:35:47.000000 payu-1.1.2/payu/profilers/darshan.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-01-23 01:35:47.000000 payu-1.1.2/payu/profilers/gprof.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-01-23 01:35:47.000000 payu-1.1.2/payu/profilers/oss.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-23 01:35:47.000000 payu-1.1.2/payu/profilers/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-01-23 01:35:47.000000 payu-1.1.2/payu/runlog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 01:35:54.760203 payu-1.1.2/payu/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-23 01:35:47.000000 payu-1.1.2/payu/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-01-23 01:35:47.000000 payu-1.1.2/payu/schedulers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-01-23 01:35:47.000000 payu-1.1.2/payu/schedulers/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-01-23 01:35:47.000000 payu-1.1.2/payu/schedulers/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 01:35:54.764203 payu-1.1.2/payu/subcommands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/archive_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/args.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/branch_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/build_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/checkout_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/clone_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/collate_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/ghsetup_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/init_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/list_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/profile_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/push_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/setup_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/sweep_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-01-23 01:35:47.000000 payu-1.1.2/payu/subcommands/sync_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-01-23 01:35:47.000000 payu-1.1.2/payu/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 01:35:54.768203 payu-1.1.2/payu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-23 01:35:54.000000 payu-1.1.2/payu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-01-23 01:35:54.000000 payu-1.1.2/payu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 01:35:54.000000 payu-1.1.2/payu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-01-23 01:35:54.000000 payu-1.1.2/payu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-23 01:35:54.000000 payu-1.1.2/payu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-23 01:35:54.000000 payu-1.1.2/payu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-01-23 01:35:47.000000 payu-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 01:35:54.768203 payu-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-23 01:35:47.000000 payu-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 01:35:54.768203 payu-1.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)    20901 2024-01-23 01:35:47.000000 payu-1.1.2/test/test_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-01-23 01:35:47.000000 payu-1.1.2/test/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-01-23 01:35:47.000000 payu-1.1.2/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-01-23 01:35:47.000000 payu-1.1.2/test/test_git_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16387 2024-01-23 01:35:47.000000 payu-1.1.2/test/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13140 2024-01-23 01:35:47.000000 payu-1.1.2/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-01-23 01:35:47.000000 payu-1.1.2/test/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-01-23 01:35:47.000000 payu-1.1.2/test/test_payu.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-01-23 01:35:47.000000 payu-1.1.2/test/test_pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-01-23 01:35:47.000000 payu-1.1.2/test/test_prune_restarts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-01-23 01:35:47.000000 payu-1.1.2/test/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-01-23 01:35:47.000000 payu-1.1.2/test/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:26.383438 payu-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 23:19:22.000000 payu-1.1.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11022 2024-04-11 23:19:22.000000 payu-1.1.3/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-11 23:19:22.000000 payu-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-11 23:19:22.000000 payu-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-11 23:19:22.000000 payu-1.1.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-11 23:19:26.383438 payu-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-11 23:19:22.000000 payu-1.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:26.371438 payu-1.1.3/payu/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-11 23:19:22.000000 payu-1.1.3/payu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-11 23:19:26.383438 payu-1.1.3/payu/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-11 23:19:22.000000 payu-1.1.3/payu/backports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-04-11 23:19:22.000000 payu-1.1.3/payu/branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-11 23:19:22.000000 payu-1.1.3/payu/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-11 23:19:22.000000 payu-1.1.3/payu/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-11 23:19:22.000000 payu-1.1.3/payu/envmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40270 2024-04-11 23:19:22.000000 payu-1.1.3/payu/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-11 23:19:22.000000 payu-1.1.3/payu/fsops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-11 23:19:22.000000 payu-1.1.3/payu/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-11 23:19:22.000000 payu-1.1.3/payu/laboratory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15861 2024-04-11 23:19:22.000000 payu-1.1.3/payu/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14700 2024-04-11 23:19:22.000000 payu-1.1.3/payu/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:26.375438 payu-1.1.3/payu/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/accessom2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/cable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/cesm_cmeps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/cice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/cice5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/fms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/gold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/matm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11511 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/mitgcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18061 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/mom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/mom6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/mom_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/nemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/oasis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/qgcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/um.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/ww3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-11 23:19:22.000000 payu-1.1.3/payu/models/yatm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-11 23:19:22.000000 payu-1.1.3/payu/namcouple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:26.375438 payu-1.1.3/payu/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-11 23:19:22.000000 payu-1.1.3/payu/profilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-11 23:19:22.000000 payu-1.1.3/payu/profilers/darshan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-11 23:19:22.000000 payu-1.1.3/payu/profilers/gprof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-11 23:19:22.000000 payu-1.1.3/payu/profilers/oss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-11 23:19:22.000000 payu-1.1.3/payu/profilers/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-04-11 23:19:22.000000 payu-1.1.3/payu/runlog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:26.379438 payu-1.1.3/payu/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-11 23:19:22.000000 payu-1.1.3/payu/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-04-11 23:19:22.000000 payu-1.1.3/payu/schedulers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-11 23:19:22.000000 payu-1.1.3/payu/schedulers/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-11 23:19:22.000000 payu-1.1.3/payu/schedulers/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:26.379438 payu-1.1.3/payu/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/archive_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/branch_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/build_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/checkout_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/clone_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/collate_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/ghsetup_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/init_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/list_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/profile_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/push_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/setup_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/sweep_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-11 23:19:22.000000 payu-1.1.3/payu/subcommands/sync_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-04-11 23:19:22.000000 payu-1.1.3/payu/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:26.383438 payu-1.1.3/payu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-11 23:19:26.000000 payu-1.1.3/payu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-11 23:19:26.000000 payu-1.1.3/payu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:19:26.000000 payu-1.1.3/payu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-11 23:19:26.000000 payu-1.1.3/payu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-11 23:19:26.000000 payu-1.1.3/payu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 23:19:26.000000 payu-1.1.3/payu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-11 23:19:22.000000 payu-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 23:19:26.383438 payu-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-11 23:19:22.000000 payu-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:26.383438 payu-1.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    20901 2024-04-11 23:19:22.000000 payu-1.1.3/test/test_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-11 23:19:22.000000 payu-1.1.3/test/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-04-11 23:19:22.000000 payu-1.1.3/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-11 23:19:22.000000 payu-1.1.3/test/test_git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16387 2024-04-11 23:19:22.000000 payu-1.1.3/test/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-11 23:19:22.000000 payu-1.1.3/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-11 23:19:22.000000 payu-1.1.3/test/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-04-11 23:19:22.000000 payu-1.1.3/test/test_payu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-11 23:19:22.000000 payu-1.1.3/test/test_pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-04-11 23:19:22.000000 payu-1.1.3/test/test_prune_restarts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-11 23:19:22.000000 payu-1.1.3/test/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-04-11 23:19:22.000000 payu-1.1.3/test/test_sync.py
```

### Comparing `payu-1.1.2/CHANGELOG` & `payu-1.1.3/CHANGELOG`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/LICENSE` & `payu-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/NOTICE` & `payu-1.1.3/NOTICE`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/PKG-INFO` & `payu-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payu
-Version: 1.1.2
+Version: 1.1.3
 Summary: A climate model workflow manager for supercomputing environments
 Author-email: Marshall Ward <python@marshallward.org>
 Maintainer-email: ACCESS-NRI <access.nri@anu.edu.au>
 License: Apache-2.0
 Keywords: climate model,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `payu-1.1.2/README.rst` & `payu-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/backports.py` & `payu-1.1.3/payu/backports.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/branch.py` & `payu-1.1.3/payu/branch.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 :license: Apache License, Version 2.0, see LICENSE for details.
 """
 
 import os
 import warnings
 from pathlib import Path
 from typing import Optional
+import shutil
 
 from ruamel.yaml import YAML, CommentedMap
 import git
 
 from payu.fsops import read_config, DEFAULT_CONFIG_FNAME, list_archive_dirs
 from payu.laboratory import Laboratory
 from payu.metadata import Metadata, UUID_FIELD, METADATA_FILENAME
-from payu.git_utils import GitRepository, git_clone
+from payu.git_utils import GitRepository, git_clone, PayuBranchError
 
 
 NO_CONFIG_FOUND_MESSAGE = """No configuration file found on this branch.
 Skipping adding new metadata file and creating archive/work symlinks.
 
 To find a branch that has a config file, you can:
     - Display local branches by running:
@@ -237,14 +238,21 @@
             Parent experiment UUID to add to generated metadata
 
     Returns: None
     """
     # Resolve directory to an absolute path
     control_path = directory.resolve()
 
+    if control_path.exists():
+        raise PayuBranchError(
+            f"Directory path `{control_path}` already exists. "
+            "Clone to a different path, or cd into the existing directory " +
+            "and use `payu checkout` if it is the same git repository"
+        )
+
     # git clone the repository
     repo = git_clone(repository, control_path, branch)
 
     owd = os.getcwd()
     try:
         # cd into cloned directory
         os.chdir(control_path)
@@ -271,14 +279,24 @@
                             keep_uuid=keep_uuid,
                             restart_path=restart_path,
                             control_path=control_path,
                             model_type=model_type,
                             lab_path=lab_path,
                             is_new_experiment=True,
                             parent_experiment=parent_experiment)
+    except PayuBranchError as e:
+        # Remove directory if incomplete checkout
+        shutil.rmtree(control_path)
+        msg = (
+            "Incomplete checkout. To run payu clone again, modify/remove " +
+            "the checkout new branch flag: --new-branch/-b, or " +
+            "checkout existing branch flag: --branch/-B " +
+            f"\n  Checkout error: {e}"
+        )
+        raise PayuBranchError(msg)
     finally:
         # Change back to original working directory
         os.chdir(owd)
 
     print(f"To change directory to control directory run:\n  cd {directory}")
```

### Comparing `payu-1.1.2/payu/calendar.py` & `payu-1.1.3/payu/calendar.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/cli.py` & `payu-1.1.3/payu/cli.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/envmod.py` & `payu-1.1.3/payu/envmod.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,19 +55,19 @@
         os.environ['MODULEPATH'] = ':'.join(modpaths)
 
     os.environ['LOADEDMODULES'] = os.environ.get('LOADEDMODULES', '')
 
     # Environment modules with certain characters will cause corruption
     # when MPI jobs get launched on other nodes (possibly a PBS issue).
     #
-    # Bash processes obscure the issue on Raijin, since it occurs in an
+    # Bash processes obscure the issue at NCI, since it occurs in an
     # environment module function, and bash moves those to the end of
     # the environment variable list.
     #
-    # Raijin's mpirun wrapper is a bash script, and therefore "fixes" by doing
+    # NCI's mpirun wrapper is a bash script, and therefore "fixes" by doing
     # the shuffle and limiting the damage to other bash functions, but some
     # wrappers (e.g. OpenMPI 2.1.x) may not be present.  So we manually patch
     # the problematic variable here.  But a more general solution would be nice
     # someday.
 
     if 'BASH_FUNC_module()' in os.environ:
         bash_func_module = os.environ['BASH_FUNC_module()']
```

### Comparing `payu-1.1.2/payu/experiment.py` & `payu-1.1.3/payu/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -486,16 +486,21 @@
 
         if self.config.get('scalasca', False):
             mpi_runcmd = ' '.join(['scalasca -analyze', mpi_runcmd])
 
         # MPI runtime flags
         mpi_flags = mpi_config.get('flags', [])
         if not mpi_flags:
-            mpi_flags = self.config.get('mpirun', [])
-            # TODO: Legacy config removal warning
+            # DEPRECATED: confusing and a duplication of flags config
+            if 'mpirun' in self.config:
+                mpi_flags = self.config.get('mpirun')
+                print('payu: warning: mpirun config option is deprecated.'
+                      '  Use mpi: flags option instead')
+            else:
+                mpi_flags = []
 
         if not isinstance(mpi_flags, list):
             mpi_flags = [mpi_flags]
 
         # TODO: More uniform support needed here
         if self.config.get('scalasca', False):
             mpi_flags = ['\"{0}\"'.format(f) for f in mpi_flags]
@@ -958,33 +963,35 @@
                               ignore_intermediate_restarts=False,
                               force=False):
         """Returns a list of restart directories that can be pruned"""
         # Check if archive path exists
         if not os.path.exists(self.archive_path):
             return []
 
-        # List all restart directories in archive
+        # Sorted list of restart directories in archive
         restarts = list_archive_dirs(archive_path=self.archive_path,
                                      dir_type='restart')
+        restart_indices = {}
+        for restart in restarts:
+            restart_indices[restart] = int(restart.lstrip('restart'))
 
         # TODO: Previous logic was to prune all restarts if self.repeat_run
         # Still need to figure out what should happen in this case
         if self.repeat_run:
             return [os.path.join(self.archive_path, restart)
                     for restart in restarts]
 
         # Use restart_freq to decide what restarts to prune
         restarts_to_prune = []
         intermediate_restarts, previous_intermediate_restarts = [], []
         restart_freq = self.config.get('restart_freq', default_restart_freq)
         if isinstance(restart_freq, int):
             # Using integer frequency to prune restarts
-            for restart in restarts:
-                restart_idx = int(restart.lstrip('restart'))
-                if not restart_idx % restart_freq == 0:
+            for restart, restart_index in restart_indices.items():
+                if not restart_index % restart_freq == 0:
                     intermediate_restarts.append(restart)
                 else:
                     # Add any intermediate restarts to restarts to prune
                     restarts_to_prune.extend(intermediate_restarts)
                     previous_intermediate_restarts = intermediate_restarts
                     intermediate_restarts = []
         else:
@@ -1044,24 +1051,26 @@
         # Restart_history override
         restart_history = self.config.get('restart_history', None)
         if restart_history is not None:
             if not isinstance(restart_history, int):
                 raise ValueError("payu: error: restart_history is not an "
                                  f"integer value: {restart_history}")
 
-            # Keep restart_history latest restarts, in addition to the
-            # permanently saved restarts defined by restart_freq
-            restarts_to_prune.extend(intermediate_restarts)
-            max_index = self.max_output_index(output_type="restart")
-            index_bound = max_index - restart_history
-            restarts_to_prune = [res for res in restarts_to_prune
-                                 if int(res.lstrip('restart')) <= index_bound]
+            if len(restarts) > 0:
+                max_index = restart_indices[restarts[-1]]
+                index_bound = max_index - restart_history
+
+                # Keep restart_history latest restarts, in addition to the
+                # permanently saved restarts defined by restart_freq
+                restarts_to_prune.extend(intermediate_restarts)
+                restarts_to_prune = [res for res in restarts_to_prune
+                                     if restart_indices[res] <= index_bound]
 
-            # Only expect at most 1 restart to be pruned with restart_history
-            is_unexpected = len(restarts_to_prune) > 1
+                # Expect at most 1 restart to be pruned with restart_history
+                is_unexpected = len(restarts_to_prune) > 1
 
         # Log out warning if more restarts than expected will be deleted
         if not force and is_unexpected:
             config_info = (f'restart pruning frequency of {restart_freq}')
             if restart_history:
                 config_info += f' and restart history of {restart_history}'
```

### Comparing `payu-1.1.2/payu/fsops.py` & `payu-1.1.3/payu/fsops.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/git_utils.py` & `payu-1.1.3/payu/git_utils.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/laboratory.py` & `payu-1.1.3/payu/laboratory.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/manifest.py` & `payu-1.1.3/payu/manifest.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/metadata.py` & `payu-1.1.3/payu/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,16 +32,15 @@
 NAME_FIELD = "name"
 GIT_URL_FIELD = "url"
 CREATED_FIELD = "created"
 MODEL_FIELD = "model"
 METADATA_FILENAME = "metadata.yaml"
 
 # Metadata Schema
-SCHEMA_URL = "https://raw.githubusercontent.com/ACCESS-NRI/schema/main/experiment_asset.json"
-
+SCHEMA_URL = "https://raw.githubusercontent.com/ACCESS-NRI/schema/80a3ce720af14b2b5e718630e1b52e7b3d22ea95/au.org.access-nri/model/output/experiment-metadata/1-0-3.json"
 
 class MetadataWarning(Warning):
     pass
 
 
 class Metadata:
     """
@@ -78,24 +77,20 @@
         # Config flag to disable creating metadata files and UUIDs
         self.enabled = self.metadata_config.get('enable', True)
 
         if self.enabled:
             self.repo = GitRepository(self.control_path, catch_error=True)
 
         self.branch = branch
-        self.branch_uuid_experiment = True
 
         # Set uuid if in metadata file
         metadata = self.read_file()
         self.uuid = metadata.get(UUID_FIELD, None)
         self.uuid_updated = False
 
-        # Experiment name configuration - this overrides experiment name
-        self.config_experiment_name = self.config.get("experiment", None)
-
     def read_file(self) -> CommentedMap:
         """Read metadata file - preserving orginal format if it exists"""
         metadata = CommentedMap()
         if self.filepath.exists():
             # Use default ruamel YAML to preserve comments and multi-line
             # strings
             metadata = YAML().load(self.filepath)
@@ -114,99 +109,111 @@
                 experiment name. This is set in payu.branch.checkout_branch.
         Return: None
 
         Note: Experiment name is the name used for the work and archive
         directories in the Laboratory.
         """
         if not self.enabled:
-            # Set experiment name only - either configured or includes branch
-            self.set_experiment_name(ignore_uuid=True)
+            # Set experiment name only - either configured or legacy name
+            self.set_experiment_name()
 
         elif self.uuid is not None and (keep_uuid or not is_new_experiment):
             self.set_experiment_name(keep_uuid=keep_uuid,
                                      is_new_experiment=is_new_experiment)
         else:
             # Generate new UUID
             if self.uuid is None and not is_new_experiment:
                 warnings.warn("No experiment uuid found in metadata. "
                               "Generating a new uuid", MetadataWarning)
             self.set_new_uuid(is_new_experiment=is_new_experiment)
 
         self.archive_path = self.lab_archive_path / self.experiment_name
 
-    def new_experiment_name(self, ignore_uuid: bool = False) -> str:
+    def new_experiment_name(self) -> str:
         """Generate a new experiment name"""
         if self.branch is None:
             self.branch = self.repo.get_branch_name()
 
         # Add branch and a truncated uuid to control directory name
         adding_branch = self.branch not in (None, 'main', 'master')
         suffix = f'-{self.branch}' if adding_branch else ''
 
-        if not ignore_uuid:
-            truncated_uuid = self.uuid[:TRUNCATED_UUID_LENGTH]
-            suffix += f'-{truncated_uuid}'
+        truncated_uuid = self.uuid[:TRUNCATED_UUID_LENGTH]
+        suffix += f'-{truncated_uuid}'
 
         return self.control_path.name + suffix
 
     def set_experiment_name(self,
                             is_new_experiment: bool = False,
-                            keep_uuid: bool = False,
-                            ignore_uuid: bool = False) -> None:
+                            keep_uuid: bool = False) -> None:
         """Set experiment name - this is used for work and archive
         sub-directories in the Laboratory"""
-        if self.config_experiment_name is not None:
-            # The configured value over-rides the experiment name
-            self.experiment_name = self.config_experiment_name
-            self.branch_uuid_experiment = False
+        # Experiment name configuration - this overrides experiment name
+        self.experiment_name = self.config.get("experiment", None)
+        if self.experiment_name is not None:
             print(f"Experiment name is configured in config.yaml: ",
                   self.experiment_name)
             return
 
-        if ignore_uuid:
-            # Leave experiment UUID out of experiment name
-            self.experiment_name = self.new_experiment_name(ignore_uuid=True)
+        # Legacy experiment name
+        legacy_name = self.control_path.name
+
+        if not self.enabled:
+            # Metadata/UUID generation is disabled, so leave UUID out of
+            # experiment name
+            self.experiment_name = legacy_name
+            print("Metadata is disabled in config.yaml.",
+                  f"Experiment name used for archival: {self.experiment_name}")
             return
 
-        # Branch-UUID experiment name and archive path
         branch_uuid_experiment_name = self.new_experiment_name()
-        archive_path = self.lab_archive_path / branch_uuid_experiment_name
-
-        # Legacy experiment name and archive path
-        legacy_name = self.control_path.name
-        legacy_archive_path = self.lab_archive_path / legacy_name
-
-        if is_new_experiment or archive_path.exists():
+        if is_new_experiment or self.has_archive(branch_uuid_experiment_name):
             # Use branch-UUID aware experiment name
             self.experiment_name = branch_uuid_experiment_name
-        elif legacy_archive_path.exists():
+        elif self.has_archive(legacy_name):
             # Use legacy CONTROL-DIR experiment name
             self.experiment_name = legacy_name
-            print(f"Pre-existing archive found at: {legacy_archive_path}. "
-                  f"Experiment name will remain: {legacy_name}")
-            self.branch_uuid_experiment = False
         elif keep_uuid:
             # Use same experiment UUID and use branch-UUID name for archive
             self.experiment_name = branch_uuid_experiment_name
         else:
             # No archive exists - Detecting new experiment
             warnings.warn(
                 "No pre-existing archive found. Generating a new uuid",
                 MetadataWarning
             )
             self.set_new_uuid(is_new_experiment=True)
 
+    def has_archive(self, experiment_name: str) -> bool:
+        """Return True if archive under the experiment name exists and
+        if it exists, check for a non-matching UUID in archive metadata."""
+        archive_path = self.lab_archive_path / experiment_name
+
+        if archive_path.exists():
+            # Check if the UUID in the archive metadata matches the
+            # UUID in metadata
+            archive_metadata_path = archive_path / METADATA_FILENAME
+            if archive_metadata_path.exists():
+                archive_metadata = YAML().load(archive_metadata_path)
+                if (UUID_FIELD in archive_metadata and
+                        archive_metadata[UUID_FIELD] != self.uuid):
+                    print("Mismatch of UUIDs between metadata and an archive "
+                          f"metadata found at: {archive_metadata_path}")
+                    return False
+            print(f"Found experiment archive: {archive_path}")
+        return archive_path.exists()
+
     def set_new_uuid(self, is_new_experiment: bool = False) -> None:
         """Generate a new uuid and set experiment name"""
         self.uuid_updated = True
         self.uuid = generate_uuid()
         self.set_experiment_name(is_new_experiment=is_new_experiment)
 
         # If experiment name does not include UUID, leave it unchanged
-        if not self.branch_uuid_experiment:
+        if self.experiment_name.endswith(self.uuid[:TRUNCATED_UUID_LENGTH]):
             return
 
         # Check experiment name is unique in local archive
         lab_archive_path = self.lab_archive_path
         if lab_archive_path.exists():
             local_experiments = [item for item in lab_archive_path.iterdir()
                                  if item.is_dir()]
@@ -263,15 +270,15 @@
         if parent_experiment is None:
             parent_experiment = self.get_parent_experiment(restart_path)
         if parent_experiment and parent_experiment != self.uuid:
             metadata[PARENT_UUID_FIELD] = parent_experiment
 
         # Add extra fields if new branch-uuid experiment
         # so to not over-write fields if it's a pre-existing legacy experiment
-        if self.branch_uuid_experiment:
+        if self.experiment_name.endswith(self.uuid[:TRUNCATED_UUID_LENGTH]):
             metadata[CREATED_FIELD] = datetime.now().strftime('%Y-%m-%d')
             metadata[NAME_FIELD] = self.experiment_name
             metadata[MODEL_FIELD] = self.get_model_name()
 
             # Add origin git URL, if defined
             url = self.repo.get_origin_url()
             if url:
```

### Comparing `payu-1.1.2/payu/models/__init__.py` & `payu-1.1.3/payu/models/__init__.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/access.py` & `payu-1.1.3/payu/models/access.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/accessom2.py` & `payu-1.1.3/payu/models/accessom2.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/cable.py` & `payu-1.1.3/payu/models/cable.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/cesm_cmeps.py` & `payu-1.1.3/payu/models/cesm_cmeps.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,20 +213,20 @@
                     self.work_path, pointer,
                     ) for pointer in self.rpointers
             ]
         restart_files = []
         for pointer in pointer_files:
             try:
                 with open(pointer,"r") as f:
-                    restart = f.readline().rstrip()
-                    restart_files.append(
-                        os.path.join(
-                            self.work_path, restart,
+                    for restart in f.readlines():
+                        restart_files.append(
+                            os.path.join(
+                                self.work_path, restart.rstrip(),
+                                )
                             )
-                        )
             except FileNotFoundError:
                 # TODO: copied this from other models. Surely we want to exit here or something
                 print(f"payu: error: Model has not produced pointer file {pointer}")
         
         for f_src in restart_files + pointer_files:
             name = os.path.basename(f_src)
             f_dst = os.path.join(self.restart_path, name)
```

### Comparing `payu-1.1.2/payu/models/cice.py` & `payu-1.1.3/payu/models/cice.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/cice5.py` & `payu-1.1.3/payu/models/cice5.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/fms.py` & `payu-1.1.3/payu/models/fms.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/gold.py` & `payu-1.1.3/payu/models/gold.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/matm.py` & `payu-1.1.3/payu/models/matm.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/mitgcm.py` & `payu-1.1.3/payu/models/mitgcm.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/model.py` & `payu-1.1.3/payu/models/model.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/mom.py` & `payu-1.1.3/payu/models/mom.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/mom6.py` & `payu-1.1.3/payu/models/mom6.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/mom_mixin.py` & `payu-1.1.3/payu/models/mom_mixin.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/nemo.py` & `payu-1.1.3/payu/models/nemo.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/oasis.py` & `payu-1.1.3/payu/models/oasis.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/qgcm.py` & `payu-1.1.3/payu/models/qgcm.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/test.py` & `payu-1.1.3/payu/models/test.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/um.py` & `payu-1.1.3/payu/models/um.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,19 @@
         if os.path.exists(restart_dump):
             shutil.copy(restart_dump, f_dst)
         else:
             print('payu: error: Model has not produced a restart dump file:\n'
                   '{} does not exist.\n'
                   'Check DUMPFREQim in namelists'.format(restart_dump))
 
+        # Now remove restart files from work directory so they're not
+        # unnecessarily archived to output
+        for f_path in glob.glob(os.path.join(self.work_path, 'aiihca.da*')):
+            os.remove(f_path)
+
     def collate(self):
         pass
 
     def setup(self):
         super(UnifiedModel, self).setup()
 
         # Set up environment variables needed to run UM.
```

### Comparing `payu-1.1.2/payu/models/ww3.py` & `payu-1.1.3/payu/models/ww3.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/models/yatm.py` & `payu-1.1.3/payu/models/yatm.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/namcouple.py` & `payu-1.1.3/payu/namcouple.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/profilers/gprof.py` & `payu-1.1.3/payu/profilers/gprof.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/profilers/oss.py` & `payu-1.1.3/payu/profilers/oss.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/runlog.py` & `payu-1.1.3/payu/runlog.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/schedulers/pbs.py` & `payu-1.1.3/payu/schedulers/pbs.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/schedulers/scheduler.py` & `payu-1.1.3/payu/schedulers/scheduler.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/schedulers/slurm.py` & `payu-1.1.3/payu/schedulers/slurm.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/subcommands/archive_cmd.py` & `payu-1.1.3/payu/subcommands/archive_cmd.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/subcommands/args.py` & `payu-1.1.3/payu/subcommands/args.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/subcommands/branch_cmd.py` & `payu-1.1.3/payu/subcommands/branch_cmd.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/subcommands/checkout_cmd.py` & `payu-1.1.3/payu/subcommands/checkout_cmd.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/subcommands/clone_cmd.py` & `payu-1.1.3/payu/subcommands/clone_cmd.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/subcommands/collate_cmd.py` & `payu-1.1.3/payu/subcommands/collate_cmd.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/subcommands/ghsetup_cmd.py` & `payu-1.1.3/payu/subcommands/ghsetup_cmd.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/subcommands/profile_cmd.py` & `payu-1.1.3/payu/subcommands/profile_cmd.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/subcommands/push_cmd.py` & `payu-1.1.3/payu/subcommands/push_cmd.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/subcommands/run_cmd.py` & `payu-1.1.3/payu/subcommands/run_cmd.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/subcommands/setup_cmd.py` & `payu-1.1.3/payu/subcommands/setup_cmd.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/subcommands/sync_cmd.py` & `payu-1.1.3/payu/subcommands/sync_cmd.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu/sync.py` & `payu-1.1.3/payu/sync.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/payu.egg-info/PKG-INFO` & `payu-1.1.3/payu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payu
-Version: 1.1.2
+Version: 1.1.3
 Summary: A climate model workflow manager for supercomputing environments
 Author-email: Marshall Ward <python@marshallward.org>
 Maintainer-email: ACCESS-NRI <access.nri@anu.edu.au>
 License: Apache-2.0
 Keywords: climate model,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `payu-1.1.2/payu.egg-info/SOURCES.txt` & `payu-1.1.3/payu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/pyproject.toml` & `payu-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/test/test_branch.py` & `payu-1.1.3/test/test_branch.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/test/test_calendar.py` & `payu-1.1.3/test/test_calendar.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/test/test_cli.py` & `payu-1.1.3/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/test/test_git_utils.py` & `payu-1.1.3/test/test_git_utils.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/test/test_manifest.py` & `payu-1.1.3/test/test_manifest.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/test/test_metadata.py` & `payu-1.1.3/test/test_metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -75,56 +75,56 @@
         shutil.rmtree(labdir)
     except Exception as e:
         print(e)
 
 
 @patch("payu.metadata.GitRepository")
 @pytest.mark.parametrize(
-    "uuid, legacy_archive_exists, previous_metadata, expected_metadata",
+    "uuid, experiment_name, previous_metadata, expected_metadata",
     [
         # Test new metadata file created
         (
             "b1f3ce3d-99da-40e4-849a-c8b352948a31",
-            False,
+            "ctrl-branch-b1f3ce3d",
             None,
             {
                 "experiment_uuid": "b1f3ce3d-99da-40e4-849a-c8b352948a31",
                 "created": '2000-01-01',
-                "name": "DefaultExperimentName",
+                "name": "ctrl-branch-b1f3ce3d",
                 "model": "TEST-MODEL",
                 "url": "mockUrl",
                 "contact": "mockUser",
                 "email": "mock@email.com"
             }
         ),
         # Test metadata file updated when new UUID
         (
             "7b90f37c-4619-44f9-a439-f76fdf6ae2bd",
-            False,
+            "Control-Branch-7b90f37c",
             {
                 "experiment_uuid": "b3298c7f-01f6-4f0a-be32-ce5d2cfb9a04",
                 "contact": "Add your name here",
                 "email": "Add your email address here",
                 "description": "Add description here",
             },
             {
                 "experiment_uuid": "7b90f37c-4619-44f9-a439-f76fdf6ae2bd",
                 "description": "Add description here",
                 "created": '2000-01-01',
-                "name": "DefaultExperimentName",
+                "name": "Control-Branch-7b90f37c",
                 "model": "TEST-MODEL",
                 "url": "mockUrl",
                 "contact": "mockUser",
                 "email": "mock@email.com"
             }
         ),
         # Test extra fields not added with legacy experiments
         (
             "7b90f37c-4619-44f9-a439-f76fdf6ae2bd",
-            True,
+            "ctrl",
             {
                 "experiment_uuid": "0f49f2a0-f45e-4c0b-a3b6-4b0bf21f2b75",
                 "name": "UserDefinedExperimentName",
                 "contact": "TestUser",
                 "email": "Test@email.com"
             },
             {
@@ -132,15 +132,15 @@
                 "name": "UserDefinedExperimentName",
                 "contact": "TestUser",
                 "email": "Test@email.com"
             }
         ),
     ]
 )
-def test_update_file(mock_repo, uuid, legacy_archive_exists,
+def test_update_file(mock_repo, uuid, experiment_name,
                      previous_metadata, expected_metadata):
     # Create pre-existing metadata file
     metadata_path = ctrldir / 'metadata.yaml'
     yaml = YAML()
     if previous_metadata is not None:
         with open(metadata_path, 'w') as file:
             yaml.dump(previous_metadata, file)
@@ -154,16 +154,15 @@
     test_config['model'] = "test-model"
     write_config(test_config)
 
     # Initialise Metadata
     with cd(ctrldir):
         metadata = Metadata(archive_dir)
     metadata.uuid = uuid
-    metadata.experiment_name = "DefaultExperimentName"
-    metadata.branch_uuid_experiment = not legacy_archive_exists
+    metadata.experiment_name = experiment_name
 
     # Mock datetime (for created date)
     with patch('payu.metadata.datetime') as mock_date:
         mock_date.now.return_value = datetime(2000, 1, 1)
 
         # Function to test
         metadata.update_file()
@@ -258,14 +257,60 @@
             metadata.setup(is_new_experiment=is_new_experiment,
                            keep_uuid=keep_uuid)
 
     assert metadata.experiment_name == expected_name
     assert metadata.uuid == expected_uuid
 
 
+@pytest.mark.parametrize(
+    "archive_metadata_exists, archive_uuid, expected_result",
+    [
+        # A legacy archive exists, but there's no corresponding metadata
+        # in archive
+        (
+            False, None, True
+        ),
+        # Archive metadata exists but has no UUID
+        (
+            True, None, True
+        ),
+        # Archive metadata exists with same UUID
+        (
+            True, "3d18b3b6-dd19-49a9-8d9e-c7fa8582f136", True
+        ),
+        # Archive metadata exists with different UUID
+        (
+            True, "cb793e91-6168-4ed2-a70c-f6f9ccf1659b", False
+        ),
+    ]
+)
+def test_has_archive(archive_metadata_exists, archive_uuid, expected_result):
+    # Setup config and metadata
+    write_config(config)
+    with cd(ctrldir):
+        metadata = Metadata(archive_dir)
+    metadata.uuid = "3d18b3b6-dd19-49a9-8d9e-c7fa8582f136"
+
+    # Setup archive and it's metadata file
+    archive_path = archive_dir / "ctrl"
+    archive_path.mkdir(parents=True)
+
+    if archive_metadata_exists:
+        archive_metadata = {}
+
+        if archive_uuid is not None:
+            archive_metadata["experiment_uuid"] = archive_uuid
+
+        with open(archive_path / 'metadata.yaml', 'w') as file:
+            YAML().dump(archive_metadata, file)
+
+    result = metadata.has_archive("ctrl")
+    assert result == expected_result
+
+
 def test_set_configured_experiment_name():
     # Set experiment in config file
     test_config = copy.deepcopy(config)
     test_config['experiment'] = "configuredExperiment"
     write_config(test_config)
 
     with cd(ctrldir):
@@ -284,42 +329,46 @@
     [(None, "ctrl-cb793e91"),
      ("main", "ctrl-cb793e91"),
      ("master", "ctrl-cb793e91"),
      ("branch", "ctrl-branch-cb793e91")]
 )
 def test_new_experiment_name(branch, expected_name):
     # Test configured experiment name is the set experiment name
+    write_config(config)
     with cd(ctrldir):
         metadata = Metadata(archive_dir)
 
     metadata.uuid = "cb793e91-6168-4ed2-a70c-f6f9ccf1659b"
 
     with patch('payu.metadata.GitRepository.get_branch_name') as mock_branch:
         mock_branch.return_value = branch
         experiment = metadata.new_experiment_name()
 
     assert experiment == expected_name
 
 
-@pytest.mark.parametrize(
-    "branch, expected_name",
-    [(None, "ctrl"),
-     ("main", "ctrl"),
-     ("branch", "ctrl-branch")]
-)
-def test_new_experiment_name_ignore_uuid(branch, expected_name):
-    # Test configured experiment name is the set experiment name
-    with cd(ctrldir):
-        metadata = Metadata(archive_dir)
+def test_metadata_enable_false():
+    # Set metadata to false in config file
+    test_config = copy.deepcopy(config)
+    test_config['metadata'] = {
+        "enable": False
+    }
+    write_config(test_config)
 
     with patch('payu.metadata.GitRepository.get_branch_name') as mock_branch:
-        mock_branch.return_value = branch
-        experiment = metadata.new_experiment_name(ignore_uuid=True)
+        mock_branch.return_value = "mock-branch"
 
-    assert experiment == expected_name
+        with cd(ctrldir):
+            metadata = Metadata(archive_dir)
+            metadata.setup()
+            metadata.write_metadata()
+
+    # Test UUID kept out of experiment name and metadata file is not written
+    assert metadata.experiment_name == "ctrl"
+    assert not (ctrldir / "metadata.yaml").exists()
 
 
 @patch("payu.metadata.GitRepository")
 def test_update_file_with_template_metadata_values(mock_repo):
     # Leave out origin URL and git user info
     mock_repo.return_value.get_origin_url.return_value = None
     mock_repo.return_value.get_user_info.return_value = None
```

### Comparing `payu-1.1.2/test/test_paths.py` & `payu-1.1.3/test/test_paths.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/test/test_payu.py` & `payu-1.1.3/test/test_payu.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/test/test_pbs.py` & `payu-1.1.3/test/test_pbs.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/test/test_prune_restarts.py` & `payu-1.1.3/test/test_prune_restarts.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import shutil
 
 import pytest
 
 import payu
 
 from test.common import cd
-from test.common import tmpdir, ctrldir, labdir
+from test.common import tmpdir, ctrldir, labdir, expt_archive_dir
 from test.common import config as config_orig
 from test.common import write_config
 from test.common import make_all_files
 from test.common import remove_expt_archive_dirs, make_expt_archive_dir
 from test.models.test_mom_mixin import make_ocean_restart_dir
 
 verbose = True
@@ -59,14 +59,17 @@
 def teardown():
     # Run test
     yield
 
     # Remove any created restart files
     remove_expt_archive_dirs(type='restart')
 
+    # Remove experiment archive
+    expt_archive_dir.rmdir()
+
 
 def create_test_2Y_1_month_frequency_restarts():
     """Create 2 years + 1 month worth of mom restarts directories
     with 1 month runtimes - starting from 1900/02/01 to 1902/02/01
     e.g (run_date, restart_directory)
     (1900/02/01, restart000)
     (1900/03/01, restart001)
@@ -84,22 +87,23 @@
         make_ocean_restart_dir(start_dt="1900-01-01 00:00:00",
                                run_dt=run_dt,
                                calendar=4,
                                restart_index=index,
                                additional_path='ocean')
 
 
-def write_test_config(restart_freq, restart_history=None):
+def write_test_config(restart_freq=None, restart_history=None):
     test_config = copy.deepcopy(config)
     test_config['model'] = 'access-om2'
     test_config['submodels'] = [
         {'name': 'atmosphere', 'model': 'yatm'},
         {'name': 'ocean', 'model': 'mom'}
     ]
-    test_config['restart_freq'] = restart_freq
+    if restart_freq:
+        test_config['restart_freq'] = restart_freq
     if restart_history:
         test_config['restart_history'] = restart_history
 
     write_config(test_config)
 
 
 @pytest.mark.parametrize(
@@ -253,7 +257,21 @@
 
     # Extract out index
     restarts_to_prune_indices = [
         int(restart.lstrip('restart')) for restart in restarts_to_prune
     ]
 
     assert restarts_to_prune_indices == [5]
+
+
+def test_restart_history_with_empty_archive():
+    write_test_config(restart_history=3)
+    expt_archive_dir.mkdir()
+
+    with cd(ctrldir):
+        lab = payu.laboratory.Laboratory(lab_path=str(labdir))
+        expt = payu.experiment.Experiment(lab, reproduce=False)
+
+        # Function to test
+        restarts_to_prune = expt.get_restarts_to_prune()
+
+    assert restarts_to_prune == []
```

### Comparing `payu-1.1.2/test/test_setup.py` & `payu-1.1.3/test/test_setup.py`

 * *Files identical despite different names*

### Comparing `payu-1.1.2/test/test_sync.py` & `payu-1.1.3/test/test_sync.py`

 * *Files identical despite different names*

