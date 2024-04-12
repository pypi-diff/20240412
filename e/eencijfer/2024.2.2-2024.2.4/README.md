# Comparing `tmp/eencijfer-2024.2.2.tar.gz` & `tmp/eencijfer-2024.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eencijfer-2024.2.2.tar", max compression
+gzip compressed data, was "eencijfer-2024.2.4.tar", max compression
```

## Comparing `eencijfer-2024.2.2.tar` & `eencijfer-2024.2.4.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0     1069 2024-03-27 21:22:09.552734 eencijfer-2024.2.2/LICENSE
--rw-r--r--   0        0        0      925 2024-03-27 21:22:09.552734 eencijfer-2024.2.2/README.md
--rw-r--r--   0        0        0     1807 2024-03-27 21:22:09.552734 eencijfer-2024.2.2/eencijfer/__init__.py
--rw-r--r--   0        0        0       43 2024-03-27 21:22:09.552734 eencijfer-2024.2.2/eencijfer/assets/__init__.py
--rw-r--r--   0        0        0    11868 2024-03-27 21:22:09.552734 eencijfer-2024.2.2/eencijfer/assets/cohorten.py
--rw-r--r--   0        0        0     1891 2024-03-27 21:22:09.552734 eencijfer-2024.2.2/eencijfer/assets/eencijfer.py
--rw-r--r--   0        0        0     3174 2024-03-27 21:22:09.552734 eencijfer-2024.2.2/eencijfer/assets/eindexamencijfers.py
--rw-r--r--   0        0        0        0 2024-03-27 21:22:09.552734 eencijfer-2024.2.2/eencijfer/assets/transformations/__init__py
--rw-r--r--   0        0        0     2159 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv
--rw-r--r--   0        0        0     1639 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/assets/transformations/diploma.py
--rw-r--r--   0        0        0       53 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/assets/transformations/local_data.py
--rw-r--r--   0        0        0     7712 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/assets/transformations/opleiding.py
--rw-r--r--   0        0        0     1455 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/assets/transformations/postcodes.py
--rw-r--r--   0        0        0     1756 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/assets/transformations/prestatieafspraken.py
--rw-r--r--   0        0        0     7437 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/assets/transformations/vooropleiding.py
--rw-r--r--   0        0        0     4009 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/cli.py
--rw-r--r--   0        0        0       61 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/__init__.py
--rw-r--r--   0        0        0     2712 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/column_converters.py
--rw-r--r--   0        0        0    10859 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/eencijfer.py
--rw-r--r--   0        0        0      710 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Croho.csv
--rw-r--r--   0        0        0      716 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Croho_vest.csv
--rw-r--r--   0        0        0      136 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_actuele_instelling.csv
--rw-r--r--   0        0        0      349 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_brinnummer.csv
--rw-r--r--   0        0        0      527 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv
--rw-r--r--   0        0        0      128 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_ho-inst.csv
--rw-r--r--   0        0        0      284 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_ho_ISCED.csv
--rw-r--r--   0        0        0      126 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_isat.csv
--rw-r--r--   0        0        0      213 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_land_naar_herkomstindikking.csv
--rw-r--r--   0        0        0      264 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_landcode.csv
--rw-r--r--   0        0        0      282 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_nationaliteitscode.csv
--rw-r--r--   0        0        0      191 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_postcodecijfers_2023.csv
--rw-r--r--   0        0        0      191 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_postcodecijfers_2024.csv
--rw-r--r--   0        0        0      249 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_vakcode.csv
--rw-r--r--   0        0        0      237 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_vestnr_ho.csv
--rw-r--r--   0        0        0      237 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_vestnr_ho_compleet.csv
--rw-r--r--   0        0        0      213 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_vooropl.csv
--rw-r--r--   0        0        0      140 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_vopl.csv
--rw-r--r--   0        0        0     6232 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/EV____24.csv
--rw-r--r--   0        0        0     1058 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/import_definitions/VAKHAVW_____.csv
--rw-r--r--   0        0        0     6559 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/convert/pii.py
--rw-r--r--   0        0        0     1378 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/io/file.py
--rw-r--r--   0        0        0     2049 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/settings.py
--rw-r--r--   0        0        0       33 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/utils/__init__.py
--rw-r--r--   0        0        0     4054 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/utils/detect_eencijfer_files.py
--rw-r--r--   0        0        0     2624 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/utils/init.py
--rw-r--r--   0        0        0      991 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/utils/local_data.py
--rw-r--r--   0        0        0     1944 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/eencijfer/utils/qa.py
--rw-r--r--   0        0        0     2501 2024-03-27 21:22:09.556734 eencijfer-2024.2.2/pyproject.toml
--rw-r--r--   0        0        0       39 2024-03-27 21:22:09.560734 eencijfer-2024.2.2/tests/__init__.py
--rw-r--r--   0        0        0      450 2024-03-27 21:22:09.560734 eencijfer-2024.2.2/tests/test_cli.py
--rw-r--r--   0        0        0      541 2024-03-27 21:22:09.560734 eencijfer-2024.2.2/tests/test_eencijfer.py
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 eencijfer-2024.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/LICENSE
+-rw-r--r--   0        0        0      925 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/README.md
+-rw-r--r--   0        0        0     1807 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/__init__.py
+-rw-r--r--   0        0        0    11868 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/cohorten.py
+-rw-r--r--   0        0        0     1891 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/eencijfer.py
+-rw-r--r--   0        0        0     3174 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/eindexamencijfers.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/__init__py
+-rw-r--r--   0        0        0     2159 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv
+-rw-r--r--   0        0        0     1639 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/diploma.py
+-rw-r--r--   0        0        0       53 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/local_data.py
+-rw-r--r--   0        0        0     7712 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/opleiding.py
+-rw-r--r--   0        0        0     1455 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/postcodes.py
+-rw-r--r--   0        0        0     1756 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/prestatieafspraken.py
+-rw-r--r--   0        0        0     7437 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/assets/transformations/vooropleiding.py
+-rw-r--r--   0        0        0     4196 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/cli.py
+-rw-r--r--   0        0        0       61 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/__init__.py
+-rw-r--r--   0        0        0     2712 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/column_converters.py
+-rw-r--r--   0        0        0    10853 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/eencijfer.py
+-rw-r--r--   0        0        0      710 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Croho.csv
+-rw-r--r--   0        0        0      716 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Croho_vest.csv
+-rw-r--r--   0        0        0      136 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_actuele_instelling.csv
+-rw-r--r--   0        0        0      349 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_brinnummer.csv
+-rw-r--r--   0        0        0      527 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv
+-rw-r--r--   0        0        0      128 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_ho-inst.csv
+-rw-r--r--   0        0        0      284 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_ho_ISCED.csv
+-rw-r--r--   0        0        0      126 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_isat.csv
+-rw-r--r--   0        0        0      213 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_land_naar_herkomstindikking.csv
+-rw-r--r--   0        0        0      264 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_landcode.csv
+-rw-r--r--   0        0        0      282 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_nationaliteitscode.csv
+-rw-r--r--   0        0        0      191 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_postcodecijfers_2023.csv
+-rw-r--r--   0        0        0      191 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_postcodecijfers_2024.csv
+-rw-r--r--   0        0        0      249 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_vakcode.csv
+-rw-r--r--   0        0        0      237 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_vestnr_ho.csv
+-rw-r--r--   0        0        0      237 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_vestnr_ho_compleet.csv
+-rw-r--r--   0        0        0      213 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_vooropl.csv
+-rw-r--r--   0        0        0      140 2024-04-12 15:25:52.716827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_vopl.csv
+-rw-r--r--   0        0        0     6232 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/EV____24.csv
+-rw-r--r--   0        0        0     1058 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/convert/import_definitions/VAKHAVW_____.csv
+-rw-r--r--   0        0        0     6559 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/convert/pii.py
+-rw-r--r--   0        0        0       28 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/io/__init__.py
+-rw-r--r--   0        0        0     3528 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/io/file.py
+-rw-r--r--   0        0        0     2049 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/settings.py
+-rw-r--r--   0        0        0       33 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/utils/__init__.py
+-rw-r--r--   0        0        0     4054 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/utils/detect_eencijfer_files.py
+-rw-r--r--   0        0        0     2624 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/utils/init.py
+-rw-r--r--   0        0        0      991 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/utils/local_data.py
+-rw-r--r--   0        0        0     1944 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/eencijfer/utils/qa.py
+-rw-r--r--   0        0        0     2503 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/tests/__init__.py
+-rw-r--r--   0        0        0      450 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/tests/test_cli.py
+-rw-r--r--   0        0        0      541 2024-04-12 15:25:52.720827 eencijfer-2024.2.4/tests/test_eencijfer.py
+-rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 eencijfer-2024.2.4/PKG-INFO
```

### Comparing `eencijfer-2024.2.2/LICENSE` & `eencijfer-2024.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/README.md` & `eencijfer-2024.2.4/README.md`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/__init__.py` & `eencijfer-2024.2.4/eencijfer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for eencijfer."""
 
 __author__ = """Bram Enning"""
 __email__ = 'bramenning@gmail.com'
-__version__ = '2024.2.2'
+__version__ = '2024.2.4'
 __app_name__ = 'eencijfer'
 
 import logging
 import shutil
 from importlib import import_module
 from pathlib import Path
```

