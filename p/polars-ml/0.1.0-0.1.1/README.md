# Comparing `tmp/polars_ml-0.1.0-cp38-abi3-win_amd64.whl.zip` & `tmp/polars_ml-0.1.1-cp38-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,15 @@
-Zip file size: 2693758 bytes, number of entries: 8
--rw-r--r--  4.6 unx      289 b- defN 24-Feb-16 11:42 polars_ml-0.1.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-Feb-16 11:42 polars_ml-0.1.0.dist-info/WHEEL
--rw-r--r--  4.6 unx      422 b- defN 24-Feb-16 11:42 polars_ml/nltk/functions.py
--rw-r--r--  4.6 unx      496 b- defN 24-Feb-16 11:42 polars_ml/nltk/nltk_namespace.py
--rw-r--r--  4.6 unx      109 b- defN 24-Feb-16 11:42 polars_ml/nltk/__init__.py
--rw-r--r--  4.6 unx       23 b- defN 24-Feb-16 11:42 polars_ml/__init__.py
--rwxr-xr-x  4.6 unx 11052544 b- defN 24-Feb-16 11:42 polars_ml/polars_ml.pyd
--rw-r--r--  4.6 unx      624 b- defN 24-Feb-16 11:42 polars_ml-0.1.0.dist-info/RECORD
-8 files, 11054601 bytes uncompressed, 2692676 bytes compressed:  75.6%
+Zip file size: 3118697 bytes, number of entries: 13
+-rw-r--r--  4.6 unx     3317 b- defN 24-Apr-12 11:32 polars_ml-0.1.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-Apr-12 11:32 polars_ml-0.1.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1068 b- defN 24-Apr-12 11:32 polars_ml-0.1.1.dist-info/license_files/LICENSE.txt
+-rw-r--r--  4.6 unx      479 b- defN 24-Apr-12 11:32 polars_ml/nltk/functions.py
+-rw-r--r--  4.6 unx      496 b- defN 24-Apr-12 11:32 polars_ml/nltk/nltk_namespace.py
+-rw-r--r--  4.6 unx      109 b- defN 24-Apr-12 11:32 polars_ml/nltk/__init__.py
+-rw-r--r--  4.6 unx       53 b- defN 24-Apr-12 11:32 polars_ml/sparse/constants.py
+-rw-r--r--  4.6 unx     1174 b- defN 24-Apr-12 11:32 polars_ml/sparse/functions.py
+-rw-r--r--  4.6 unx      502 b- defN 24-Apr-12 11:32 polars_ml/sparse/sparse_namespace.py
+-rw-r--r--  4.6 unx      126 b- defN 24-Apr-12 11:32 polars_ml/sparse/__init__.py
+-rw-r--r--  4.6 unx       48 b- defN 24-Apr-12 11:32 polars_ml/__init__.py
+-rwxr-xr-x  4.6 unx 12606976 b- defN 24-Apr-12 11:32 polars_ml/polars_ml.pyd
+-rw-r--r--  4.6 unx     1079 b- defN 24-Apr-12 11:32 polars_ml-0.1.1.dist-info/RECORD
+13 files, 12615521 bytes uncompressed, 3116889 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -1,25 +1,40 @@
-Filename: polars_ml-0.1.0.dist-info/METADATA
+Filename: polars_ml-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: polars_ml-0.1.0.dist-info/WHEEL
+Filename: polars_ml-0.1.1.dist-info/WHEEL
+Comment: 
+
+Filename: polars_ml-0.1.1.dist-info/license_files/LICENSE.txt
 Comment: 
 
 Filename: polars_ml/nltk/functions.py
 Comment: 
 
 Filename: polars_ml/nltk/nltk_namespace.py
 Comment: 
 
 Filename: polars_ml/nltk/__init__.py
 Comment: 
 
+Filename: polars_ml/sparse/constants.py
+Comment: 
+
+Filename: polars_ml/sparse/functions.py
+Comment: 
+
+Filename: polars_ml/sparse/sparse_namespace.py
+Comment: 
+
+Filename: polars_ml/sparse/__init__.py
+Comment: 
+
 Filename: polars_ml/__init__.py
 Comment: 
 
 Filename: polars_ml/polars_ml.pyd
 Comment: 
 
-Filename: polars_ml-0.1.0.dist-info/RECORD
+Filename: polars_ml-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## polars_ml/nltk/functions.py

```diff
@@ -1,15 +1,17 @@
 import os.path
-from typing import Union
 import polars as pl
 from polars.utils.udfs import _get_shared_lib_location
+from polars.plugins import register_plugin_function
+
 
 _lib = _get_shared_lib_location(os.path.dirname(__file__))
 
 
-def snowball_stem(expr: Union[str, pl.Expr], *, language: str) -> pl.Expr:
-    return expr.register_plugin(
-        lib=_lib,
-        symbol="snowball_stem",
+def snowball_stem(expr: pl.Expr, *, language: str) -> pl.Expr:
+    return register_plugin_function(
+        args=[expr],
+        plugin_path=_lib,
+        function_name='snowball_stem',
         is_elementwise=True,
-        kwargs={'language': language},
+        kwargs={'language': language}
     )
```

## polars_ml/__init__.py

```diff
@@ -1 +1,2 @@
 import polars_ml.nltk
+import polars_ml.sparse
```

