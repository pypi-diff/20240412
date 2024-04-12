# Comparing `tmp/lapa_database-0.0.8.tar.gz` & `tmp/lapa_database-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapa_database-0.0.8.tar", last modified: Mon Feb  5 15:57:28 2024, max compression
+gzip compressed data, was "lapa_database-0.0.9.tar", last modified: Fri Mar  8 09:56:51 2024, max compression
```

## Comparing `lapa_database-0.0.8.tar` & `lapa_database-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 15:57:28.056527 lapa_database-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-02-05 15:57:28.056527 lapa_database-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-02-05 15:57:14.000000 lapa_database-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 15:57:28.056527 lapa_database-0.0.8/lapa_database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 15:57:14.000000 lapa_database-0.0.8/lapa_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-02-05 15:57:14.000000 lapa_database-0.0.8/lapa_database/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-02-05 15:57:14.000000 lapa_database-0.0.8/lapa_database/create_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 15:57:28.056527 lapa_database-0.0.8/lapa_database/data/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-05 15:57:14.000000 lapa_database-0.0.8/lapa_database/data/config.example.ini
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-05 15:57:14.000000 lapa_database-0.0.8/lapa_database/data/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)    24229 2024-02-05 15:57:14.000000 lapa_database-0.0.8/lapa_database/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 15:57:28.056527 lapa_database-0.0.8/lapa_database/pydantic_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 15:57:14.000000 lapa_database-0.0.8/lapa_database/pydantic_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-02-05 15:57:14.000000 lapa_database-0.0.8/lapa_database/pydantic_models/pydantic_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 15:57:28.056527 lapa_database-0.0.8/lapa_database/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-05 15:57:14.000000 lapa_database-0.0.8/lapa_database/utils/CommonOperations.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 15:57:14.000000 lapa_database-0.0.8/lapa_database/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 15:57:28.056527 lapa_database-0.0.8/lapa_database/web_socket/
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-02-05 15:57:14.000000 lapa_database-0.0.8/lapa_database/web_socket/Trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-02-05 15:57:14.000000 lapa_database-0.0.8/lapa_database/web_socket/WebsocketOperation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 15:57:14.000000 lapa_database-0.0.8/lapa_database/web_socket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 15:57:28.056527 lapa_database-0.0.8/lapa_database.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-02-05 15:57:28.000000 lapa_database-0.0.8/lapa_database.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-02-05 15:57:28.000000 lapa_database-0.0.8/lapa_database.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 15:57:28.000000 lapa_database-0.0.8/lapa_database.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-05 15:57:28.000000 lapa_database-0.0.8/lapa_database.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-05 15:57:28.000000 lapa_database-0.0.8/lapa_database.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 15:57:28.056527 lapa_database-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-05 15:57:14.000000 lapa_database-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:56:51.415004 lapa_database-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-08 09:56:51.415004 lapa_database-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-03-08 09:56:43.000000 lapa_database-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:56:51.415004 lapa_database-0.0.9/lapa_database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 09:56:43.000000 lapa_database-0.0.9/lapa_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-03-08 09:56:43.000000 lapa_database-0.0.9/lapa_database/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-03-08 09:56:43.000000 lapa_database-0.0.9/lapa_database/create_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:56:51.415004 lapa_database-0.0.9/lapa_database/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-08 09:56:43.000000 lapa_database-0.0.9/lapa_database/data/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    24229 2024-03-08 09:56:43.000000 lapa_database-0.0.9/lapa_database/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:56:51.415004 lapa_database-0.0.9/lapa_database/pydantic_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 09:56:43.000000 lapa_database-0.0.9/lapa_database/pydantic_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-08 09:56:43.000000 lapa_database-0.0.9/lapa_database/pydantic_models/pydantic_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:56:51.415004 lapa_database-0.0.9/lapa_database/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-08 09:56:43.000000 lapa_database-0.0.9/lapa_database/utils/CommonOperations.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 09:56:43.000000 lapa_database-0.0.9/lapa_database/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:56:51.415004 lapa_database-0.0.9/lapa_database/web_socket/
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-03-08 09:56:43.000000 lapa_database-0.0.9/lapa_database/web_socket/Trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-03-08 09:56:43.000000 lapa_database-0.0.9/lapa_database/web_socket/WebsocketOperation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 09:56:43.000000 lapa_database-0.0.9/lapa_database/web_socket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:56:51.415004 lapa_database-0.0.9/lapa_database.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-08 09:56:51.000000 lapa_database-0.0.9/lapa_database.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-08 09:56:51.000000 lapa_database-0.0.9/lapa_database.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 09:56:51.000000 lapa_database-0.0.9/lapa_database.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-08 09:56:51.000000 lapa_database-0.0.9/lapa_database.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-08 09:56:51.000000 lapa_database-0.0.9/lapa_database.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 09:56:51.415004 lapa_database-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-08 09:56:43.000000 lapa_database-0.0.9/setup.py
```

### Comparing `lapa_database-0.0.8/PKG-INFO` & `lapa_database-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lapa_database
-Version: 0.0.8
+Version: 0.0.9
 Summary: database layer for my personal server.
 Home-page: https://github.com/thepmsquare/lapa_database
