# Comparing `tmp/kurumii-1.4.6.tar.gz` & `tmp/kurumii-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kurumii-1.4.6.tar", last modified: Wed Mar 27 11:53:36 2024, max compression
+gzip compressed data, was "kurumii-1.4.7.tar", last modified: Fri Apr 12 08:50:24 2024, max compression
```

## Comparing `kurumii-1.4.6.tar` & `kurumii-1.4.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 11:53:36.455620 kurumii-1.4.6/
--rw-rw-rw-   0        0        0      307 2024-03-27 11:53:36.454623 kurumii-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 kurumii-1.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 11:53:36.423706 kurumii-1.4.6/kurumii/
--rw-rw-rw-   0        0        0     3788 2024-03-27 11:43:30.000000 kurumii-1.4.6/kurumii/__init__.py
--rw-rw-rw-   0        0        0     9448 2024-03-27 11:43:23.000000 kurumii-1.4.6/kurumii/additional_functions.py
--rw-rw-rw-   0        0        0    13965 2024-03-21 08:42:39.000000 kurumii-1.4.6/kurumii/ascii.py
--rw-rw-rw-   0        0        0      812 2024-03-23 12:05:44.000000 kurumii-1.4.6/kurumii/data_manipulation.py
--rw-rw-rw-   0        0        0    18350 2024-03-27 11:52:27.000000 kurumii-1.4.6/kurumii/databases.py
--rw-rw-rw-   0        0        0     9440 2024-03-21 08:42:40.000000 kurumii-1.4.6/kurumii/files.py
--rw-rw-rw-   0        0        0     1499 2024-03-07 12:31:49.000000 kurumii-1.4.6/kurumii/id.py
--rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 kurumii-1.4.6/kurumii/jsonify.py
--rw-rw-rw-   0        0        0     5435 2024-03-20 08:56:03.000000 kurumii-1.4.6/kurumii/keyboard.py
--rw-rw-rw-   0        0        0     3797 2024-03-15 08:52:32.000000 kurumii-1.4.6/kurumii/print_additions.py
--rw-rw-rw-   0        0        0     3704 2024-03-22 09:41:46.000000 kurumii-1.4.6/kurumii/profanities.py
--rw-rw-rw-   0        0        0    17308 2024-03-16 22:17:26.000000 kurumii-1.4.6/kurumii/youtube.py
-drwxrwxrwx   0        0        0        0 2024-03-27 11:53:36.453625 kurumii-1.4.6/kurumii.egg-info/
--rw-rw-rw-   0        0        0      307 2024-03-27 11:53:36.000000 kurumii-1.4.6/kurumii.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2024-03-27 11:53:36.000000 kurumii-1.4.6/kurumii.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 11:53:36.000000 kurumii-1.4.6/kurumii.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-03-27 11:53:36.000000 kurumii-1.4.6/kurumii.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-27 11:53:36.000000 kurumii-1.4.6/kurumii.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 11:53:36.455620 kurumii-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0      387 2024-03-27 11:53:23.000000 kurumii-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:50:24.356714 kurumii-1.4.7/
+-rw-rw-rw-   0        0        0      307 2024-04-12 08:50:24.354564 kurumii-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 kurumii-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 08:50:24.302254 kurumii-1.4.7/kurumii/
+-rw-rw-rw-   0        0        0     3847 2024-04-12 08:45:13.000000 kurumii-1.4.7/kurumii/__init__.py
+-rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 kurumii-1.4.7/kurumii/additional_functions.py
+-rw-rw-rw-   0        0        0    13965 2024-04-08 07:07:29.000000 kurumii-1.4.7/kurumii/ascii.py
+-rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 kurumii-1.4.7/kurumii/data_manipulation.py
+-rw-rw-rw-   0        0        0    35843 2024-04-12 08:47:35.000000 kurumii-1.4.7/kurumii/database.py
+-rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 kurumii-1.4.7/kurumii/files.py
+-rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 kurumii-1.4.7/kurumii/id.py
+-rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 kurumii-1.4.7/kurumii/jsonify.py
+-rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 kurumii-1.4.7/kurumii/keyboard.py
+-rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 kurumii-1.4.7/kurumii/print_additions.py
+-rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 kurumii-1.4.7/kurumii/profanities.py
+-rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 kurumii-1.4.7/kurumii/youtube.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:50:24.351394 kurumii-1.4.7/kurumii.egg-info/
+-rw-rw-rw-   0        0        0      307 2024-04-12 08:50:24.000000 kurumii-1.4.7/kurumii.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2024-04-12 08:50:24.000000 kurumii-1.4.7/kurumii.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 08:50:24.000000 kurumii-1.4.7/kurumii.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-12 08:50:24.000000 kurumii-1.4.7/kurumii.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 08:50:24.000000 kurumii-1.4.7/kurumii.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 08:50:24.356714 kurumii-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      386 2024-04-12 08:49:43.000000 kurumii-1.4.7/setup.py
```

### Comparing `kurumii-1.4.6/kurumii/__init__.py` & `kurumii-1.4.7/kurumii/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import pkg_resources
-import xmlrpc.client
-import socket
-import os
+# import pkg_resources
+# import xmlrpc.client
+# import socket
+# import os
 
 
 # Function to check internet connection
 # def is_connected():
 #     try:
 #         # Connect to PyPI server to check internet connection
 #         socket.create_connection(("pypi.org", 443), timeout=1)
