# Comparing `tmp/dserver-0.2.5-py3-none-any.whl.zip` & `tmp/dserver-0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 17779 bytes, number of entries: 18
+Zip file size: 17781 bytes, number of entries: 18
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-08 07:45 dserver/__init__.py
 -rw-r--r--  2.0 unx      169 b- defN 24-Jan-11 06:36 dserver/__main__.py
 -rw-r--r--  2.0 unx     6215 b- defN 24-Feb-26 03:00 dserver/main.py
 -rw-r--r--  2.0 unx      871 b- defN 24-Jan-11 06:36 dserver/utils.py
 -rw-r--r--  2.0 unx       42 b- defN 24-Jan-08 07:42 sserver/__init__.py
 -rw-r--r--  2.0 unx      169 b- defN 24-Jan-11 06:36 sserver/__main__.py
 -rw-r--r--  2.0 unx      914 b- defN 24-Mar-14 08:40 sserver/filters.py
 -rw-r--r--  2.0 unx     9928 b- defN 24-Mar-18 06:53 sserver/main.py
 -rw-r--r--  2.0 unx     2891 b- defN 24-Mar-14 08:40 sserver/model.py
 -rw-r--r--  2.0 unx     1309 b- defN 24-Mar-14 09:24 sserver/utils.py
 -rw-r--r--  2.0 unx     9442 b- defN 24-Mar-15 03:34 sserver/templates/index.html
 -rw-r--r--  2.0 unx      956 b- defN 24-Jan-05 09:31 sserver/templates/media.html
 -rw-r--r--  2.0 unx     1485 b- defN 24-Jan-05 09:31 sserver/templates/message.html
 -rw-r--r--  2.0 unx    67646 b- defN 24-Jan-09 02:46 sserver/upload/favicon.ico
--rw-r--r--  2.0 unx      283 b- defN 24-Mar-18 06:54 dserver-0.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-18 06:54 dserver-0.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Mar-18 06:54 dserver-0.2.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1370 b- defN 24-Mar-18 06:54 dserver-0.2.5.dist-info/RECORD
-18 files, 103798 bytes uncompressed, 15565 bytes compressed:  85.0%
+-rw-r--r--  2.0 unx      283 b- defN 24-Apr-12 15:22 dserver-0.2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 15:22 dserver-0.2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-12 15:22 dserver-0.2.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1370 b- defN 24-Apr-12 15:22 dserver-0.2.6.dist-info/RECORD
+18 files, 103798 bytes uncompressed, 15567 bytes compressed:  85.0%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: sserver/templates/message.html
 Comment: 
 
 Filename: sserver/upload/favicon.ico
 Comment: 
 
-Filename: dserver-0.2.5.dist-info/METADATA
+Filename: dserver-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: dserver-0.2.5.dist-info/WHEEL
+Filename: dserver-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: dserver-0.2.5.dist-info/top_level.txt
+Filename: dserver-0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: dserver-0.2.5.dist-info/RECORD
+Filename: dserver-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `dserver-0.2.5.dist-info/RECORD` & `dserver-0.2.6.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 sserver/main.py,sha256=ZIW5nRJb9_1xSmd25eDNbZHl2_kEdRxjXJZfrDikkHs,9928
 sserver/model.py,sha256=N3zWoSTuSsm_O0Ba3t9YIJJF1nZ_FvG1VH7Mj7JcIEA,2891
 sserver/utils.py,sha256=aZE_gPDK3EQi59m3e6U6EBTxyoc4-qiLEF42Y3m9w_4,1309
 sserver/templates/index.html,sha256=Y_1tucpIBR9p9IiRY3jvCg8HLcE5mMmMd1EJnlipGzM,9442
 sserver/templates/media.html,sha256=XORUp0Wj-kq8L5oNLuLe7VxiVnL4Qn8wHMN5w0GyDI8,956
 sserver/templates/message.html,sha256=sP3TlrScBuH19Nm7WLkLabD4DDmM3Ynk-ZL189NgIvM,1485
 sserver/upload/favicon.ico,sha256=Tgs5rN3sYkx3KXC2GfEy5ggUldH-I_nH6bR27A8-CUo,67646
-dserver-0.2.5.dist-info/METADATA,sha256=gwo3RwwSuZMsHTWCVvt2qhpTeWBp30lNAJZl3JrOfhk,283
-dserver-0.2.5.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-dserver-0.2.5.dist-info/top_level.txt,sha256=N-vaTOxCZp44JisKy4P3VbvVjobIuHmAEBTH706kCvo,16
-dserver-0.2.5.dist-info/RECORD,,
+dserver-0.2.6.dist-info/METADATA,sha256=6ihPIbHdAY2w5XMRRHUEvXqa5XRZQIfZs95XmRsFcGo,283
+dserver-0.2.6.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+dserver-0.2.6.dist-info/top_level.txt,sha256=N-vaTOxCZp44JisKy4P3VbvVjobIuHmAEBTH706kCvo,16
+dserver-0.2.6.dist-info/RECORD,,
```

