# Comparing `tmp/lapa_file_store-0.0.7.tar.gz` & `tmp/lapa_file_store-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapa_file_store-0.0.7.tar", last modified: Sat Mar 16 12:16:54 2024, max compression
+gzip compressed data, was "lapa_file_store-0.0.8.tar", last modified: Fri Apr 12 17:16:01 2024, max compression
```

## Comparing `lapa_file_store-0.0.7.tar` & `lapa_file_store-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 12:16:54.155294 lapa_file_store-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-03-16 12:16:54.155294 lapa_file_store-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-16 12:16:43.000000 lapa_file_store-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 12:16:54.155294 lapa_file_store-0.0.7/lapa_file_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 12:16:43.000000 lapa_file_store-0.0.7/lapa_file_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-16 12:16:43.000000 lapa_file_store-0.0.7/lapa_file_store/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 12:16:54.155294 lapa_file_store-0.0.7/lapa_file_store/data/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-16 12:16:43.000000 lapa_file_store-0.0.7/lapa_file_store/data/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-03-16 12:16:43.000000 lapa_file_store-0.0.7/lapa_file_store/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 12:16:54.155294 lapa_file_store-0.0.7/lapa_file_store/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-03-16 12:16:43.000000 lapa_file_store-0.0.7/lapa_file_store/utils/Helper.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 12:16:43.000000 lapa_file_store-0.0.7/lapa_file_store/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 12:16:54.155294 lapa_file_store-0.0.7/lapa_file_store.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-03-16 12:16:54.000000 lapa_file_store-0.0.7/lapa_file_store.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-16 12:16:54.000000 lapa_file_store-0.0.7/lapa_file_store.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 12:16:54.000000 lapa_file_store-0.0.7/lapa_file_store.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-16 12:16:54.000000 lapa_file_store-0.0.7/lapa_file_store.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-16 12:16:54.000000 lapa_file_store-0.0.7/lapa_file_store.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 12:16:54.155294 lapa_file_store-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-16 12:16:43.000000 lapa_file_store-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:16:01.002038 lapa_file_store-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-12 17:16:01.002038 lapa_file_store-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:16:00.998038 lapa_file_store-0.0.8/lapa_file_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/lapa_file_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/lapa_file_store/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:16:01.002038 lapa_file_store-0.0.8/lapa_file_store/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/lapa_file_store/data/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/lapa_file_store/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:16:01.002038 lapa_file_store-0.0.8/lapa_file_store/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/lapa_file_store/utils/Helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/lapa_file_store/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:16:01.002038 lapa_file_store-0.0.8/lapa_file_store.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-12 17:16:00.000000 lapa_file_store-0.0.8/lapa_file_store.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-12 17:16:00.000000 lapa_file_store-0.0.8/lapa_file_store.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:16:00.000000 lapa_file_store-0.0.8/lapa_file_store.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 17:16:00.000000 lapa_file_store-0.0.8/lapa_file_store.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 17:16:00.000000 lapa_file_store-0.0.8/lapa_file_store.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:16:01.002038 lapa_file_store-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-12 17:15:52.000000 lapa_file_store-0.0.8/setup.py
```

### Comparing `lapa_file_store-0.0.7/PKG-INFO` & `lapa_file_store-0.0.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lapa_file_store
-Version: 0.0.7
+Version: 0.0.8
 Summary: file storage layer for my personal server.
 Home-page: https://github.com/adityashetty35/lapa_file_store
 Author: Aaditya sangishetty, thePmSquare
 Author-email: adityashetty35@gmail.com, thepmsquare@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -31,14 +31,18 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.8
+
+- update import logic from lapa_database_structure.
+
 ### v0.0.7
 
 - bug fix in utils->Helper.py import.
 
 ### v0.0.6
 
 - read database configuration from config using enums from lapa database structure.
```

### Comparing `lapa_file_store-0.0.7/README.md` & `lapa_file_store-0.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.8
+
+- update import logic from lapa_database_structure.
+
 ### v0.0.7
 
 - bug fix in utils->Helper.py import.
 
 ### v0.0.6
 
 - read database configuration from config using enums from lapa database structure.
```

### Comparing `lapa_file_store-0.0.7/lapa_file_store/configuration.py` & `lapa_file_store-0.0.8/lapa_file_store/configuration.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 import os
 import sys
 
 from lapa_commons.main import read_configuration_from_file_path
