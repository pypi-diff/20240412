# Comparing `tmp/connectionhandler-0.0.81.tar.gz` & `tmp/ConnectionHandler-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectionhandler-0.0.81.tar", last modified: Fri Apr 12 18:24:38 2024, max compression
+gzip compressed data, was "ConnectionHandler-0.0.9.tar", last modified: Thu Jan  5 18:27:17 2023, max compression
```

## Comparing `connectionhandler-0.0.81.tar` & `ConnectionHandler-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 18:24:38.500686 connectionhandler-0.0.81/
--rw-rw-rw-   0        0        0     1091 2023-01-05 16:08:11.000000 connectionhandler-0.0.81/LICENSE.txt
--rw-rw-rw-   0        0        0       14 2023-01-10 15:03:05.000000 connectionhandler-0.0.81/MANIFEST.in
--rw-rw-rw-   0        0        0      136 2024-04-12 18:24:38.499817 connectionhandler-0.0.81/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-05 15:07:43.000000 connectionhandler-0.0.81/README.txt
--rw-rw-rw-   0        0        0       80 2023-01-10 14:46:41.000000 connectionhandler-0.0.81/pyproject.toml
--rw-rw-rw-   0        0        0      330 2024-04-12 18:24:38.502698 connectionhandler-0.0.81/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 18:24:38.434121 connectionhandler-0.0.81/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 18:24:38.497689 connectionhandler-0.0.81/src/ConnectionHandler.egg-info/
--rw-rw-rw-   0        0        0      136 2024-04-12 18:24:38.000000 connectionhandler-0.0.81/src/ConnectionHandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      915 2024-04-12 18:24:38.000000 connectionhandler-0.0.81/src/ConnectionHandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 18:24:38.000000 connectionhandler-0.0.81/src/ConnectionHandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-12 18:24:38.000000 connectionhandler-0.0.81/src/ConnectionHandler.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 18:24:38.461576 connectionhandler-0.0.81/src/connectionhandler/
--rw-rw-rw-   0        0        0      192 2023-01-17 20:14:50.000000 connectionhandler-0.0.81/src/connectionhandler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:24:38.481686 connectionhandler-0.0.81/src/connectionhandler/connectiontypes/
--rw-rw-rw-   0        0        0       46 2023-01-10 14:21:58.000000 connectionhandler-0.0.81/src/connectionhandler/connectiontypes/__init__.py
--rw-rw-rw-   0        0        0      860 2023-01-24 16:12:52.000000 connectionhandler-0.0.81/src/connectionhandler/connectiontypes/database_handler.py
--rw-rw-rw-   0        0        0     6758 2023-01-24 14:36:12.000000 connectionhandler-0.0.81/src/connectionhandler/connectiontypes/dynamo_handler.py
--rw-rw-rw-   0        0        0    13244 2024-04-12 18:12:18.000000 connectionhandler-0.0.81/src/connectionhandler/connectiontypes/mssql_handler.py
--rw-rw-rw-   0        0        0    12266 2024-04-12 18:13:25.000000 connectionhandler-0.0.81/src/connectionhandler/connectiontypes/mysql_handler.py
--rw-rw-rw-   0        0        0    12991 2024-04-12 18:11:06.000000 connectionhandler-0.0.81/src/connectionhandler/connectiontypes/postgres_handler.py
--rw-rw-rw-   0        0        0      367 2023-01-17 20:09:39.000000 connectionhandler-0.0.81/src/connectionhandler/connectiontypes/sql_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:24:38.488688 connectionhandler-0.0.81/src/connectionhandler/dbImxLog/
--rw-rw-rw-   0        0        0       32 2023-10-10 16:22:06.000000 connectionhandler-0.0.81/src/connectionhandler/dbImxLog/__init__.py
--rw-rw-rw-   0        0        0     9850 2024-03-11 16:24:25.000000 connectionhandler-0.0.81/src/connectionhandler/dbImxLog/dbImxLog.py
--rw-rw-rw-   0        0        0     2106 2024-03-11 16:24:25.000000 connectionhandler-0.0.81/src/connectionhandler/dbImxLog/sampleLoggingHandler.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:24:38.494687 connectionhandler-0.0.81/src/connectionhandler/enums/
--rw-rw-rw-   0        0        0       28 2023-01-05 20:47:58.000000 connectionhandler-0.0.81/src/connectionhandler/enums/__init__.py
--rw-rw-rw-   0        0        0      140 2023-01-05 15:25:06.000000 connectionhandler-0.0.81/src/connectionhandler/enums/db_type.py
--rw-rw-rw-   0        0        0      215 2023-01-17 20:15:09.000000 connectionhandler-0.0.81/src/connectionhandler/get_handler.py
+drwxrwxrwx   0        0        0        0 2023-01-05 18:27:17.128634 ConnectionHandler-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-01-05 18:27:14.093827 ConnectionHandler-0.0.9/ConnectionHandler.egg-info/
+-rw-rw-rw-   0        0        0      280 2023-01-05 18:27:12.000000 ConnectionHandler-0.0.9/ConnectionHandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-01-05 18:27:13.000000 ConnectionHandler-0.0.9/ConnectionHandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-05 18:27:12.000000 ConnectionHandler-0.0.9/ConnectionHandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-01-05 18:27:12.000000 ConnectionHandler-0.0.9/ConnectionHandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-01-05 18:27:12.000000 ConnectionHandler-0.0.9/ConnectionHandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-01-05 16:08:11.000000 ConnectionHandler-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-01-05 15:07:12.000000 ConnectionHandler-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      280 2023-01-05 18:27:16.807633 ConnectionHandler-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-05 15:07:43.000000 ConnectionHandler-0.0.9/README.txt
+drwxrwxrwx   0        0        0        0 2023-01-05 18:27:14.822829 ConnectionHandler-0.0.9/connectionhandler/
+-rw-rw-rw-   0        0        0       30 2023-01-05 15:25:28.000000 ConnectionHandler-0.0.9/connectionhandler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-01-05 18:27:16.027348 ConnectionHandler-0.0.9/connectionhandler/connectiontypes/
+-rw-rw-rw-   0        0        0       30 2023-01-05 15:26:17.000000 ConnectionHandler-0.0.9/connectionhandler/connectiontypes/__init__.py
+-rw-rw-rw-   0        0        0     8259 2023-01-05 15:26:10.000000 ConnectionHandler-0.0.9/connectionhandler/connectiontypes/postgres_handler.py
+-rw-rw-rw-   0        0        0      367 2023-01-05 15:25:51.000000 ConnectionHandler-0.0.9/connectionhandler/connectiontypes/sql_handler.py
+-rw-rw-rw-   0        0        0      571 2023-01-05 15:26:47.000000 ConnectionHandler-0.0.9/connectionhandler/database_handler.py
+drwxrwxrwx   0        0        0        0 2023-01-05 18:27:16.728634 ConnectionHandler-0.0.9/connectionhandler/enums/
+-rw-rw-rw-   0        0        0       21 2023-01-05 15:25:20.000000 ConnectionHandler-0.0.9/connectionhandler/enums/__init__.py
+-rw-rw-rw-   0        0        0      140 2023-01-05 15:25:06.000000 ConnectionHandler-0.0.9/connectionhandler/enums/db_type.py
+-rw-rw-rw-   0        0        0      278 2023-01-05 18:26:43.000000 ConnectionHandler-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-01-05 18:27:17.165633 ConnectionHandler-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      554 2023-01-05 18:26:39.000000 ConnectionHandler-0.0.9/setup.py
```

### Comparing `connectionhandler-0.0.81/LICENSE.txt` & `ConnectionHandler-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

