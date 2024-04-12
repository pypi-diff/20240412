# Comparing `tmp/fgtools-2.1.8.tar.gz` & `tmp/fgtools-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgtools-2.1.8.tar", last modified: Sat Nov 11 00:11:05 2023, max compression
+gzip compressed data, was "fgtools-2.1.9.tar", last modified: Sat Nov 11 02:26:16 2023, max compression
```

## Comparing `fgtools-2.1.8.tar` & `fgtools-2.1.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 00:11:05.358247 fgtools-2.1.8/
--rwxrwxr-x   0 frederic  (1000) frederic  (1000)    35149 2022-08-13 11:54:59.000000 fgtools-2.1.8/LICENSE
--rw-r--r--   0 frederic  (1000) frederic  (1000)     2091 2023-11-11 00:11:05.358247 fgtools-2.1.8/PKG-INFO
--rwxrwxr-x   0 frederic  (1000) frederic  (1000)     1376 2023-04-15 10:35:34.000000 fgtools-2.1.8/README.md
-drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 00:11:05.239246 fgtools-2.1.8/fgtools/
--rwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2022-08-13 11:54:59.000000 fgtools-2.1.8/fgtools/__init__.py
-drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 00:11:05.245246 fgtools-2.1.8/fgtools/aircraft/
--rw-rw-r--   0 frederic  (1000) frederic  (1000)        0 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/aircraft/__init__.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     3885 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/aircraft/javaprop2jsbcpct.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     7604 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/aircraft/vsphist2jsbtable.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     7697 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/aircraft/vspstab2jsbtable.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)    19285 2023-11-08 02:01:01.000000 fgtools-2.1.8/fgtools/aptdat.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)    26403 2023-07-26 19:58:07.000000 fgtools-2.1.8/fgtools/btg.py
--rwxrwxr-x   0 frederic  (1000) frederic  (1000)    34716 2022-08-13 11:55:00.000000 fgtools-2.1.8/fgtools/dsf2stg_lookup.py
--rwxrwxr-x   0 frederic  (1000) frederic  (1000)      807 2022-08-13 11:55:00.000000 fgtools-2.1.8/fgtools/fgelev.py
-drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 00:11:05.265246 fgtools-2.1.8/fgtools/geo/
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     4440 2023-11-10 14:30:25.000000 fgtools-2.1.8/fgtools/geo/__init__.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     4333 2023-09-25 21:32:35.000000 fgtools-2.1.8/fgtools/geo/coord.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     2937 2023-11-10 12:19:45.000000 fgtools-2.1.8/fgtools/geo/rectangle.py
-drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 00:11:05.268246 fgtools-2.1.8/fgtools/math/
--rw-rw-r--   0 frederic  (1000) frederic  (1000)      503 2023-09-25 21:32:35.000000 fgtools-2.1.8/fgtools/math/__init__.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)      505 2022-09-09 15:38:42.000000 fgtools-2.1.8/fgtools/math/coord.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)      748 2023-09-25 21:32:35.000000 fgtools-2.1.8/fgtools/math/rectangle.py
-drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 00:11:05.273246 fgtools-2.1.8/fgtools/misc/
--rw-rw-r--   0 frederic  (1000) frederic  (1000)        0 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/misc/__init__.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)      978 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/misc/coord_converter.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     2124 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/misc/scrape_emanualonline.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     3286 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/misc/scrape_scribd.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     4197 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/misc/tabletool.py
-drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 00:11:05.288246 fgtools-2.1.8/fgtools/scenery/
--rw-rw-r--   0 frederic  (1000) frederic  (1000)        0 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/scenery/__init__.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)    16110 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/scenery/aptdat2airportsxml.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     3570 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/scenery/create_day_night_xml.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     4920 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/scenery/dsftxt2stg.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     7006 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/scenery/edit_stg.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     5431 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/scenery/fix_aptdat_icaos.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)    31739 2023-11-09 17:31:39.000000 fgtools-2.1.8/fgtools/scenery/genws20.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)    19247 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/scenery/osm2aptdat.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     5712 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/scenery/osmconf.ini
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     4881 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/scenery/pull_xplane_aptdat.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     5140 2023-11-07 14:40:46.000000 fgtools-2.1.8/fgtools/scenery/stg2ufo.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     9177 2023-11-09 23:26:35.000000 fgtools-2.1.8/fgtools/scenery/ungap_btg.py
-drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 00:11:05.355247 fgtools-2.1.8/fgtools/utils/
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     3372 2023-11-10 11:57:47.000000 fgtools-2.1.8/fgtools/utils/__init__.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     2456 2023-07-23 23:28:58.000000 fgtools-2.1.8/fgtools/utils/binary.py
--rwxrwxr-x   0 frederic  (1000) frederic  (1000)      385 2023-11-10 11:57:04.000000 fgtools-2.1.8/fgtools/utils/constants.py
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     2700 2023-09-25 21:32:35.000000 fgtools-2.1.8/fgtools/utils/files.py
--rwxrwxr-x   0 frederic  (1000) frederic  (1000)     3204 2022-09-20 15:46:33.000000 fgtools-2.1.8/fgtools/utils/interpolator.py
--rwxrwxr-x   0 frederic  (1000) frederic  (1000)      133 2022-08-13 11:55:01.000000 fgtools-2.1.8/fgtools/utils/unit_convert.py
-drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 00:11:05.242246 fgtools-2.1.8/fgtools.egg-info/
--rw-r--r--   0 frederic  (1000) frederic  (1000)     2091 2023-11-11 00:11:04.000000 fgtools-2.1.8/fgtools.egg-info/PKG-INFO
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     1299 2023-11-11 00:11:04.000000 fgtools-2.1.8/fgtools.egg-info/SOURCES.txt
--rw-rw-r--   0 frederic  (1000) frederic  (1000)        1 2023-11-11 00:11:04.000000 fgtools-2.1.8/fgtools.egg-info/dependency_links.txt
--rw-rw-r--   0 frederic  (1000) frederic  (1000)      890 2023-11-11 00:11:04.000000 fgtools-2.1.8/fgtools.egg-info/entry_points.txt
--rw-rw-r--   0 frederic  (1000) frederic  (1000)       96 2023-11-11 00:11:04.000000 fgtools-2.1.8/fgtools.egg-info/requires.txt
--rw-rw-r--   0 frederic  (1000) frederic  (1000)        8 2023-11-11 00:11:04.000000 fgtools-2.1.8/fgtools.egg-info/top_level.txt
--rw-rw-r--   0 frederic  (1000) frederic  (1000)       81 2023-11-07 14:40:46.000000 fgtools-2.1.8/pyproject.toml
--rw-rw-r--   0 frederic  (1000) frederic  (1000)     1717 2023-11-11 00:11:05.360247 fgtools-2.1.8/setup.cfg
+drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 02:26:16.025906 fgtools-2.1.9/
+-rwxrwxr-x   0 frederic  (1000) frederic  (1000)    35149 2022-08-13 11:54:59.000000 fgtools-2.1.9/LICENSE
+-rw-r--r--   0 frederic  (1000) frederic  (1000)     2091 2023-11-11 02:26:16.025906 fgtools-2.1.9/PKG-INFO
+-rwxrwxr-x   0 frederic  (1000) frederic  (1000)     1376 2023-04-15 10:35:34.000000 fgtools-2.1.9/README.md
+drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 02:26:15.902905 fgtools-2.1.9/fgtools/
+-rwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2022-08-13 11:54:59.000000 fgtools-2.1.9/fgtools/__init__.py
+drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 02:26:15.909905 fgtools-2.1.9/fgtools/aircraft/
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)        0 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/aircraft/__init__.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     3885 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/aircraft/javaprop2jsbcpct.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     7604 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/aircraft/vsphist2jsbtable.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     7697 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/aircraft/vspstab2jsbtable.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)    19285 2023-11-08 02:01:01.000000 fgtools-2.1.9/fgtools/aptdat.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)    26403 2023-07-26 19:58:07.000000 fgtools-2.1.9/fgtools/btg.py
+-rwxrwxr-x   0 frederic  (1000) frederic  (1000)    34716 2022-08-13 11:55:00.000000 fgtools-2.1.9/fgtools/dsf2stg_lookup.py
+-rwxrwxr-x   0 frederic  (1000) frederic  (1000)      807 2022-08-13 11:55:00.000000 fgtools-2.1.9/fgtools/fgelev.py
+drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 02:26:15.918905 fgtools-2.1.9/fgtools/geo/
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     4409 2023-11-11 02:19:03.000000 fgtools-2.1.9/fgtools/geo/__init__.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     4333 2023-09-25 21:32:35.000000 fgtools-2.1.9/fgtools/geo/coord.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     2894 2023-11-11 02:18:59.000000 fgtools-2.1.9/fgtools/geo/rectangle.py
+drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 02:26:15.938905 fgtools-2.1.9/fgtools/math/
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)      503 2023-09-25 21:32:35.000000 fgtools-2.1.9/fgtools/math/__init__.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)      505 2022-09-09 15:38:42.000000 fgtools-2.1.9/fgtools/math/coord.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)      748 2023-09-25 21:32:35.000000 fgtools-2.1.9/fgtools/math/rectangle.py
+drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 02:26:15.942905 fgtools-2.1.9/fgtools/misc/
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)        0 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/misc/__init__.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)      978 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/misc/coord_converter.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     2124 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/misc/scrape_emanualonline.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     3286 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/misc/scrape_scribd.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     4197 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/misc/tabletool.py
+drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 02:26:15.974906 fgtools-2.1.9/fgtools/scenery/
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)        0 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/scenery/__init__.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)    16110 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/scenery/aptdat2airportsxml.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     3570 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/scenery/create_day_night_xml.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     4920 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/scenery/dsftxt2stg.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     7006 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/scenery/edit_stg.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     5431 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/scenery/fix_aptdat_icaos.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)    31739 2023-11-09 17:31:39.000000 fgtools-2.1.9/fgtools/scenery/genws20.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)    19247 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/scenery/osm2aptdat.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     5712 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/scenery/osmconf.ini
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     4881 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/scenery/pull_xplane_aptdat.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     5140 2023-11-07 14:40:46.000000 fgtools-2.1.9/fgtools/scenery/stg2ufo.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     9687 2023-11-11 02:19:55.000000 fgtools-2.1.9/fgtools/scenery/ungap_btg.py
+drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 02:26:16.023906 fgtools-2.1.9/fgtools/utils/
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     3372 2023-11-10 11:57:47.000000 fgtools-2.1.9/fgtools/utils/__init__.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     2456 2023-07-23 23:28:58.000000 fgtools-2.1.9/fgtools/utils/binary.py
+-rwxrwxr-x   0 frederic  (1000) frederic  (1000)      385 2023-11-10 11:57:04.000000 fgtools-2.1.9/fgtools/utils/constants.py
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     2700 2023-09-25 21:32:35.000000 fgtools-2.1.9/fgtools/utils/files.py
+-rwxrwxr-x   0 frederic  (1000) frederic  (1000)     3204 2022-09-20 15:46:33.000000 fgtools-2.1.9/fgtools/utils/interpolator.py
+-rwxrwxr-x   0 frederic  (1000) frederic  (1000)      133 2022-08-13 11:55:01.000000 fgtools-2.1.9/fgtools/utils/unit_convert.py
+drwxrwxr-x   0 frederic  (1000) frederic  (1000)        0 2023-11-11 02:26:15.906905 fgtools-2.1.9/fgtools.egg-info/
+-rw-r--r--   0 frederic  (1000) frederic  (1000)     2091 2023-11-11 02:26:15.000000 fgtools-2.1.9/fgtools.egg-info/PKG-INFO
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     1299 2023-11-11 02:26:15.000000 fgtools-2.1.9/fgtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)        1 2023-11-11 02:26:15.000000 fgtools-2.1.9/fgtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)      890 2023-11-11 02:26:15.000000 fgtools-2.1.9/fgtools.egg-info/entry_points.txt
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)       96 2023-11-11 02:26:15.000000 fgtools-2.1.9/fgtools.egg-info/requires.txt
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)        8 2023-11-11 02:26:15.000000 fgtools-2.1.9/fgtools.egg-info/top_level.txt
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)       81 2023-11-07 14:40:46.000000 fgtools-2.1.9/pyproject.toml
+-rw-rw-r--   0 frederic  (1000) frederic  (1000)     1717 2023-11-11 02:26:16.027906 fgtools-2.1.9/setup.cfg
```

### Comparing `fgtools-2.1.8/LICENSE` & `fgtools-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/PKG-INFO` & `fgtools-2.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgtools
-Version: 2.1.8
+Version: 2.1.9
 Summary: Tools for FlightGear scenery generation and aircraft development
 Home-page: https://github.com/TheFGFSEagle/fgtools
 Author: TheFGFSEagle
 Author-email: thefgfseagle@gmail.com
 License: GPLv3
 Project-URL: Homepage, https://github.com/TheFGFSEagle/fgtools
 Project-URL: Bug Tracker, https://github.com/TheFGFSEagle/fgtools/issues