### Comparing `eencijfer-2024.2.2/eencijfer/assets/cohorten.py` & `eencijfer-2024.2.4/eencijfer/assets/cohorten.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/assets/eencijfer.py` & `eencijfer-2024.2.4/eencijfer/assets/eencijfer.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/assets/eindexamencijfers.py` & `eencijfer-2024.2.4/eencijfer/assets/eindexamencijfers.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv` & `eencijfer-2024.2.4/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/assets/transformations/diploma.py` & `eencijfer-2024.2.4/eencijfer/assets/transformations/diploma.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/assets/transformations/opleiding.py` & `eencijfer-2024.2.4/eencijfer/assets/transformations/opleiding.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/assets/transformations/postcodes.py` & `eencijfer-2024.2.4/eencijfer/assets/transformations/postcodes.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/assets/transformations/prestatieafspraken.py` & `eencijfer-2024.2.4/eencijfer/assets/transformations/prestatieafspraken.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/assets/transformations/vooropleiding.py` & `eencijfer-2024.2.4/eencijfer/assets/transformations/vooropleiding.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/cli.py` & `eencijfer-2024.2.4/eencijfer/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import typer
 from typing_extensions import Annotated
 
 from eencijfer import APP_NAME, CONFIG_FILE, __version__
 from eencijfer.assets.cohorten import create_cohorten_met_indicatoren
 from eencijfer.assets.eencijfer import _create_eencijfer_df
 from eencijfer.assets.eindexamencijfers import _create_eindexamencijfer_df
