# Comparing `tmp/m3-gar-1.0.9.tar.gz` & `tmp/m3-gar-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3-gar-1.0.9.tar", last modified: Fri Oct 29 22:33:17 2021, max compression
+gzip compressed data, was "m3-gar-1.1.0.tar", last modified: Fri Apr 12 07:22:52 2024, max compression
```

## Comparing `m3-gar-1.0.9.tar` & `m3-gar-1.1.0.tar`

### file list

```diff
@@ -1,84 +1,104 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 22:33:17.792215 m3-gar-1.0.9/
--rw-r--r--   0 root         (0) root         (0)       23 2021-10-21 16:50:27.000000 m3-gar-1.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12067 2021-10-29 22:33:17.792215 m3-gar-1.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11426 2021-10-21 16:50:27.000000 m3-gar-1.0.9/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 22:33:17.781215 m3-gar-1.0.9/m3_gar/
--rw-r--r--   0 root         (0) root         (0)        0 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28000 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/base_models.py
--rw-r--r--   0 root         (0) root         (0)      757 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/compat.py
--rw-r--r--   0 root         (0) root         (0)     1131 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/config.py
--rw-r--r--   0 root         (0) root         (0)      174 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 22:33:17.784215 m3-gar-1.0.9/m3_gar/importer/
--rw-r--r--   0 root         (0) root         (0)        0 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/__init__.py
--rw-r--r--   0 root         (0) root         (0)      343 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/client.py
--rw-r--r--   0 root         (0) root         (0)    15691 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/commands.py
--rw-r--r--   0 root         (0) root         (0)     2590 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/constraints.py
--rw-r--r--   0 root         (0) root         (0)       27 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/consts.py
--rw-r--r--   0 root         (0) root         (0)     4160 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/db_wrapper.py
--rw-r--r--   0 root         (0) root         (0)       96 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     4588 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/loader.py
--rw-r--r--   0 root         (0) root         (0)     1097 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/models_sort.py
--rw-r--r--   0 root         (0) root         (0)      964 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 22:33:17.785215 m3-gar-1.0.9/m3_gar/importer/source/
--rw-r--r--   0 root         (0) root         (0)      175 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/source/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2318 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/source/archive.py
--rw-r--r--   0 root         (0) root         (0)      312 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/source/directory.py
--rw-r--r--   0 root         (0) root         (0)      567 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/source/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2090 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/source/tablelist.py
--rw-r--r--   0 root         (0) root         (0)     2071 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/source/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 22:33:17.786215 m3-gar-1.0.9/m3_gar/importer/table/
--rw-r--r--   0 root         (0) root         (0)      722 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/table/__init__.py
--rw-r--r--   0 root         (0) root         (0)       26 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/table/consts.py
--rw-r--r--   0 root         (0) root         (0)      160 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/table/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1728 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/table/table.py
--rw-r--r--   0 root         (0) root         (0)     2040 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/table/xml.py
--rw-r--r--   0 root         (0) root         (0)     3091 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/timer.py
--rw-r--r--   0 root         (0) root         (0)     1435 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/importer/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 22:33:17.786215 m3-gar-1.0.9/m3_gar/management/
--rw-r--r--   0 root         (0) root         (0)        0 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 22:33:17.787215 m3-gar-1.0.9/m3_gar/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1024 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/management/commands/gar_check_models.py
--rw-r--r--   0 root         (0) root         (0)     1744 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/management/commands/gar_generate_base_models.py
--rw-r--r--   0 root         (0) root         (0)     4924 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/management/commands/gar_load_data.py
--rw-r--r--   0 root         (0) root         (0)     4328 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/management/commands/gar_update_schema.py
--rw-r--r--   0 root         (0) root         (0)     4475 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/management/commands/manage_constraints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 22:33:17.788215 m3-gar-1.0.9/m3_gar/migrations/
--rw-r--r--   0 root         (0) root         (0)    39585 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      967 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/migrations/0002_auto_20210707_1352.py
--rw-r--r--   0 root         (0) root         (0)    14432 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/migrations/0003_auto_20210906_0744.py
--rw-r--r--   0 root         (0) root         (0)    10218 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/migrations/0004_auto_20211013_1106.py
--rw-r--r--   0 root         (0) root         (0)     2097 2021-10-29 22:33:09.000000 m3-gar-1.0.9/m3_gar/migrations/0005_auto_20211029_1212.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 22:33:17.792215 m3-gar-1.0.9/m3_gar/models/
--rw-r--r--   0 root         (0) root         (0)      463 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2250 2021-10-29 22:33:09.000000 m3-gar-1.0.9/m3_gar/models/addrobj.py
--rw-r--r--   0 root         (0) root         (0)     1045 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/models/apartment.py
--rw-r--r--   0 root         (0) root         (0)      673 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/models/carplace.py
--rw-r--r--   0 root         (0) root         (0)     1657 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/models/hierarchy.py
--rw-r--r--   0 root         (0) root         (0)      494 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/models/history.py
--rw-r--r--   0 root         (0) root         (0)     1463 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/models/house.py
--rw-r--r--   0 root         (0) root         (0)     1729 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/models/normdoc.py
--rw-r--r--   0 root         (0) root         (0)      361 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/models/op_type.py
--rw-r--r--   0 root         (0) root         (0)     1379 2021-10-29 22:33:09.000000 m3-gar-1.0.9/m3_gar/models/param.py
--rw-r--r--   0 root         (0) root         (0)     2386 2021-10-29 22:33:09.000000 m3-gar-1.0.9/m3_gar/models/reestr.py
--rw-r--r--   0 root         (0) root         (0)      974 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/models/room.py
--rw-r--r--   0 root         (0) root         (0)      713 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/models/stead.py
--rw-r--r--   0 root         (0) root         (0)     1389 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/models/util.py
--rw-r--r--   0 root         (0) root         (0)      869 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/models/version.py
--rw-r--r--   0 root         (0) root         (0)    11637 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/publish_tools.py
--rw-r--r--   0 root         (0) root         (0)      960 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/routers.py
--rw-r--r--   0 root         (0) root         (0)     2936 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/util.py
--rwxr-xr-x   0 root         (0) root         (0)       83 2021-10-29 22:33:09.000000 m3-gar-1.0.9/m3_gar/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 22:33:17.792215 m3-gar-1.0.9/m3_gar/xsd_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/xsd_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7271 2021-10-21 16:50:27.000000 m3-gar-1.0.9/m3_gar/xsd_generator/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 22:33:17.782215 m3-gar-1.0.9/m3_gar.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12067 2021-10-29 22:33:17.000000 m3-gar-1.0.9/m3_gar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2062 2021-10-29 22:33:17.000000 m3-gar-1.0.9/m3_gar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-29 22:33:17.000000 m3-gar-1.0.9/m3_gar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2021-10-29 22:33:17.000000 m3-gar-1.0.9/m3_gar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2021-10-29 22:33:17.000000 m3-gar-1.0.9/m3_gar.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-10-29 22:33:17.793215 m3-gar-1.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      116 2021-10-21 16:50:27.000000 m3-gar-1.0.9/setup.py
--rw-r--r--   0 root         (0) root         (0)     1211 2021-10-21 16:50:27.000000 m3-gar-1.0.9/setup_kwargs.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-12 07:22:52.776952 m3-gar-1.1.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)       23 2021-12-09 09:34:10.000000 m3-gar-1.1.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    14741 2024-04-12 07:22:52.775952 m3-gar-1.1.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)    13880 2022-06-14 19:44:09.000000 m3-gar-1.1.0/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-12 07:22:52.592952 m3-gar-1.1.0/m3_gar/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    28529 2022-05-18 19:32:18.000000 m3-gar-1.1.0/m3_gar/base_models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      757 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/compat.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1131 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/config.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      548 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      571 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      174 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/exceptions.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-12 07:22:52.610952 m3-gar-1.1.0/m3_gar/importer/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/importer/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1822 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/importer/client.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    18385 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/importer/commands.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2590 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/importer/constraints.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       27 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/importer/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4160 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/importer/db_wrapper.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      852 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/importer/exceptions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4588 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/importer/loader.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1097 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/importer/models_sort.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      964 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/importer/signals.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-12 07:22:52.621952 m3-gar-1.1.0/m3_gar/importer/source/
+-rw-r--r--   0 toor      (1000) toor      (1000)      175 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/importer/source/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2344 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/importer/source/archive.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      312 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/importer/source/directory.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      618 2022-05-13 06:47:55.000000 m3-gar-1.1.0/m3_gar/importer/source/exceptions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2248 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/importer/source/tablelist.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2071 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/importer/source/wrapper.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-12 07:22:52.633952 m3-gar-1.1.0/m3_gar/importer/table/
+-rw-r--r--   0 toor      (1000) toor      (1000)      722 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/importer/table/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       26 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/importer/table/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      160 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/importer/table/exceptions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1728 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/importer/table/table.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2196 2022-05-31 07:59:24.000000 m3-gar-1.1.0/m3_gar/importer/table/xml.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3333 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/importer/timer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2754 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/importer/version.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-12 07:22:52.635952 m3-gar-1.1.0/m3_gar/management/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/management/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-12 07:22:52.657952 m3-gar-1.1.0/m3_gar/management/commands/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/management/commands/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11958 2024-01-25 13:10:33.000000 m3-gar-1.1.0/m3_gar/management/commands/fill_custom_fields.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1024 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/management/commands/gar_check_models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1857 2022-05-20 05:39:49.000000 m3-gar-1.1.0/m3_gar/management/commands/gar_generate_base_models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5506 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/management/commands/gar_load_data.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4271 2022-05-20 05:39:49.000000 m3-gar-1.1.0/m3_gar/management/commands/gar_update_schema.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4475 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/management/commands/manage_constraints.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-12 07:22:52.708952 m3-gar-1.1.0/m3_gar/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)    39585 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      967 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/migrations/0002_auto_20210707_1352.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    14432 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/migrations/0003_auto_20210906_0744.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    10218 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/migrations/0004_auto_20211013_1106.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2097 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/migrations/0005_auto_20211029_1212.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      460 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/migrations/0006_auto_20211105_0937.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      427 2022-02-24 06:34:53.000000 m3-gar-1.1.0/m3_gar/migrations/0007_version_processed.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1158 2022-05-20 05:39:49.000000 m3-gar-1.1.0/m3_gar/migrations/0008_auto_20220217_0556.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      294 2022-02-24 06:34:53.000000 m3-gar-1.1.0/m3_gar/migrations/0009_delete_status.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      823 2022-02-25 10:15:33.000000 m3-gar-1.1.0/m3_gar/migrations/0010_auto_20220225_0934.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      782 2022-03-23 11:24:27.000000 m3-gar-1.1.0/m3_gar/migrations/0011_auto_20220323_1022.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1346 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/migrations/0012_auto_20220415_1452.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1331 2022-05-18 19:32:18.000000 m3-gar-1.1.0/m3_gar/migrations/0013_auto_20220513_0825.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      516 2022-05-18 19:32:18.000000 m3-gar-1.1.0/m3_gar/migrations/0014_addrobj_name_with_typename.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      538 2022-06-01 06:58:09.000000 m3-gar-1.1.0/m3_gar/migrations/0015_alter_normativedocs_orgname.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      539 2022-10-24 07:33:27.000000 m3-gar-1.1.0/m3_gar/migrations/0016_alter_normativedocs_orgname.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      483 2024-03-29 16:59:39.000000 m3-gar-1.1.0/m3_gar/migrations/0017_apartments_m3_gar_apar_objectg_0e459a_hash.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      532 2024-03-30 05:17:19.000000 m3-gar-1.1.0/m3_gar/migrations/0018_addrobj_addrobj_name_with_typename_gin.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      614 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/migrations/0019_version_status.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1180 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/migrations/0020_update_version_status.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      344 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/migrations/0021_remove_version_processed.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/migrations/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-12 07:22:52.763952 m3-gar-1.1.0/m3_gar/models/
+-rw-r--r--   0 toor      (1000) toor      (1000)      463 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/models/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3875 2024-03-30 05:17:19.000000 m3-gar-1.1.0/m3_gar/models/addrobj.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1201 2024-03-29 16:59:39.000000 m3-gar-1.1.0/m3_gar/models/apartment.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      673 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/models/carplace.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3546 2022-05-18 19:32:18.000000 m3-gar-1.1.0/m3_gar/models/hierarchy.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      494 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/models/history.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1635 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/models/house.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1238 2022-05-18 19:32:18.000000 m3-gar-1.1.0/m3_gar/models/indexes.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2602 2022-10-24 07:33:27.000000 m3-gar-1.1.0/m3_gar/models/normdoc.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      361 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/models/op_type.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1379 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/models/param.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2386 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/models/reestr.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      974 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/models/room.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      713 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/models/stead.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3451 2021-12-26 06:47:21.000000 m3-gar-1.1.0/m3_gar/models/util.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1618 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/models/version.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11809 2022-05-20 05:39:49.000000 m3-gar-1.1.0/m3_gar/publish_tools.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      960 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/routers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2936 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/util.py
+-rwxr-xr-x   0 toor      (1000) toor      (1000)       83 2024-04-12 07:22:47.000000 m3-gar-1.1.0/m3_gar/version.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-12 07:22:52.764952 m3-gar-1.1.0/m3_gar/xsd_generator/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-12-09 09:34:10.000000 m3-gar-1.1.0/m3_gar/xsd_generator/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7289 2022-05-20 05:39:49.000000 m3-gar-1.1.0/m3_gar/xsd_generator/base.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-12 07:22:52.774953 m3-gar-1.1.0/m3_gar.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    14741 2024-04-12 07:22:52.000000 m3-gar-1.1.0/m3_gar.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     2958 2024-04-12 07:22:52.000000 m3-gar-1.1.0/m3_gar.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-12 07:22:52.000000 m3-gar-1.1.0/m3_gar.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      108 2024-04-12 07:22:52.000000 m3-gar-1.1.0/m3_gar.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        7 2024-04-12 07:22:52.000000 m3-gar-1.1.0/m3_gar.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-04-12 07:22:52.776952 m3-gar-1.1.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)      128 2022-05-20 05:39:49.000000 m3-gar-1.1.0/setup.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1428 2022-05-20 05:39:49.000000 m3-gar-1.1.0/setup_kwargs.py
```

### Comparing `m3-gar-1.0.9/PKG-INFO` & `m3-gar-1.1.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: m3-gar
-Version: 1.0.9
-Summary: GAR Django integration for m3
-Home-page: UNKNOWN
-Author: BARS Group
-Author-email: bars@bars.group
-License: MIT license
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Russian
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-
 Приложение для работы с базой данных ГАР в Django
 
 Основные возможности
 ====================
 
 * Импорт базы ГАР из:
     * архива XML