```

### Comparing `fgtools-2.1.8/README.md` & `fgtools-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/aircraft/javaprop2jsbcpct.py` & `fgtools-2.1.9/fgtools/aircraft/javaprop2jsbcpct.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/aircraft/vsphist2jsbtable.py` & `fgtools-2.1.9/fgtools/aircraft/vsphist2jsbtable.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/aircraft/vspstab2jsbtable.py` & `fgtools-2.1.9/fgtools/aircraft/vspstab2jsbtable.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/aptdat.py` & `fgtools-2.1.9/fgtools/aptdat.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/btg.py` & `fgtools-2.1.9/fgtools/btg.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/dsf2stg_lookup.py` & `fgtools-2.1.9/fgtools/dsf2stg_lookup.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/fgelev.py` & `fgtools-2.1.9/fgtools/fgelev.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/geo/__init__.py` & `fgtools-2.1.9/fgtools/geo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,17 +162,14 @@
 		for lon in range(bbox.left, bbox.right - get_fg_tile_span(lat), get_fg_tile_span(lat)):
 			tiles.append(get_fg_tile_index(lon, lat))
 	
 	return tiles
 
 def get_fg_tile_paths(bbox: Rectangle) -> list[str]:
 	bbox = Rectangle(bbox)
-	print()
-	print(bbox)
-	print()
 	bbox.set_left(fgmath.floor(bbox.left, get_fg_tile_span(max(abs(bbox.top), abs(bbox.bottom)))))
 	bbox.set_right(fgmath.ceil(bbox.right, get_fg_tile_span(max(abs(bbox.top), abs(bbox.bottom)))))
 	bbox.set_bottom(fgmath.floor(bbox.bottom, 0.125))
 	bbox.set_top(fgmath.ceil(bbox.top, 0.125))
 	
 	paths = []
 	for lat in range(bbox.bottom, bbox.top - 0.125, 0.125):
