# Comparing `tmp/databricks_aws_utils-1.5.0.tar.gz` & `tmp/databricks_aws_utils-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_aws_utils-1.5.0.tar", max compression
+gzip compressed data, was "databricks_aws_utils-1.5.1.tar", max compression
```

## Comparing `databricks_aws_utils-1.5.0.tar` & `databricks_aws_utils-1.5.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-09-06 13:40:22.809930 databricks_aws_utils-1.5.0/LICENSE
--rw-r--r--   0        0        0     2530 2023-09-06 13:40:22.809930 databricks_aws_utils-1.5.0/README.md
--rw-r--r--   0        0        0     2087 2023-09-06 13:40:22.809930 databricks_aws_utils-1.5.0/databricks_aws_utils/__init__.py
--rw-r--r--   0        0        0    12212 2023-09-06 13:40:22.809930 databricks_aws_utils-1.5.0/databricks_aws_utils/delta_table.py
--rw-r--r--   0        0        0     4331 2023-09-06 13:40:22.809930 databricks_aws_utils-1.5.0/databricks_aws_utils/rds.py
--rw-r--r--   0        0        0     2174 2023-09-06 13:40:22.809930 databricks_aws_utils-1.5.0/databricks_aws_utils/s3.py
--rw-r--r--   0        0        0     1499 2023-09-06 13:40:22.809930 databricks_aws_utils-1.5.0/databricks_aws_utils/session.py
--rw-r--r--   0        0        0     1297 2023-09-06 13:40:23.929939 databricks_aws_utils-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 databricks_aws_utils-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-12 09:29:07.279437 databricks_aws_utils-1.5.1/LICENSE
+-rw-r--r--   0        0        0     2530 2024-04-12 09:29:07.279437 databricks_aws_utils-1.5.1/README.md
+-rw-r--r--   0        0        0     2087 2024-04-12 09:29:07.279437 databricks_aws_utils-1.5.1/databricks_aws_utils/__init__.py
+-rw-r--r--   0        0        0    12252 2024-04-12 09:29:07.279437 databricks_aws_utils-1.5.1/databricks_aws_utils/delta_table.py
+-rw-r--r--   0        0        0     4331 2024-04-12 09:29:07.279437 databricks_aws_utils-1.5.1/databricks_aws_utils/rds.py
+-rw-r--r--   0        0        0     2174 2024-04-12 09:29:07.279437 databricks_aws_utils-1.5.1/databricks_aws_utils/s3.py
+-rw-r--r--   0        0        0     1499 2024-04-12 09:29:07.279437 databricks_aws_utils-1.5.1/databricks_aws_utils/session.py
+-rw-r--r--   0        0        0     1297 2024-04-12 09:29:08.019443 databricks_aws_utils-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 databricks_aws_utils-1.5.1/PKG-INFO
```

### Comparing `databricks_aws_utils-1.5.0/LICENSE` & `databricks_aws_utils-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.5.0/README.md` & `databricks_aws_utils-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.5.0/databricks_aws_utils/__init__.py` & `databricks_aws_utils-1.5.1/databricks_aws_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.5.0/databricks_aws_utils/delta_table.py` & `databricks_aws_utils-1.5.1/databricks_aws_utils/delta_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         del table['CreateTime']
         del table['UpdateTime']
         del table['DatabaseName']
         del table['IsRegisteredWithLakeFormation']
         del table['CreatedBy']
         del table['VersionId']
         del table['CatalogId']
+        del table['IsMultiDialectView']
 
         params = table['Parameters'] or {}
         params['table_type'] = 'DELTA'
 
         table['Parameters'] = params
         table['StorageDescriptor']['Columns'] = columns
         table['PartitionKeys'] = partitions
```

### Comparing `databricks_aws_utils-1.5.0/databricks_aws_utils/rds.py` & `databricks_aws_utils-1.5.1/databricks_aws_utils/rds.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.5.0/databricks_aws_utils/s3.py` & `databricks_aws_utils-1.5.1/databricks_aws_utils/s3.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.5.0/databricks_aws_utils/session.py` & `databricks_aws_utils-1.5.1/databricks_aws_utils/session.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.5.0/pyproject.toml` & `databricks_aws_utils-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-aws-utils"
-version = "1.5.0"
+version = "1.5.1"
 description = "Databricks AWS Utils"
 license = "Proprietary"
 authors = [ "Lucas Vieira <lucas.vieira94@outlook.com>" ]
 maintainers = [ "Lucas Vieira <lucas.vieira94@outlook.com>" ]
 readme = "README.md"
 repository = "https://github.com/lucasvieirasilva/databricks-aws-utils"
```

### Comparing `databricks_aws_utils-1.5.0/PKG-INFO` & `databricks_aws_utils-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-aws-utils
-Version: 1.5.0
+Version: 1.5.1
 Summary: Databricks AWS Utils
 Home-page: https://github.com/lucasvieirasilva/databricks-aws-utils
 License: Proprietary
 Author: Lucas Vieira
 Author-email: lucas.vieira94@outlook.com
 Maintainer: Lucas Vieira
 Maintainer-email: lucas.vieira94@outlook.com
```