@@ -175,15 +156,15 @@
 --commit
     запись изменений в БД, в противном случае происходит только генерация SQL-кода
 
 Полный порядок действий:
 
 1. Отключить ограничения:::
 
-        python manage.py manage_constraints disable --constraints --logged --commit
+        python manage.py manage_constraints disable --fk --unique --index --logged --commit
 
 2. Произвести загрузку общих справочников::
 
         python manage.py gar_load_data --no-truncate --no-transaction /path/to/gar_data/
 
 В директории /path/to/gar_data/ должны лежать файлы AS_*.xml из корня архива, т.е.::
 
@@ -204,15 +185,15 @@
         ...
         /path/to/gar_data/02/AS_STEADS_PARAMS_20211004_738598d9-38b0-441d-9276-c7ac7e41d606.XML
 
 4. Повторить п.3 для других регионов
 
 5. После успешной загрузки всех данных включить ограничения обратно:::
 
-        python manage.py manage_constraints enable --constraints --logged --commit
+        python manage.py manage_constraints enable --fk --unique --index --logged --commit
 
 
 Удаление данных из БД
 ----------------------
 Используется опция --truncate команды manage_constraints.
 Принимает ничего, либо список регионов, разделённых запятой.
 Для удаления данных по общим справочникам используется регион с кодом "0"
@@ -263,7 +244,41 @@
 
 
 Настройка settings.py
 =====================
 `GAR_DATABASE_ALIAS` - алиас БД в `DATABASES` для данных ГАР
 
 
+Заполнение полей name_with_parents в модели иерархий и полей name_with_typename в модели AddrOdj
+================================================================================================
+
+В БД были добавлены дополнительные поля name_with_parents (в модели иерархий) и name_with_typename (в модели AddrOdj).
+Для заполнения данных полей данными предоставлена команда `fill_custom_fields`
+Для нее доступны следующие параметры:
+
+--parents
+    Заполняем поля name_with_parents в модели иерархий, по умолчанию в муниципальной иерархии, можно указать ключи:
+        --adm - поля заполняются для административной иерархии
+        --guids - можно через запятую указать guid-ы объектов, для которых нужно заполнить поле
+        --levels - можно через запятую указать уровни объектов, для которых нужно заполнить поле
+
+--typenames
+    Заполняем поля name_with_typename в модели AddrOdj для уровней 7 и 8 (улицы, микрорайоны, территории и т.д.)
+        --guids_typenames - можно через запятую указать guid-ы объектов, для которых нужно заполнить поле
+
+Примеры выполнения команды:
+
+    - Обновление всех полей name_with_parents в модели муниципальной иерархии:
+
+            python manage.py fill_custom_fields --parents
+
+    - Обновление полей name_with_parents в модели муниципальной иерархии для уровней 1 и 2:
+
+            python manage.py fill_custom_fields --parents --levels=1,2
+
+    - Обновление всех полей name_with_typename в модели AddrObj:
+
+            python manage.py fill_custom_fields --typenames
+
+    - Обновление поля name_with_typename в модели AddrObj для объекта по guid:
+
+            python manage.py fill_custom_fields --typenames --guids_typenames=6b87470a-ac30-418b-991b-3c0d42515192
```

### Comparing `m3-gar-1.0.9/README.rst` & `m3-gar-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: m3-gar
+Version: 1.1.0
+Summary: GAR Django integration for m3
+Author: BARS Group
+Author-email: bars@bars.group
+License: MIT license
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Russian
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: Django>=3.2
+Requires-Dist: requests
+Requires-Dist: lxml
+Requires-Dist: progress
+Requires-Dist: gitpython
+Requires-Dist: twine
+Requires-Dist: asyncpg
+Requires-Dist: uvloop
+Requires-Dist: django-cte==1.1.5
+Requires-Dist: m3-gar-constants==1.0.3
+
 Приложение для работы с базой данных ГАР в Django
 
 Основные возможности
 ====================
 
 * Импорт базы ГАР из:
     * архива XML