```

### Comparing `fgtools-2.1.8/fgtools/geo/coord.py` & `fgtools-2.1.9/fgtools/geo/coord.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/geo/rectangle.py` & `fgtools-2.1.9/fgtools/geo/rectangle.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,14 @@
 		self.right = other.right
 		self.bottom = other.bottom
 	
 	def __iter__(self):
 		return iter([self.ll, self.ul, self.ur, self.ul])
 	
 	def __repr__(self):
-		print(dir(self))
-		print(dir(Rectangle))
 		return f"Rectangle(left={self.left}, top={self.top}, right={self.right}, bottom={self.bottom})"
 	
 	def set_left(self, left: float):
 		self.left = left
 		self.ll.lon = left
 		self.ul.lon = left
```

### Comparing `fgtools-2.1.8/fgtools/math/rectangle.py` & `fgtools-2.1.9/fgtools/math/rectangle.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/misc/coord_converter.py` & `fgtools-2.1.9/fgtools/misc/coord_converter.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/misc/scrape_emanualonline.py` & `fgtools-2.1.9/fgtools/misc/scrape_emanualonline.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/misc/scrape_scribd.py` & `fgtools-2.1.9/fgtools/misc/scrape_scribd.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/misc/tabletool.py` & `fgtools-2.1.9/fgtools/misc/tabletool.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/scenery/aptdat2airportsxml.py` & `fgtools-2.1.9/fgtools/scenery/aptdat2airportsxml.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/scenery/create_day_night_xml.py` & `fgtools-2.1.9/fgtools/scenery/create_day_night_xml.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/scenery/dsftxt2stg.py` & `fgtools-2.1.9/fgtools/scenery/dsftxt2stg.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/scenery/edit_stg.py` & `fgtools-2.1.9/fgtools/scenery/edit_stg.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/scenery/fix_aptdat_icaos.py` & `fgtools-2.1.9/fgtools/scenery/fix_aptdat_icaos.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/scenery/genws20.py` & `fgtools-2.1.9/fgtools/scenery/genws20.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/scenery/osm2aptdat.py` & `fgtools-2.1.9/fgtools/scenery/osm2aptdat.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/scenery/osmconf.ini` & `fgtools-2.1.9/fgtools/scenery/osmconf.ini`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/scenery/pull_xplane_aptdat.py` & `fgtools-2.1.9/fgtools/scenery/pull_xplane_aptdat.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/scenery/stg2ufo.py` & `fgtools-2.1.9/fgtools/scenery/stg2ufo.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/scenery/ungap_btg.py` & `fgtools-2.1.9/fgtools/scenery/ungap_btg.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 
 VERTEX_DISTANCE_MAX_DEG = 0.000001
 
 def create_border_data(tile_index: int, btg_file: str):
 	print("\nCreating border data")
 	tile_rect = get_fg_tile_bbox(tile_index)
 	border_data = {edge: list() for edge in "nesw"}
+	if not os.path.isfile(btg_file):
+		# assume ocean tile, return None so that in process_btg_file the altitude of the vertices wont be changed
+		return None
+	
 	btg_object = btg.ReaderWriterBTG(btg_file)
 	for v in btg_object.vertex_list.elements[0].items:
 		if math.dist(v.coord.lon, tile_rect.left) < VERTEX_DISTANCE_MAX_DEG:
 			border_data["e"].append(v.coord)
 		if math.dist(v.coord.lon, tile_rect.right) < VERTEX_DISTANCE_MAX_DEG:
 			border_data["w"].append(v.coord)
 		if math.dist(v.coord.lat, tile_rect.bottom) < VERTEX_DISTANCE_MAX_DEG:
@@ -46,31 +50,34 @@
 			if parts[0] in "nesw":
 				cur_side = parts[0]
 			else:
 				border_data[cur_side].append(Coord(float(parts[0]), float(parts[1]), float(parts[2])))
 	
 	return border_data
 
-def write_border_data(border_file: str, border_data: typing.Mapping[str, typing.Iterable[Coord]]):
+def write_border_data(border_file: str, border_data: typing.Optional[typing.Mapping[str, typing.Iterable[Coord]]]):
+	if not border_data:
+		return
+	 
 	os.makedirs(os.path.dirname(border_file), exist_ok=True)
 	with open(border_file, "w") as f:
 		for side in "nesw":
 			f.write(side + "\n")
 			for c in border_data[side]:
 				f.write(" ".join(map(str, [c.lon, c.lat, c.alt])) + "\n")
 
 def get_border_data(tile_index: int, terrain_dir: str, border_dir: str):
 	tile_path = get_fg_tile_path(tile_index)
 	btg_file = os.path.join(terrain_dir, tile_path + ".btg.gz")
 	if border_dir == "terrain-dir":
-		border_dir == terrain_dir
+		border_dir = terrain_dir
 	border_file = ""
 	if border_dir != "direct":
 		border_file = os.path.join(border_dir, tile_path) + "_edges.dat"
-		if os.path.exists(border_file) and os.path.getmtime(border_file) > os.path.getmtime(btg_file):
+		if os.path.isfile(border_file) and os.path.getmtime(border_file) > os.path.getmtime(btg_file):
 			return read_border_data(border_file)
 	
 	border_data = create_border_data(tile_index, btg_file)
 	if border_dir != "direct":
 		write_border_data(border_file, border_data)
 	return border_data
 
@@ -91,14 +98,16 @@
 		sibling_indices[side] = get_fg_tile_index(sibling_coords[side].lon, sibling_coords[side].lat)
 	del sibling_coords
 
 	sibling_borders = {}
 	for i, side in enumerate(sibling_indices):
 		padded_print(f"Processing BTG file {nth_input + 1} of {total} ({tile_path}) - Getting border data for neighbor BTG files ({i} of {len(sibling_indices)})", end="\r")
 		border_data = get_border_data(sibling_indices[side], terrain_dir, border_dir)
+		if not border_data:
+			sibling_borders[side] = None
 		if side == "n":
 			border_data = border_data["s"]
 		elif side == "e":
 			border_data = border_data["w"]
 		elif side == "s":
 			border_data = border_data["n"]
 		elif side == "w":
@@ -106,14 +115,16 @@
 		sibling_borders[side] = border_data
 	padded_print(f"Processing BTG file {nth_input + 1} of {total} ({tile_path}) - Getting border data for neighbor BTG files ({len(sibling_indices)} of {len(sibling_indices)})", end="\r")
 	del sibling_indices
 	
 	sibling_border_interpolators = {}
 	for i, side in enumerate(sibling_borders):
 		padded_print(f"Processing BTG file {nth_input + 1} of {total} ({tile_path}) - Creating interpolation tables for border data ({i} of {len(sibling_borders)})", end="\r")
+		if not sibling_borders[side]:
+			sibling_border_interpolators[side] = None
 		sibling_border_interpolator = Interpolator()
 		if side in "ns":
 			attrib = "lon"
 		else:
 			attrib = "lat"
 		
 		for coord in sibling_borders[side]:
@@ -143,21 +154,25 @@
 	
 	for i, (obj_index, tri_index) in enumerate(tri_indices_to_process):
 		padded_print(f"Processing BTG file {nth_input + 1} of {total} ({tile_path}) - Fixing triangles ({i} of {len(tri_indices_to_process)})", end="\r")
 		tri = btg_object.triangle_faces[obj_index].elements[tri_index]
 		for vi in tri.vertex_indices:
 			v = btg_object.vertex_list.elements[0].items[vi]
 			if math.dist(v.coord.lon, tile_rect.left) < VERTEX_DISTANCE_MAX_DEG:
-				v.coord.alt = sibling_border_interpolators["e"].interpolate(v.coord.lat)
+				if sibling_border_interpolators["e"]:
+					v.coord.alt = sibling_border_interpolators["e"].interpolate(v.coord.lat)
 			elif math.dist(v.coord.lon, tile_rect.right) < VERTEX_DISTANCE_MAX_DEG:
-				v.coord.alt = sibling_border_interpolators["w"].interpolate(v.coord.lat)
+				if sibling_border_interpolators["w"]:
+					v.coord.alt = sibling_border_interpolators["w"].interpolate(v.coord.lat)
 			elif math.dist(v.coord.lat, tile_rect.bottom) < VERTEX_DISTANCE_MAX_DEG:
-				v.coord.alt = sibling_border_interpolators["s"].interpolate(v.coord.lon)
+				if sibling_border_interpolators["s"]:
+					v.coord.alt = sibling_border_interpolators["s"].interpolate(v.coord.lon)
 			elif math.dist(v.coord.lat, tile_rect.top) < VERTEX_DISTANCE_MAX_DEG:
-				v.coord.alt = sibling_border_interpolators["n"].interpolate(v.coord.lon)
+				if sibling_border_interpolators["n"]:
+					v.coord.alt = sibling_border_interpolators["n"].interpolate(v.coord.lon)
 	padded_print(f"Processing BTG file {nth_input + 1} of {total} ({tile_path}) - Fixing triangles ({len(tri_indices_to_process)} of {len(tri_indices_to_process)})", end="\r")
 	
 	padded_print(f"Processing BTG file {nth_input + 1} of {total} ({tile_path}) - Writing processed BTG file")
 	center = Coord.from_cartesian(btg_object.bs.elements[0].x, btg_object.bs.elements[0].y, btg_object.bs.elements[0].z)
 	btg_object.write(tile_path)
 
 def map_border_data_dir(value):
```