-from eencijfer.convert.eencijfer import _convert_to_export_format
+from eencijfer.convert.eencijfer import _convert_to_parquet
 from eencijfer.convert.pii import _replace_all_pgn_with_pseudo_id_remove_pii_local_id
-from eencijfer.io.file import ExportFormat, _save_to_file
+from eencijfer.io.file import ExportFormat, _convert_to_export_format_remove_parquet, _save_to_file
 from eencijfer.settings import config
 from eencijfer.utils.init import _create_default_config
 from eencijfer.utils.qa import compare_eencijfer_files_and_definitions
 
 app = typer.Typer(name="eencijfer", help="ETL-tool for Dutch eencijfer", no_args_is_help=True)
 
 
@@ -73,25 +73,28 @@
 
     source_dir = config.getpath('default', 'source_dir')
 
     result_dir = config.getpath('default', 'result_dir')
     if not result_dir.is_dir():
         Path(result_dir).mkdir(parents=True, exist_ok=True)
 
-    _convert_to_export_format(
+    _convert_to_parquet(
         source_dir=source_dir,
         result_dir=result_dir,
-        export_format=export_format,
+        export_format=ExportFormat.parquet,
         use_column_converters=use_column_converters,
     )
 
     _replace_all_pgn_with_pseudo_id_remove_pii_local_id(
-        export_format=export_format, remove_pii=remove_pii, add_local_id=add_local_id
+        export_format=ExportFormat.parquet, remove_pii=remove_pii, add_local_id=add_local_id
     )
 
+    if export_format.value != 'parquet':
+        _convert_to_export_format_remove_parquet(result_dir=result_dir, export_format=export_format)
+
 
 @app.command()
 def qa():
     """Show overlap between eencijfer-files and definitions."""
     overlap = compare_eencijfer_files_and_definitions()
     typer.echo(overlap)
     typer.echo(Path().absolute())
```

### Comparing `eencijfer-2024.2.2/eencijfer/convert/column_converters.py` & `eencijfer-2024.2.4/eencijfer/convert/column_converters.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/convert/eencijfer.py` & `eencijfer-2024.2.4/eencijfer/convert/eencijfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
     except Exception as e:
         logger.warning(f"...reading of {fpath.name} failed.")
         logger.warning(f"{e}")
 
     return data
 
 
-def _convert_to_export_format(
+def _convert_to_parquet(
     source_dir: Path,
     result_dir: Path,
     export_format: ExportFormat = ExportFormat.parquet,
     use_column_converters: bool = False,
 ) -> None:
     """Saves data to the export format.
```

### Comparing `eencijfer-2024.2.2/eencijfer/convert/import_definitions/Croho.csv` & `eencijfer-2024.2.4/eencijfer/convert/import_definitions/Croho.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/convert/import_definitions/Croho_vest.csv` & `eencijfer-2024.2.4/eencijfer/convert/import_definitions/Croho_vest.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv` & `eencijfer-2024.2.4/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/convert/import_definitions/EV____24.csv` & `eencijfer-2024.2.4/eencijfer/convert/import_definitions/EV____24.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/convert/import_definitions/VAKHAVW_____.csv` & `eencijfer-2024.2.4/eencijfer/convert/import_definitions/VAKHAVW_____.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/convert/pii.py` & `eencijfer-2024.2.4/eencijfer/convert/pii.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/settings.py` & `eencijfer-2024.2.4/eencijfer/settings.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/utils/detect_eencijfer_files.py` & `eencijfer-2024.2.4/eencijfer/utils/detect_eencijfer_files.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/utils/init.py` & `eencijfer-2024.2.4/eencijfer/utils/init.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/utils/local_data.py` & `eencijfer-2024.2.4/eencijfer/utils/local_data.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/eencijfer/utils/qa.py` & `eencijfer-2024.2.4/eencijfer/utils/qa.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/pyproject.toml` & `eencijfer-2024.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "eencijfer"
-version = "2024.2.2"
+version = "2024.2.4"
 homepage = "https://github.com/enningb/eencijfer"
 description = "ETL-tool for Dutch eencijfer."
 authors = ["Bram Enning <bramenning@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -21,15 +21,15 @@
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9.0,<4.0"
 typer = {extras = ["all"], version = "^0.9.0"}
 pandas =">=2.0.0"
-numpy = ">=1.26.2"
+numpy = ">=1.26.1"
 pyarrow= "^15.0.0"
 case-converter = ">=1.1.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.12.1"
 isort = "^5.13.2"
 flake8 = "^6.1.0"
@@ -86,15 +86,15 @@
 #skip_glob = docs/conf.py
 
 
 [tool.mypy]
 disable_error_code = ["attr-defined"]
 
 [tool.bumpversion]
-current_version = "2024.2.2"
+current_version = "2024.2.4"
 commit = true
 commit_args = "--no-verify"
 tag = true
 tag_name = "{new_version}"
 allow_dirty = true
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\.(?P<dev>post)\\d+\\.dev\\d+)?"
 message = "Version updated from {current_version} to {new_version}"
@@ -110,10 +110,12 @@
 
 
 
 
 
 
 
+
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `eencijfer-2024.2.2/tests/test_eencijfer.py` & `eencijfer-2024.2.4/tests/test_eencijfer.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.2.2/PKG-INFO` & `eencijfer-2024.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eencijfer
-Version: 2024.2.2
+Version: 2024.2.4
 Summary: ETL-tool for Dutch eencijfer.
 Home-page: https://github.com/enningb/eencijfer
 License: MIT
 Author: Bram Enning
 Author-email: bramenning@gmail.com
 Requires-Python: >=3.9.0,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,15 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: case-converter (>=1.1.0)
-Requires-Dist: numpy (>=1.26.2)
+Requires-Dist: numpy (>=1.26.1)
 Requires-Dist: pandas (>=2.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # eencijfer
 [![pypi](https://img.shields.io/pypi/v/eencijfer.svg)](https://pypi.org/project/eencijfer/)
```

