# Comparing `tmp/OSS_Class-0.0.2-py3-none-any.whl.zip` & `tmp/OSS_Class-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 2072 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat       67 b- defN 24-Apr-12 06:58 package_oss/app.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-12 06:59 OSS_Class-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      130 b- defN 24-Apr-12 06:59 OSS_Class-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-12 06:59 OSS_Class-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-12 06:59 OSS_Class-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      468 b- defN 24-Apr-12 06:59 OSS_Class-0.0.2.dist-info/RECORD
-6 files, 1854 bytes uncompressed, 1220 bytes compressed:  34.2%
+-rw-rw-rw-  2.0 fat       69 b- defN 24-Apr-12 07:21 package_oss/app.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-12 07:22 OSS_Class-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      130 b- defN 24-Apr-12 07:22 OSS_Class-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-12 07:22 OSS_Class-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-12 07:22 OSS_Class-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      468 b- defN 24-Apr-12 07:22 OSS_Class-0.0.3.dist-info/RECORD
+6 files, 1856 bytes uncompressed, 1220 bytes compressed:  34.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: package_oss/app.py
 Comment: 
 
-Filename: OSS_Class-0.0.2.dist-info/LICENSE
+Filename: OSS_Class-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: OSS_Class-0.0.2.dist-info/METADATA
+Filename: OSS_Class-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: OSS_Class-0.0.2.dist-info/WHEEL
+Filename: OSS_Class-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: OSS_Class-0.0.2.dist-info/top_level.txt
+Filename: OSS_Class-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: OSS_Class-0.0.2.dist-info/RECORD
+Filename: OSS_Class-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## package_oss/app.py

```diff
@@ -1,4 +1,4 @@
 def plus(a,b):
   x = a+b
   return x
-print(f"정답 : {plus(x)}")
+print(f"정답 : {plus(a,b)}")
```

## Comparing `OSS_Class-0.0.2.dist-info/LICENSE` & `OSS_Class-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