@@ -156,15 +183,15 @@
 --commit
     запись изменений в БД, в противном случае происходит только генерация SQL-кода
 
 Полный порядок действий:
 
 1. Отключить ограничения:::
 
-        python manage.py manage_constraints disable --constraints --logged --commit
+        python manage.py manage_constraints disable --fk --unique --index --logged --commit
 
 2. Произвести загрузку общих справочников::
 
         python manage.py gar_load_data --no-truncate --no-transaction /path/to/gar_data/
 
 В директории /path/to/gar_data/ должны лежать файлы AS_*.xml из корня архива, т.е.::
 
@@ -185,15 +212,15 @@
         ...
         /path/to/gar_data/02/AS_STEADS_PARAMS_20211004_738598d9-38b0-441d-9276-c7ac7e41d606.XML
 
 4. Повторить п.3 для других регионов
 
 5. После успешной загрузки всех данных включить ограничения обратно:::
 
-        python manage.py manage_constraints enable --constraints --logged --commit
+        python manage.py manage_constraints enable --fk --unique --index --logged --commit
 
 
 Удаление данных из БД
 ----------------------
 Используется опция --truncate команды manage_constraints.
 Принимает ничего, либо список регионов, разделённых запятой.
 Для удаления данных по общим справочникам используется регион с кодом "0"
@@ -242,7 +269,43 @@
 --testmode
     Указывает полностью удалять все данные из таблицы перед импортом в неё
 
 
 Настройка settings.py
 =====================
 `GAR_DATABASE_ALIAS` - алиас БД в `DATABASES` для данных ГАР
+
+
+Заполнение полей name_with_parents в модели иерархий и полей name_with_typename в модели AddrOdj
+================================================================================================
+
+В БД были добавлены дополнительные поля name_with_parents (в модели иерархий) и name_with_typename (в модели AddrOdj).
+Для заполнения данных полей данными предоставлена команда `fill_custom_fields`
+Для нее доступны следующие параметры:
+
+--parents
+    Заполняем поля name_with_parents в модели иерархий, по умолчанию в муниципальной иерархии, можно указать ключи:
+        --adm - поля заполняются для административной иерархии
+        --guids - можно через запятую указать guid-ы объектов, для которых нужно заполнить поле
+        --levels - можно через запятую указать уровни объектов, для которых нужно заполнить поле
+
+--typenames
+    Заполняем поля name_with_typename в модели AddrOdj для уровней 7 и 8 (улицы, микрорайоны, территории и т.д.)
+        --guids_typenames - можно через запятую указать guid-ы объектов, для которых нужно заполнить поле
+
+Примеры выполнения команды:
+
+    - Обновление всех полей name_with_parents в модели муниципальной иерархии:
+
+            python manage.py fill_custom_fields --parents
+
+    - Обновление полей name_with_parents в модели муниципальной иерархии для уровней 1 и 2:
+
+            python manage.py fill_custom_fields --parents --levels=1,2
+
+    - Обновление всех полей name_with_typename в модели AddrObj:
+
+            python manage.py fill_custom_fields --typenames
+
+    - Обновление поля name_with_typename в модели AddrObj для объекта по guid:
+
+            python manage.py fill_custom_fields --typenames --guids_typenames=6b87470a-ac30-418b-991b-3c0d42515192
```

### Comparing `m3-gar-1.0.9/m3_gar/base_models.py` & `m3-gar-1.1.0/m3_gar/base_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 class AddrObj(models.Model):
     id = models.BigIntegerField(primary_key=True, verbose_name='Уникальный идентификатор записи. Ключевое поле')
     objectid = models.BigIntegerField(verbose_name='Глобальный уникальный идентификатор адресного объекта типа INTEGER')
     objectguid = models.CharField(max_length=36, verbose_name='Глобальный уникальный идентификатор адресного объекта типа UUID')
     changeid = models.BigIntegerField(verbose_name='ID изменившей транзакции')
     name = models.CharField(max_length=250, verbose_name='Наименование')
     typename = models.CharField(max_length=50, verbose_name='Краткое наименование типа объекта')
+    name_with_typename = models.CharField(
+        max_length=300,
+        verbose_name='Наименование c полным наименованием типа объекта',
+        null=True,
+    )
     level = models.CharField(max_length=10, verbose_name='Уровень адресного объекта')
     opertypeid = models.IntegerField(verbose_name='Статус действия над записью – причина появления записи')
     previd = models.BigIntegerField(verbose_name='Идентификатор записи связывания с предыдущей исторической записью', blank=True, null=True)
     nextid = models.BigIntegerField(verbose_name='Идентификатор записи связывания с последующей исторической записью', blank=True, null=True)
     updatedate = models.DateField(verbose_name='Дата внесения (обновления) записи')
     startdate = models.DateField(verbose_name='Начало действия записи')
     enddate = models.DateField(verbose_name='Окончание действия записи')
@@ -67,14 +72,15 @@
     streetcode = models.CharField(max_length=4, verbose_name='Код улицы', blank=True, null=True)
     previd = models.BigIntegerField(verbose_name='Идентификатор записи связывания с предыдущей исторической записью', blank=True, null=True)
     nextid = models.BigIntegerField(verbose_name='Идентификатор записи связывания с последующей исторической записью', blank=True, null=True)
     updatedate = models.DateField(verbose_name='Дата внесения (обновления) записи')
     startdate = models.DateField(verbose_name='Начало действия записи')
     enddate = models.DateField(verbose_name='Окончание действия записи')
     isactive = models.BooleanField(verbose_name='Признак действующего адресного объекта')
+    path = models.TextField(verbose_name='Материализованный путь к объекту (полная иерархия)', blank=True, null=True)
 
     class Meta:
         abstract = True
 
 
 class Apartments(models.Model):
     id = models.BigIntegerField(primary_key=True, verbose_name='Уникальный идентификатор записи. Ключевое поле')
@@ -187,14 +193,15 @@
     oktmo = models.CharField(max_length=11, verbose_name='Код ОКТМО', blank=True, null=True)
     previd = models.BigIntegerField(verbose_name='Идентификатор записи связывания с предыдущей исторической записью', blank=True, null=True)
     nextid = models.BigIntegerField(verbose_name='Идентификатор записи связывания с последующей исторической записью', blank=True, null=True)
     updatedate = models.DateField(verbose_name='Дата внесения (обновления) записи')
     startdate = models.DateField(verbose_name='Начало действия записи')
     enddate = models.DateField(verbose_name='Окончание действия записи')
     isactive = models.BooleanField(verbose_name='Признак действующего адресного объекта')
+    path = models.TextField(verbose_name='Материализованный путь к объекту (полная иерархия)', blank=True, null=True)
 
     class Meta:
         abstract = True
 
 
 class NormativeDocs(models.Model):
     id = models.BigIntegerField(primary_key=True, verbose_name='Уникальный идентификатор документа')
```

### Comparing `m3-gar-1.0.9/m3_gar/compat.py` & `m3-gar-1.1.0/m3_gar/compat.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/config.py` & `m3-gar-1.1.0/m3_gar/config.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/importer/commands.py` & `m3-gar-1.1.0/m3_gar/importer/commands.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,18 +3,22 @@
 import queue
 from concurrent.futures import (
     ThreadPoolExecutor,
 )
 from contextlib import (
     asynccontextmanager,
 )
