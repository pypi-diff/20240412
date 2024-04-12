# Comparing `tmp/vnpy_bybit-2021.6.21.tar.gz` & `tmp/vnpy_bybit-2024.4.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vnpy_bybit-2021.6.21.tar", last modified: Mon Jun 21 05:27:51 2021, max compression
+gzip compressed data, was "vnpy_bybit-2024.4.12.tar", last modified: Fri Apr 12 07:44:32 2024, max compression
```

## Comparing `vnpy_bybit-2021.6.21.tar` & `vnpy_bybit-2024.4.12.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2021-06-21 05:27:51.000000 vnpy_bybit-2021.6.21/
--rw-rw-rw-   0        0        0     2642 2021-06-21 05:27:51.000000 vnpy_bybit-2021.6.21/PKG-INFO
--rw-rw-rw-   0        0        0     1240 2021-06-21 05:17:53.000000 vnpy_bybit-2021.6.21/README.md
--rw-rw-rw-   0        0        0     1004 2021-06-21 05:27:51.000000 vnpy_bybit-2021.6.21/setup.cfg
--rw-rw-rw-   0        0        0       43 2021-06-21 04:33:42.000000 vnpy_bybit-2021.6.21/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-21 05:27:51.000000 vnpy_bybit-2021.6.21/vnpy_bybit/
--rw-rw-rw-   0        0        0     1277 2021-06-21 05:26:02.000000 vnpy_bybit-2021.6.21/vnpy_bybit/__init__.py
--rw-rw-rw-   0        0        0    63726 2021-06-21 05:26:40.000000 vnpy_bybit-2021.6.21/vnpy_bybit/bybit_gateway.py
-drwxrwxrwx   0        0        0        0 2021-06-21 05:27:51.000000 vnpy_bybit-2021.6.21/vnpy_bybit.egg-info/
--rw-rw-rw-   0        0        0     2642 2021-06-21 05:27:50.000000 vnpy_bybit-2021.6.21/vnpy_bybit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2021-06-21 05:27:50.000000 vnpy_bybit-2021.6.21/vnpy_bybit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-21 05:27:50.000000 vnpy_bybit-2021.6.21/vnpy_bybit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2021-06-21 05:27:50.000000 vnpy_bybit-2021.6.21/vnpy_bybit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-06-21 05:27:50.000000 vnpy_bybit-2021.6.21/vnpy_bybit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 07:44:32.103567 vnpy_bybit-2024.4.12/
+-rw-rw-rw-   0        0        0     1101 2024-04-12 07:41:08.000000 vnpy_bybit-2024.4.12/LICENSE
+-rw-rw-rw-   0        0        0     2991 2024-04-12 07:44:32.104622 vnpy_bybit-2024.4.12/PKG-INFO
+-rw-rw-rw-   0        0        0     1994 2024-04-12 07:39:13.000000 vnpy_bybit-2024.4.12/README.md
+-rw-rw-rw-   0        0        0     1082 2024-04-12 07:44:32.106565 vnpy_bybit-2024.4.12/setup.cfg
+-rw-rw-rw-   0        0        0       43 2024-03-05 02:02:55.000000 vnpy_bybit-2024.4.12/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:44:32.079419 vnpy_bybit-2024.4.12/vnpy_bybit/
+-rw-rw-rw-   0        0        0     1223 2024-04-12 07:41:55.000000 vnpy_bybit-2024.4.12/vnpy_bybit/__init__.py
+-rw-rw-rw-   0        0        0    40029 2024-04-12 07:34:06.000000 vnpy_bybit-2024.4.12/vnpy_bybit/bybit_gateway.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:44:32.102551 vnpy_bybit-2024.4.12/vnpy_bybit.egg-info/
+-rw-rw-rw-   0        0        0     2991 2024-04-12 07:44:31.000000 vnpy_bybit-2024.4.12/vnpy_bybit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-04-12 07:44:31.000000 vnpy_bybit-2024.4.12/vnpy_bybit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 07:44:31.000000 vnpy_bybit-2024.4.12/vnpy_bybit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 07:44:31.000000 vnpy_bybit-2024.4.12/vnpy_bybit.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2024-04-12 07:44:31.000000 vnpy_bybit-2024.4.12/vnpy_bybit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-12 07:44:31.000000 vnpy_bybit-2024.4.12/vnpy_bybit.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vnpy_bybit-2021.6.21/setup.cfg` & `vnpy_bybit-2024.4.12/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,68 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 6279 6269 740d 0a76   = vnpy_bybit..v
-00000020: 6572 7369 6f6e 203d 2032 3032 312e 362e  ersion = 2021.6.
-00000030: 3231 0d0a 7572 6c20 3d20 6874 7470 733a  21..url = https:
-00000040: 2f2f 7777 772e 766e 7079 2e63 6f6d 0d0a  //www.vnpy.com..
-00000050: 6c69 6365 6e73 6520 3d20 4d49 540d 0a61  license = MIT..a
-00000060: 7574 686f 7220 3d20 5869 616f 796f 7520  uthor = Xiaoyou 
-00000070: 4368 656e 0d0a 6175 7468 6f72 5f65 6d61  Chen..author_ema
-00000080: 696c 203d 2078 6961 6f79 6f75 2e63 6865  il = xiaoyou.che
-00000090: 6e40 6d61 696c 2e76 6e70 792e 636f 6d0d  n@mail.vnpy.com.
-000000a0: 0a64 6573 6372 6970 7469 6f6e 203d 2042  .description = B
-000000b0: 7962 6974 2067 6174 6577 6179 2066 6f72  ybit gateway for
-000000c0: 2076 6e2e 7079 2071 7561 6e74 2074 7261   vn.py quant tra
-000000d0: 6469 6e67 2066 7261 6d65 776f 726b 2e0d  ding framework..
-000000e0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000000f0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
-00000100: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
-00000110: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
-00000120: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
-00000130: 776e 0d0a 6b65 7977 6f72 6473 203d 200d  wn..keywords = .
-00000140: 0a09 7175 616e 740d 0a09 7175 616e 7469  ..quant...quanti
-00000150: 7461 7469 7665 0d0a 0969 6e76 6573 746d  tative...investm
-00000160: 656e 740d 0a09 7472 6164 696e 670d 0a09  ent...trading...
-00000170: 616c 676f 7472 6164 696e 670d 0a63 6c61  algotrading..cla
-00000180: 7373 6966 6965 7273 203d 200d 0a09 4465  ssifiers = ...De
-00000190: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-000001a0: 203a 3a20 3520 2d20 5072 6f64 7563 7469   :: 5 - Producti
-000001b0: 6f6e 2f53 7461 626c 650d 0a09 4f70 6572  on/Stable...Oper
-000001c0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-000001d0: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-000001e0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000001f0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000200: 3a3a 2033 0d0a 0950 726f 6772 616d 6d69  :: 3...Programmi
-00000210: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000220: 7974 686f 6e20 3a3a 2033 2e37 0d0a 0950  ython :: 3.7...P
-00000230: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000240: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000250: 2033 2e38 0d0a 0950 726f 6772 616d 6d69   3.8...Programmi
-00000260: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000270: 7974 686f 6e20 3a3a 2033 2e39 0d0a 0950  ython :: 3.9...P
-00000280: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000290: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002a0: 2033 2e31 300d 0a09 546f 7069 6320 3a3a   3.10...Topic ::
-000002b0: 204f 6666 6963 652f 4275 7369 6e65 7373   Office/Business
-000002c0: 203a 3a20 4669 6e61 6e63 6961 6c20 3a3a   :: Financial ::
-000002d0: 2049 6e76 6573 746d 656e 740d 0a09 5072   Investment...Pr
-000002e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000002f0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000300: 496d 706c 656d 656e 7461 7469 6f6e 203a  Implementation :
-00000310: 3a20 4350 7974 686f 6e0d 0a09 4c69 6365  : CPython...Lice
-00000320: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-00000330: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
-00000340: 7365 0d0a 094e 6174 7572 616c 204c 616e  se...Natural Lan
-00000350: 6775 6167 6520 3a3a 2043 6869 6e65 7365  guage :: Chinese
-00000360: 2028 5369 6d70 6c69 6669 6564 290d 0a0d   (Simplified)...
-00000370: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-00000380: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
-00000390: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-000003a0: 200d 0a09 766e 7079 5f77 6562 736f 636b   ...vnpy_websock
-000003b0: 6574 0d0a 0976 6e70 795f 7265 7374 0d0a  et...vnpy_rest..
-000003c0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000003d0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-000003e0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000020: 6572 7369 6f6e 203d 2061 7474 723a 2076  ersion = attr: v
+00000030: 6e70 795f 6279 6269 742e 5f5f 7665 7273  npy_bybit.__vers
+00000040: 696f 6e5f 5f0d 0a61 7574 686f 7220 3d20  ion__..author = 
+00000050: 5665 6967 684e 6120 476c 6f62 616c 0d0a  VeighNa Global..
+00000060: 6175 7468 6f72 5f65 6d61 696c 203d 2076  author_email = v
+00000070: 6569 6768 6e61 4068 6f74 6d61 696c 2e63  eighna@hotmail.c
+00000080: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
+00000090: 3d20 4279 6269 7420 7472 6164 696e 6720  = Bybit trading 
+000000a0: 6761 7465 7761 7920 666f 7220 5665 6967  gateway for Veig
+000000b0: 684e 6120 4576 6f2e 0d0a 6c6f 6e67 5f64  hNa Evo...long_d
+000000c0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+000000d0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
+000000e0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+000000f0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
+00000100: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
+00000110: 203d 2068 7474 7073 3a2f 2f77 7777 2e67   = https://www.g
+00000120: 6974 6875 622e 636f 6d2f 7665 6967 686e  ithub.com/veighn
+00000130: 612d 676c 6f62 616c 0d0a 6b65 7977 6f72  a-global..keywor
+00000140: 6473 203d 200d 0a09 7175 616e 740d 0a09  ds = ...quant...
+00000150: 7175 616e 7469 7461 7469 7665 0d0a 0969  quantitative...i
+00000160: 6e76 6573 746d 656e 740d 0a09 7472 6164  nvestment...trad
+00000170: 696e 670d 0a09 616c 676f 7472 6164 696e  ing...algotradin
+00000180: 670d 0a09 6279 6269 740d 0a09 6274 630d  g...bybit...btc.
+00000190: 0a09 6372 7970 746f 0d0a 636c 6173 7369  ..crypto..classi
+000001a0: 6669 6572 7320 3d20 0d0a 0944 6576 656c  fiers = ...Devel
+000001b0: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
+000001c0: 2035 202d 2050 726f 6475 6374 696f 6e2f   5 - Production/
+000001d0: 5374 6162 6c65 0d0a 094f 7065 7261 7469  Stable...Operati
+000001e0: 6e67 2053 7973 7465 6d20 3a3a 204d 6963  ng System :: Mic
+000001f0: 726f 736f 6674 203a 3a20 5769 6e64 6f77  rosoft :: Window
+00000200: 730d 0a09 4f70 6572 6174 696e 6720 5379  s...Operating Sy
+00000210: 7374 656d 203a 3a20 504f 5349 5820 3a3a  stem :: POSIX ::
+00000220: 204c 696e 7578 0d0a 094f 7065 7261 7469   Linux...Operati
+00000230: 6e67 2053 7973 7465 6d20 3a3a 204d 6163  ng System :: Mac
+00000240: 4f53 0d0a 0950 726f 6772 616d 6d69 6e67  OS...Programming
+00000250: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000260: 686f 6e20 3a3a 2033 0d0a 0950 726f 6772  hon :: 3...Progr
+00000270: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000280: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000290: 300d 0a09 5072 6f67 7261 6d6d 696e 6720  0...Programming 
+000002a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002b0: 6f6e 203a 3a20 332e 3131 0d0a 0950 726f  on :: 3.11...Pro
+000002c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000002d0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000002e0: 2e31 320d 0a09 546f 7069 6320 3a3a 204f  .12...Topic :: O
+000002f0: 6666 6963 652f 4275 7369 6e65 7373 203a  ffice/Business :
+00000300: 3a20 4669 6e61 6e63 6961 6c20 3a3a 2049  : Financial :: I
+00000310: 6e76 6573 746d 656e 740d 0a09 5072 6f67  nvestment...Prog
+00000320: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000330: 203a 3a20 5079 7468 6f6e 203a 3a20 496d   :: Python :: Im
+00000340: 706c 656d 656e 7461 7469 6f6e 203a 3a20  plementation :: 
+00000350: 4350 7974 686f 6e0d 0a09 4c69 6365 6e73  CPython...Licens
+00000360: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000370: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+00000380: 0d0a 094e 6174 7572 616c 204c 616e 6775  ...Natural Langu
+00000390: 6167 6520 3a3a 2045 6e67 6c69 7368 0d0a  age :: English..
+000003a0: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
+000003b0: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a7a  kages = find:..z
+000003c0: 6970 5f73 6166 6520 3d20 4661 6c73 650d  ip_safe = False.
+000003d0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+000003e0: 7320 3d20 0d0a 0976 6e70 795f 6576 6f0d  s = ...vnpy_evo.
+000003f0: 0a09 766e 7079 5f72 6573 740d 0a09 766e  ..vnpy_rest...vn
+00000400: 7079 5f77 6562 736f 636b 6574 0d0a 0d0a  py_websocket....
+00000410: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+00000420: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+00000430: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `vnpy_bybit-2021.6.21/vnpy_bybit/__init__.py` & `vnpy_bybit-2024.4.12/vnpy_bybit/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # The MIT License (MIT)
 #
-# Copyright (c) 2015-present, Xiaoyou Chen
+# Copyright (c) 2023-present, VeighNa Global
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,13 +16,11 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import importlib_metadata
-
 from .bybit_gateway import BybitGateway
 
 
-__version__ = importlib_metadata.version("vnpy_bybit")
+__version__ = "2024.4.12"
```

