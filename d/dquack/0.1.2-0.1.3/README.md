# Comparing `tmp/dquack-0.1.2.tar.gz` & `tmp/dquack-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dquack-0.1.2.tar", max compression
+gzip compressed data, was "dquack-0.1.3.tar", max compression
```

## Comparing `dquack-0.1.2.tar` & `dquack-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       65 2024-03-28 01:09:54.591665 dquack-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-03-28 01:09:54.591665 dquack-0.1.2/dquack/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 01:09:54.591665 dquack-0.1.2/dquack/cli/__init__.py
--rw-r--r--   0        0        0       37 2024-03-28 01:09:54.591665 dquack-0.1.2/dquack/constant.py
--rw-r--r--   0        0        0        0 2024-03-28 01:09:54.591665 dquack-0.1.2/dquack/core/__init__.py
--rw-r--r--   0        0        0    12658 2024-03-28 01:09:54.591665 dquack-0.1.2/dquack/core/constraint.py
--rw-r--r--   0        0        0      494 2024-03-28 01:09:54.591665 dquack-0.1.2/dquack/core/contract.py
--rw-r--r--   0        0        0     4833 2024-03-28 01:09:54.591665 dquack-0.1.2/dquack/core/engine.py
--rw-r--r--   0        0        0        0 2024-03-28 01:09:54.591665 dquack-0.1.2/dquack/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-28 01:09:54.591665 dquack-0.1.2/dquack/logger.py
--rw-r--r--   0        0        0     1881 2024-03-28 01:09:54.591665 dquack-0.1.2/dquack/validation.py
--rw-r--r--   0        0        0     1173 2024-03-28 01:10:15.639526 dquack-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 dquack-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       65 2024-04-12 06:22:50.156534 dquack-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 06:22:50.156534 dquack-0.1.3/dquack/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:22:50.156534 dquack-0.1.3/dquack/cli/__init__.py
+-rw-r--r--   0        0        0       37 2024-04-12 06:22:50.156534 dquack-0.1.3/dquack/constant.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:22:50.156534 dquack-0.1.3/dquack/core/__init__.py
+-rw-r--r--   0        0        0    12831 2024-04-12 06:22:50.156534 dquack-0.1.3/dquack/core/constraint.py
+-rw-r--r--   0        0        0      526 2024-04-12 06:22:50.156534 dquack-0.1.3/dquack/core/contract.py
+-rw-r--r--   0        0        0     4833 2024-04-12 06:22:50.160534 dquack-0.1.3/dquack/core/engine.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:22:50.160534 dquack-0.1.3/dquack/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:22:50.160534 dquack-0.1.3/dquack/logger.py
+-rw-r--r--   0        0        0     1881 2024-04-12 06:22:50.160534 dquack-0.1.3/dquack/validation.py
+-rw-r--r--   0        0        0     1173 2024-04-12 06:23:13.768592 dquack-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 dquack-0.1.3/PKG-INFO
```

### Comparing `dquack-0.1.2/dquack/core/constraint.py` & `dquack-0.1.3/dquack/core/constraint.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,22 +284,28 @@
         # Ensure that the expression is not empty
         if not constraint.expression:
             raise ValueError("Expression cannot be empty")
 
         constraint_name = constraint.type_
         constraint_id = f"{column_name}_{constraint_name}_{self.random_string()}"
         constraint_details = f"Failed expression: {constraint.expression}"
+        where_clause = constraint.where
+
+        if where_clause:
+            where_clause = f"{where_clause} and "
+        else:
+            where_clause = ""
 
         query = f"""
-        select 
+        select
             row_id,
             {', '.join(self.extra_columns)},
             {column_name} as 'column_value'
         from {self.table.name}
-        where not ({constraint.expression})
+        where {where_clause}not ({constraint.expression})
         """
 
         failed_records: DataSeries = self.engine.fetchall(query)  # type: ignore
         return ColumnConstraintResult(
             column_name=column_name,
             constraint_name=constraint_name,
             constraint_id=constraint_id,
```

### Comparing `dquack-0.1.2/dquack/core/engine.py` & `dquack-0.1.3/dquack/core/engine.py`

 * *Files identical despite different names*

### Comparing `dquack-0.1.2/dquack/validation.py` & `dquack-0.1.3/dquack/validation.py`

 * *Files identical despite different names*

### Comparing `dquack-0.1.2/pyproject.toml` & `dquack-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dquack"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Duc Nguyen <me@vanducng.dev>"]
 readme = "README.md"
 packages = [{include = "dquack"}]
 
 [tool.poetry.dependencies]
 python = ">= 3.9, < 4.0"
```

### Comparing `dquack-0.1.2/PKG-INFO` & `dquack-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dquack
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Duc Nguyen
 Author-email: me@vanducng.dev
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