+from datetime import (
+    timedelta,
+)
 from operator import (
     attrgetter,
 )
 from typing import (
+    TYPE_CHECKING,
     Optional,
 )
 
 import asyncpg
 import uvloop
 from asgiref.sync import (
     async_to_sync,
@@ -25,91 +29,97 @@
 from django.core.validators import (
     URLValidator,
 )
 from django.db import (
     models,
     transaction,
 )
-from django.db.models import (
-    Min,
+from django.utils import (
+    timezone,
 )
 
 from m3_gar import (
     config,
 )
 from m3_gar.compat import (
     nullcontext,
 )
+from m3_gar.consts import (
+    VERSION_WITHOUT_URL_TIMEOUT_HOURS,
+)
+from m3_gar.enums import (
+    VersionUpdateStatus,
+)
 from m3_gar.importer import (
     db_wrapper,
 )
 from m3_gar.importer.consts import (
     DEFAULT_BULK_LIMIT,
 )
 from m3_gar.importer.exceptions import (
     DatabaseNotEmptyError,
+    ImporterError,
+    VersionDoesNotHaveUrl,
 )
 from m3_gar.importer.loader import (
     TableUpdater,
 )
 from m3_gar.importer.signals import (
     post_import,
     post_update,
     pre_import,
     pre_update,
 )
 from m3_gar.importer.source import *
 from m3_gar.importer.source.exceptions import (
-    BadArchiveError,
     TableListLoadingError,
 )
+from m3_gar.importer.version import (
+    check_version_is_processed,
+    update_version_status,
+)
 from m3_gar.models import (
-    Status,
     Version,
 )
 from m3_gar.util import (
     get_table_names_from_models,
 )
 
 
-def get_tablelist(path, version=None, tempdir=None, for_update=False):
-
-    tablelist = None
-
-    if path is None:
-        if for_update:
-            latest_version = version
-            url_attr = 'delta_xml_url'
-        else:
-            latest_version = Version.objects.latest('dumpdate')
-            url_attr = 'complete_xml_url'
+if TYPE_CHECKING:
+    from m3_gar.importer.source.tablelist import (
+        TableList,
+    )
 
-        url = getattr(latest_version, url_attr)
 
-        tablelist = RemoteArchiveTableList(src=url, version=latest_version, tempdir=tempdir)
+def get_tablelist(
+    path: str,
+    version: Optional[Version] = None,
+    tempdir: Optional[str] = None,
+) -> 'TableList':
+    """Возвращает объект одной из реализаций TableList в зависимости от параметров."""
+    if os.path.isfile(path):
+        # Путь до файла
+        tablelist = LocalArchiveTableList(src=path, version=version, tempdir=tempdir)
+
+    elif os.path.isdir(path):
+        # Путь до директории
+        tablelist = DirectoryTableList(src=path, version=version, tempdir=tempdir)
 
     else:
-        if os.path.isfile(path):
-            tablelist = LocalArchiveTableList(src=path, version=version, tempdir=tempdir)
-
-        elif os.path.isdir(path):
-            tablelist = DirectoryTableList(src=path, version=version, tempdir=tempdir)
-
+        # Если не файл и не директория, то полагаем, что передан URL
+        try:
+            URLValidator()(path)
+        except ValidationError:
+            tablelist = None
         else:
-            try:
-                URLValidator()(path)
-            except ValidationError:
-                pass
-            else:
-                tablelist = RemoteArchiveTableList(src=path, version=version, tempdir=tempdir)
+            tablelist = RemoteArchiveTableList(src=path, version=version, tempdir=tempdir)
 
     if not tablelist:
-        raise TableListLoadingError(
-            f'Path `{path}` is not valid table list source',
-        )
+        raise TableListLoadingError(f'Путь `{path}` не является валидным источником для обновления')
 
     return tablelist
 
 
 def get_table_names(tables):
     return tables if tables else get_table_names_from_models()
 
@@ -169,23 +179,19 @@
     table_names = [
         # Пропускаем таблицы, которых нет в архиве
         tbl for tbl in table_names
         if tbl in tablelist.tables
     ]
 
     if truncate is True:
-        Status.objects.filter(table__in=table_names).delete()
+        Version.objects.update(status=VersionUpdateStatus.NEW)
 
-    if truncate is not False and Status.objects.filter(table__in=table_names).exists():
+    if truncate is not False and Version.objects.filter(processed=True).exists():
         raise DatabaseNotEmptyError()
 
-    for tbl in table_names:
-        st = Status(table=tbl, ver=tablelist.version)
-        st.save()
-
     @async_to_sync
     async def do_the_async_load():
 
         @asynccontextmanager
         async def make_conn():
             if no_transaction:
                 # Если работаем без транзакции, можно делать запросы прямо к
@@ -342,14 +348,47 @@
                 if not t.done():
                     await t
                     print(f'{i} out of {len(create_tasks)} tasks done')
 
     uvloop.install()
     do_the_async_load()
 
+    # только если path был равен None - мы имеем право зарегистрировать все версии как обработанные, потому что в этом
+    # случае автоматически разворачивается дамп с последней версии. иначе мы этого точно знать не можем, но попробуем
+    # определить версию из url (если он был передан)
+    if path:
+        error_msg = (
+            'Unknown uploaded version. Please set attribute status=VersionUpdateStatus.FINISHED to all instances of '
+            'Version model that less or equal to uploaded version yourself, or next update will be more time consuming'
+        )
+        try:
+            URLValidator()(path)
+        except ValidationError:
+            print(error_msg)
+        else:
+            try:
+                url_ver = int(path.split('/')[-2].replace('.', ''))
+
+                Version.objects.filter(
+                    ver__lte=url_ver,
+                ).exclude(
+                    status=VersionUpdateStatus.SKIPPED,
+                ).update(
+                    status=VersionUpdateStatus.FINISHED,
+                )
+            except (IndexError, ValueError):
+                print(error_msg)
+
+    else:
+        Version.objects.exclude(
+            status=VersionUpdateStatus.SKIPPED,
+        ).update(
+            status=VersionUpdateStatus.FINISHED,
+        )
+
     post_import.send(
         sender=object.__class__,
         version=tablelist.version,
     )
 
 
 def _load_rows_into_queue(tablelist, table, results):
@@ -362,106 +401,114 @@
     except Exception as e:
         put_result(e)
 
     put_result(StopIteration)
 
 
 @transaction.atomic(using=config.DATABASE_ALIAS)
-def update_data(path=None, version=None, limit=1000, tables=None, tempdir=None):
+def update_data(
+    version: Version,
+    limit: int = 1000,
+    tables: Optional[tuple[str, ...]] = None,
+    tempdir: Optional[str] = None,
+) -> None:
     """
-    Загрузка дельта-архива БД ГАР
+    Загрузка дельта-архива БД ГАР.
 
     Args:
-        path: путь на диске или URL до загруженного архива или директории с
-            распакованным архивом. Если передан None, используется URL
-            из version.
-        version (тип Version): объект версии архива. Должен быть передан, если
-            не передан path.
+        version: объект версии архива
         limit: количество записей для пакетного сохранения. Не влияет на
             обновляемые объекты.
         tables: список импортируемых таблиц. Если передан None, импортируются
             все данные
         tempdir: путь до временной директории для загрузки и распаковки архивов
-
     """
+    check_version_is_processed(version)
 
-    tablelist = get_tablelist(path=path, version=version, tempdir=tempdir, for_update=True)
+    tablelist = get_tablelist(path=version.delta_xml_url, version=version, tempdir=tempdir)
 
-    for tbl in get_table_names(tables):
+    for table_name in get_table_names(tables):
         # Пропускаем таблицы, которых нет в архиве
-        if tbl not in tablelist.tables:
+        if table_name not in tablelist.tables:
             continue
 
-        try:
-            st = Status.objects.get(table=tbl)
-        except Status.DoesNotExist:
-            st = Status()
-            st.table = tbl
-        else:
-            if st.ver.ver >= tablelist.version.ver:
-                continue
-
-        for table in tablelist.tables[tbl]:
+        for table in tablelist.tables[table_name]:
             loader = TableUpdater(limit=limit)
             loader.load(tablelist=tablelist, table=table)
 
-        st.ver = tablelist.version
-        st.save()
+    update_version_status(version, VersionUpdateStatus.FINISHED)
+
+    # удаляем временный файл с архивом обновления
+    temp_file_name = tablelist.wrapper.source.filename
+    if os.path.exists(temp_file_name):
+        os.remove(temp_file_name)
 
 
-def auto_update_data(limit=1000, tables=None, tempdir=None):
+def auto_update_data(
+    limit: int = 1000,
+    tables: Optional[tuple[str, ...]] = None,
+    tempdir: Optional[str] = None,
+    skip_versions: Optional[list[int]] = None,
+):
     """
     Последовательное обновление БД ГАР на основе текущей версии БД и известных
     новых версий с сайта ФИАС.
 
     Args:
         limit: количество записей для пакетного сохранения. Не влияет на
             обновляемые объекты.
         tables: список импортируемых таблиц. Если передан None, импортируются
             все данные
         tempdir: путь до временной директории для загрузки и распаковки архивов
-
+        skip_versions: номера версий обновлений, которые не будут выполняться и будут
+            отмечены как пропущенные
     """
+    last_processed_version = Version.objects.last_processed()
 
-    min_version = Status.objects.filter(
-        table__in=get_table_names(None),
-    ).aggregate(Min('ver'))['ver__min']
-
-    if min_version is not None:
-        min_ver = Version.objects.get(ver=min_version)
-        versions = Version.objects.filter(ver__gt=min_version).order_by('ver')
-
-        for version in versions:
-            pre_update.send(sender=object.__class__, before=min_ver, after=version)
-
-            urls = (
-                getattr(version, 'delta_xml_url'),
-                get_reserve_delta_url(version),
-            )
+    if last_processed_version is None:
+        raise TableListLoadingError('Not available. Please import the data before updating')
 
-            for url in urls:
-                try:
-                    update_data(
-                        path=url,
-                        version=version,
-                        limit=limit,
-                        tables=tables,
-                        tempdir=tempdir,
-                    )
-                except BadArchiveError:
-                    continue
-                else:
-                    break
+    skip_versions = set(skip_versions) if skip_versions is not None else set()
+
+    versions = Version.objects.filter(ver__gt=last_processed_version.ver).order_by('ver')
+
+    for version in versions:
+        pre_update.send(sender=object.__class__, before=last_processed_version, after=version)
+
+        if version.ver in skip_versions:
+            update_version_status(version, VersionUpdateStatus.SKIPPED)
+
+        elif version.delta_xml_url:
+            try:
+                update_data(
+                    version=version,
+                    limit=limit,
+                    tables=tables,
+                    tempdir=tempdir,
+                )
+            except ImporterError:
+                update_version_status(version, VersionUpdateStatus.ERROR)
+
+                raise
+        else:
+            # в версии нет ссылки на дельту
+            if timezone.now().date() < (version.dumpdate + timedelta(hours=VERSION_WITHOUT_URL_TIMEOUT_HOURS)):
+                # Время ожидания, когда ссылка для версии на сайте могла появиться ещё не прошло,
+                # поэтому вызываем ошибку обновления
+                update_version_status(version, VersionUpdateStatus.ERROR)
+
+                raise VersionDoesNotHaveUrl(f'Версия {version} не имеет ссылки на файл с дельтой!')
             else:
-                raise BadArchiveError(f'ver. {version.ver}')
+                # Время ожидания, когда ссылка для версии на сайте могла появиться уже прошло,
+                # поэтому больше не ждём и пропускаем версию
+                update_version_status(version, VersionUpdateStatus.SKIPPED)
 
-            post_update.send(sender=object.__class__, before=min_ver, after=version)
-            min_ver = version
-    else:
-        raise TableListLoadingError('Not available. Please import the data before updating')
+        post_update.send(sender=object.__class__, before=last_processed_version, after=version)
+
+        last_processed_version = version
 
 
 def get_reserve_delta_url(version):
     """
     Возвращает резервную ссылку для скачивания дельты
     """
     version_str = version.dumpdate.strftime('%Y.%m.%d')
```

### Comparing `m3-gar-1.0.9/m3_gar/importer/constraints.py` & `m3-gar-1.1.0/m3_gar/importer/constraints.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/importer/db_wrapper.py` & `m3-gar-1.1.0/m3_gar/importer/db_wrapper.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/importer/loader.py` & `m3-gar-1.1.0/m3_gar/importer/loader.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/importer/models_sort.py` & `m3-gar-1.1.0/m3_gar/importer/models_sort.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/importer/signals.py` & `m3-gar-1.1.0/m3_gar/importer/signals.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/importer/source/archive.py` & `m3-gar-1.1.0/m3_gar/importer/source/archive.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import tempfile
 import zipfile
 from urllib.error import (
     HTTPError,
+    URLError,
 )
 from urllib.request import (
     urlretrieve,
 )
 from uuid import (
     uuid4,
 )
@@ -81,15 +82,15 @@
             tmp_file = os.path.join(self.tempdir, str(uuid4()))
         else:
             tmp_file = None
 
         pre_download.send(sender=self.__class__, url=source)
         try:
             path = urlretrieve(source, reporthook=update_progress, filename=tmp_file)[0]
-        except HTTPError as e:
+        except (HTTPError, URLError) as e:
             raise RetrieveError(
                 f'Can not download data archive at url `{source}`. '
                 f'Error occurred: "{e}"'
             )
         progress.finish()
         post_download.send(sender=self.__class__, url=source, path=path)
```

### Comparing `m3-gar-1.0.9/m3_gar/importer/source/exceptions.py` & `m3-gar-1.1.0/m3_gar/importer/source/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 )
 
 
 class TableListLoadingError(ImporterError):
     pass
 
 
+class NoNewVersionError(ImporterError):
+    pass
+
+
 class BadArchiveError(TableListLoadingError):
 
     def __init__(self, source, *args):
         super().__init__(
             f'Archive: `{source}` corrupted or is not archive',
             *args,
         )
```

### Comparing `m3-gar-1.0.9/m3_gar/importer/source/tablelist.py` & `m3-gar-1.1.0/m3_gar/importer/source/tablelist.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from typing import (
+    TYPE_CHECKING,
+)
+
 from m3_gar.importer.signals import (
     post_load,
     pre_load,
 )
 from m3_gar.importer.source.wrapper import (
     SourceWrapper,
 )
@@ -9,14 +13,20 @@
     TableFactory,
 )
 from m3_gar.models import (
     Version,
 )
 
 
