# Comparing `tmp/anyon-4.1.7-cp312-none-win_amd64.whl.zip` & `tmp/anyon-4.1.8-cp311-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 469652 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-12 01:39 anyon-4.1.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2334 b- defN 24-Apr-12 01:39 anyon-4.1.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-12 01:39 anyon-4.1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-12 01:39 anyon-4.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      376 b- defN 24-Apr-12 01:39 anyon-4.1.7.dist-info/RECORD
--rw-rw-rw-  2.0 fat    20992 b- defN 24-Apr-12 01:39 anyon/__init__.pyd
--rw-rw-rw-  2.0 fat    96256 b- defN 24-Apr-12 01:39 anyon/loader.pyd
--rw-rw-rw-  2.0 fat   121344 b- defN 24-Apr-12 01:39 anyon/remote.pyd
--rw-rw-rw-  2.0 fat   230912 b- defN 24-Apr-12 01:39 anyon/server.pyd
--rw-rw-rw-  2.0 fat    22016 b- defN 24-Apr-12 01:39 anyon/stage/__init__.pyd
--rw-rw-rw-  2.0 fat   251904 b- defN 24-Apr-12 01:39 anyon/stage/assembler.pyd
--rw-rw-rw-  2.0 fat   100352 b- defN 24-Apr-12 01:39 anyon/stage/calculator.pyd
--rw-rw-rw-  2.0 fat   140288 b- defN 24-Apr-12 01:39 anyon/stage/device.pyd
--rw-rw-rw-  2.0 fat    67584 b- defN 24-Apr-12 01:39 anyon/stage/processor.pyd
-14 files, 1055544 bytes uncompressed, 467892 bytes compressed:  55.7%
+Zip file size: 475013 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-12 08:01 anyon-4.1.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2344 b- defN 24-Apr-12 08:01 anyon-4.1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-12 08:01 anyon-4.1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-12 08:01 anyon-4.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      376 b- defN 24-Apr-12 08:01 anyon-4.1.8.dist-info/RECORD
+-rw-rw-rw-  2.0 fat    20480 b- defN 24-Apr-12 08:01 anyon/__init__.pyd
+-rw-rw-rw-  2.0 fat    96768 b- defN 24-Apr-12 08:01 anyon/loader.pyd
+-rw-rw-rw-  2.0 fat   121856 b- defN 24-Apr-12 08:01 anyon/remote.pyd
+-rw-rw-rw-  2.0 fat   220160 b- defN 24-Apr-12 08:01 anyon/server.pyd
+-rw-rw-rw-  2.0 fat    21504 b- defN 24-Apr-12 08:01 anyon/stage/__init__.pyd
+-rw-rw-rw-  2.0 fat   245248 b- defN 24-Apr-12 08:01 anyon/stage/assembler.pyd
+-rw-rw-rw-  2.0 fat    97792 b- defN 24-Apr-12 08:01 anyon/stage/calculator.pyd
+-rw-rw-rw-  2.0 fat   138240 b- defN 24-Apr-12 08:01 anyon/stage/device.pyd
+-rw-rw-rw-  2.0 fat    66048 b- defN 24-Apr-12 08:01 anyon/stage/processor.pyd
+14 files, 1032002 bytes uncompressed, 473253 bytes compressed:  54.1%
```

## zipnote {}

```diff
@@ -1,20 +1,20 @@
-Filename: anyon-4.1.7.dist-info/LICENSE
+Filename: anyon-4.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: anyon-4.1.7.dist-info/METADATA
+Filename: anyon-4.1.8.dist-info/METADATA
 Comment: 
 
-Filename: anyon-4.1.7.dist-info/WHEEL
+Filename: anyon-4.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: anyon-4.1.7.dist-info/top_level.txt
+Filename: anyon-4.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: anyon-4.1.7.dist-info/RECORD
+Filename: anyon-4.1.8.dist-info/RECORD
 Comment: 
 
 Filename: anyon/__init__.pyd
 Comment: 
 
 Filename: anyon/loader.pyd
 Comment:
```

## Comparing `anyon-4.1.7.dist-info/LICENSE` & `anyon-4.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `anyon-4.1.7.dist-info/METADATA` & `anyon-4.1.8.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyon
-Version: 4.1.7
+Version: 4.1.8
 Summary: description
 Author-email: YL <fengyl@pku.edu.cn>
 License: MIT License
         
         Copyright (c) 2021 YL Feng
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,14 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy >=1.20.0
-Requires-Dist: axion >=3.4.5
-Requires-Dist: srpc >=4.2.8
-Requires-Dist: zee >=0.0.3
-Requires-Dist: requests >=2.28.0
+Requires-Dist: numpy (>=1.20.0)
+Requires-Dist: axion (>=3.4.5)
+Requires-Dist: srpc (>=4.2.8)
+Requires-Dist: zee (>=0.0.3)
+Requires-Dist: requests (>=2.28.0)
 Requires-Dist: APScheduler
```

