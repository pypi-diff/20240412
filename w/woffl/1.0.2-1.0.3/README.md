# Comparing `tmp/woffl-1.0.2.tar.gz` & `tmp/woffl-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woffl-1.0.2.tar", last modified: Fri Apr 12 16:51:01 2024, max compression
+gzip compressed data, was "woffl-1.0.3.tar", last modified: Fri Apr 12 17:05:05 2024, max compression
```

## Comparing `woffl-1.0.2.tar` & `woffl-1.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 16:51:01.891031 woffl-1.0.2/
--rw-rw-rw-   0        0        0     1090 2024-01-10 03:00:27.000000 woffl-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     4028 2024-04-12 16:51:01.885789 woffl-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1926 2024-01-11 23:52:57.000000 woffl-1.0.2/README.md
--rw-rw-rw-   0        0        0     1592 2024-04-12 16:50:47.000000 woffl-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 16:51:01.891222 woffl-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 16:51:01.800491 woffl-1.0.2/tests/
--rw-rw-rw-   0        0        0        0 2024-01-10 03:00:27.000000 woffl-1.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0     2061 2024-04-11 21:37:06.000000 woffl-1.0.2/tests/boil_test.py
--rw-rw-rw-   0        0        0     1853 2024-04-11 21:38:00.000000 woffl-1.0.2/tests/e41_test.py
--rw-rw-rw-   0        0        0     2010 2024-04-11 21:38:27.000000 woffl-1.0.2/tests/fgas_test.py
--rw-rw-rw-   0        0        0     3080 2024-04-11 21:39:03.000000 woffl-1.0.2/tests/flow_test.py
--rw-rw-rw-   0        0        0     2697 2024-04-11 21:39:58.000000 woffl-1.0.2/tests/jpump_test.py
--rw-rw-rw-   0        0        0     1628 2024-04-11 21:40:16.000000 woffl-1.0.2/tests/outflow_test.py
--rw-rw-rw-   0        0        0      932 2024-04-12 01:06:46.000000 woffl-1.0.2/tests/pvt_test.py
--rw-rw-rw-   0        0        0     2375 2024-04-12 01:33:15.000000 woffl-1.0.2/tests/rmix_test.py
--rw-rw-rw-   0        0        0      358 2024-04-11 21:40:46.000000 woffl-1.0.2/tests/wprof_test.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:51:01.803440 woffl-1.0.2/woffl/
--rw-rw-rw-   0        0        0       56 2024-04-12 16:50:47.000000 woffl-1.0.2/woffl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:51:01.827781 woffl-1.0.2/woffl/assembly/
--rw-rw-rw-   0        0        0      324 2024-03-27 23:41:15.000000 woffl-1.0.2/woffl/assembly/__init__.py
--rw-rw-rw-   0        0        0     2313 2024-04-11 21:31:27.000000 woffl-1.0.2/woffl/assembly/batchrun.py
--rw-rw-rw-   0        0        0     3756 2024-04-12 15:24:00.000000 woffl-1.0.2/woffl/assembly/easypump.py
--rw-rw-rw-   0        0        0     6051 2024-04-11 21:47:40.000000 woffl-1.0.2/woffl/assembly/sysops.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:51:01.851906 woffl-1.0.2/woffl/flow/
--rw-rw-rw-   0        0        0      202 2024-03-14 00:29:33.000000 woffl-1.0.2/woffl/flow/__init__.py
--rw-rw-rw-   0        0        0     1359 2024-04-11 21:44:39.000000 woffl-1.0.2/woffl/flow/annflow.py
--rw-rw-rw-   0        0        0     3213 2024-01-10 03:00:27.000000 woffl-1.0.2/woffl/flow/inflow.py
--rw-rw-rw-   0        0        0     6639 2024-04-11 21:45:21.000000 woffl-1.0.2/woffl/flow/jetcheck.py
--rw-rw-rw-   0        0        0    18742 2024-04-11 21:45:56.000000 woffl-1.0.2/woffl/flow/jetflow.py
--rw-rw-rw-   0        0        0    18559 2024-04-11 21:46:16.000000 woffl-1.0.2/woffl/flow/jetplot.py
--rw-rw-rw-   0        0        0     8850 2024-04-11 21:46:30.000000 woffl-1.0.2/woffl/flow/outflow.py
--rw-rw-rw-   0        0        0     6306 2024-02-12 23:51:08.000000 woffl-1.0.2/woffl/flow/singlephase.py
--rw-rw-rw-   0        0        0    16499 2024-04-11 21:46:45.000000 woffl-1.0.2/woffl/flow/twophase.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:51:01.863914 woffl-1.0.2/woffl/geometry/
--rw-rw-rw-   0        0        0      113 2024-02-18 01:31:16.000000 woffl-1.0.2/woffl/geometry/__init__.py
--rw-rw-rw-   0        0        0     1786 2024-02-13 20:25:30.000000 woffl-1.0.2/woffl/geometry/forms.py
--rw-rw-rw-   0        0        0     3388 2024-01-31 19:16:45.000000 woffl-1.0.2/woffl/geometry/jetpump.py
--rw-rw-rw-   0        0        0     2674 2024-02-19 03:49:34.000000 woffl-1.0.2/woffl/geometry/pipe.py
--rw-rw-rw-   0        0        0    26650 2024-04-12 15:30:05.000000 woffl-1.0.2/woffl/geometry/wellprofile.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:51:01.878069 woffl-1.0.2/woffl/pvt/
--rw-rw-rw-   0        0        0      330 2024-04-12 01:14:17.000000 woffl-1.0.2/woffl/pvt/__init__.py
--rw-rw-rw-   0        0        0    23100 2024-04-12 16:12:06.000000 woffl-1.0.2/woffl/pvt/blackoil.py
--rw-rw-rw-   0        0        0      609 2024-01-10 03:00:27.000000 woffl-1.0.2/woffl/pvt/deadoil.py
--rw-rw-rw-   0        0        0    13803 2024-04-12 15:28:33.000000 woffl-1.0.2/woffl/pvt/formgas.py
--rw-rw-rw-   0        0        0     4192 2024-04-12 15:27:26.000000 woffl-1.0.2/woffl/pvt/formwat.py
--rw-rw-rw-   0        0        0    19555 2024-04-11 22:34:02.000000 woffl-1.0.2/woffl/pvt/resmix.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:51:01.880080 woffl-1.0.2/woffl.egg-info/
--rw-rw-rw-   0        0        0     4028 2024-04-12 16:51:01.000000 woffl-1.0.2/woffl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      953 2024-04-12 16:51:01.000000 woffl-1.0.2/woffl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 16:51:01.000000 woffl-1.0.2/woffl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2024-04-12 16:51:01.000000 woffl-1.0.2/woffl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-12 16:51:01.000000 woffl-1.0.2/woffl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.132566 woffl-1.0.3/
+-rw-rw-rw-   0        0        0     1090 2024-01-10 03:00:27.000000 woffl-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4028 2024-04-12 17:05:05.132566 woffl-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1926 2024-01-11 23:52:57.000000 woffl-1.0.3/README.md
+-rw-rw-rw-   0        0        0     1592 2024-04-12 17:04:14.000000 woffl-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 17:05:05.134901 woffl-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.052110 woffl-1.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-01-10 03:00:27.000000 woffl-1.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     2061 2024-04-11 21:37:06.000000 woffl-1.0.3/tests/boil_test.py
+-rw-rw-rw-   0        0        0     1853 2024-04-11 21:38:00.000000 woffl-1.0.3/tests/e41_test.py
+-rw-rw-rw-   0        0        0     2010 2024-04-11 21:38:27.000000 woffl-1.0.3/tests/fgas_test.py
+-rw-rw-rw-   0        0        0     3080 2024-04-11 21:39:03.000000 woffl-1.0.3/tests/flow_test.py
+-rw-rw-rw-   0        0        0     2697 2024-04-11 21:39:58.000000 woffl-1.0.3/tests/jpump_test.py
+-rw-rw-rw-   0        0        0     1628 2024-04-11 21:40:16.000000 woffl-1.0.3/tests/outflow_test.py
+-rw-rw-rw-   0        0        0      932 2024-04-12 01:06:46.000000 woffl-1.0.3/tests/pvt_test.py
+-rw-rw-rw-   0        0        0     2375 2024-04-12 01:33:15.000000 woffl-1.0.3/tests/rmix_test.py
+-rw-rw-rw-   0        0        0      358 2024-04-11 21:40:46.000000 woffl-1.0.3/tests/wprof_test.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.053622 woffl-1.0.3/woffl/
+-rw-rw-rw-   0        0        0       56 2024-04-12 17:04:14.000000 woffl-1.0.3/woffl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.077712 woffl-1.0.3/woffl/assembly/
+-rw-rw-rw-   0        0        0      324 2024-03-27 23:41:15.000000 woffl-1.0.3/woffl/assembly/__init__.py
+-rw-rw-rw-   0        0        0     2313 2024-04-11 21:31:27.000000 woffl-1.0.3/woffl/assembly/batchrun.py
+-rw-rw-rw-   0        0        0     3756 2024-04-12 15:24:00.000000 woffl-1.0.3/woffl/assembly/easypump.py
+-rw-rw-rw-   0        0        0     6051 2024-04-11 21:47:40.000000 woffl-1.0.3/woffl/assembly/sysops.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.099772 woffl-1.0.3/woffl/flow/
+-rw-rw-rw-   0        0        0      202 2024-03-14 00:29:33.000000 woffl-1.0.3/woffl/flow/__init__.py
+-rw-rw-rw-   0        0        0     1359 2024-04-11 21:44:39.000000 woffl-1.0.3/woffl/flow/annflow.py
+-rw-rw-rw-   0        0        0     3213 2024-01-10 03:00:27.000000 woffl-1.0.3/woffl/flow/inflow.py
+-rw-rw-rw-   0        0        0     6639 2024-04-11 21:45:21.000000 woffl-1.0.3/woffl/flow/jetcheck.py
+-rw-rw-rw-   0        0        0    18742 2024-04-11 21:45:56.000000 woffl-1.0.3/woffl/flow/jetflow.py
+-rw-rw-rw-   0        0        0    18559 2024-04-11 21:46:16.000000 woffl-1.0.3/woffl/flow/jetplot.py
+-rw-rw-rw-   0        0        0     8850 2024-04-11 21:46:30.000000 woffl-1.0.3/woffl/flow/outflow.py
+-rw-rw-rw-   0        0        0     6306 2024-02-12 23:51:08.000000 woffl-1.0.3/woffl/flow/singlephase.py
+-rw-rw-rw-   0        0        0    16499 2024-04-11 21:46:45.000000 woffl-1.0.3/woffl/flow/twophase.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.111478 woffl-1.0.3/woffl/geometry/
+-rw-rw-rw-   0        0        0      113 2024-02-18 01:31:16.000000 woffl-1.0.3/woffl/geometry/__init__.py
+-rw-rw-rw-   0        0        0     1786 2024-02-13 20:25:30.000000 woffl-1.0.3/woffl/geometry/forms.py
+-rw-rw-rw-   0        0        0     3388 2024-01-31 19:16:45.000000 woffl-1.0.3/woffl/geometry/jetpump.py
+-rw-rw-rw-   0        0        0     2674 2024-02-19 03:49:34.000000 woffl-1.0.3/woffl/geometry/pipe.py
+-rw-rw-rw-   0        0        0    26650 2024-04-12 15:30:05.000000 woffl-1.0.3/woffl/geometry/wellprofile.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.126874 woffl-1.0.3/woffl/pvt/
+-rw-rw-rw-   0        0        0      330 2024-04-12 01:14:17.000000 woffl-1.0.3/woffl/pvt/__init__.py
+-rw-rw-rw-   0        0        0    23100 2024-04-12 16:12:06.000000 woffl-1.0.3/woffl/pvt/blackoil.py
+-rw-rw-rw-   0        0        0      609 2024-01-10 03:00:27.000000 woffl-1.0.3/woffl/pvt/deadoil.py
+-rw-rw-rw-   0        0        0    13803 2024-04-12 15:28:33.000000 woffl-1.0.3/woffl/pvt/formgas.py
+-rw-rw-rw-   0        0        0     4192 2024-04-12 17:03:55.000000 woffl-1.0.3/woffl/pvt/formwat.py
+-rw-rw-rw-   0        0        0    19555 2024-04-11 22:34:02.000000 woffl-1.0.3/woffl/pvt/resmix.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.130124 woffl-1.0.3/woffl.egg-info/
+-rw-rw-rw-   0        0        0     4028 2024-04-12 17:05:04.000000 woffl-1.0.3/woffl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      953 2024-04-12 17:05:05.000000 woffl-1.0.3/woffl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 17:05:04.000000 woffl-1.0.3/woffl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2024-04-12 17:05:04.000000 woffl-1.0.3/woffl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-12 17:05:04.000000 woffl-1.0.3/woffl.egg-info/top_level.txt
```

### Comparing `woffl-1.0.2/LICENSE` & `woffl-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/PKG-INFO` & `woffl-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woffl
-Version: 1.0.2
+Version: 1.0.3
 Summary: Numerically solve jet pump equations in multiphase oil wells
 License: MIT License
         
         Copyright (c) 2023 Kaelin Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `woffl-1.0.2/README.md` & `woffl-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/pyproject.toml` & `woffl-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 000000a0: 6e64 5d0d 0a65 7863 6c75 6465 203d 205b  nd]..exclude = [
 000000b0: 2264 6174 6122 5d20 2023 2061 6c74 6572  "data"]  # alter
 000000c0: 6e61 7469 7665 6c79 3a20 6065 7863 6c75  natively: `exclu
 000000d0: 6465 203d 205b 2261 6464 6974 696f 6e61  de = ["additiona
 000000e0: 6c2a 225d 600d 0a0d 0a5b 7072 6f6a 6563  l*"]`....[projec
 000000f0: 745d 0d0a 6e61 6d65 203d 2022 776f 6666  t]..name = "woff
 00000100: 6c22 0d0a 7665 7273 696f 6e20 3d20 2231  l"..version = "1