+if TYPE_CHECKING:
+    from m3_gar.importer.table import (
+        XMLTable,
+    )
+
+
 class TableList:
     """
     Базовый класс для работы с набором импортируемых файлов
     """
 
     wrapper_class = SourceWrapper
     wrapper = None
@@ -42,15 +52,15 @@
     def load_data(self, source):
         return self.wrapper_class(source=source)
 
     def get_table_list(self):
         return self.wrapper.get_file_list()
 
     @property
-    def tables(self):
+    def tables(self) -> dict[str, list['XMLTable']]:
         if self.table_list is None:
             self.table_list = {}
             for filename in self.get_table_list():
                 table = TableFactory.parse(filename=filename)
                 if table is None:
                     continue
                 self.table_list.setdefault(table.name, []).append(table)
```

### Comparing `m3-gar-1.0.9/m3_gar/importer/source/wrapper.py` & `m3-gar-1.1.0/m3_gar/importer/source/wrapper.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/importer/table/__init__.py` & `m3-gar-1.1.0/m3_gar/importer/table/__init__.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/importer/table/table.py` & `m3-gar-1.1.0/m3_gar/importer/table/table.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/importer/table/xml.py` & `m3-gar-1.1.0/m3_gar/importer/table/xml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from datetime import (
     date,
 )
-
 from django.db import (
     models,
 )
 from django.db.models import (
     UUIDField,
 )
+from html import (
+    unescape,
+)
 from lxml import (
     etree,
 )
 
 from m3_gar.importer.table import (
     BadTableError,
 )
@@ -43,14 +45,16 @@
                     value = int(value) if value else None
                 if field.null and (not value or value == '0'):
                     value = None
             elif isinstance(field, models.BooleanField):
                 value = value in ['1', 'true', True]
             elif isinstance(field, models.IntegerField):
                 value = int(value) if value else None
+            else:
+                value = ' '.join(unescape(value).strip().replace('\n', ' ').replace('\r', ' ').split())
 
             yield key, value
 
     def get_next(self):
         event, row = next(self._context)
 
         if row.getparent() is None:
```

### Comparing `m3-gar-1.0.9/m3_gar/importer/timer.py` & `m3-gar-1.1.0/m3_gar/importer/timer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from django.dispatch import (
     receiver,
 )
 from django.utils import (
     timezone,
 )
 
