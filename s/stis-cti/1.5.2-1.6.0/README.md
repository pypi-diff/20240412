# Comparing `tmp/stis_cti-1.5.2.tar.gz` & `tmp/stis_cti-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stis_cti-1.5.2.tar", last modified: Tue Mar  5 17:55:35 2024, max compression
+gzip compressed data, was "stis_cti-1.6.0.tar", last modified: Fri Apr 12 15:24:51 2024, max compression
```

## Comparing `stis_cti-1.5.2.tar` & `stis_cti-1.6.0.tar`

### file list

```diff
@@ -1,42 +1,38 @@
-drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-03-05 17:55:35.132540 stis_cti-1.5.2/
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      108 2020-12-15 11:24:35.000000 stis_cti-1.5.2/.gitattributes
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)       50 2021-07-27 15:04:12.000000 stis_cti-1.5.2/.gitignore
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     1464 2020-12-15 11:24:35.000000 stis_cti-1.5.2/LICENSE.txt
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      306 2020-12-15 11:24:35.000000 stis_cti-1.5.2/MANIFEST.in
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     2459 2024-03-05 17:55:35.132392 stis_cti-1.5.2/PKG-INFO
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     1154 2024-03-05 17:37:38.000000 stis_cti-1.5.2/README.rst
-drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-03-05 17:55:35.129047 stis_cti-1.5.2/doc/
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     6770 2020-12-15 11:24:35.000000 stis_cti-1.5.2/doc/Makefile
-drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-03-05 17:55:35.129218 stis_cti-1.5.2/doc/_templates/
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      487 2020-12-15 11:24:35.000000 stis_cti-1.5.2/doc/_templates/layout.html
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    10828 2024-03-05 17:55:11.000000 stis_cti-1.5.2/doc/conf.py
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      344 2024-03-01 19:23:31.000000 stis_cti-1.5.2/doc/index.rst
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     6705 2020-12-15 11:24:35.000000 stis_cti-1.5.2/doc/make.bat
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)  1108934 2020-12-15 11:24:35.000000 stis_cti-1.5.2/doc/obr101010_comparison.png
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      943 2020-12-15 11:24:35.000000 stis_cti-1.5.2/doc/obr101010_comparison.pro
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     5748 2024-03-01 21:43:38.000000 stis_cti-1.5.2/doc/qsg.rst
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    20298 2024-03-05 17:55:11.000000 stis_cti-1.5.2/doc/readme.rst
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      621 2024-03-01 19:23:45.000000 stis_cti-1.5.2/doc/stis_cti.rst
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)       38 2024-03-05 17:55:35.132591 stis_cti-1.5.2/setup.cfg
--rwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)     2379 2024-03-05 17:55:11.000000 stis_cti-1.5.2/setup.py
-drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-03-05 17:55:35.129938 stis_cti-1.5.2/src/
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    11110 2020-12-15 11:24:35.000000 stis_cti-1.5.2/src/StisFixYCte.c
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     2759 2020-12-15 11:24:35.000000 stis_cti-1.5.2/src/StisPixCteCorr.h
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    13400 2020-12-15 11:24:35.000000 stis_cti-1.5.2/src/StisPixCteCorr_funcs.c
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    15113 2021-07-27 15:04:12.000000 stis_cti-1.5.2/src/StisPixCte_FixY.c
-drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-03-05 17:55:35.131036 stis_cti-1.5.2/stis_cti/
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    33710 2024-02-26 20:40:16.000000 stis_cti-1.5.2/stis_cti/StisPixCteCorr.py
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      437 2021-07-27 15:04:12.000000 stis_cti-1.5.2/stis_cti/__init__.py
--rwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)    13815 2024-02-26 22:03:22.000000 stis_cti-1.5.2/stis_cti/archive_dark_query.py
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     3378 2021-07-27 15:04:12.000000 stis_cti-1.5.2/stis_cti/custom_superdark_info.py
-drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-03-05 17:55:35.132138 stis_cti-1.5.2/stis_cti/data/
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    51840 2020-12-15 11:24:35.000000 stis_cti-1.5.2/stis_cti/data/a01_stis_pcte.fits
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    58980 2024-03-05 17:55:11.000000 stis_cti-1.5.2/stis_cti/stis_cti.py
--rwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)    21193 2021-07-27 15:04:12.000000 stis_cti-1.5.2/stis_cti/unit_tests.py
-drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-03-05 17:55:35.131981 stis_cti-1.5.2/stis_cti.egg-info/
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     2459 2024-03-05 17:55:35.000000 stis_cti-1.5.2/stis_cti.egg-info/PKG-INFO
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      722 2024-03-05 17:55:35.000000 stis_cti-1.5.2/stis_cti.egg-info/SOURCES.txt
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)        1 2024-03-05 17:55:35.000000 stis_cti-1.5.2/stis_cti.egg-info/dependency_links.txt
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      134 2024-03-05 17:55:35.000000 stis_cti-1.5.2/stis_cti.egg-info/entry_points.txt
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)       88 2024-03-05 17:55:35.000000 stis_cti-1.5.2/stis_cti.egg-info/requires.txt
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)        9 2024-03-05 17:55:35.000000 stis_cti-1.5.2/stis_cti.egg-info/top_level.txt
+drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-04-12 15:24:51.330191 stis_cti-1.6.0/
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     1464 2020-12-15 11:24:35.000000 stis_cti-1.6.0/LICENSE.txt
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      306 2020-12-15 11:24:35.000000 stis_cti-1.6.0/MANIFEST.in
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     2459 2024-04-12 15:24:51.330021 stis_cti-1.6.0/PKG-INFO
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     1154 2024-03-05 17:37:38.000000 stis_cti-1.6.0/README.rst
+drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-04-12 15:24:51.323955 stis_cti-1.6.0/doc/
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     6770 2020-12-15 11:24:35.000000 stis_cti-1.6.0/doc/Makefile
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    10828 2024-04-12 15:21:44.000000 stis_cti-1.6.0/doc/conf.py
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      344 2024-03-01 19:23:31.000000 stis_cti-1.6.0/doc/index.rst
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     6705 2020-12-15 11:24:35.000000 stis_cti-1.6.0/doc/make.bat
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)  1108934 2020-12-15 11:24:35.000000 stis_cti-1.6.0/doc/obr101010_comparison.png
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     5748 2024-03-01 21:43:38.000000 stis_cti-1.6.0/doc/qsg.rst
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    20583 2024-04-12 15:21:44.000000 stis_cti-1.6.0/doc/readme.rst
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      621 2024-03-01 19:23:45.000000 stis_cti-1.6.0/doc/stis_cti.rst
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)       38 2024-04-12 15:24:51.330242 stis_cti-1.6.0/setup.cfg
+-rwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)     2378 2024-04-12 15:21:44.000000 stis_cti-1.6.0/setup.py
+drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-04-12 15:24:51.325096 stis_cti-1.6.0/src/
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    11110 2020-12-15 11:24:35.000000 stis_cti-1.6.0/src/StisFixYCte.c
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     2759 2020-12-15 11:24:35.000000 stis_cti-1.6.0/src/StisPixCteCorr.h
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    13400 2020-12-15 11:24:35.000000 stis_cti-1.6.0/src/StisPixCteCorr_funcs.c
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    15113 2021-07-27 15:04:12.000000 stis_cti-1.6.0/src/StisPixCte_FixY.c
+drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-04-12 15:24:51.326862 stis_cti-1.6.0/stis_cti/
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    33710 2024-02-26 20:40:16.000000 stis_cti-1.6.0/stis_cti/StisPixCteCorr.py
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      437 2021-07-27 15:04:12.000000 stis_cti-1.6.0/stis_cti/__init__.py
+-rwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)    13815 2024-02-26 22:03:22.000000 stis_cti-1.6.0/stis_cti/archive_dark_query.py
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     3378 2021-07-27 15:04:12.000000 stis_cti-1.6.0/stis_cti/custom_superdark_info.py
+drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-04-12 15:24:51.329111 stis_cti-1.6.0/stis_cti/data/
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    51840 2020-12-15 11:24:35.000000 stis_cti-1.6.0/stis_cti/data/a01_stis_pcte.fits
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    51840 2024-04-12 15:21:44.000000 stis_cti-1.6.0/stis_cti/data/a02_stis_pcte.fits
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    58980 2024-04-12 15:21:44.000000 stis_cti-1.6.0/stis_cti/stis_cti.py
+-rwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)    21193 2021-07-27 15:04:12.000000 stis_cti-1.6.0/stis_cti/unit_tests.py
+drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-04-12 15:24:51.328142 stis_cti-1.6.0/stis_cti.egg-info/
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     2459 2024-04-12 15:24:51.000000 stis_cti-1.6.0/stis_cti.egg-info/PKG-INFO
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      673 2024-04-12 15:24:51.000000 stis_cti-1.6.0/stis_cti.egg-info/SOURCES.txt
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)        1 2024-04-12 15:24:51.000000 stis_cti-1.6.0/stis_cti.egg-info/dependency_links.txt
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      134 2024-04-12 15:24:51.000000 stis_cti-1.6.0/stis_cti.egg-info/entry_points.txt
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)       88 2024-04-12 15:24:51.000000 stis_cti-1.6.0/stis_cti.egg-info/requires.txt
+-rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)        9 2024-04-12 15:24:51.000000 stis_cti-1.6.0/stis_cti.egg-info/top_level.txt
```

### Comparing `stis_cti-1.5.2/LICENSE.txt` & `stis_cti-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/PKG-INFO` & `stis_cti-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stis_cti
-Version: 1.5.2
+Version: 1.6.0
 Summary: Pixel-based CTI-correction for HST/STIS CCD data
 Home-page: https://www.stsci.edu/hst/instrumentation/stis/data-analysis-and-software-tools/pixel-based-cti
 Author: Sean Lockwood, Phil Hodge, Pey Lian Lim, W.J. Hack, J. Anderson, Matt Davis
 Author-email: lockwood@stsci.edu
 Maintainer: Sean Lockwood
 Maintainer-email: lockwood@stsci.edu
 License: BSD-new