-from lapa_database_structure.main import DatabasesEnum, SchemaEnum, TablesEnum
 from square_logger.main import SquareLogger
 
 try:
 
     config_file_path = (
-        os.path.dirname(os.path.abspath(__file__))
-        + os.sep
-        + "data"
-        + os.sep
-        + "config.ini"
+            os.path.dirname(os.path.abspath(__file__))
+            + os.sep
+            + "data"
+            + os.sep
+            + "config.ini"
     )
     ldict_configuration = read_configuration_from_file_path(config_file_path)
 
     # get all vars and typecast
     config_str_module_name = ldict_configuration["GENERAL"]["MODULE_NAME"]
 
     config_str_host_ip = ldict_configuration["ENVIRONMENT"]["HOST_IP"]
     config_int_host_port = int(ldict_configuration["ENVIRONMENT"]["HOST_PORT"])
 
     config_str_log_file_name = ldict_configuration["ENVIRONMENT"]["LOG_FILE_NAME"]
     config_str_local_storage_folder_path = ldict_configuration["ENVIRONMENT"][
         "LOCAL_STORAGE_PATH"
     ]
 
-    config_str_database_name = DatabasesEnum.lapa.value
-    config_str_schema_name = SchemaEnum.file_storage.value
-    config_str_file_table_name = TablesEnum.file.value
-
     # initialize logger
     global_object_square_logger = SquareLogger(config_str_log_file_name)
 except Exception as e:
     print(
         "\033[91mMissing or incorrect config.ini file.\n"
         "Error details: " + str(e) + "\033[0m"
     )
```

### Comparing `lapa_file_store-0.0.7/lapa_file_store/main.py` & `lapa_file_store-0.0.8/lapa_file_store/main.py`

 * *Files identical despite different names*

### Comparing `lapa_file_store-0.0.7/lapa_file_store/utils/Helper.py` & `lapa_file_store-0.0.8/lapa_file_store/utils/Helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from fastapi import status
 from fastapi.exceptions import HTTPException
 from lapa_database_helper.main import LAPADatabaseHelper
+from lapa_database_structure.lapa.file_storage.tables import local_string_database_name, local_string_schema_name, File
 
-from lapa_file_store.configuration import global_object_square_logger, config_str_database_name, config_str_schema_name, \
-    config_str_file_table_name
+from lapa_file_store.configuration import global_object_square_logger
 
 local_object_lapa_database_helper = LAPADatabaseHelper()
 
 
 def create_entry_in_file_store(
         file_name_with_extention: str,
         content_type: str,
@@ -16,42 +16,42 @@
         file_purpose: str,
         system_relative_path: str,
 ):
     try:
 
         data = [
             {
-                "file_name_with_extension": file_name_with_extention,
-                "file_content_type": content_type,
-                "file_system_file_name_with_extension": system_file_name_with_extension,
-                "file_system_relative_path": system_relative_path,
-                "file_storage_token": file_storage_token,
-                "file_purpose": file_purpose,
+                File.file_name_with_extension.name: file_name_with_extention,
+                File.file_content_type.name: content_type,
+                File.file_system_file_name_with_extension.name: system_file_name_with_extension,
+                File.file_system_relative_path.name: system_relative_path,
+                File.file_storage_token.name: file_storage_token,
+                File.file_purpose.name: file_purpose,
             }
         ]
 
         response = local_object_lapa_database_helper.insert_rows(
-            data, config_str_database_name, config_str_schema_name, config_str_file_table_name
+            data, local_string_database_name, local_string_schema_name, File.__tablename__
         )
 
         return response
     except Exception as e:
         raise e
 
 
 def get_file_row(file_storage_token):
     try:
 
-        filters = {"file_storage_token": file_storage_token}
+        filters = {File.file_storage_token.name: file_storage_token}
 
         response = local_object_lapa_database_helper.get_rows(
             filters,
-            config_str_database_name,
-            config_str_schema_name,
-            config_str_file_table_name,
+            local_string_database_name,
+            local_string_schema_name,
+            File.__tablename__,
             ignore_filters_and_get_all=False,
         )
         if isinstance(response, list) and len(response) == 1 and response[0]:
             return response[0]
         elif len(response) > 1:
             global_object_square_logger.logger.warning(
                 f"Multiple files with same file_storage_token: {file_storage_token}"
```

### Comparing `lapa_file_store-0.0.7/lapa_file_store.egg-info/PKG-INFO` & `lapa_file_store-0.0.8/lapa_file_store.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lapa-file-store
-Version: 0.0.7
+Version: 0.0.8
 Summary: file storage layer for my personal server.
 Home-page: https://github.com/adityashetty35/lapa_file_store
 Author: Aaditya sangishetty, thePmSquare
 Author-email: adityashetty35@gmail.com, thepmsquare@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -31,14 +31,18 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.8
+
+- update import logic from lapa_database_structure.
+
 ### v0.0.7
 
 - bug fix in utils->Helper.py import.
 
 ### v0.0.6
 
 - read database configuration from config using enums from lapa database structure.
```

### Comparing `lapa_file_store-0.0.7/setup.py` & `lapa_file_store-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 package_name = "lapa_file_store"
 
 setup(
     name=package_name,
-    version="0.0.7",
+    version="0.0.8",
     packages=find_packages(),
     package_data={
         package_name: ["data/*", "pydantic_models/*"],
     },
     install_requires=[
         "uvicorn>=0.24.0.post1",
         "fastapi>=0.104.1",
```