+from m3_gar.enums import (
+    VersionUpdateStatus,
+)
 from m3_gar.importer.signals import (
     post_download,
     post_fetch_version,
     post_import,
     post_import_table,
     post_load,
     post_unpack,
@@ -123,15 +126,21 @@
 def pre_update_callback(sender, before, after, **kwargs):
     print(f'Updating from v.{before.ver} to v.{after.ver} started at {timezone.now()}')
 
 
 @receiver(post_update)
 def post_update_callback(sender, before, after, **kwargs):
     time = timezone.now()
-    print(f'Data v.{before.ver} is updated to v.{after.ver} at {time}')
-    print(
-        f'Download: {Timer.unpack or 0}. '
-        f'Unpack: {time - Timer.load}. '
-        f'Import: {time - Timer.start}. '
-        f'Total time: {Timer.download or 0}.'
-    )
+
+    if after.status == VersionUpdateStatus.FINISHED:
+        print(f'Data v.{before.ver} is updated to v.{after.ver} at {time}')
+        print(
+            f'Download: {Timer.unpack or 0}. '
+            f'Unpack: {time - Timer.load}. '
+            f'Import: {time - Timer.start}. '
+            f'Total time: {Timer.download or 0}.'
+        )
+
+    elif after.status == VersionUpdateStatus.SKIPPED:
+        print(f'Data v.{after.ver} was skipped!')
+
     Timer.reset_counters()
```

### Comparing `m3-gar-1.0.9/m3_gar/management/commands/gar_check_models.py` & `m3-gar-1.1.0/m3_gar/management/commands/gar_check_models.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/management/commands/gar_generate_base_models.py` & `m3-gar-1.1.0/m3_gar/management/commands/gar_generate_base_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,17 @@
                 f.write(f'{line}\n')
 
     def get_field_type(self, connection, table_name, row):
         field_type, field_params, field_notes = super().get_field_type(
             connection, table_name, row)
         field_params['verbose_name'] = row.description
 
+        if field_type == 'CharField' and 'max_length' not in field_params:
+            field_type = 'TextField'
+
         return field_type, field_params, field_notes
 
     def get_meta(self, table_name, constraints, column_to_field_name, is_view, is_partition):
         result = super().get_meta(
             table_name, constraints, column_to_field_name, is_view, is_partition)
 
         for index, row in enumerate(result):
```

### Comparing `m3-gar-1.0.9/m3_gar/management/commands/gar_load_data.py` & `m3-gar-1.1.0/m3_gar/management/commands/gar_load_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import os
 from argparse import (
     BooleanOptionalAction,
 )
+from typing import (
+    Optional,
+)
 
 from django.conf import (
     settings,
 )
 from django.core.management import (
     BaseCommand,
     CommandError,
@@ -17,22 +20,25 @@
 from m3_gar.importer.commands import (
     auto_update_data,
     load_complete_data,
 )
 from m3_gar.importer.consts import (
     DEFAULT_BULK_LIMIT,
 )
+from m3_gar.importer.exceptions import (
+    ImporterError,
+)
 from m3_gar.importer.timer import (
     Timer,
 )
 from m3_gar.importer.version import (
     fetch_version_info,
 )
 from m3_gar.models import (
-    Status,
+    Version,
 )
 from m3_gar.util import (
     get_table_names_from_models,
 )
 
 
 class Command(BaseCommand):
@@ -81,38 +87,45 @@
             default=True,
             help='Update list of available database versions from http://fias.nalog.ru',
         )
         parser.add_argument(
             '--tempdir',
             help="Path to the temporary files directory"
         )
+        parser.add_argument(
+            '--skip-versions',
+            type=int,
+            nargs='*',
+            help='Номера версий обновлений, которые не будут выполняться',
+        )
 
     def handle(
         self, *args,
         src,
         truncate,
         no_transaction,
         update,
         limit,
         tables,
         update_version_info,
         tempdir,
+        skip_versions,
         **options,
     ):
         Timer.init()
 
         # признак обновления из внешнего источника
         remote = False
         if src and src.lower() == 'auto':
             src = None
             remote = True
 
         tempdir = self.parse_tempdir_arg(tempdir)
 
-        if (src or remote) and Status.objects.exists() and truncate is None:
+        if (src or remote) and Version.objects.filter(processed=True).exists() and truncate is None:
             self.stderr.write(
                 'One of the tables contains data. '
                 'Truncate all GAR tables manually or use '
                 '--truncate/--no-truncate option'
             )
 
             raise CommandError
@@ -133,19 +146,23 @@
                 no_transaction=no_transaction,
                 limit=limit,
                 tables=tables,
                 tempdir=tempdir,
             )
 
         if update:
-            auto_update_data(
-                limit=limit,
-                tables=tables,
-                tempdir=tempdir,
-            )
+            try:
+                auto_update_data(
+                    limit=limit,
+                    tables=tables,
+                    tempdir=tempdir,
+                    skip_versions=skip_versions,
+                )
+            except ImporterError as e:
+                self.stdout.write(str(e))
 
     def parse_tempdir_arg(self, tempdir):
         """
         Возвращает временную директорую
         """
         if tempdir:
             error = None
@@ -160,25 +177,25 @@
             if error:
                 self.stderr.write(error)
 
                 raise CommandError
 
         return tempdir
 
-    def parse_tables_arg(self, tables):
+    def parse_tables_arg(self, tables: Optional[str]) -> tuple[str, ...]:
         """
-        Возвращает перечень таблиц для загрузки
+        Возвращает перечень таблиц для загрузки.
         """
         tables = set(tables.split(',')) if tables else set()
         tables_from_db = get_table_names_from_models()
 
         if not tables.issubset(set(tables_from_db)):
             diff = ', '.join(tables.difference(tables_from_db))
             self.stderr.write(
                 f'Tables `{diff}` are not of GAR schema models and can not be processed'
             )
 
             raise CommandError
 
-        tables = tuple(x for x in tables_from_db if x in list(tables))
+        tables = [x for x in tables_from_db if x in tables]
 
-        return tables
+        return tuple(tables)
```

### Comparing `m3-gar-1.0.9/m3_gar/management/commands/gar_update_schema.py` & `m3-gar-1.1.0/m3_gar/management/commands/gar_update_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,60 +52,64 @@
             help=(
                 'Тестовый режим - пуш будет сделан в отдельную ветку, '
                 'пакет релизнется на тестовом PyPi. '
                 'Для включения нужно добавить флаг --testmode'
             ),
         )
 
-    def handle(self, *args, url, path, testmode):
+    def handle(
+        self,
+        *args,
+        url,
+        path,
+        testmode,
+        **options,
+    ):
         try:
             if url and path or not (url or path):
                 raise PublisherError('Необходимо указать или url, или path!')
 
             self.stdout.write('Запуск обновления пакета по схемам ГАР')
 
             repo_manager = RepoManager(testmode)
             repo = repo_manager.repo
 
-            self.stdout.write('1/8 Получение схем...')
+            self.stdout.write('1/7 Получение схем...')
             if url:
                 gar_schema_manager = DownloadGARSchemaManager(url, repo)
 
             elif path:
                 gar_schema_manager = ArchiveGARSchemaManager(path, repo)
 
             gar_schema_manager.process_schemas()
             if not gar_schema_manager.has_schema_changes():
                 # по схемам не было изменений, прекращаем работу
                 raise PublisherError('Изменения в формате ГАР не найдены')
 
-            self.stdout.write('2/8 Генерация моделей...')
+            self.stdout.write('2/7 Генерация моделей...')
             call_command(
                 'gar_generate_base_models',
                 dst=settings.GAR_BASE_DIR / 'base_models.py',
             )
 
-            self.stdout.write('3/8 Проверка моделей...')
+            self.stdout.write('3/7 Проверка моделей...')
             call_command('gar_check_models')
 
-            self.stdout.write('4/8 Создание и применение миграций...')
+            self.stdout.write('4/7 Создание и применение миграций...')
             call_command('makemigrations', 'm3_gar')
             call_command('migrate', 'm3_gar')
 
-            self.stdout.write('5/8 Добавление новых файлов в репозиторий...')
+            self.stdout.write('5/7 Добавление новых файлов в репозиторий...')
             repo_manager.index_add()
 
-            self.stdout.write('6/8 Обновление версии и лога изменений...')
+            self.stdout.write('6/7 Обновление версии и лога изменений...')
             preparer = ReleasePreparer()
             preparer.prepare()
             new_version = preparer.new_version_str
 
-            self.stdout.write('7/8 Обновление репозитория...')
+            self.stdout.write('7/7 Обновление репозитория...')
             repo_manager.save_changes(new_version)
 
-            self.stdout.write('8/8 Релиз нового пакета...')
-            Releaser(new_version, testmode).release()
-
-            self.stdout.write('Обновление пакета по новым схемам ГАР выполнено успешно')
+            self.stdout.write('Обновление репозитория новыми схемами ГАР выполнено успешно')
 
         except PublisherError as e:
             self.stderr.write(str(e))
```

### Comparing `m3-gar-1.0.9/m3_gar/management/commands/manage_constraints.py` & `m3-gar-1.1.0/m3_gar/management/commands/manage_constraints.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/migrations/0001_initial.py` & `m3-gar-1.1.0/m3_gar/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/migrations/0002_auto_20210707_1352.py` & `m3-gar-1.1.0/m3_gar/migrations/0002_auto_20210707_1352.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/migrations/0003_auto_20210906_0744.py` & `m3-gar-1.1.0/m3_gar/migrations/0003_auto_20210906_0744.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/migrations/0004_auto_20211013_1106.py` & `m3-gar-1.1.0/m3_gar/migrations/0004_auto_20211013_1106.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/migrations/0005_auto_20211029_1212.py` & `m3-gar-1.1.0/m3_gar/migrations/0005_auto_20211029_1212.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/models/carplace.py` & `m3-gar-1.1.0/m3_gar/models/carplace.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/models/house.py` & `m3-gar-1.1.0/m3_gar/models/house.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from django.contrib.postgres.indexes import (
+    HashIndex,
+)
+
 from m3_gar.base_models import (
     Houses as BaseHouses,
     HouseTypes as BaseHouseTypes,
 )
 from m3_gar.models.op_type import (
     OperationTypes,
 )
