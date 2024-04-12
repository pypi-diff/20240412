# Comparing `tmp/funcnodes_pandas-0.1.1.tar.gz` & `tmp/funcnodes_pandas-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_pandas-0.1.1.tar", max compression
+gzip compressed data, was "funcnodes_pandas-0.1.2.tar", max compression
```

## Comparing `funcnodes_pandas-0.1.1.tar` & `funcnodes_pandas-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1678 2024-03-26 11:54:21.143660 funcnodes_pandas-0.1.1/funcnodes_pandas/__init__.py
--rw-r--r--   0        0        0     8482 2024-03-22 13:02:52.112318 funcnodes_pandas-0.1.1/funcnodes_pandas/dataframe.py
--rw-r--r--   0        0        0     2568 2024-03-22 12:12:52.232463 funcnodes_pandas-0.1.1/funcnodes_pandas/dataseries.py
--rw-r--r--   0        0        0      438 2024-03-26 11:54:10.287139 funcnodes_pandas-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 16:14:38.723499 funcnodes_pandas-0.1.1/README.md
--rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 funcnodes_pandas-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1722 2024-04-12 11:28:49.809772 funcnodes_pandas-0.1.2/funcnodes_pandas/__init__.py
+-rw-r--r--   0        0        0     9272 2024-04-12 10:54:18.814562 funcnodes_pandas-0.1.2/funcnodes_pandas/dataframe.py
+-rw-r--r--   0        0        0     2568 2024-03-22 12:12:52.232463 funcnodes_pandas-0.1.2/funcnodes_pandas/dataseries.py
+-rw-r--r--   0        0        0      460 2024-04-12 11:28:37.497161 funcnodes_pandas-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 16:14:38.723499 funcnodes_pandas-0.1.2/README.md
+-rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 funcnodes_pandas-0.1.2/PKG-INFO
```

### Comparing `funcnodes_pandas-0.1.1/funcnodes_pandas/__init__.py` & `funcnodes_pandas-0.1.2/funcnodes_pandas/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     GetColumnNode as get_column,
     to_orient_dict,
     from_orient_dict,
     df_iloc,
     df_loc,
     to_csv_str,
     df_from_array,
+    DfFromExcelNode,
 )
 
 from .dataseries import (
     ser_to_dict,
     ser_values,
     ser_to_list,
     ser_loc,
@@ -54,15 +55,15 @@
 FUNCNODES_RENDER_OPTIONS: fn.RenderOptions = {
     "typemap": {
         type_to_string(pd.DataFrame): "table",
         type_to_string(pd.Series): "list",
     },
 }
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 __all__ = [
     "NODE_SHELF",
     "to_dict",
     "from_dict",
     "from_csv_str",
     "get_column",
@@ -77,8 +78,9 @@
     "ser_iloc",
     "ser_from_dict",
     "ser_from_list",
     "SERIES_SHELF",
     "DF_SHELF",
     "to_csv_str",
     "df_from_array",
+    "DfFromExcelNode",
 ]
```

### Comparing `funcnodes_pandas-0.1.1/funcnodes_pandas/dataframe.py` & `funcnodes_pandas-0.1.2/funcnodes_pandas/dataframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,14 +158,41 @@
         decimal = DecimalEnum[decimal].value
     elif isinstance(decimal, DecimalEnum):  # Direct instance of DecimalEnum
         decimal = decimal.value
 
     return pandas.read_csv(StringIO(source), sep=sep, decimal=decimal)
 
 
+class DfFromExcelNode(fn.Node):
+    node_id = "pd.df_from_xlsx"
+    node_name = "From Excel"
+
+    data = fn.NodeInput(
+        id="data",
+        type=bytes,
+    )
+    sheet = fn.NodeInput(
+        id="sheet",
+        type=str,
+        default=None,
+        required=False,
+    )
+
+    df = fn.NodeOutput(id="df", type=pandas.DataFrame)
+
+    async def func(self, data: bytes, sheet: str = None):
+        # get sheet names
+        sheets = pandas.ExcelFile(data).sheet_names
+        self.inputs["sheet"].value_options = {s: s for s in sheets}
+        if sheet is None or sheet not in sheets:
+            sheet = sheets[0]
+        self.inputs["sheet"].set_value(sheet, does_trigger=False)
+        self.outputs["df"].value = pandas.read_excel(data, sheet_name=sheet)
+
+
 @fn.NodeDecorator(
     node_id="pd.df_to_csv_str",
     name="To CSV",
     description="Writes a DataFrame to a CSV string.",
     outputs=[{"name": "csv", "type": str}],
 )
 def to_csv_str(
@@ -289,12 +316,13 @@
         to_csv_str,
         GetColumnNode,
         to_orient_dict,
         from_orient_dict,
         df_loc,
         df_iloc,
         df_from_array,
+        DfFromExcelNode,
     ],
     name="Datataframe",
     description="Pandas DataFrame nodes",
     subshelves=[],
 )
```

### Comparing `funcnodes_pandas-0.1.1/funcnodes_pandas/dataseries.py` & `funcnodes_pandas-0.1.2/funcnodes_pandas/dataseries.py`

 * *Files identical despite different names*

### Comparing `funcnodes_pandas-0.1.1/PKG-INFO` & `funcnodes_pandas-0.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: funcnodes-pandas
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: funcnodes (>=0.1.10,<0.2.0)
-Requires-Dist: funcnodes-numpy (>=0.1.2,<0.2.0)
+Requires-Dist: funcnodes (>=0.1.30,<0.2.0)
+Requires-Dist: funcnodes-numpy (>=0.1.51,<0.2.0)
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
```