-Author: thePmSquare, Amish Palkar, Lav Sharma
-Author-email: thepmsquare@gmail.com, amishpalkar302001@gmail.com, lavsharma2016@gmail.com
+Author: thePmSquare, Amish Palkar, Lav Sharma, Aaditya Sangsihetty
+Author-email: thepmsquare@gmail.com, amishpalkar302001@gmail.com, lavsharma2016@gmail.com, adityashetty35@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -23,33 +23,38 @@
 
 ## installation
 
 > pip install lapa_database[all]
 
 ## usage (WIP)
 
-### config.example.ini to config.ini.
+### change password in config.ini.
 
 ### CREATE_SCHEMA = True to create database from scratch.
 
 ### LOG_FILE_NAME and configure logger
 
 ### link to lapa_database_structure
 
 ## configs
 
-1. lapa_database\data\config.ini (can be created using lapa_database\data\config.example.ini)
+1. lapa_database\data\config.ini
 2. lapa_logger\data\config.ini
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.9
+
+- removed config.example.ini.
+- bug fix: create_database -> data insertion now takes schema into account.
+
 ### v0.0.8
 
 - add module name in config.
 - add first test case.
 - add dependencies for testing.
 - add GitHub workflow for testing.
 - remove config from gitignore.
```

### Comparing `lapa_database-0.0.8/README.md` & `lapa_database-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,33 +6,38 @@
 
 ## installation
 
 > pip install lapa_database[all]
 
 ## usage (WIP)
 
-### config.example.ini to config.ini.
+### change password in config.ini.
 
 ### CREATE_SCHEMA = True to create database from scratch.
 
 ### LOG_FILE_NAME and configure logger
 
 ### link to lapa_database_structure
 
 ## configs
 
-1. lapa_database\data\config.ini (can be created using lapa_database\data\config.example.ini)
+1. lapa_database\data\config.ini
 2. lapa_logger\data\config.ini
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.9
+
+- removed config.example.ini.
+- bug fix: create_database -> data insertion now takes schema into account.
+
 ### v0.0.8
 
 - add module name in config.
 - add first test case.
 - add dependencies for testing.
 - add GitHub workflow for testing.
 - remove config from gitignore.
```

### Comparing `lapa_database-0.0.8/lapa_database/configuration.py` & `lapa_database-0.0.9/lapa_database/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         ldict_configuration["ENVIRONMENT"]["CREATE_SCHEMA"]
     )
     config_str_database_module_name = ldict_configuration["ENVIRONMENT"][
         "DATABASE_PACKAGE_NAME"
     ]
 except Exception as e:
     print(
-        "\033[91mMissing or incorrect config.ini file, have you tried creating it from config.example.ini?\n"
+        "\033[91mMissing or incorrect config.ini file.\n"
         "Error details: " + str(e) + "\033[0m"
     )
     sys.exit()
 
 global_object_square_logger = SquareLogger("lapa_database")
 
 # extra logic for this module
```

### Comparing `lapa_database-0.0.8/lapa_database/create_database.py` & `lapa_database-0.0.9/lapa_database/create_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
                         )
                     # ===========================================
                     database_connection.execute(
                         text(f"SET search_path TO {local_str_schema_name}")
                     )
 
                     inspector = inspect(database_engine)
-                    existing_table_names = inspector.get_table_names()
+                    existing_table_names = inspector.get_table_names(schema=local_str_schema_name)
 
                     tables_module_path = (
                         f"{config_str_database_module_name}"
                         f".{local_str_database_name}.{local_str_schema_name}.tables"
                     )
                     tables_module = importlib.import_module(tables_module_path)
                     base = getattr(tables_module, "Base")