@@ -43,14 +47,19 @@
 
     level = 10
 
     class Meta:
         verbose_name = 'Номер дома'
         verbose_name_plural = 'Номера домов'
 
+        indexes = (
+            HashIndex(
+                fields=('objectguid',),
+            ),
+        )
 
 make_fk(Houses, 'housetype', to=HouseTypes, null=True, blank=True)
 make_fk(Houses, 'addtype1', to=AddhouseTypes, null=True, blank=True)
 make_fk(Houses, 'addtype2', to=AddhouseTypes, null=True, blank=True)
 make_fk(Houses, 'opertypeid', to=OperationTypes)
 make_fk(Houses, 'objectid', to=ReestrObjects)
```

### Comparing `m3-gar-1.0.9/m3_gar/models/param.py` & `m3-gar-1.1.0/m3_gar/models/param.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/models/reestr.py` & `m3-gar-1.1.0/m3_gar/models/reestr.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/models/room.py` & `m3-gar-1.1.0/m3_gar/models/room.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/models/stead.py` & `m3-gar-1.1.0/m3_gar/models/stead.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/publish_tools.py` & `m3-gar-1.1.0/m3_gar/publish_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import datetime
 import fileinput
 import io
 import os
-import re
 from io import (
     BytesIO,
 )
 from shutil import (
     rmtree,
 )
 from zipfile import (
@@ -28,15 +27,15 @@
     main,
 )
 
 from m3_gar.exceptions import (
     PublisherError,
 )
 from setup_kwargs import (
-    setup_kwargs,
+    make_setup_kwargs,
 )
 
 
 class GARSchemaManager:
     """
     Базовый класс, отвечающий за получение схем ГАР
     """
@@ -211,24 +210,26 @@
 
         self.repo.index.add(map(str, files_to_add))
 
     def save_changes(self, new_version):
         """
         Сохраняет изменения в пакете путем коммита и пуша
         """
-        origin = self.repo.remote()
-        push_args = [origin, self.repo.head.ref]
+        push_args = []
+
         if self.test_mode:
             # в этом случае создадим новую ветку по названию версии
             # и закоммитим туда, а не в мастер
             new_branch_name = f'test-patch-{new_version}'
             new_branch = self.repo.create_head(new_branch_name)
             new_branch.checkout()
 
-            push_args = ['--set-upstream'] + push_args
+            push_args.append('--set-upstream')
+
+        push_args.extend([self.repo.remote(), self.repo.head.ref])
 
         self.repo.git.commit(
             '-a',
             '-m',
             f'Автогенерация патча {new_version} по обновлению формата ГАР',
         )
         self.repo.git.push(*push_args)
@@ -275,24 +276,28 @@
         Создает новую запись в чейнжлоге о текущей версии
         """
         if not self.new_version_str:
             return
 
         today = datetime.date.today()
         today_str = today.strftime('%Y.%m.%d')
+        log_entry_text = (
+            f'**{self.new_version_str}**\n'
+            f'- Автогенерируемый патч по обновлению формата ГАР ({today_str})\n'
+        )
 
         with io.open(self.changelog_file, 'r+', encoding='utf-8') as changelog_file:
             content = changelog_file.read()
-            changelog_file.seek(0, 0)
 
-            changelog_file.write(f'{today_str} v.{self.new_version_str}\n')
-            changelog_file.write('\n')
-            changelog_file.write('* Автогенерируемый патч по обновлению формата ГАР\n')
-            changelog_file.write('\n')
+        content = content.split('\n', 2)
+        content.insert(-1, log_entry_text)
+        content = '\n'.join(content)
 
+        with io.open(self.changelog_file, 'w', encoding='utf-8') as changelog_file:
+            changelog_file.seek(0, 0)
             changelog_file.write(content)
 
 
 class Releaser:
     """
     Класс, отвечающий за создание и выпуск пакета
     """
@@ -312,35 +317,34 @@
         finally:
             self._clear_build_folder()
 
     def _build_dist(self):
         """
         Создание пакета
         """
-        new_setup_kwargs = setup_kwargs.copy()
-        new_setup_kwargs.update({
-            'version': self.new_version,
-            'script_name': 'setup.py',
-            'script_args': ['sdist', 'bdist_wheel'],
-        })
-
         cwd = os.getcwd()
-        os.chdir(settings.BASE_DIR.parent)
+        os.chdir(settings.GAR_BASE_DIR.parent)
 
         try:
+            new_setup_kwargs = make_setup_kwargs()
+            new_setup_kwargs.update({
+                'version': self.new_version,
+                'script_name': 'setup.py',
+                'script_args': ['sdist', 'bdist_wheel'],
+            })
             setup(**new_setup_kwargs)
         finally:
             os.chdir(cwd)
 
     def _clear_build_folder(self):
         """
         Очистка после билда пакета
         """
-        rmtree(settings.BASE_DIR / 'build')
-        rmtree(settings.BASE_DIR / 'dist')
+        rmtree(settings.GAR_BASE_DIR.parent / 'build')
+        rmtree(settings.GAR_BASE_DIR.parent / 'dist')
 
     def _publish(self):
         """
         Загрузка пакета на pypi
         Для получения логина-пароля используется файл ~/.pypirc, там должен
         быть указан адрес до pypi под категорией pypi,
         и адрес до тестового pypi под категорией testpypi, если нужно
@@ -349,13 +353,13 @@
         pypirc_config = ['-r', 'pypi']
         if self.test_mode:
             pypirc_config = ['-r', 'testpypi']
 
         args = pypirc_config + ['dist/*']
 
         cwd = os.getcwd()
-        os.chdir(settings.BASE_DIR.parent)
+        os.chdir(settings.GAR_BASE_DIR.parent)
 
         try:
             main(args)
         finally:
             os.chdir(cwd)
```

### Comparing `m3-gar-1.0.9/m3_gar/routers.py` & `m3-gar-1.1.0/m3_gar/routers.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/util.py` & `m3-gar-1.1.0/m3_gar/util.py`

 * *Files identical despite different names*

### Comparing `m3-gar-1.0.9/m3_gar/xsd_generator/base.py` & `m3-gar-1.1.0/m3_gar/xsd_generator/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,25 @@
 import re
-from importlib import (
-    import_module,
-)
 from os import (
     listdir,
 )
 
-from django.apps import (
-    apps,
-)
 from django.conf import (
     settings,
 )
-from django.core.exceptions import (
-    ImproperlyConfigured,
-)
 from django.db.backends.base.base import (
     BaseDatabaseWrapper,
 )
 from django.db.backends.base.introspection import (
     BaseDatabaseIntrospection,
 )
 from lxml import (
     etree,
 )
 
-from m3_gar.exceptions import (
-    PublisherError,
-)
-
 
 def get_by_xpath(element, xpath):
     """
     Возвращает все объекты по xpath
     """
     return element.xpath(
         xpath,
@@ -66,14 +53,15 @@
         3: 'internal_size',
         4: 'precision',
         5: 'scale',
         6: 'null_ok',
         7: 'default',
         8: 'collation',
         9: 'description',
+        10: 'path',
     }
 
     def __init__(self, element):
         super().__init__()
 
         self.name = element.get('name', '').lower()
         self.type_code = None
@@ -104,18 +92,24 @@
                         self,
                         attr_name,
                         convertor(
                             attr_element.get('value')
                         ),
                     )
 
-        self.type_code = self.type_code.replace(f'{element.prefix}:', '')
+        if self.type_code:
+            self.type_code = self.type_code.replace(f'{element.prefix}:', '')
+
+            if self.name in ['isactive', 'isactual'] and self.type_code == 'integer':
+                self.type_code = 'boolean'
 
