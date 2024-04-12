# Comparing `tmp/lxfcode-0.2.4-py2.py3-none-any.whl.zip` & `tmp/lxfcode-0.2.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -39,12 +39,12 @@
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-12 01:49 lxf_code/calcores/raman/__init__.py
 -rw-rw-r--  2.0 unx     3396 b- defN 24-Apr-12 01:49 lxf_code/calcores/raman/raman_cal.py
 -rw-rw-r--  2.0 unx    16985 b- defN 24-Apr-12 01:49 lxf_code/calcores/raman/raman_plot.py
 -rw-rw-r--  2.0 unx     8465 b- defN 24-Apr-12 01:49 lxf_code/calcores/superlattices/TwistedGra.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-12 01:49 lxf_code/calcores/superlattices/__init__.py
 -rw-rw-r--  2.0 unx     2845 b- defN 24-Apr-12 01:49 lxf_code/calcores/superlattices/comm_stru.py
 -rw-rw-r--  2.0 unx     2448 b- defN 24-Apr-12 01:49 lxf_code/calcores/superlattices/stru_plot.py
--rw-rw-r--  2.0 unx      754 b- defN 24-Apr-12 01:58 lxfcode-0.2.4.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 24-Apr-12 01:58 lxfcode-0.2.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 24-Apr-12 01:58 lxfcode-0.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4353 b- defN 24-Apr-12 01:58 lxfcode-0.2.4.dist-info/RECORD
+-rw-rw-r--  2.0 unx      754 b- defN 24-Apr-12 02:02 lxfcode-0.2.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 24-Apr-12 02:02 lxfcode-0.2.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 24-Apr-12 02:02 lxfcode-0.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4353 b- defN 24-Apr-12 02:02 lxfcode-0.2.5.dist-info/RECORD
 48 files, 175910 bytes uncompressed, 43858 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -126,20 +126,20 @@
 
 Filename: lxf_code/calcores/superlattices/comm_stru.py
 Comment: 
 
 Filename: lxf_code/calcores/superlattices/stru_plot.py
 Comment: 
 
-Filename: lxfcode-0.2.4.dist-info/METADATA
+Filename: lxfcode-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: lxfcode-0.2.4.dist-info/WHEEL
+Filename: lxfcode-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: lxfcode-0.2.4.dist-info/top_level.txt
+Filename: lxfcode-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: lxfcode-0.2.4.dist-info/RECORD
+Filename: lxfcode-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `lxfcode-0.2.4.dist-info/METADATA` & `lxfcode-0.2.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxfcode
-Version: 0.2.4
+Version: 0.2.5
 Summary: Calculation Package for 2D Materials
 Home-page: https://github.com/Aoxv/aoxvli
 Author: Li Xiaofeng
 Author-email: 951973793@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

## Comparing `lxfcode-0.2.4.dist-info/RECORD` & `lxfcode-0.2.5.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -38,11 +38,11 @@
 lxf_code/calcores/raman/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lxf_code/calcores/raman/raman_cal.py,sha256=Mwx4dmHQQqgofmL7RAOodUtN1juSHzUV4fOy7WVR__o,3396
 lxf_code/calcores/raman/raman_plot.py,sha256=yRHEsFiOm9UpPwsJLJw_9WAtDYQDIibmuY6349Vz_pQ,16985
 lxf_code/calcores/superlattices/TwistedGra.py,sha256=ST_y8ias9Sb2cQ0HfQMbKTwqXSG_RVWqQtds5zrLbug,8465
 lxf_code/calcores/superlattices/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lxf_code/calcores/superlattices/comm_stru.py,sha256=96515Sobm_MsipZlWYCDQOgnB_t0eyhwvbog5XWdM4M,2845
 lxf_code/calcores/superlattices/stru_plot.py,sha256=CQ7_krNrH5QE60Ap44jM4NxKGSiKdmDAgTBOYXFzs7A,2448
-lxfcode-0.2.4.dist-info/METADATA,sha256=yAV04dbuDlEPv-2b5e_JvqsV69vEUbvKlwmbjiOfOck,754
-lxfcode-0.2.4.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
-lxfcode-0.2.4.dist-info/top_level.txt,sha256=lwPPuMB1Y4Wdvlf8JRMRNGCD3sNuHd-PORra1IPBDCY,9
-lxfcode-0.2.4.dist-info/RECORD,,
+lxfcode-0.2.5.dist-info/METADATA,sha256=vmkMA5LNQutsDN_kZ9zu3TMFQ3t9GI81nVtnVHfrFl8,754
+lxfcode-0.2.5.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
+lxfcode-0.2.5.dist-info/top_level.txt,sha256=lwPPuMB1Y4Wdvlf8JRMRNGCD3sNuHd-PORra1IPBDCY,9
+lxfcode-0.2.5.dist-info/RECORD,,
```

