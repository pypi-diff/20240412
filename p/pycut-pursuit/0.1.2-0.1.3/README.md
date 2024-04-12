# Comparing `tmp/pycut_pursuit-0.1.2-cp312-cp312-macosx_14_0_arm64.whl.zip` & `tmp/pycut_pursuit-0.1.3-cp312-cp312-musllinux_1_1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,22 @@
-Zip file size: 818815 bytes, number of entries: 14
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-16 12:48 pycut_pursuit/__init__.py
--rw-r--r--  2.0 unx    15221 b- defN 24-Mar-16 12:48 pycut_pursuit/cp_d0_dist.py
--rwxr-xr-x  2.0 unx   448504 b- defN 24-Mar-26 09:20 pycut_pursuit/cp_d0_dist_cpy.cpython-312-darwin.so
--rw-r--r--  2.0 unx    14646 b- defN 24-Mar-16 12:48 pycut_pursuit/cp_d1_lsx.py
--rwxr-xr-x  2.0 unx   857280 b- defN 24-Mar-26 09:20 pycut_pursuit/cp_d1_lsx_cpy.cpython-312-darwin.so
--rw-r--r--  2.0 unx    15702 b- defN 24-Mar-16 12:48 pycut_pursuit/cp_d1_ql1b.py
--rwxr-xr-x  2.0 unx   920952 b- defN 24-Mar-26 09:20 pycut_pursuit/cp_d1_ql1b_cpy.cpython-312-darwin.so
--rw-r--r--  2.0 unx    13560 b- defN 24-Mar-16 12:48 pycut_pursuit/cp_prox_tv.py
--rwxr-xr-x  2.0 unx   726920 b- defN 24-Mar-26 09:20 pycut_pursuit/cp_prox_tv_cpy.cpython-312-darwin.so
--rw-r--r--  2.0 unx    35149 b- defN 24-Mar-26 09:20 pycut_pursuit-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    61831 b- defN 24-Mar-26 09:20 pycut_pursuit-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Mar-26 09:20 pycut_pursuit-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-Mar-26 09:20 pycut_pursuit-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1272 b- defN 24-Mar-26 09:20 pycut_pursuit-0.1.2.dist-info/RECORD
-14 files, 3111161 bytes uncompressed, 816689 bytes compressed:  73.8%
+Zip file size: 7349275 bytes, number of entries: 20
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-12 09:37 pycut_pursuit/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-12 09:37 pycut_pursuit-0.1.3.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-12 09:37 pycut_pursuit.libs/
+-rw-r--r--  2.0 unx    15702 b- defN 24-Apr-12 09:37 pycut_pursuit/cp_d1_ql1b.py
+-rwxr-xr-x  2.0 unx  8358497 b- defN 24-Apr-12 09:37 pycut_pursuit/cp_d1_lsx_cpy.cpython-312-x86_64-linux-musl.so
+-rwxr-xr-x  2.0 unx  7553121 b- defN 24-Apr-12 09:37 pycut_pursuit/cp_d0_dist_cpy.cpython-312-x86_64-linux-musl.so
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-12 09:37 pycut_pursuit/__init__.py
+-rwxr-xr-x  2.0 unx  6144345 b- defN 24-Apr-12 09:37 pycut_pursuit/cp_prox_tv_cpy.cpython-312-x86_64-linux-musl.so
+-rw-r--r--  2.0 unx    15221 b- defN 24-Apr-12 09:37 pycut_pursuit/cp_d0_dist.py
+-rw-r--r--  2.0 unx    13560 b- defN 24-Apr-12 09:37 pycut_pursuit/cp_prox_tv.py
+-rwxr-xr-x  2.0 unx  6697281 b- defN 24-Apr-12 09:37 pycut_pursuit/cp_d1_ql1b_cpy.cpython-312-x86_64-linux-musl.so
+-rw-r--r--  2.0 unx    14646 b- defN 24-Apr-12 09:37 pycut_pursuit/cp_d1_lsx.py
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-12 09:37 pycut_pursuit-0.1.3.dist-info/top_level.txt
+-rw-r--r--  2.0 unx    62312 b- defN 24-Apr-12 09:37 pycut_pursuit-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      113 b- defN 24-Apr-12 09:37 pycut_pursuit-0.1.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     1646 b- defN 24-Apr-12 09:37 pycut_pursuit-0.1.3.dist-info/RECORD
+-rw-r--r--  2.0 unx    35149 b- defN 24-Apr-12 09:37 pycut_pursuit-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    81257 b- defN 24-Apr-12 09:37 pycut_pursuit.libs/libgcc_s-a04fdf82.so.1
+-rwxr-xr-x  2.0 unx   187009 b- defN 24-Apr-12 09:37 pycut_pursuit.libs/libgomp-cd951527.so.1.0.0
+-rwxr-xr-x  2.0 unx  2447393 b- defN 24-Apr-12 09:37 pycut_pursuit.libs/libstdc++-a9383cce.so.6.0.28
+20 files, 31627266 bytes uncompressed, 7346215 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -1,43 +1,61 @@
-Filename: pycut_pursuit/__init__.py
+Filename: pycut_pursuit/
 Comment: 
 