-        if self.name in ['isactive', 'isactual'] and self.type_code == 'integer':
-            self.type_code = 'boolean'
+        else:
+            self.type_code = 'string'
+            self.null_ok = True
+            self.default = ''
 
     def __getitem__(self, i):
         return getattr(self, self.indexes[i])
 
 
 class XSDObject:
     """
@@ -176,15 +170,17 @@
 
     def __init__(self, folder_path):
         super().__init__()
 
         self.files = {}
 
         files = [
-            f for f in listdir(folder_path) if (folder_path / f).is_file()
+            f for f
+            in listdir(folder_path)
+            if (folder_path / f).is_file() and f.endswith('.xsd')
         ]
 
         for file_ in files:
             xsd_obj = XSDObject(folder_path, file_)
             self.files[xsd_obj.name] = xsd_obj
 
     def get_files_list(self):
```

### Comparing `m3-gar-1.0.9/m3_gar.egg-info/PKG-INFO` & `m3-gar-1.1.0/m3_gar.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 Metadata-Version: 2.1
 Name: m3-gar
-Version: 1.0.9
+Version: 1.1.0
 Summary: GAR Django integration for m3
-Home-page: UNKNOWN
 Author: BARS Group
 Author-email: bars@bars.group
 License: MIT license
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Russian
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: Django>=3.2
+Requires-Dist: requests
+Requires-Dist: lxml
+Requires-Dist: progress
+Requires-Dist: gitpython
+Requires-Dist: twine
+Requires-Dist: asyncpg
+Requires-Dist: uvloop
+Requires-Dist: django-cte==1.1.5
+Requires-Dist: m3-gar-constants==1.0.3
 
 Приложение для работы с базой данных ГАР в Django
 
 Основные возможности
 ====================
 
 * Импорт базы ГАР из:
@@ -175,15 +183,15 @@
 --commit
     запись изменений в БД, в противном случае происходит только генерация SQL-кода
 
 Полный порядок действий:
 
 1. Отключить ограничения:::
 
-        python manage.py manage_constraints disable --constraints --logged --commit
+        python manage.py manage_constraints disable --fk --unique --index --logged --commit
 
 2. Произвести загрузку общих справочников::
 
         python manage.py gar_load_data --no-truncate --no-transaction /path/to/gar_data/
 
 В директории /path/to/gar_data/ должны лежать файлы AS_*.xml из корня архива, т.е.::
 
@@ -204,15 +212,15 @@
         ...
         /path/to/gar_data/02/AS_STEADS_PARAMS_20211004_738598d9-38b0-441d-9276-c7ac7e41d606.XML
 
 4. Повторить п.3 для других регионов
 
 5. После успешной загрузки всех данных включить ограничения обратно:::
 
-        python manage.py manage_constraints enable --constraints --logged --commit
+        python manage.py manage_constraints enable --fk --unique --index --logged --commit
 
 
 Удаление данных из БД
 ----------------------
 Используется опция --truncate команды manage_constraints.
 Принимает ничего, либо список регионов, разделённых запятой.
 Для удаления данных по общим справочникам используется регион с кодом "0"
@@ -263,7 +271,41 @@
 
 
 Настройка settings.py
 =====================
 `GAR_DATABASE_ALIAS` - алиас БД в `DATABASES` для данных ГАР
 
 
+Заполнение полей name_with_parents в модели иерархий и полей name_with_typename в модели AddrOdj
+================================================================================================
+
+В БД были добавлены дополнительные поля name_with_parents (в модели иерархий) и name_with_typename (в модели AddrOdj).
+Для заполнения данных полей данными предоставлена команда `fill_custom_fields`
+Для нее доступны следующие параметры:
+
+--parents
+    Заполняем поля name_with_parents в модели иерархий, по умолчанию в муниципальной иерархии, можно указать ключи:
+        --adm - поля заполняются для административной иерархии
+        --guids - можно через запятую указать guid-ы объектов, для которых нужно заполнить поле
+        --levels - можно через запятую указать уровни объектов, для которых нужно заполнить поле
+
+--typenames
+    Заполняем поля name_with_typename в модели AddrOdj для уровней 7 и 8 (улицы, микрорайоны, территории и т.д.)
+        --guids_typenames - можно через запятую указать guid-ы объектов, для которых нужно заполнить поле
+
+Примеры выполнения команды:
+
+    - Обновление всех полей name_with_parents в модели муниципальной иерархии:
+
+            python manage.py fill_custom_fields --parents
+
+    - Обновление полей name_with_parents в модели муниципальной иерархии для уровней 1 и 2:
+
+            python manage.py fill_custom_fields --parents --levels=1,2
+
+    - Обновление всех полей name_with_typename в модели AddrObj:
+
+            python manage.py fill_custom_fields --typenames
+
+    - Обновление поля name_with_typename в модели AddrObj для объекта по guid:
+
+            python manage.py fill_custom_fields --typenames --guids_typenames=6b87470a-ac30-418b-991b-3c0d42515192
```

### Comparing `m3-gar-1.0.9/m3_gar.egg-info/SOURCES.txt` & `m3-gar-1.1.0/m3_gar.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 README.rst
 setup.py
 setup_kwargs.py
 m3_gar/__init__.py
 m3_gar/base_models.py
 m3_gar/compat.py
 m3_gar/config.py
+m3_gar/consts.py
+m3_gar/enums.py
 m3_gar/exceptions.py
 m3_gar/publish_tools.py
 m3_gar/routers.py
 m3_gar/util.py
 m3_gar/version.py
 m3_gar.egg-info/PKG-INFO
 m3_gar.egg-info/SOURCES.txt
@@ -37,32 +39,50 @@
 m3_gar/importer/table/__init__.py
 m3_gar/importer/table/consts.py
 m3_gar/importer/table/exceptions.py
 m3_gar/importer/table/table.py
 m3_gar/importer/table/xml.py
 m3_gar/management/__init__.py
 m3_gar/management/commands/__init__.py
+m3_gar/management/commands/fill_custom_fields.py
 m3_gar/management/commands/gar_check_models.py
 m3_gar/management/commands/gar_generate_base_models.py
 m3_gar/management/commands/gar_load_data.py
 m3_gar/management/commands/gar_update_schema.py
 m3_gar/management/commands/manage_constraints.py
 m3_gar/migrations/0001_initial.py
 m3_gar/migrations/0002_auto_20210707_1352.py
 m3_gar/migrations/0003_auto_20210906_0744.py
 m3_gar/migrations/0004_auto_20211013_1106.py
 m3_gar/migrations/0005_auto_20211029_1212.py
+m3_gar/migrations/0006_auto_20211105_0937.py
+m3_gar/migrations/0007_version_processed.py
+m3_gar/migrations/0008_auto_20220217_0556.py
+m3_gar/migrations/0009_delete_status.py
+m3_gar/migrations/0010_auto_20220225_0934.py
+m3_gar/migrations/0011_auto_20220323_1022.py
+m3_gar/migrations/0012_auto_20220415_1452.py
+m3_gar/migrations/0013_auto_20220513_0825.py
+m3_gar/migrations/0014_addrobj_name_with_typename.py
+m3_gar/migrations/0015_alter_normativedocs_orgname.py
+m3_gar/migrations/0016_alter_normativedocs_orgname.py
+m3_gar/migrations/0017_apartments_m3_gar_apar_objectg_0e459a_hash.py
+m3_gar/migrations/0018_addrobj_addrobj_name_with_typename_gin.py
+m3_gar/migrations/0019_version_status.py
+m3_gar/migrations/0020_update_version_status.py
+m3_gar/migrations/0021_remove_version_processed.py
 m3_gar/migrations/__init__.py
 m3_gar/models/__init__.py
 m3_gar/models/addrobj.py
 m3_gar/models/apartment.py
 m3_gar/models/carplace.py
 m3_gar/models/hierarchy.py
 m3_gar/models/history.py
 m3_gar/models/house.py
+m3_gar/models/indexes.py
 m3_gar/models/normdoc.py
 m3_gar/models/op_type.py
 m3_gar/models/param.py
 m3_gar/models/reestr.py
 m3_gar/models/room.py
 m3_gar/models/stead.py
 m3_gar/models/util.py
```

### Comparing `m3-gar-1.0.9/setup_kwargs.py` & `m3-gar-1.1.0/setup_kwargs.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,39 +12,42 @@
 )
 
 
 def read(fn):
     return codecs.open(Path(__file__).resolve().parent / fn).read()
 
 
-setup_kwargs = dict(
-    name='m3-gar',
-    version=__version__,
-    author='BARS Group',
-    author_email='bars@bars.group',
-    description='GAR Django integration for m3',
-    long_description=read('README.rst'),
-    license='MIT license',
-    install_requires=[
-        'Django>=3.2',
-        'requests',
-        'lxml',
-        'progress',
-        'gitpython',
-        'twine',
-        'asyncpg',
-        'uvloop',
-    ],
-    packages=find_packages(exclude=['tests', 'test_project']),
-    include_package_data=True,
-    classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Developers',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: Russian',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.9',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-    ],
-)
+def make_setup_kwargs():
+    return dict(
+        name='m3-gar',
+        version=__version__,
+        author='BARS Group',
+        author_email='bars@bars.group',
+        description='GAR Django integration for m3',
+        long_description=read('README.rst'),
+        license='MIT license',
+        install_requires=[
+            'Django>=3.2',
+            'requests',
+            'lxml',
+            'progress',
+            'gitpython',
+            'twine',
+            'asyncpg',
+            'uvloop',
+            'django-cte==1.1.5',
+            'm3-gar-constants==1.0.3',
+        ],
+        packages=find_packages(exclude=['tests', 'test_project']),
+        include_package_data=True,
+        classifiers=[
+            'Development Status :: 4 - Beta',
+            'Intended Audience :: Developers',
+            'Intended Audience :: Science/Research',
+            'License :: OSI Approved :: MIT License',
+            'Natural Language :: Russian',
+            'Programming Language :: Python',
+            'Programming Language :: Python :: 3',
+            'Programming Language :: Python :: 3.9',
+            'Topic :: Software Development :: Libraries :: Python Modules',
+        ],
+    )
```