```

### Comparing `lapa_database-0.0.8/lapa_database/main.py` & `lapa_database-0.0.9/lapa_database/main.py`

 * *Files identical despite different names*

### Comparing `lapa_database-0.0.8/lapa_database/pydantic_models/pydantic_models.py` & `lapa_database-0.0.9/lapa_database/pydantic_models/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `lapa_database-0.0.8/lapa_database/web_socket/Trigger.py` & `lapa_database-0.0.9/lapa_database/web_socket/Trigger.py`

 * *Files identical despite different names*

### Comparing `lapa_database-0.0.8/lapa_database/web_socket/WebsocketOperation.py` & `lapa_database-0.0.9/lapa_database/web_socket/WebsocketOperation.py`

 * *Files identical despite different names*

### Comparing `lapa_database-0.0.8/lapa_database.egg-info/PKG-INFO` & `lapa_database-0.0.9/lapa_database.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lapa-database
-Version: 0.0.8
+Version: 0.0.9
 Summary: database layer for my personal server.
 Home-page: https://github.com/thepmsquare/lapa_database
-Author: thePmSquare, Amish Palkar, Lav Sharma
-Author-email: thepmsquare@gmail.com, amishpalkar302001@gmail.com, lavsharma2016@gmail.com
+Author: thePmSquare, Amish Palkar, Lav Sharma, Aaditya Sangsihetty
+Author-email: thepmsquare@gmail.com, amishpalkar302001@gmail.com, lavsharma2016@gmail.com, adityashetty35@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -23,33 +23,38 @@
 
 ## installation
 
 > pip install lapa_database[all]
 
 ## usage (WIP)
 
-### config.example.ini to config.ini.
+### change password in config.ini.
 
 ### CREATE_SCHEMA = True to create database from scratch.
 
 ### LOG_FILE_NAME and configure logger
 
 ### link to lapa_database_structure
 
 ## configs
 
-1. lapa_database\data\config.ini (can be created using lapa_database\data\config.example.ini)
+1. lapa_database\data\config.ini
 2. lapa_logger\data\config.ini
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.9
+
+- removed config.example.ini.
+- bug fix: create_database -> data insertion now takes schema into account.
+
 ### v0.0.8
 
 - add module name in config.
 - add first test case.
 - add dependencies for testing.
 - add GitHub workflow for testing.
 - remove config from gitignore.
```

### Comparing `lapa_database-0.0.8/lapa_database.egg-info/SOURCES.txt` & `lapa_database-0.0.9/lapa_database.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 lapa_database/create_database.py
 lapa_database/main.py
 lapa_database.egg-info/PKG-INFO
 lapa_database.egg-info/SOURCES.txt
 lapa_database.egg-info/dependency_links.txt
 lapa_database.egg-info/requires.txt
 lapa_database.egg-info/top_level.txt
-lapa_database/data/config.example.ini
 lapa_database/data/config.ini
 lapa_database/pydantic_models/__init__.py
 lapa_database/pydantic_models/pydantic_models.py
 lapa_database/utils/CommonOperations.py
 lapa_database/utils/__init__.py
 lapa_database/web_socket/Trigger.py
 lapa_database/web_socket/WebsocketOperation.py
```

### Comparing `lapa_database-0.0.8/setup.py` & `lapa_database-0.0.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 package_name = "lapa_database"
 
 setup(
     name=package_name,
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(),
     package_data={
         package_name: ["data/*", "pydantic_models/*"],
     },
     install_requires=[
         "sqlalchemy>=2.0.23",
         "psycopg2-binary>=2.9.9",
@@ -22,16 +22,17 @@
         "pytest>=8.0.0",
     ],
     extras_require={
         "all": [
             "lapa_database_structure~=0.0.1",
         ],
     },
-    author="thePmSquare, Amish Palkar, Lav Sharma",
-    author_email="thepmsquare@gmail.com, amishpalkar302001@gmail.com, lavsharma2016@gmail.com",
+    author="thePmSquare, Amish Palkar, Lav Sharma, Aaditya Sangsihetty",
+    author_email="thepmsquare@gmail.com, amishpalkar302001@gmail.com, lavsharma2016@gmail.com, "
+                 "adityashetty35@gmail.com",
     description="database layer for my personal server.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url=f"https://github.com/thepmsquare/{package_name}",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

