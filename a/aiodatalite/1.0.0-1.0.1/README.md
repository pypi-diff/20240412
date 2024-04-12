# Comparing `tmp/aiodatalite-1.0.0-py3-none-any.whl.zip` & `tmp/aiodatalite-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 15356 bytes, number of entries: 12
+Zip file size: 15345 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      182 b- defN 80-Jan-01 00:00 aiodatalite/__init__.py
--rw-r--r--  2.0 unx     6222 b- defN 80-Jan-01 00:00 aiodatalite/commons.py
+-rw-r--r--  2.0 unx     6134 b- defN 80-Jan-01 00:00 aiodatalite/commons.py
 -rw-r--r--  2.0 unx      600 b- defN 80-Jan-01 00:00 aiodatalite/constraints.py
 -rw-r--r--  2.0 unx     6588 b- defN 80-Jan-01 00:00 aiodatalite/datalite_decorator.py
 -rw-r--r--  2.0 unx     8120 b- defN 80-Jan-01 00:00 aiodatalite/fetch.py
 -rw-r--r--  2.0 unx     5523 b- defN 80-Jan-01 00:00 aiodatalite/mass_actions.py
 -rw-r--r--  2.0 unx     7741 b- defN 80-Jan-01 00:00 aiodatalite/migrations.py
 -rw-r--r--  2.0 unx      830 b- defN 80-Jan-01 00:00 aiodatalite/typed.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 aiodatalite-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5557 b- defN 80-Jan-01 00:00 aiodatalite-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 aiodatalite-1.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      959 b- defN 16-Jan-01 00:00 aiodatalite-1.0.0.dist-info/RECORD
-12 files, 43483 bytes uncompressed, 13754 bytes compressed:  68.4%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 aiodatalite-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5557 b- defN 80-Jan-01 00:00 aiodatalite-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 aiodatalite-1.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx      959 b- defN 16-Jan-01 00:00 aiodatalite-1.0.1.dist-info/RECORD
+12 files, 43395 bytes uncompressed, 13743 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: aiodatalite/migrations.py
 Comment: 
 
 Filename: aiodatalite/typed.py
 Comment: 
 
-Filename: aiodatalite-1.0.0.dist-info/LICENSE
+Filename: aiodatalite-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: aiodatalite-1.0.0.dist-info/METADATA
+Filename: aiodatalite-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: aiodatalite-1.0.0.dist-info/WHEEL
+Filename: aiodatalite-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: aiodatalite-1.0.0.dist-info/RECORD
+Filename: aiodatalite-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiodatalite/commons.py

```diff
@@ -151,16 +151,14 @@
     :param type_overload: Overload the Python -> SQLDatatype table
     with a custom table, this is that custom table.
     :return: None.
     """
     sql_fields, def_params = _get_creation_data(
         class_, type_overload, type_converter=type_converter
     )
-    print(sql_fields)
-    print(def_params)
     await cursor.execute(
         f"CREATE TABLE IF NOT EXISTS {class_.__name__.lower()} ({sql_fields});",
         def_params if def_params else None,
     )
 
 
 # noinspection PyDefaultArgument
@@ -169,16 +167,14 @@
     cursor: sqlite3.Cursor,
     type_overload: Dict[Optional[type], str] = type_table,
     type_converter=_convert_type,
 ) -> None:
     sql_fields, def_params = _get_creation_data(
         class_, type_overload, type_converter=type_converter
     )
-    print(sql_fields)
-    print(def_params)
     cursor.execute(
         f"CREATE TABLE IF NOT EXISTS {class_.__name__.lower()} ({sql_fields});",
         def_params if def_params else (),
     )
 
 
 # noinspection PyDefaultArgument
```

## Comparing `aiodatalite-1.0.0.dist-info/LICENSE` & `aiodatalite-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiodatalite-1.0.0.dist-info/METADATA` & `aiodatalite-1.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodatalite
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple Python library to bind dataclasses with databases. Now asynchronous!
 Home-page: https://github.com/kotikotprojects/aiodatalite
 Author: hhh
 Author-email: shshshsh@horsefucker.org
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `aiodatalite-1.0.0.dist-info/RECORD` & `aiodatalite-1.0.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 aiodatalite/__init__.py,sha256=ynmTG-AJpNLrq4VHfhrzw6mnQv-5UEAQsSYLodVnmsU,182
-aiodatalite/commons.py,sha256=MU1mcxsuBbqqyOMYTLElCdvNQkcU-pGqNLews3mpb3g,6222
+aiodatalite/commons.py,sha256=9NA6uiNvvQ9H55IR6Cu8ygAl3GsVHG1VJSMWlkIbXyU,6134
 aiodatalite/constraints.py,sha256=EPdFBdFKNdGrRaDucHQLjCz0Tc00szmes6r8HCHRWjk,600
 aiodatalite/datalite_decorator.py,sha256=aqyWBJp6GgoAPa6eD4o0Fpgjr8tyUy_JtSm5mVwzpWY,6588
 aiodatalite/fetch.py,sha256=bzFU9UEoC3jwqkVhha-MfjxuoN5NN-SidtAeArN0d00,8120
 aiodatalite/mass_actions.py,sha256=4jon9WoQYRsW9WqxYsQqU0JZ_YBMsDrGrvMTky0FOWM,5523
 aiodatalite/migrations.py,sha256=ocSDyuNoR93iqzF-8ZrNTVhS30CvtjvMIQdWcedcZ2I,7741
 aiodatalite/typed.py,sha256=29sXc593UB30Olo9088zOeiIbm12PYsL4D1SHP4Q5Pk,830
-aiodatalite-1.0.0.dist-info/LICENSE,sha256=7qASuCdNNl2RJgmj8AMNV3sC2Z9-6TeELxc8aA6UJu0,1073
-aiodatalite-1.0.0.dist-info/METADATA,sha256=1oScilrNbHT6_S9JLf4tX3AKD2ijSG5FeFU_XtjdM3s,5557
-aiodatalite-1.0.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-aiodatalite-1.0.0.dist-info/RECORD,,
+aiodatalite-1.0.1.dist-info/LICENSE,sha256=7qASuCdNNl2RJgmj8AMNV3sC2Z9-6TeELxc8aA6UJu0,1073
+aiodatalite-1.0.1.dist-info/METADATA,sha256=vhpoN3-YeR77Q8fI53Exph-hXlNitSP-_M3UAFEKjG8,5557
+aiodatalite-1.0.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+aiodatalite-1.0.1.dist-info/RECORD,,
```