```

### Comparing `stis_cti-1.5.2/README.rst` & `stis_cti-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/doc/Makefile` & `stis_cti-1.6.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/doc/conf.py` & `stis_cti-1.6.0/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,17 @@
 copyright = '2015, AURA-STScI'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '1.5.2'
+version = '1.6.0'
 # The full version, including alpha/beta/rc tags.
-release = '1.5.2'
+release = '1.6.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `stis_cti-1.5.2/doc/make.bat` & `stis_cti-1.6.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/doc/obr101010_comparison.png` & `stis_cti-1.6.0/doc/obr101010_comparison.png`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/doc/qsg.rst` & `stis_cti-1.6.0/doc/qsg.rst`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/doc/readme.rst` & `stis_cti-1.6.0/doc/readme.rst`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     --clean           remove intermediate and final products from previous runs
                       of this script ('*.txt' files are skipped and clobbered)
     --clean_all       '--clean' + remove previous super-darks and CTI-corrected
                       component darks
     --ignore_missing  process data even with an incomplete set of dark FLTs
     -v VERBOSE_LEVEL  verbosity ({0,1,2}; default=1)
 
-  Written by Sean Lockwood; v1.5.2
+  Written by Sean Lockwood; v1.6.0
 
 The script is designed to run the pixel-based correction in parallel on the component 
 darks, and in parallel on the science files.  The maximum number of processes may be 
 specified via the ``-n #`` option.
 
 A typical call looks like::
 
