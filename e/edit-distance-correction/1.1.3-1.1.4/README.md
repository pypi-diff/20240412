# Comparing `tmp/edit_distance_correction-1.1.3-py3-none-any.whl.zip` & `tmp/edit_distance_correction-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 101073 bytes, number of entries: 17
+Zip file size: 101075 bytes, number of entries: 17
 -rw-r--r--  2.0 unx      139 b- defN 24-Feb-05 09:12 edit_distance_correction/__init__.py
 -rw-r--r--  2.0 unx     1256 b- defN 24-Feb-23 02:50 edit_distance_correction/correction.csv
--rw-r--r--  2.0 unx    11816 b- defN 24-Apr-10 06:57 edit_distance_correction/correction.py
+-rw-r--r--  2.0 unx    11817 b- defN 24-Apr-12 06:50 edit_distance_correction/correction.py
 -rw-r--r--  2.0 unx     9578 b- defN 24-Mar-19 02:11 edit_distance_correction/correction_copy.py
 -rw-r--r--  2.0 unx     1089 b- defN 24-Feb-27 08:37 edit_distance_correction/heteronym.txt
 -rw-r--r--  2.0 unx     6795 b- defN 24-Mar-11 07:24 edit_distance_correction/same_stroke.txt
 -rw-r--r--  2.0 unx     1765 b- defN 24-Mar-25 11:40 edit_distance_correction/target_words
 -rw-r--r--  2.0 unx      546 b- defN 24-Mar-05 08:16 edit_distance_correction/temp.py
 -rw-r--r--  2.0 unx   305220 b- defN 24-Mar-05 02:49 edit_distance_correction/temp.txt
 -rw-r--r--  2.0 unx      391 b- defN 24-Mar-20 06:47 edit_distance_correction/test.py
 -rw-r--r--  2.0 unx     2339 b- defN 24-Mar-25 11:40 edit_distance_correction/test_file
 -rw-r--r--  2.0 unx     8819 b- defN 24-Mar-25 11:38 edit_distance_correction/utils.py
 -rw-r--r--  2.0 unx     1676 b- defN 24-Jan-25 06:28 edit_distance_correction/valid_pinyin
--rw-r--r--  2.0 unx      291 b- defN 24-Apr-10 07:07 edit_distance_correction-1.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 07:07 edit_distance_correction-1.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 24-Apr-10 07:07 edit_distance_correction-1.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1578 b- defN 24-Apr-10 07:07 edit_distance_correction-1.1.3.dist-info/RECORD
-17 files, 353415 bytes uncompressed, 98423 bytes compressed:  72.2%
+-rw-r--r--  2.0 unx      291 b- defN 24-Apr-12 06:50 edit_distance_correction-1.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 06:50 edit_distance_correction-1.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 24-Apr-12 06:50 edit_distance_correction-1.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1578 b- defN 24-Apr-12 06:50 edit_distance_correction-1.1.4.dist-info/RECORD
+17 files, 353416 bytes uncompressed, 98425 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: edit_distance_correction/utils.py
 Comment: 
 
 Filename: edit_distance_correction/valid_pinyin
 Comment: 
 
-Filename: edit_distance_correction-1.1.3.dist-info/METADATA
+Filename: edit_distance_correction-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: edit_distance_correction-1.1.3.dist-info/WHEEL
+Filename: edit_distance_correction-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: edit_distance_correction-1.1.3.dist-info/top_level.txt
+Filename: edit_distance_correction-1.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: edit_distance_correction-1.1.3.dist-info/RECORD
+Filename: edit_distance_correction-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## edit_distance_correction/correction.py

```diff
@@ -1,15 +1,15 @@
 import Levenshtein
 import edit_distance_correction.utils as utils
 import pandas as pd
 import re
 from itertools import chain
 import os
 import time
-import kenlm
+#import kenlm
 
 _get_module_path = lambda path: os.path.normpath(os.path.join(os.getcwd(),
                                                  os.path.dirname(__file__), path))
 class Corrector:
     def __init__(self):
         self.max_k = 0
         #pinyin:set(word)
```

## Comparing `edit_distance_correction-1.1.3.dist-info/RECORD` & `edit_distance_correction-1.1.4.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 edit_distance_correction/__init__.py,sha256=iEwR-MyXazzbaotC3qWLZykxG-cA4hyVlazXyWsxR2c,139
 edit_distance_correction/correction.csv,sha256=Z15Pkoxu0BqTse-b0Vx6p8VhDVRi_2ct3NjCB84OuTA,1256
-edit_distance_correction/correction.py,sha256=Q6AQXNoUgv9vJ8YUoLk-LSNAlctl3CTa35KC_YBhQBo,11816
+edit_distance_correction/correction.py,sha256=TJYdmtgse7VjGZdB3_DZ15dElhTdx9A6UmClpuQ5Ebc,11817
 edit_distance_correction/correction_copy.py,sha256=uKZjntYbrVUc695RAZMId4lnnjgihl4Vg1_c-NhvIL8,9578
 edit_distance_correction/heteronym.txt,sha256=-cGHvlDxqZm9QuTUEClUx7kLDETYZaNGc8QhJqV1kyI,1089
 edit_distance_correction/same_stroke.txt,sha256=IBODeWIgQwun_Si-cysULmEkGCKDQe1SOSG2beegIkM,6795
 edit_distance_correction/target_words,sha256=BOmPlH8n0A7xsaD8S0n9f3JCzN7nm9IHMtRJltiu1XI,1765
 edit_distance_correction/temp.py,sha256=s35J407s6ap1dkWg0AKmeL_nLM059RwcwAR-GZqcOEw,546
 edit_distance_correction/temp.txt,sha256=2l1TiLjVg9Kij3XsOg3IJhmC1hVZtimzHB_kuZvVkbY,305220
 edit_distance_correction/test.py,sha256=oG_UfMwTOEBAFlLD_N7CJzmDwvNibktFNaDR1dcR0m0,391
 edit_distance_correction/test_file,sha256=_XlLhGNIFbjfQKmkkVmCIHl-izGjhGOXUUnsLbJTy6A,2339
 edit_distance_correction/utils.py,sha256=XtywpJdMVp_50kfMyqhEYo5UBhXk3E-3HejnfICCLPc,8819
 edit_distance_correction/valid_pinyin,sha256=6EqB5E8P3jAIukFOBvQtagZ4DCqQCjemjwo2bykSpJc,1676
-edit_distance_correction-1.1.3.dist-info/METADATA,sha256=Nq2gz45IXu7TraOUW0OvvuaKGkmgvtC-FqCsrBmR41I,291
-edit_distance_correction-1.1.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-edit_distance_correction-1.1.3.dist-info/top_level.txt,sha256=GzUwTYJvGTyxnBCc_IqRXlNzEQr5gg0oQ96jXfgwu2s,25
-edit_distance_correction-1.1.3.dist-info/RECORD,,
+edit_distance_correction-1.1.4.dist-info/METADATA,sha256=UKfLQw6FZ7ZInfz816vxZDZCdIeY6pjDU245I5e5urQ,291
+edit_distance_correction-1.1.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+edit_distance_correction-1.1.4.dist-info/top_level.txt,sha256=GzUwTYJvGTyxnBCc_IqRXlNzEQr5gg0oQ96jXfgwu2s,25
+edit_distance_correction-1.1.4.dist-info/RECORD,,
```

