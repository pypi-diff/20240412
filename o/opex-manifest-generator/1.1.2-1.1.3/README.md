# Comparing `tmp/opex_manifest_generator-1.1.2.tar.gz` & `tmp/opex_manifest_generator-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opex_manifest_generator-1.1.2.tar", last modified: Fri Apr 12 13:12:32 2024, max compression
+gzip compressed data, was "opex_manifest_generator-1.1.3.tar", last modified: Fri Apr 12 13:58:53 2024, max compression
```

## Comparing `opex_manifest_generator-1.1.2.tar` & `opex_manifest_generator-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 13:12:32.138027 opex_manifest_generator-1.1.2/
--rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.1.2/LICENSE.md
--rw-rw-rw-   0        0        0      701 2024-04-12 13:12:32.135662 opex_manifest_generator-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    19695 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 13:12:32.092160 opex_manifest_generator-1.1.2/opex_manifest_generator/
--rw-rw-rw-   0        0        0      439 2024-02-20 12:38:50.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/__init__.py
--rw-rw-rw-   0        0        0     6050 2024-04-12 13:08:38.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/cli.py
--rw-rw-rw-   0        0        0      676 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/common.py
--rw-rw-rw-   0        0        0      966 2024-02-18 22:01:42.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/hash.py
--rw-rw-rw-   0        0        0    27307 2024-04-12 13:07:29.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/opex_manifest.py
--rw-rw-rw-   0        0        0    20008 2024-03-26 21:35:58.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/opex_manifest_reference.py
--rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/test_cli.py
--rw-rw-rw-   0        0        0       21 2024-04-12 13:09:20.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/version.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:12:32.133647 opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/
--rw-rw-rw-   0        0        0      701 2024-04-12 13:12:31.000000 opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      615 2024-04-12 13:12:32.000000 opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 13:12:31.000000 opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-12 13:12:31.000000 opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2024-04-12 13:12:32.000000 opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-12 13:12:32.000000 opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      864 2024-04-12 13:09:27.000000 opex_manifest_generator-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 13:12:32.139025 opex_manifest_generator-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 13:58:53.012601 opex_manifest_generator-1.1.3/
+-rw-rw-rw-   0        0        0      124 2024-04-12 13:39:12.000000 opex_manifest_generator-1.1.3/.gitignore
+-rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.1.3/LICENSE.md
+-rw-rw-rw-   0        0        0      701 2024-04-12 13:58:53.009603 opex_manifest_generator-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    19695 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 13:58:52.933728 opex_manifest_generator-1.1.3/opex_manifest_generator/
+-rw-rw-rw-   0        0        0      439 2024-02-20 12:38:50.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/__init__.py
+-rw-rw-rw-   0        0        0     6050 2024-04-12 13:08:38.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/cli.py
+-rw-rw-rw-   0        0        0      676 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/common.py
+-rw-rw-rw-   0        0        0      966 2024-02-18 22:01:42.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/hash.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:58:52.987603 opex_manifest_generator-1.1.3/opex_manifest_generator/metadata/
+-rw-rw-rw-   0        0        0      775 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/metadata/DublinCore Template.xml
+-rw-rw-rw-   0        0        0     2268 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/metadata/EAD Template.xml
+-rw-rw-rw-   0        0        0      483 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/metadata/GDPR Template.xml
+-rw-rw-rw-   0        0        0     2701 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/metadata/MODS Template.xml
+-rw-rw-rw-   0        0        0    27307 2024-04-12 13:07:29.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/opex_manifest.py
+-rw-rw-rw-   0        0        0    20008 2024-03-26 21:35:58.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/opex_manifest_reference.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:58:52.993604 opex_manifest_generator-1.1.3/opex_manifest_generator/samples/
+-rw-rw-rw-   0        0        0      389 2023-02-23 12:37:11.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/samples/Opex.xml
+-rw-rw-rw-   0        0        0    29091 2024-04-04 10:37:30.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx
+drwxrwxrwx   0        0        0        0 2024-04-12 13:58:53.003604 opex_manifest_generator-1.1.3/opex_manifest_generator/samples/spreads/
+-rw-rw-rw-   0        0        0    22794 2024-04-04 14:48:01.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/samples/spreads/dctemplate.xlsx
+-rw-rw-rw-   0        0        0    19299 2024-04-04 14:45:30.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/samples/spreads/eadtemplate.xlsx
+-rw-rw-rw-   0        0        0    18662 2024-04-04 14:51:01.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx
+-rw-rw-rw-   0        0        0    19509 2024-04-04 14:46:22.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/samples/spreads/modstemplate.xlsx
+-rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/test_cli.py
+-rw-rw-rw-   0        0        0       21 2024-04-12 13:57:41.000000 opex_manifest_generator-1.1.3/opex_manifest_generator/version.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:58:53.006602 opex_manifest_generator-1.1.3/opex_manifest_generator.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-04-12 13:58:52.000000 opex_manifest_generator-1.1.3/opex_manifest_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1176 2024-04-12 13:58:52.000000 opex_manifest_generator-1.1.3/opex_manifest_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 13:58:52.000000 opex_manifest_generator-1.1.3/opex_manifest_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-12 13:58:52.000000 opex_manifest_generator-1.1.3/opex_manifest_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2024-04-12 13:58:52.000000 opex_manifest_generator-1.1.3/opex_manifest_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-12 13:58:52.000000 opex_manifest_generator-1.1.3/opex_manifest_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      837 2024-04-12 13:57:35.000000 opex_manifest_generator-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 13:58:53.013601 opex_manifest_generator-1.1.3/setup.cfg
```

### Comparing `opex_manifest_generator-1.1.2/LICENSE.md` & `opex_manifest_generator-1.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.2/PKG-INFO` & `opex_manifest_generator-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.1.2
+Version: 1.1.3
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.1.2/README.md` & `opex_manifest_generator-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.2/opex_manifest_generator/cli.py` & `opex_manifest_generator-1.1.3/opex_manifest_generator/cli.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.2/opex_manifest_generator/common.py` & `opex_manifest_generator-1.1.3/opex_manifest_generator/common.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.2/opex_manifest_generator/hash.py` & `opex_manifest_generator-1.1.3/opex_manifest_generator/hash.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.2/opex_manifest_generator/opex_manifest.py` & `opex_manifest_generator-1.1.3/opex_manifest_generator/opex_manifest.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.2/opex_manifest_generator/opex_manifest_reference.py` & `opex_manifest_generator-1.1.3/opex_manifest_generator/opex_manifest_reference.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/PKG-INFO` & `opex_manifest_generator-1.1.3/opex_manifest_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.1.2
+Version: 1.1.3
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.1.2/pyproject.toml` & `opex_manifest_generator-1.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
-00000020: 7570 746f 6f6c 7322 5d0d 0a62 7569 6c64  uptools"]..build
-00000030: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
-00000040: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
-00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
-00000060: 0a6e 616d 6520 3d20 226f 7065 785f 6d61  .name = "opex_ma
-00000070: 6e69 6665 7374 5f67 656e 6572 6174 6f72  nifest_generator
-00000080: 220d 0a76 6572 7369 6f6e 203d 2022 312e  "..version = "1.
-00000090: 312e 3222 0d0a 6175 7468 6f72 7320 3d20  1.2"..authors = 
-000000a0: 5b0d 0a20 2020 207b 6e61 6d65 3d22 4368  [..    {name="Ch
-000000b0: 7269 7374 6f70 6865 7220 5072 696e 6365  ristopher Prince
-000000c0: 222c 2065 6d61 696c 3d22 632e 706a 2e70  ", email="c.pj.p
-000000d0: 7269 6e63 6540 676d 6169 6c2e 636f 6d22  rince@gmail.com"
-000000e0: 7d0d 0a20 2020 205d 0d0a 6465 7363 7269  }..    ]..descri
-000000f0: 7074 696f 6e20 3d20 224f 7065 7820 4d61  ption = "Opex Ma
-00000100: 6e69 6665 7374 2047 656e 6572 6174 6f72  nifest Generator
-00000110: 2054 6f6f 6c20 666f 7220 7573 6520 7769   Tool for use wi
-00000120: 7468 204f 7065 7820 2f20 5072 6573 6572  th Opex / Preser
-00000130: 7669 6361 220d 0a63 6c61 7373 6966 6965  vica"..classifie
-00000140: 7273 203d 205b 0d0a 2020 2020 2250 726f  rs = [..    "Pro
-00000150: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000160: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000170: 222c 0d0a 2020 2020 224c 6963 656e 7365  ",..    "License
-00000180: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000190: 203a 3a20 4170 6163 6865 2053 6f66 7477   :: Apache Softw
-000001a0: 6172 6520 4c69 6365 6e73 6522 2c0d 0a20  are License",.. 
-000001b0: 2020 2022 4f70 6572 6174 696e 6720 5379     "Operating Sy
-000001c0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-000001d0: 656e 6465 6e74 222c 0d0a 2020 2020 2254  endent",..    "T
-000001e0: 6f70 6963 203a 3a20 5379 7374 656d 203a  opic :: System :
-000001f0: 3a20 4172 6368 6976 696e 6722 0d0a 2020  : Archiving"..  
-00000200: 2020 5d0d 0a64 6570 656e 6465 6e63 6965    ]..dependencie
-00000210: 733d 5b22 6175 746f 5f63 6c61 7373 6966  s=["auto_classif
-00000220: 6963 6174 696f 6e5f 6765 6e65 7261 746f  ication_generato
-00000230: 7222 2c22 7061 6e64 6173 222c 226f 7065  r","pandas","ope
-00000240: 6e70 7978 6c22 2c22 6c78 6d6c 225d 0d0a  npyxl","lxml"]..
-00000250: 5b70 726f 6a65 6374 2e75 726c 735d 0d0a  [project.urls]..
-00000260: 486f 6d65 7061 6765 203d 2022 6874 7470  Homepage = "http
-00000270: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f43  s://github.com/C
-00000280: 504a 5052 494e 4345 2f6f 7065 785f 6d61  PJPRINCE/opex_ma
-00000290: 6e69 6665 7374 5f67 656e 6572 6174 6f72  nifest_generator
-000002a0: 220d 0a49 7373 7565 7320 3d20 2268 7474  "..Issues = "htt
-000002b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000002c0: 4350 4a50 5249 4e43 452f 6f70 6578 5f6d  CPJPRINCE/opex_m
-000002d0: 616e 6966 6573 745f 6765 6e65 7261 746f  anifest_generato
-000002e0: 722f 6973 7375 6573 220d 0a5b 7072 6f6a  r/issues"..[proj
-000002f0: 6563 742e 7363 7269 7074 735d 0d0a 6f70  ect.scripts]..op
-00000300: 6578 5f67 656e 6572 6174 6520 3d20 226f  ex_generate = "o
-00000310: 7065 785f 6d61 6e69 6665 7374 5f67 656e  pex_manifest_gen
-00000320: 6572 6174 6f72 2e63 6c69 3a72 756e 5f63  erator.cli:run_c
-00000330: 6c69 220d 0a0d 0a5b 746f 6f6c 2e68 6174  li"....[tool.hat
-00000340: 6368 2e62 756c 645d 0d0a 696e 636c 7564  ch.buld]..includ
-00000350: 6520 3d20 5b27 6d65 7461 6461 7461 275d  e = ['metadata']
+00000020: 7570 746f 6f6c 7322 2c20 2273 6574 7570  uptools", "setup
+00000030: 746f 6f6c 732d 7363 6d22 5d0d 0a62 7569  tools-scm"]..bui
+00000040: 6c64 2d62 6163 6b65 6e64 203d 2022 7365  ld-backend = "se
+00000050: 7475 7074 6f6f 6c73 2e62 7569 6c64 5f6d  tuptools.build_m
+00000060: 6574 6122 0d0a 0d0a 5b70 726f 6a65 6374  eta"....[project
+00000070: 5d0d 0a6e 616d 6520 3d20 226f 7065 785f  ]..name = "opex_
+00000080: 6d61 6e69 6665 7374 5f67 656e 6572 6174  manifest_generat
+00000090: 6f72 220d 0a76 6572 7369 6f6e 203d 2022  or"..version = "
+000000a0: 312e 312e 3322 0d0a 6175 7468 6f72 7320  1.1.3"..authors 
+000000b0: 3d20 5b0d 0a20 2020 207b 6e61 6d65 3d22  = [..    {name="
+000000c0: 4368 7269 7374 6f70 6865 7220 5072 696e  Christopher Prin
+000000d0: 6365 222c 2065 6d61 696c 3d22 632e 706a  ce", email="c.pj
+000000e0: 2e70 7269 6e63 6540 676d 6169 6c2e 636f  .prince@gmail.co
+000000f0: 6d22 7d0d 0a20 2020 205d 0d0a 6465 7363  m"}..    ]..desc
+00000100: 7269 7074 696f 6e20 3d20 224f 7065 7820  ription = "Opex 
+00000110: 4d61 6e69 6665 7374 2047 656e 6572 6174  Manifest Generat
+00000120: 6f72 2054 6f6f 6c20 666f 7220 7573 6520  or Tool for use 
+00000130: 7769 7468 204f 7065 7820 2f20 5072 6573  with Opex / Pres
+00000140: 6572 7669 6361 220d 0a63 6c61 7373 6966  ervica"..classif
+00000150: 6965 7273 203d 205b 0d0a 2020 2020 2250  iers = [..    "P
+00000160: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000170: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000180: 2033 222c 0d0a 2020 2020 224c 6963 656e   3",..    "Licen
+00000190: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+000001a0: 6564 203a 3a20 4170 6163 6865 2053 6f66  ed :: Apache Sof
+000001b0: 7477 6172 6520 4c69 6365 6e73 6522 2c0d  tware License",.
+000001c0: 0a20 2020 2022 4f70 6572 6174 696e 6720  .    "Operating 
+000001d0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+000001e0: 6570 656e 6465 6e74 222c 0d0a 2020 2020  ependent",..    
+000001f0: 2254 6f70 6963 203a 3a20 5379 7374 656d  "Topic :: System
+00000200: 203a 3a20 4172 6368 6976 696e 6722 0d0a   :: Archiving"..
+00000210: 2020 2020 5d0d 0a64 6570 656e 6465 6e63      ]..dependenc
+00000220: 6965 733d 5b22 6175 746f 5f63 6c61 7373  ies=["auto_class
+00000230: 6966 6963 6174 696f 6e5f 6765 6e65 7261  ification_genera
+00000240: 746f 7222 2c22 7061 6e64 6173 222c 226f  tor","pandas","o
+00000250: 7065 6e70 7978 6c22 2c22 6c78 6d6c 225d  penpyxl","lxml"]
+00000260: 0d0a 5b70 726f 6a65 6374 2e75 726c 735d  ..[project.urls]
+00000270: 0d0a 486f 6d65 7061 6765 203d 2022 6874  ..Homepage = "ht
+00000280: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000290: 2f43 504a 5052 494e 4345 2f6f 7065 785f  /CPJPRINCE/opex_
+000002a0: 6d61 6e69 6665 7374 5f67 656e 6572 6174  manifest_generat
+000002b0: 6f72 220d 0a49 7373 7565 7320 3d20 2268  or"..Issues = "h
+000002c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000002d0: 6d2f 4350 4a50 5249 4e43 452f 6f70 6578  m/CPJPRINCE/opex
+000002e0: 5f6d 616e 6966 6573 745f 6765 6e65 7261  _manifest_genera
+000002f0: 746f 722f 6973 7375 6573 220d 0a5b 7072  tor/issues"..[pr
+00000300: 6f6a 6563 742e 7363 7269 7074 735d 0d0a  oject.scripts]..
+00000310: 6f70 6578 5f67 656e 6572 6174 6520 3d20  opex_generate = 
+00000320: 226f 7065 785f 6d61 6e69 6665 7374 5f67  "opex_manifest_g
+00000330: 656e 6572 6174 6f72 2e63 6c69 3a72 756e  enerator.cli:run
+00000340: 5f63 6c69 22                             _cli"
```