@@ -389,14 +389,18 @@
 ============
 
 .. Warning::
    If you use ``stistools.x1d.x1d()`` to manually extract your spectra, we recommend using 
    the argument ``ctecorr="OMIT"`` for pixel-based CTI-corrected data to avoid applying 
    the empirical flux correction on already-corrected data.
 
+- ``stis_cti <= 1.5.2`` fails to process data taken after MJD 60000 (2023-February-25) 
+  due to a hard-coded date in the PCTETAB = ``a01_stis_pcte.fits``.  This date has been 
+  corrected in the new default PCTETAB = ``a02_stis_pcte.fits`` (v0.2) available in ``stis_cti >= 1.6.0``.
+
 - The ``--crds_update`` option breaks with ``CRDS v7.0.10``.  Please use a more recent 
   version.
 
 - Some annealing months contain non-standard amplifier=A dark files (typical 
   observations are taken with amp=D).  These files do not produce ``FLT`` files in the
   Archive, but are still expected by ``stis_cti`` (even though they are excluded from any 
   amp=D super-darks).  As of ``v1.1``, users may bypass the missing file check by specifying
```

### Comparing `stis_cti-1.5.2/doc/stis_cti.rst` & `stis_cti-1.6.0/doc/stis_cti.rst`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/setup.py` & `stis_cti-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! /usr/bin/env python
+#!/usr/bin/env python
 
 from setuptools import setup, Extension
 import os
 import numpy
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'README.rst')) as f:
@@ -17,15 +17,15 @@
     url = 'https://www.stsci.edu/hst/instrumentation/stis/data-analysis-and-software-tools/pixel-based-cti',
     project_urls={
         'Homepage': 'https://www.stsci.edu/hst/instrumentation/stis/data-analysis-and-software-tools/pixel-based-cti',
         'Documentation': 'https://stis-cti.readthedocs.io',
         'Help Desk': 'https://hsthelp.stsci.edu',
         'Source Code': 'https://github.com/spacetelescope/stis_cti',
         'Issues': 'https://github.com/spacetelescope/stis_cti/issues',},
-    version = '1.5.2',
+    version = '1.6.0',
     description = 'Pixel-based CTI-correction for HST/STIS CCD data',
     long_description = long_description,
     author = 'Sean Lockwood, Phil Hodge, Pey Lian Lim, W.J. Hack, J. Anderson, Matt Davis',
     author_email = 'lockwood@stsci.edu',
     maintainer = 'Sean Lockwood',
     maintainer_email = 'lockwood@stsci.edu',
     license = 'BSD-new',
```