@@ -31,24 +31,28 @@
     editJson, loadJsonData, overwriteJson, sortJsonFile,
     validateJson, renameJson,readJson
 )
 from .additional_functions import (
     camel_to_snake, deep_copy, factorial, flatten_list, is_prime,
     is_valid_date, is_valid_email, log_error, log_info, log_warning,
     merge_dicts, read_csv, remove_whitespace, retry_func, reverse_list,
-    timer, write_to_file, unique_elements, truncate_string,validateHex
+    timer, write_to_file, unique_elements, truncate_string
 )
 from .files import (
     addFile,backupFile,createFile,deleteDataFromFile,deleteFile,editFile,
     loadDataFromFile,overwriteFile,readFile,renameFile,sortFile,validateFile
 )
 from .profanities import(has_profanity)
 from .youtube import downloadYoutube
-from .databases import(check_if_key_exists,add_to_database,backup_database,create_sqlite_db,delete_sqlite_db,edit_database_data,get_primary_key_columns,load_all_data,load_data_by_key,overwrite_database,rename_database,purge_db_data,remove_data_by_key)
-from .data_manipulation import(print_dir)
+
+from .database import(add_data_to_table,check_if_database_exists,check_if_key_exists,
+convert_to_db_format,create_sqlite_database,create_table,delete_database,unconvert,
+table_exists,edit_data_in_table,edit_table,get_primary_columns,load_all_data,load_data_from_key,
+purge_database,purge_table,remove_data_from_table,purge_database_data,remove_table)
+
 
 # if is_connected():
 #     def get_latest_version(package_name):
 #         """Get the latest version of a package from PyPI."""
 #         try:
 #             client = xmlrpc.client.ServerProxy('https://pypi.org/pypi')
 #             releases = client.package_releases(package_name)
```

### Comparing `kurumii-1.4.6/kurumii/additional_functions.py` & `kurumii-1.4.7/kurumii/additional_functions.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.6/kurumii/ascii.py` & `kurumii-1.4.7/kurumii/ascii.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.6/kurumii/data_manipulation.py` & `kurumii-1.4.7/kurumii/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.6/kurumii/files.py` & `kurumii-1.4.7/kurumii/files.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.6/kurumii/id.py` & `kurumii-1.4.7/kurumii/id.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.6/kurumii/jsonify.py` & `kurumii-1.4.7/kurumii/jsonify.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.6/kurumii/keyboard.py` & `kurumii-1.4.7/kurumii/keyboard.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.6/kurumii/print_additions.py` & `kurumii-1.4.7/kurumii/print_additions.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.6/kurumii/profanities.py` & `kurumii-1.4.7/kurumii/profanities.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.6/kurumii/youtube.py` & `kurumii-1.4.7/kurumii/youtube.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
             final = clip.fx(vfx.speedx, speed)
 
             # Save video clip
             final.write_videofile(output_filepath)
             os.remove(path=f"{output}\\{filename}")
             if logging == True:
                 print_info_("Done")
-                print_system_("Download comleted")
+                print_system_("Download completed")
             return(True, filename_edit)
     except Exception as e:
         if logging == True:
             print_red_(e)
         return(False)
```

