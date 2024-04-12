# Comparing `tmp/RS2024-0.0.3-py3-none-any.whl.zip` & `tmp/RS2024-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2185 bytes, number of entries: 7
+Zip file size: 2150 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      688 b- defN 24-Apr-12 08:40 RS/RS.py
--rw-r--r--  2.0 unx      689 b- defN 24-Apr-12 08:24 RS/app.py
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-12 08:40 RS2024-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      121 b- defN 24-Apr-12 08:40 RS2024-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 08:40 RS2024-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 24-Apr-12 08:40 RS2024-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      506 b- defN 24-Apr-12 08:40 RS2024-0.0.3.dist-info/RECORD
-7 files, 2116 bytes uncompressed, 1289 bytes compressed:  39.1%
+-rw-r--r--  2.0 unx      688 b- defN 24-Apr-12 08:44 RS/app.py
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-12 08:45 RS2024-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      121 b- defN 24-Apr-12 08:45 RS2024-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 08:45 RS2024-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 24-Apr-12 08:45 RS2024-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      506 b- defN 24-Apr-12 08:45 RS2024-0.0.4.dist-info/RECORD
+7 files, 2115 bytes uncompressed, 1254 bytes compressed:  40.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: RS/RS.py
 Comment: 
 
 Filename: RS/app.py
 Comment: 
 
-Filename: RS2024-0.0.3.dist-info/LICENSE
+Filename: RS2024-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: RS2024-0.0.3.dist-info/METADATA
+Filename: RS2024-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: RS2024-0.0.3.dist-info/WHEEL
+Filename: RS2024-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: RS2024-0.0.3.dist-info/top_level.txt
+Filename: RS2024-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: RS2024-0.0.3.dist-info/RECORD
+Filename: RS2024-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## RS/app.py

```diff
@@ -1,12 +1,11 @@
 
 import re 
 import string
 
-
 def validate_email(email):
     pattern = r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$'
     if re.match(pattern, email):
         return True
     else:
         return False
```