### Comparing `stis_cti-1.5.2/src/StisFixYCte.c` & `stis_cti-1.6.0/src/StisFixYCte.c`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/src/StisPixCteCorr.h` & `stis_cti-1.6.0/src/StisPixCteCorr.h`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/src/StisPixCteCorr_funcs.c` & `stis_cti-1.6.0/src/StisPixCteCorr_funcs.c`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/src/StisPixCte_FixY.c` & `stis_cti-1.6.0/src/StisPixCte_FixY.c`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/stis_cti/StisPixCteCorr.py` & `stis_cti-1.6.0/stis_cti/StisPixCteCorr.py`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/stis_cti/archive_dark_query.py` & `stis_cti-1.6.0/stis_cti/archive_dark_query.py`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/stis_cti/custom_superdark_info.py` & `stis_cti-1.6.0/stis_cti/custom_superdark_info.py`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/stis_cti/data/a01_stis_pcte.fits` & `stis_cti-1.6.0/stis_cti/data/a01_stis_pcte.fits`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/stis_cti/stis_cti.py` & `stis_cti-1.6.0/stis_cti/stis_cti.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from . import archive_dark_query
 from . import StisPixCteCorr
 from crds.bestrefs import BestrefsScript
 from multiprocessing import cpu_count
 
 
 __author__  = 'Sean Lockwood'
-__version__ = '1.5.2'
+__version__ = '1.6.0'
 
 crds_server_url = 'https://hst-crds.stsci.edu'
 
 class FileError(Exception):
     pass
 
 class VersionError(Exception):
```

### Comparing `stis_cti-1.5.2/stis_cti/unit_tests.py` & `stis_cti-1.6.0/stis_cti/unit_tests.py`

 * *Files identical despite different names*

### Comparing `stis_cti-1.5.2/stis_cti.egg-info/PKG-INFO` & `stis_cti-1.6.0/stis_cti.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stis-cti
-Version: 1.5.2
+Version: 1.6.0
 Summary: Pixel-based CTI-correction for HST/STIS CCD data
 Home-page: https://www.stsci.edu/hst/instrumentation/stis/data-analysis-and-software-tools/pixel-based-cti
 Author: Sean Lockwood, Phil Hodge, Pey Lian Lim, W.J. Hack, J. Anderson, Matt Davis
 Author-email: lockwood@stsci.edu
 Maintainer: Sean Lockwood
 Maintainer-email: lockwood@stsci.edu
 License: BSD-new
```

### Comparing `stis_cti-1.5.2/stis_cti.egg-info/SOURCES.txt` & `stis_cti-1.6.0/stis_cti.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-.gitattributes
-.gitignore
 LICENSE.txt
 MANIFEST.in
 README.rst
 setup.py
 doc/Makefile
 doc/conf.py
 doc/index.rst
 doc/make.bat
 doc/obr101010_comparison.png
-doc/obr101010_comparison.pro
 doc/qsg.rst
 doc/readme.rst
 doc/stis_cti.rst
-doc/_templates/layout.html
 src/StisFixYCte.c
 src/StisPixCteCorr.h
 src/StisPixCteCorr_funcs.c
 src/StisPixCte_FixY.c
 stis_cti/StisPixCteCorr.py
 stis_cti/__init__.py
 stis_cti/archive_dark_query.py
@@ -26,8 +22,9 @@
 stis_cti/unit_tests.py
 stis_cti.egg-info/PKG-INFO
 stis_cti.egg-info/SOURCES.txt
 stis_cti.egg-info/dependency_links.txt
 stis_cti.egg-info/entry_points.txt
 stis_cti.egg-info/requires.txt
 stis_cti.egg-info/top_level.txt
-stis_cti/data/a01_stis_pcte.fits
+stis_cti/data/a01_stis_pcte.fits
+stis_cti/data/a02_stis_pcte.fits
```