-Filename: pycut_pursuit/cp_d0_dist.py
+Filename: pycut_pursuit-0.1.3.dist-info/
 Comment: 
 
-Filename: pycut_pursuit/cp_d0_dist_cpy.cpython-312-darwin.so
+Filename: pycut_pursuit.libs/
 Comment: 
 
-Filename: pycut_pursuit/cp_d1_lsx.py
+Filename: pycut_pursuit/cp_d1_ql1b.py
 Comment: 
 
-Filename: pycut_pursuit/cp_d1_lsx_cpy.cpython-312-darwin.so
+Filename: pycut_pursuit/cp_d1_lsx_cpy.cpython-312-x86_64-linux-musl.so
 Comment: 
 
-Filename: pycut_pursuit/cp_d1_ql1b.py
+Filename: pycut_pursuit/cp_d0_dist_cpy.cpython-312-x86_64-linux-musl.so
+Comment: 
+
+Filename: pycut_pursuit/__init__.py
+Comment: 
+
+Filename: pycut_pursuit/cp_prox_tv_cpy.cpython-312-x86_64-linux-musl.so
 Comment: 
 
-Filename: pycut_pursuit/cp_d1_ql1b_cpy.cpython-312-darwin.so
+Filename: pycut_pursuit/cp_d0_dist.py
 Comment: 
 
 Filename: pycut_pursuit/cp_prox_tv.py
 Comment: 
 
-Filename: pycut_pursuit/cp_prox_tv_cpy.cpython-312-darwin.so
+Filename: pycut_pursuit/cp_d1_ql1b_cpy.cpython-312-x86_64-linux-musl.so
+Comment: 
+
+Filename: pycut_pursuit/cp_d1_lsx.py
+Comment: 
+
+Filename: pycut_pursuit-0.1.3.dist-info/top_level.txt
+Comment: 
+
+Filename: pycut_pursuit-0.1.3.dist-info/METADATA
+Comment: 
+
+Filename: pycut_pursuit-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pycut_pursuit-0.1.2.dist-info/LICENSE
+Filename: pycut_pursuit-0.1.3.dist-info/RECORD
 Comment: 
 
-Filename: pycut_pursuit-0.1.2.dist-info/METADATA
+Filename: pycut_pursuit-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: pycut_pursuit-0.1.2.dist-info/WHEEL
+Filename: pycut_pursuit.libs/libgcc_s-a04fdf82.so.1
 Comment: 
 
-Filename: pycut_pursuit-0.1.2.dist-info/top_level.txt
+Filename: pycut_pursuit.libs/libgomp-cd951527.so.1.0.0
 Comment: 
 
-Filename: pycut_pursuit-0.1.2.dist-info/RECORD
+Filename: pycut_pursuit.libs/libstdc++-a9383cce.so.6.0.28
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `pycut_pursuit-0.1.2.dist-info/LICENSE` & `pycut_pursuit-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pycut_pursuit-0.1.2.dist-info/METADATA` & `pycut_pursuit-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycut-pursuit
-Version: 0.1.2
+Version: 0.1.3
 Summary: cut pursuit algorithms
 Author-email: Hugo Raguet <hugo.raguet@insa-cvl.fr>, Loic Landrieu <loic.landrieu@enpc.fr>
 Maintainer-email: Hugo Raguet <hugo.raguet@insa-cvl.fr>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -685,15 +685,27 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Cut-Pursuit Algorithms, Parallelized Along Components
+# Cut-Pursuit Algorithms, Parallelized Along Components (fork)
+
+## About this fork
+
+The original code in available in this repository. https://gitlab.com/1a7r0ch3/parallel-cut-pursuit.
+
+This a fork for python packaging purposes.
+
+Please post issues in this repos only if you are sure your problem is related to the packaging... and please post issue on the upstream repository __only__ if you are sure your problem is not related to the packaging.
+
+See below the original README (only the python section was modified)
+
+# Original README
 
 Generic C++ classes for implementing cut-pursuit algorithms.  
 Specialization to convex problems involving **graph total variation**, and nonconvex problems involving **contour length**, as explained in our articles [(Landrieu and Obozinski, 2016; Raguet and Landrieu, 2018)](#references).   
 Parallel implementation with OpenMP.  
 MEX interfaces for GNU Octave or Matlab.  
 Extension modules for Python.
```

