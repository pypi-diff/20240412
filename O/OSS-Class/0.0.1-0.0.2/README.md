# Comparing `tmp/OSS_Class-0.0.1-py3-none-any.whl.zip` & `tmp/OSS_Class-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2058 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat       48 b- defN 24-Apr-03 01:23 package_oss/app.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-03 01:51 OSS_Class-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      130 b- defN 24-Apr-03 01:51 OSS_Class-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-03 01:51 OSS_Class-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-03 01:51 OSS_Class-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      468 b- defN 24-Apr-03 01:51 OSS_Class-0.0.1.dist-info/RECORD
-6 files, 1835 bytes uncompressed, 1206 bytes compressed:  34.3%
+Zip file size: 2072 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat       67 b- defN 24-Apr-12 06:58 package_oss/app.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-12 06:59 OSS_Class-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      130 b- defN 24-Apr-12 06:59 OSS_Class-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-12 06:59 OSS_Class-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-12 06:59 OSS_Class-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      468 b- defN 24-Apr-12 06:59 OSS_Class-0.0.2.dist-info/RECORD
+6 files, 1854 bytes uncompressed, 1220 bytes compressed:  34.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: package_oss/app.py
 Comment: 
 
-Filename: OSS_Class-0.0.1.dist-info/LICENSE
+Filename: OSS_Class-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: OSS_Class-0.0.1.dist-info/METADATA
+Filename: OSS_Class-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: OSS_Class-0.0.1.dist-info/WHEEL
+Filename: OSS_Class-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: OSS_Class-0.0.1.dist-info/top_level.txt
+Filename: OSS_Class-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: OSS_Class-0.0.1.dist-info/RECORD
+Filename: OSS_Class-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## package_oss/app.py

```diff
@@ -1,3 +1,4 @@
 def plus(a,b):
-  return a + b
-print(plus(5,2))
+  x = a+b
+  return x
+print(f"정답 : {plus(x)}")
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `OSS_Class-0.0.1.dist-info/LICENSE` & `OSS_Class-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

