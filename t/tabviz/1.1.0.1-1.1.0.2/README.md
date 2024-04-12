# Comparing `tmp/tabviz-1.1.0.1.tar.gz` & `tmp/tabviz-1.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabviz-1.1.0.1.tar", max compression
+gzip compressed data, was "tabviz-1.1.0.2.tar", max compression
```

## Comparing `tabviz-1.1.0.1.tar` & `tabviz-1.1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35821 2024-03-17 16:39:19.651924 tabviz-1.1.0.1/LICENSE
--rw-r--r--   0        0        0     8615 2024-04-08 17:43:17.025130 tabviz-1.1.0.1/pyproject.toml
--rw-r--r--   0        0        0      409 2024-04-08 17:44:11.421254 tabviz-1.1.0.1/README.md
--rw-r--r--   0        0        0        0 2024-03-19 00:43:43.742786 tabviz-1.1.0.1/tabviz/__init__.py
--rw-r--r--   0        0        0    14555 2024-03-19 04:18:25.864918 tabviz-1.1.0.1/tabviz/__main__.py
--rw-r--r--   0        0        0   149794 2024-03-14 20:44:18.566877 tabviz-1.1.0.1/tabviz/static/example.twbx
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 tabviz-1.1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-03-17 16:39:19.651924 tabviz-1.1.0.2/LICENSE
+-rw-r--r--   0        0        0     8615 2024-04-12 13:40:42.819206 tabviz-1.1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      409 2024-04-08 17:44:11.421254 tabviz-1.1.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 00:43:43.742786 tabviz-1.1.0.2/tabviz/__init__.py
+-rw-r--r--   0        0        0    14563 2024-04-12 13:40:34.778261 tabviz-1.1.0.2/tabviz/__main__.py
+-rw-r--r--   0        0        0   149794 2024-03-14 20:44:18.566877 tabviz-1.1.0.2/tabviz/static/example.twbx
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 tabviz-1.1.0.2/PKG-INFO
```

### Comparing `tabviz-1.1.0.1/LICENSE` & `tabviz-1.1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.1/pyproject.toml` & `tabviz-1.1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tabviz"
-version = "1.1.0.1"
+version = "1.1.0.2"
 description = "A Python module for working with the Tableau"
 authors = ["Ayush Dhiman <ayushdhiman272@gmail.com>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `tabviz-1.1.0.1/tabviz/__main__.py` & `tabviz-1.1.0.2/tabviz/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,29 +319,29 @@
     replace_data_in_csv(csv_file,dataset)
     erv = extract_random_values(csv_file)
     run_generative_model(api_key,erv,table_contents)
     run_with_api_key(api_key,erv,table_contents_column,xml_column_data)
     replace_table_contents_with_xml_data(xml_file, xml_Data)
     replace_table_contents_with_xml_data_for_columns(xml_file,xml_column_data)
     process_file_repack(tabviz_folder)
+    workbook_name = generate_random_text(5)
     url = construct_url(site, site_id, workbook_name)
-    publish_workbook(token_name,token_secret, site_id, project_id, workbook_name, path_to_workbook,site)
+    publish_workbook(token_name,token_secret, site_id, project_id, workbook_name, path_to_workbook,site,txt)
     display_tableau_viz(url)
 
 project_id = " "
 destination_file = os.path.join(tabviz_folder, "example.twbx")
 xml_file = os.path.join(tabviz_folder, "tabviz","example.xml")
 dataset = os.path.join(tabviz_folder, "tabviz", "Data", "1vib26g1r4ena71b8a85o12srz3b", "Product.csv")
 path_to_workbook = os.path.join(tabviz_folder, "..", "Data.twbx")
 table_contents = ""
 table_contents_column = ""
 xml_column_data = ' '
 xml_Data = " "
 api_version = '3.22'
-workbook_name = generate_random_text(5)
 path_to_workbook = os.path.join(tabviz_folder, "..", "Data.twbx")
 
 #ENVS
 site_id = os.getenv('site_id')
 site = os.getenv('site')
 token_name = os.getenv('token_name')
 token_secret = os.getenv('token_secret')
```

### Comparing `tabviz-1.1.0.1/tabviz/static/example.twbx` & `tabviz-1.1.0.2/tabviz/static/example.twbx`

 * *Files identical despite different names*

### Comparing `tabviz-1.1.0.1/PKG-INFO` & `tabviz-1.1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabviz
-Version: 1.1.0.1
+Version: 1.1.0.2
 Summary: A Python module for working with the Tableau
 License: GNU
 Author: Ayush Dhiman
 Author-email: ayushdhiman272@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