### Comparing `fgtools-2.1.8/fgtools/utils/__init__.py` & `fgtools-2.1.9/fgtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/utils/binary.py` & `fgtools-2.1.9/fgtools/utils/binary.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/utils/files.py` & `fgtools-2.1.9/fgtools/utils/files.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools/utils/interpolator.py` & `fgtools-2.1.9/fgtools/utils/interpolator.py`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools.egg-info/PKG-INFO` & `fgtools-2.1.9/fgtools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgtools
-Version: 2.1.8
+Version: 2.1.9
 Summary: Tools for FlightGear scenery generation and aircraft development
 Home-page: https://github.com/TheFGFSEagle/fgtools
 Author: TheFGFSEagle
 Author-email: thefgfseagle@gmail.com
 License: GPLv3
 Project-URL: Homepage, https://github.com/TheFGFSEagle/fgtools
 Project-URL: Bug Tracker, https://github.com/TheFGFSEagle/fgtools/issues
```

### Comparing `fgtools-2.1.8/fgtools.egg-info/SOURCES.txt` & `fgtools-2.1.9/fgtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/fgtools.egg-info/entry_points.txt` & `fgtools-2.1.9/fgtools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `fgtools-2.1.8/setup.cfg` & `fgtools-2.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fgtools
-version = 2.1.8
+version = 2.1.9
 description = Tools for FlightGear scenery generation and aircraft development
 author = TheFGFSEagle
 author_email = thefgfseagle@gmail.com
 long_description_content_type = text/markdown
 long_description = file: README.md
 keywords = flightgear
 license = GPLv3
```