## Comparing `pycut_pursuit-0.1.2.dist-info/RECORD` & `pycut_pursuit-0.1.3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-pycut_pursuit/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pycut_pursuit/cp_d0_dist.py,sha256=WJtZAdwEKelRzzl4ECDP5tYqMPEahnVVWT75XiZwvtI,15221
-pycut_pursuit/cp_d0_dist_cpy.cpython-312-darwin.so,sha256=di2FaHlULF10Cx9h-XpPa7RF4RCwj5MXhmhGZGHUwXM,448504
-pycut_pursuit/cp_d1_lsx.py,sha256=Jf_QHDx2rwS7Mm0reQwfxEfVu3aPr1h8wBwzm6a26H0,14646
-pycut_pursuit/cp_d1_lsx_cpy.cpython-312-darwin.so,sha256=XwjNrCDIru2tiMrV7FbFBoaiURsO0urnxvHSAxkIAoQ,857280
-pycut_pursuit/cp_d1_ql1b.py,sha256=Qagjl8kJoedq5-CzNBAXlsjWZNMg4Mp9c5ikllwu5_s,15702
-pycut_pursuit/cp_d1_ql1b_cpy.cpython-312-darwin.so,sha256=Jyj2cMa0HRVDsnKL-R4a-DZ_VHM2iVSZCTKAmzKmR_k,920952
-pycut_pursuit/cp_prox_tv.py,sha256=-CdlZ5ekJiaX8Y5wAdTb3CZjY6U53xCiSfyJROt5Hbs,13560
-pycut_pursuit/cp_prox_tv_cpy.cpython-312-darwin.so,sha256=b04wcVeqgnTV98VN4K_6LakxPe3LM8olj-4wJQImcX8,726920
-pycut_pursuit-0.1.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-pycut_pursuit-0.1.2.dist-info/METADATA,sha256=f1FCK_tsG8C4GIfoWa3usSuZ80NRxOTbiHRXWpX82Rc,61831
-pycut_pursuit-0.1.2.dist-info/WHEEL,sha256=7JDuPzVOv4CZsKy48sNdyhB46r1YWjorSeGtQr_7vOg,110
-pycut_pursuit-0.1.2.dist-info/top_level.txt,sha256=WfCj7iWfmdlP04bcobqvtlB_ALvbiw8qb2UXGc0RXfg,14
-pycut_pursuit-0.1.2.dist-info/RECORD,,
+pycut_pursuit/cp_d1_ql1b.py,sha256=Qagjl8kJoedq5-CzNBAXlsjWZNMg4Mp9c5ikllwu5_s,15702
+pycut_pursuit/cp_d1_lsx_cpy.cpython-312-x86_64-linux-musl.so,sha256=FHqH7szxWtlGo5RTCZ5G1ZEG6OKIyzRlI3BpNRDqCro,8358497
+pycut_pursuit/cp_d0_dist_cpy.cpython-312-x86_64-linux-musl.so,sha256=Eu-1CJJlZZdzhQyNl3FUiWaptZRp6uqcjqIMfz_Qkd4,7553121
+pycut_pursuit/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+pycut_pursuit/cp_prox_tv_cpy.cpython-312-x86_64-linux-musl.so,sha256=QKCu_DwrgcKwfqSrVTo22669Io5KSNFmanOeUJiFDkc,6144345
+pycut_pursuit/cp_d0_dist.py,sha256=WJtZAdwEKelRzzl4ECDP5tYqMPEahnVVWT75XiZwvtI,15221
+pycut_pursuit/cp_prox_tv.py,sha256=-CdlZ5ekJiaX8Y5wAdTb3CZjY6U53xCiSfyJROt5Hbs,13560
+pycut_pursuit/cp_d1_ql1b_cpy.cpython-312-x86_64-linux-musl.so,sha256=hLEZmNeUZYYx2PBrO4ah-jCeAz89BoV2c_o-wXZRZJk,6697281
+pycut_pursuit/cp_d1_lsx.py,sha256=Jf_QHDx2rwS7Mm0reQwfxEfVu3aPr1h8wBwzm6a26H0,14646
+pycut_pursuit-0.1.3.dist-info/top_level.txt,sha256=WfCj7iWfmdlP04bcobqvtlB_ALvbiw8qb2UXGc0RXfg,14
+pycut_pursuit-0.1.3.dist-info/METADATA,sha256=MSuOIKUpZbPBO0t4v2B5tVBnIslIYgrKQ0T-BhR8l70,62312
+pycut_pursuit-0.1.3.dist-info/WHEEL,sha256=u3WJvwcnUGXBzVB5YEzh4MIq4CvlLxbaEALwCGrbBH8,113
+pycut_pursuit-0.1.3.dist-info/RECORD,,
+pycut_pursuit-0.1.3.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+pycut_pursuit.libs/libgcc_s-a04fdf82.so.1,sha256=YxqJNaesQMhDswHEQpXsiLnVvMBBbYO6KYMDZFPWKSM,81257
+pycut_pursuit.libs/libgomp-cd951527.so.1.0.0,sha256=U2zda7o5P6DwCQHNyzt7Hw13pk9wKHfh-c4ZgCzbfsU,187009
+pycut_pursuit.libs/libstdc++-a9383cce.so.6.0.28,sha256=Wy9UCdwS1rwI9GU5e7qE61S0AkRqqwti1q_adWSs-Rk,2447393
```

