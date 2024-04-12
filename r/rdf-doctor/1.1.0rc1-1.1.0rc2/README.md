# Comparing `tmp/rdf_doctor-1.1.0rc1-py3-none-any.whl.zip` & `tmp/rdf_doctor-1.1.0rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 59789 bytes, number of entries: 12
--rw-r--r--  2.0 unx       25 b- defN 24-Apr-11 00:44 doctor/__init__.py
+Zip file size: 59803 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       25 b- defN 24-Apr-12 04:53 doctor/__init__.py
 -rw-r--r--  2.0 unx     1754 b- defN 24-Mar-29 08:43 doctor/consts.py
--rw-r--r--  2.0 unx    80752 b- defN 24-Apr-11 00:43 doctor/doctor.py
+-rw-r--r--  2.0 unx    80863 b- defN 24-Apr-12 03:03 doctor/doctor.py
 -rw-r--r--  2.0 unx   134314 b- defN 24-Mar-12 04:38 doctor/reference/prefixes.tsv
 -rw-r--r--  2.0 unx       90 b- defN 24-Mar-06 07:08 doctor/reference/refine-class-uris.tsv
 -rw-r--r--  2.0 unx      577 b- defN 24-Mar-06 07:13 doctor/reference/refine-prefix-uris.tsv
--rw-r--r--  2.0 unx     1061 b- defN 24-Apr-11 01:18 rdf_doctor-1.1.0rc1.dist-info/LICENSE
--rw-r--r--  2.0 unx    10690 b- defN 24-Apr-11 01:18 rdf_doctor-1.1.0rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 01:18 rdf_doctor-1.1.0rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-Apr-11 01:18 rdf_doctor-1.1.0rc1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-11 01:18 rdf_doctor-1.1.0rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1013 b- defN 24-Apr-11 01:18 rdf_doctor-1.1.0rc1.dist-info/RECORD
-12 files, 230427 bytes uncompressed, 58073 bytes compressed:  74.8%
+-rw-r--r--  2.0 unx     1061 b- defN 24-Apr-12 04:57 rdf_doctor-1.1.0rc2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10690 b- defN 24-Apr-12 04:57 rdf_doctor-1.1.0rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 04:57 rdf_doctor-1.1.0rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-Apr-12 04:57 rdf_doctor-1.1.0rc2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-12 04:57 rdf_doctor-1.1.0rc2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1013 b- defN 24-Apr-12 04:57 rdf_doctor-1.1.0rc2.dist-info/RECORD
+12 files, 230538 bytes uncompressed, 58087 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: doctor/reference/refine-class-uris.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefix-uris.tsv
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc1.dist-info/LICENSE
+Filename: rdf_doctor-1.1.0rc2.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc1.dist-info/METADATA
+Filename: rdf_doctor-1.1.0rc2.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc1.dist-info/WHEEL
+Filename: rdf_doctor-1.1.0rc2.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc1.dist-info/entry_points.txt
+Filename: rdf_doctor-1.1.0rc2.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc1.dist-info/top_level.txt
+Filename: rdf_doctor-1.1.0rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.0rc1.dist-info/RECORD
+Filename: rdf_doctor-1.1.0rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.0rc1"
+__version__ = "1.1.0rc2"
```

## doctor/doctor.py

```diff
@@ -1103,15 +1103,16 @@
 
         if compression_mode == GZ:
             with gzip.open(input_file, "rb") as f:
                 data = f.read()
             g.parse(data=data, format=input_format)
         elif compression_mode == ZIP:
             with ZipFile(input_file, "r") as f:
-                data = f.read(Path(input_file).name.replace(".zip", "")).decode().splitlines()
+                data = f.read(Path(input_file).name.replace(".zip", "")).decode()
+            g.parse(data=data, format=input_format)
         else:
             g.parse(input_file, format=input_format)
 
         # Filter by classes(command line arguments)
         class_filter = "<" + ">, <".join(target_classes) + ">"
 
         query = """
@@ -1291,15 +1292,17 @@
                             else:
                                 # If there is no ENTITY declaration, leave the URI empty
                                 # In this case, an exception error will occur on the sheXer side.
                                 uri = ""
                         else:
                             uri = line_mod[line_mod.find("=")+1:]
 
-                        input_prefixes.append([namespace, uri])
+                        if [namespace, uri] not in input_prefixes:
+                            input_prefixes.append([namespace, uri])
+
                         for input_prefix in input_prefixes:
                             if input_prefix[0] == namespace and input_prefix[1] != uri and namespace not in duplicated_namespaces:
                                 duplicated_namespaces.append(namespace)
 
     # Detects Prefixes with duplicate Namespace and stores them in the dictionary
     for input_prefix in input_prefixes:
         if input_prefix[0] in duplicated_namespaces:
```

## Comparing `rdf_doctor-1.1.0rc1.dist-info/LICENSE` & `rdf_doctor-1.1.0rc2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-1.1.0rc1.dist-info/METADATA` & `rdf_doctor-1.1.0rc2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `rdf_doctor-1.1.0rc1.dist-info/RECORD` & `rdf_doctor-1.1.0rc2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-doctor/__init__.py,sha256=HbJ-vOkAfzbdyxN5cS2iUVQnG4gW0aAj35zU0HLa_ZU,25
+doctor/__init__.py,sha256=2DW4CDF3GisId6QRWoUv6R9Y8dfyAxXlpENtY6pGBd4,25
 doctor/consts.py,sha256=U8KOzdPFgMuf_nMul1Vw9qtAvKtZbu8WLwkiYD49IAs,1754
-doctor/doctor.py,sha256=VTULsns6uaKYz1iXmm3eLGOoo4GN_1x9mOqPL3jw6Hg,80752
+doctor/doctor.py,sha256=F46476QuaWxPNoUKP20H-CZUYTFUaeVrhLLixxlYKfw,80863
 doctor/reference/prefixes.tsv,sha256=_1hW0wBl6K1YvcM8stdiEdD4elzST_ecJqQEvhD9Auk,134314
 doctor/reference/refine-class-uris.tsv,sha256=pd_nOSjR7bia96u9hhcjhBg9J6LUAuDFlyy-JE9tsys,90
 doctor/reference/refine-prefix-uris.tsv,sha256=KY5PZ4WCaLeB0APNBjAWq7_Q5Whc6FLg9ncX7BSPeuw,577
-rdf_doctor-1.1.0rc1.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
-rdf_doctor-1.1.0rc1.dist-info/METADATA,sha256=5xCN-Mu1tKX7eVogT9rs9-MzN7BokP08pnf9VIB19Fc,10690
-rdf_doctor-1.1.0rc1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rdf_doctor-1.1.0rc1.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
-rdf_doctor-1.1.0rc1.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
-rdf_doctor-1.1.0rc1.dist-info/RECORD,,
+rdf_doctor-1.1.0rc2.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
+rdf_doctor-1.1.0rc2.dist-info/METADATA,sha256=1gso0ycDN5DIGl9Vo0PLXup2xIY-wukgP2dNMFveVCs,10690
+rdf_doctor-1.1.0rc2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rdf_doctor-1.1.0rc2.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
+rdf_doctor-1.1.0rc2.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
+rdf_doctor-1.1.0rc2.dist-info/RECORD,,
```