-00000110: 2e30 2e32 2220 2320 6275 6d70 7665 7220  .0.2" # bumpver 
+00000110: 2e30 2e33 2220 2320 6275 6d70 7665 7220  .0.3" # bumpver 
 00000120: 6175 746f 6d61 7469 6361 6c6c 7920 7570  automatically up
 00000130: 6461 7465 730d 0a64 6573 6372 6970 7469  dates..descripti
 00000140: 6f6e 203d 2022 4e75 6d65 7269 6361 6c6c  on = "Numericall
 00000150: 7920 736f 6c76 6520 6a65 7420 7075 6d70  y solve jet pump
 00000160: 2065 7175 6174 696f 6e73 2069 6e20 6d75   equations in mu
 00000170: 6c74 6970 6861 7365 206f 696c 2077 656c  ltiphase oil wel
 00000180: 6c73 220d 0a72 6561 646d 6520 3d20 2252  ls"..readme = "R
@@ -65,15 +65,15 @@
 00000400: 2022 626c 6163 6b22 5d0d 0a0d 0a5b 7072   "black"]....[pr
 00000410: 6f6a 6563 742e 7572 6c73 5d0d 0a48 6f6d  oject.urls]..Hom
 00000420: 6570 6167 6520 3d20 2268 7474 7073 3a2f  epage = "https:/
 00000430: 2f67 6974 6875 622e 636f 6d2f 6b77 656c  /github.com/kwel
 00000440: 6c69 732f 776f 6666 6c22 0d0a 0d0a 0d0a  lis/woffl"......
 00000450: 5b74 6f6f 6c2e 6275 6d70 7665 725d 0d0a  [tool.bumpver]..
 00000460: 6375 7272 656e 745f 7665 7273 696f 6e20  current_version 
-00000470: 3d20 2231 2e30 2e32 2220 2320 6275 6d70  = "1.0.2" # bump
+00000470: 3d20 2231 2e30 2e33 2220 2320 6275 6d70  = "1.0.3" # bump
 00000480: 7665 7220 7570 6461 7465 2070 6174 6368  ver update patch
 00000490: 0d0a 7665 7273 696f 6e5f 7061 7474 6572  ..version_patter
 000004a0: 6e20 3d20 224d 414a 4f52 2e4d 494e 4f52  n = "MAJOR.MINOR
 000004b0: 2e50 4154 4348 220d 0a23 2063 6f6d 6d69  .PATCH"..# commi
 000004c0: 745f 6d65 7373 6167 6520 3d20 2262 756d  t_message = "bum
 000004d0: 7020 7665 7273 696f 6e20 7b6f 6c64 5f76  p version {old_v
 000004e0: 6572 7369 6f6e 7d20 2d3e 207b 6e65 775f  ersion} -> {new_
```

### Comparing `woffl-1.0.2/tests/boil_test.py` & `woffl-1.0.3/tests/boil_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/tests/e41_test.py` & `woffl-1.0.3/tests/e41_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/tests/fgas_test.py` & `woffl-1.0.3/tests/fgas_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/tests/flow_test.py` & `woffl-1.0.3/tests/flow_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/tests/jpump_test.py` & `woffl-1.0.3/tests/jpump_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/tests/outflow_test.py` & `woffl-1.0.3/tests/outflow_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/tests/pvt_test.py` & `woffl-1.0.3/tests/pvt_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/tests/rmix_test.py` & `woffl-1.0.3/tests/rmix_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/assembly/batchrun.py` & `woffl-1.0.3/woffl/assembly/batchrun.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/assembly/easypump.py` & `woffl-1.0.3/woffl/assembly/easypump.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/assembly/sysops.py` & `woffl-1.0.3/woffl/assembly/sysops.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/flow/annflow.py` & `woffl-1.0.3/woffl/flow/annflow.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/flow/inflow.py` & `woffl-1.0.3/woffl/flow/inflow.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/flow/jetcheck.py` & `woffl-1.0.3/woffl/flow/jetcheck.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/flow/jetflow.py` & `woffl-1.0.3/woffl/flow/jetflow.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/flow/jetplot.py` & `woffl-1.0.3/woffl/flow/jetplot.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/flow/outflow.py` & `woffl-1.0.3/woffl/flow/outflow.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/flow/singlephase.py` & `woffl-1.0.3/woffl/flow/singlephase.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/flow/twophase.py` & `woffl-1.0.3/woffl/flow/twophase.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/geometry/forms.py` & `woffl-1.0.3/woffl/geometry/forms.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/geometry/jetpump.py` & `woffl-1.0.3/woffl/geometry/jetpump.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/geometry/pipe.py` & `woffl-1.0.3/woffl/geometry/pipe.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/geometry/wellprofile.py` & `woffl-1.0.3/woffl/geometry/wellprofile.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/pvt/blackoil.py` & `woffl-1.0.3/woffl/pvt/blackoil.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/pvt/deadoil.py` & `woffl-1.0.3/woffl/pvt/deadoil.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/pvt/formgas.py` & `woffl-1.0.3/woffl/pvt/formgas.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/pvt/formwat.py` & `woffl-1.0.3/woffl/pvt/formwat.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl/pvt/resmix.py` & `woffl-1.0.3/woffl/pvt/resmix.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.2/woffl.egg-info/PKG-INFO` & `woffl-1.0.3/woffl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woffl
-Version: 1.0.2
+Version: 1.0.3
 Summary: Numerically solve jet pump equations in multiphase oil wells
 License: MIT License
         
         Copyright (c) 2023 Kaelin Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `woffl-1.0.2/woffl.egg-info/SOURCES.txt` & `woffl-1.0.3/woffl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

