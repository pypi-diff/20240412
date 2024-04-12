# Comparing `tmp/thanosql-0.1.0.tar.gz` & `tmp/thanosql-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thanosql-0.1.0.tar", last modified: Thu Apr  4 10:08:12 2024, max compression
+gzip compressed data, was "thanosql-0.2.0.tar", last modified: Fri Apr 12 05:51:34 2024, max compression
```

## Comparing `thanosql-0.1.0.tar` & `thanosql-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:12.623872 thanosql-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-04 10:08:08.000000 thanosql-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-04 10:08:12.623872 thanosql-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-04 10:08:08.000000 thanosql-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:08.000000 thanosql-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 10:08:12.623872 thanosql-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-04 10:08:08.000000 thanosql-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:12.615872 thanosql-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-04 10:08:08.000000 thanosql-0.1.0/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-04-04 10:08:08.000000 thanosql-0.1.0/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-04 10:08:08.000000 thanosql-0.1.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-04-04 10:08:08.000000 thanosql-0.1.0/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-04 10:08:08.000000 thanosql-0.1.0/tests/test_table_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-04 10:08:08.000000 thanosql-0.1.0/tests/test_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:12.619872 thanosql-0.1.0/thanosql/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/_service.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:12.619872 thanosql-0.1.0/thanosql/magic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/magic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/magic/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/magic/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/magic/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/magic/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:12.619872 thanosql-0.1.0/thanosql/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/resources/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/resources/_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/resources/_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/resources/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/resources/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/resources/_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:12.619872 thanosql-0.1.0/thanosql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-04 10:08:12.000000 thanosql-0.1.0/thanosql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-04 10:08:12.000000 thanosql-0.1.0/thanosql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:08:12.000000 thanosql-0.1.0/thanosql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:08:12.000000 thanosql-0.1.0/thanosql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-04 10:08:12.000000 thanosql-0.1.0/thanosql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 10:08:12.000000 thanosql-0.1.0/thanosql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:51:34.543325 thanosql-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-12 05:51:28.000000 thanosql-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-12 05:51:34.543325 thanosql-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-12 05:51:28.000000 thanosql-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 05:51:28.000000 thanosql-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 05:51:34.543325 thanosql-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-12 05:51:28.000000 thanosql-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:51:34.535325 thanosql-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-12 05:51:28.000000 thanosql-0.2.0/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-04-12 05:51:28.000000 thanosql-0.2.0/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-12 05:51:28.000000 thanosql-0.2.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-04-12 05:51:28.000000 thanosql-0.2.0/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-12 05:51:28.000000 thanosql-0.2.0/tests/test_table_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-12 05:51:28.000000 thanosql-0.2.0/tests/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:51:34.535325 thanosql-0.2.0/thanosql/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:51:34.539325 thanosql-0.2.0/thanosql/magic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/magic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/magic/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/magic/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/magic/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/magic/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:51:34.539325 thanosql-0.2.0/thanosql/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/resources/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/resources/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/resources/_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/resources/_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/resources/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/resources/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-12 05:51:28.000000 thanosql-0.2.0/thanosql/resources/_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:51:34.539325 thanosql-0.2.0/thanosql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-12 05:51:34.000000 thanosql-0.2.0/thanosql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-12 05:51:34.000000 thanosql-0.2.0/thanosql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 05:51:34.000000 thanosql-0.2.0/thanosql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 05:51:34.000000 thanosql-0.2.0/thanosql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-12 05:51:34.000000 thanosql-0.2.0/thanosql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 05:51:34.000000 thanosql-0.2.0/thanosql.egg-info/top_level.txt
```

### Comparing `thanosql-0.1.0/LICENSE` & `thanosql-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thanosql-0.1.0/PKG-INFO` & `thanosql-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: thanosql
-Version: 0.1.0
+Version: 0.2.0
 Summary: ThanoSQL SDK for Python
 Home-page: https://github.com/smartmind-team/thanosql-python
 Author: SmartMind
 Author-email: dev@smartmind.team
 License: MIT
 Keywords: smartmind thanosql sdk
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: urllib3
+Requires-Dist: openpyxl
+Requires-Dist: pandas
 Requires-Dist: pydantic>=2.0
+Requires-Dist: requests
 Requires-Dist: tqdm
+Requires-Dist: urllib3
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
 Requires-Dist: faker; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 Requires-Dist: myst-nb; extra == "dev"
 Requires-Dist: sphinx-autoapi; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Provides-Extra: magic
 Requires-Dist: ipython; extra == "magic"
-Requires-Dist: pandas; extra == "magic"
 Requires-Dist: sqlalchemy; extra == "magic"
-Requires-Dist: numpy; extra == "magic"
 Requires-Dist: matplotlib; extra == "magic"
+Requires-Dist: numpy; extra == "magic"
 Requires-Dist: websocket-client; extra == "magic"
 Requires-Dist: pglast; extra == "magic"
 
 # ThanoSQL Python Library
 
 The ThanoSQL Python library provides convenient access to the ThanoSQL API from any Python 3.8+ application. The library covers all ThanoSQL operations that users can do, such as querying, editing tables, and much more.
```

### Comparing `thanosql-0.1.0/README.md` & `thanosql-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `thanosql-0.1.0/setup.py` & `thanosql-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,29 +26,29 @@
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords="smartmind thanosql sdk",
     packages=find_packages(exclude=["tests", "tests.*"]),
-    install_requires=["requests", "urllib3", "pydantic>=2.0", "tqdm"],
+    install_requires=[
+        "openpyxl",
+        "pandas",
+        "pydantic>=2.0",
+        "requests",
+        "tqdm",
+        "urllib3",
+    ],
     extras_require={
-        "dev": [
-            "pytest",
-            "faker",
-            "myst-nb",
-            "sphinx-autoapi",
-            "sphinx-rtd-theme"
-        ],
+        "dev": ["faker", "pytest", "myst-nb", "sphinx-autoapi", "sphinx-rtd-theme"],
         "magic": [
             "ipython",
-            "pandas",
             "sqlalchemy",
-            "numpy",
             "matplotlib",
+            "numpy",
             "websocket-client",
             "pglast",
         ],
     },
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `thanosql-0.1.0/tests/test_file.py` & `thanosql-0.2.0/tests/test_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,28 +59,28 @@
     # note that we cannot check the existence of uploaded files as it requires user_data_root
     # which can technically be saved, but it increases complexity and safety risk
     res = client.file.upload(path=file_name)
     assert res["data"]["file_path"] == default_file_path
 
     # upload with db_commit and dir
     target_table = client.table.get(name=basic_table_name)
-    record_count_before = target_table.get_records()["total"]
+    record_count_before = target_table.get_records().total
 
     res = client.file.upload(
         path=file_name,
         db_commit=True,
         table=basic_table_name,
         column=column_name,
         dir=dir_name,
     )
     assert res["data"]["file_path"] == f"drive/{dir_name}/{file_name}"
     assert res["data"]["table_name"] == basic_table_name
     assert res["data"]["column_name"] == column_name
 
-    record_count_after = target_table.get_records()["total"]
+    record_count_after = target_table.get_records().total
     assert record_count_after == record_count_before + 1
 
 
 def test_get_files(client: ThanoSQL):
     # path must start with drive/
     with pytest.raises(ThanoSQLValueError):
         client.file.list(path=dir_name)
@@ -115,16 +115,16 @@
             path=path,
             db_commit=True,
             table=basic_table_name,
             column=fake.unique.pystr(8),
         )
 
     target_table = client.table.get(name=basic_table_name)
-    record_count_before = target_table.get_records()["total"]
+    record_count_before = target_table.get_records().total
 
     res = client.file.delete(
         path=path, db_commit=True, table=basic_table_name, column=column_name
     )
     assert "message" in res
 
-    record_count_after = target_table.get_records()["total"]
+    record_count_after = target_table.get_records().total
     assert record_count_after == record_count_before - 1
```

### Comparing `thanosql-0.1.0/tests/test_query.py` & `thanosql-0.2.0/tests/test_query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
+import pandas as pd
 import pytest
 
 from tests.faker import fake
 from thanosql._error import (
     ThanoSQLAlreadyExistsError,
     ThanoSQLNotFoundError,
     ThanoSQLValueError,
 )
-from thanosql.resources import QueryLog, QueryTemplate
+from thanosql.resources import QueryLog, QueryTemplate, Records
 
 if TYPE_CHECKING:
     from thanosql._client import ThanoSQL
 
 plain_query_template_name = (
     f"test_plain_{fake.unique.pystr(min_chars=8, max_chars=8).lower()}"
 )
@@ -23,15 +24,15 @@
 )
 changed_query_template_name = (
     f"test_changed_{fake.unique.pystr(min_chars=8, max_chars=8).lower()}"
 )
 
 plain_query_template_string = "LIST THANOSQL MODEL"
 basic_query_template_string = "SELECT * FROM {{ table_name }}"
-changed_query_template_string = "SELECT {% for col in columns %}{{ col }}{% if not loop.last %}, {% endif %}{% endfor %} FROM {{ table_name }}"
+changed_query_template_string = "SELECT {% for col in columns %}{{ col }}{% if not loop.last %}, {% endif %}{% endfor %} FROM {{ table_name }} LIMIT 0"
 invalid_query_template_string = "DELETE MODEL {% model_name %}"
 
 query_test_table_name = (
     f"test_query_{fake.unique.pystr(min_chars=8, max_chars=8).lower()}"
 )
 query_test_selected_columns = ["name", "price"]
 
@@ -205,23 +206,28 @@
     with pytest.raises(ThanoSQLValueError):
         params = {"table_name": "random_table", "cols": ["column_1", "column_2"]}
         client.query.execute(template_name=basic_query_template_name, parameters=params)
 
 
 def test_post_query_success(client: ThanoSQL, basic_table_name, empty_table_name):
     params = {"table_name": basic_table_name, "columns": query_test_selected_columns}
-    completed_changed_query = f"SELECT name, price FROM {basic_table_name}"
+    completed_changed_query = f"SELECT name, price FROM {basic_table_name} LIMIT 0"
 
     # direct entry template
-    res = client.query.execute(query=changed_query_template_string, parameters=params)
+    res = client.query.execute(
+        query=changed_query_template_string, parameters=params, max_results=10
+    )
     assert isinstance(res, QueryLog)
     assert res.error_result is None
     assert res.destination_schema == "qm"
     assert res.query == completed_changed_query
 
+    # there should be empty record([]) even if max_results is > 0 as we set LIMIT 0 in the query
+    assert len(res.records.data) == 0
+
     # make sure the qm table is created
     qm_table_name = res.destination_table_name
     res = client.table.get(name=qm_table_name, schema="qm")
     assert res
 
     # direct entry without template or parameters
     res = client.query.execute(
@@ -229,14 +235,17 @@
     )
     assert isinstance(res, QueryLog)
     assert res.error_result is None
     assert res.destination_schema == "public"
     assert res.query == plain_query_template_string
     assert res.destination_table_name == query_test_table_name
 
+    # since max_results is 0 by default, there should be no records at all
+    assert res.records is None
+
     # make sure the table is created in public schema
     res = client.table.get(name=query_test_table_name)
     assert res
 
     # using saved query template
     res = client.query.execute(
         template_name=basic_query_template_name,
@@ -247,14 +256,32 @@
     assert isinstance(res, QueryLog)
     assert res.error_result is None
     assert res.destination_schema == "public"
     assert res.query == completed_changed_query
     assert res.destination_table_name == empty_table_name
 
 
+def test_query_log_records(client: ThanoSQL, empty_table):
+    # we want to check if the records section of QueryLog is working properly
+    # since we didn't create any tables in this module, we will use the
+    # empty_table fixture to ensure that there is at least one table in
+    # the list of public tables in information_schema
+    query = """
+    SELECT table_name FROM information_schema.tables
+    WHERE table_schema = 'public'
+    """
+    res = client.query.execute(query=query, max_results=100)
+    assert isinstance(res.records, Records)
+
+    # check if to_df is working and check that records is nonempty
+    df = res.records.to_df()
+    assert isinstance(df, pd.DataFrame)
+    assert len(df.index) > 0
+
+
 @pytest.mark.parametrize(
     "name", [changed_query_template_name, basic_query_template_name]
 )
 def test_delete_query_template_success(client: ThanoSQL, name: str):
     res = client.query.template.delete(name=name)
     assert "message" in res
```

### Comparing `thanosql-0.1.0/tests/test_schema.py` & `thanosql-0.2.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.1.0/tests/test_table.py` & `thanosql-0.2.0/tests/test_table.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 from __future__ import annotations
 
 import glob
 import logging
 import os
 from typing import TYPE_CHECKING
 
+import pandas as pd
 import pytest
 
 from tests.faker import fake
 from thanosql._error import (
     ThanoSQLAlreadyExistsError,
     ThanoSQLNotFoundError,
     ThanoSQLValueError,
 )
 from thanosql.resources import (
     BaseColumn,
     BaseTable,
     Constraints,
     PrimaryKey,
+    Records,
     Table,
     TableObject,
 )
 
 if TYPE_CHECKING:
     from _pytest.fixtures import FixtureRequest
 
     from thanosql._client import ThanoSQL
 
 test_table_name = f"test_table_{fake.unique.pystr(8).lower()}"
 test_table_name_old = test_table_name + "_old"
 test_table_name_excel = test_table_name + "_excel"
+test_table_name_df = test_table_name + "_df"
 
 
 def test_get_table_not_found(client: ThanoSQL):
     with pytest.raises(ThanoSQLNotFoundError):
         client.table.get(name=fake.unique.pystr(10))
 
 
@@ -139,20 +142,43 @@
 def test_insert_get_records_success(client: ThanoSQL, new_schema: str):
     target_table = client.table.get(name=test_table_name, schema=new_schema)
     records = [{"number": i + 1} for i in range(5)]
     res = target_table.insert(records=records)
 
     # check if the records are successfully inserted
     res = target_table.get_records()
-    assert {"records", "total"} == set(res.keys())
-    assert res["total"] == len(records)
-    assert res["records"] == records
+    assert isinstance(res, Records)
+    assert res.total == len(records)
+    assert res.data == records
+
+    # check if records can be converted to df
+    df = res.to_df()
+    assert isinstance(df, pd.DataFrame)
+    assert len(df.index) == len(records)
+
+
+def test_get_records_empty_table(client: ThanoSQL, empty_table_name: str):
+    target_table = client.table.get(name=empty_table_name)
+    res = target_table.get_records()
+    assert isinstance(res, Records)
+    assert res.total == 0
+    assert len(res.data) == 0
 
 
 def test_upload_table_invalid(client: ThanoSQL, new_schema: str):
+    # file or df must be provided
+    with pytest.raises(ThanoSQLValueError):
+        client.table.upload(name=test_table_name)
+
+    # file and df cannot be provided at the same time
+    with pytest.raises(ThanoSQLValueError):
+        client.table.upload(
+            name=test_table_name, file="file_csv.csv", df=pd.DataFrame()
+        )
+
     # only CSV or Excel accepted
     with pytest.raises(ThanoSQLValueError):
         client.table.upload(name=test_table_name, file="file_txt.txt")
 
     # schema should exist
     with pytest.raises(ThanoSQLNotFoundError):
         client.table.upload(
@@ -200,15 +226,15 @@
     # check that the table and records are indeed uploaded
     target_table = client.table.get(name=basic_table_name)
     assert len(target_table.columns) == 9
 
     # check get records with limit in the meantime
     limit = 5
     res = target_table.get_records(limit=limit)
-    assert len(res["records"]) == limit
+    assert len(res.data) == limit
 
 
 def test_upload_table_excel(client: ThanoSQL, new_schema: str):
     # using upload with a suitable body should work
     table_object = TableObject(
         columns=[
             BaseColumn(type="varchar", name="title"),
@@ -228,15 +254,53 @@
     # check that the table and records are indeed uploaded
     target_table = client.table.get(name=test_table_name_excel, schema=new_schema)
     assert len(target_table.columns) == 3
 
     # check get records with limit in the meantime
     limit = 5
     res = target_table.get_records(limit=limit)
-    assert len(res["records"]) == limit
+    assert len(res.data) == limit
+
+
+# we do more thorough testing for upload with df as it is an SDK-exclusive feature
+def test_upload_table_df(client: ThanoSQL):
+    df = pd.read_csv("file_csv.csv")
+
+    # make sure a new table is created even if if_exists is 'append' if
+    # the name is not already taken by another table
+    res = client.table.upload(name=test_table_name_df, df=df, if_exists="append")
+    assert isinstance(res, Table)
+
+    # get the number of records
+    num_records_initial = res.get_records().total
+
+    # make sure records are appended if the table exists
+    res = client.table.upload(name=test_table_name_df, df=df, if_exists="append")
+    num_records_appended = res.get_records().total
+    assert num_records_appended == 2 * num_records_initial
+
+    # make sure creating a table of the same name fails by default
+    with pytest.raises(ThanoSQLAlreadyExistsError):
+        client.table.upload(name=test_table_name_df, df=df)
+
+    # make sure the table is overwritten if if_exists is 'replace'
+    res = client.table.upload(name=test_table_name_df, df=df, if_exists="replace")
+    num_records_replaced = res.get_records().total
+    assert num_records_replaced == num_records_initial
+
+    table_object = TableObject(
+        columns=[BaseColumn(type="integer", name="number")],
+        constraints=Constraints(primary_key=PrimaryKey(columns=["number"])),
+    )
+
+    # should not succeed if table body does not match cdf
+    with pytest.raises(ThanoSQLValueError):
+        client.table.upload(
+            name=test_table_name_df, df=df, table=table_object, if_exists="replace"
+        )
 
 
 def test_get_records_as_csv(client: ThanoSQL, new_schema: str):
     target_table = client.table.get(name=test_table_name_excel, schema=new_schema)
     target_table.get_records_as_csv()
 
     # check that the csv file is created
@@ -263,14 +327,15 @@
     with pytest.raises(ThanoSQLNotFoundError):
         client.table.delete(name=test_table_name, schema=fake.unique.pystr(10))
 
     # the other two tables will be automatically deleted when fixtures are destroyed
     # so we just need to "manually" delete these
     client.table.delete(name=test_table_name, schema=new_schema)
     client.table.delete(name=test_table_name_excel, schema=new_schema)
+    client.table.delete(name=test_table_name_df)
 
     # check that the table is indeed deleted
     with pytest.raises(ThanoSQLNotFoundError):
         client.table.get(name=test_table_name, schema=new_schema)
 
     # trying to delete the table again should not be allowed
     with pytest.raises(ThanoSQLNotFoundError):
```

### Comparing `thanosql-0.1.0/tests/test_table_template.py` & `thanosql-0.2.0/tests/test_table_template.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.1.0/tests/test_view.py` & `thanosql-0.2.0/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.1.0/thanosql/_base_client.py` & `thanosql-0.2.0/thanosql/_base_client.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.1.0/thanosql/_client.py` & `thanosql-0.2.0/thanosql/_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,22 +23,41 @@
     ) -> None:
         if api_token is None:
             api_token = os.environ.get("THANOSQL_API_TOKEN", "")
         if not api_token:
             raise ThanoSQLValueError(
                 "Please input a valid API token. You can do this either by passing it as a parameter or setting the THANOSQL_API_TOKEN environment variable."
             )
-        
+
         if engine_url is None:
             engine_url = os.environ.get("THANOSQL_ENGINE_URL", "")
         if not engine_url:
             raise ThanoSQLValueError(
                 "Please input a valid engine URL. You can do this either by passing it as a parameter or setting the THANOSQL_ENGINE_URL environment variable."
             )
 
         super().__init__(token=api_token, base_url=engine_url, version=api_version)
 
-        self.file: FileService = FileService(self)
-        self.query: QueryService = QueryService(self)
-        self.schema: SchemaService = SchemaService(self)
-        self.table: TableService = TableService(self)
-        self.view: ViewService = ViewService(self)
+    @property
+    def query(self) -> QueryService:
+        """Access the QueryService."""
+        return QueryService(self)
+
+    @property
+    def file(self) -> FileService:
+        """Access the FileService."""
+        return FileService(self)
+
+    @property
+    def schema(self) -> SchemaService:
+        """Access the SchemaService."""
+        return SchemaService(self)
+
+    @property
+    def table(self) -> TableService:
+        """Access the TableService."""
+        return TableService(self)
+
+    @property
+    def view(self) -> ViewService:
+        """Access the ViewService."""
+        return ViewService(self)
```

### Comparing `thanosql-0.1.0/thanosql/_error.py` & `thanosql-0.2.0/thanosql/_error.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.1.0/thanosql/_service.py` & `thanosql-0.2.0/thanosql/_service.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.1.0/thanosql/magic/magic.py` & `thanosql-0.2.0/thanosql/magic/magic.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.1.0/thanosql/magic/parse.py` & `thanosql-0.2.0/thanosql/magic/parse.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.1.0/thanosql/magic/util.py` & `thanosql-0.2.0/thanosql/magic/util.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.1.0/thanosql/resources/_file.py` & `thanosql-0.2.0/thanosql/resources/_file.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,33 +23,43 @@
 
     def upload(
         self,
         path: Union[str, os.PathLike],
         db_commit: Optional[bool] = None,
         table: Optional[str] = None,
         column: Optional[str] = None,
+        schema: Optional[str] = None,
         dir: Optional[str] = None,
     ) -> dict:
         api_path = f"/{self.tag}/"
         query_params = self._create_input_dict(
-            db_commit=db_commit, table_name=table, column_name=column, dir=dir
+            db_commit=db_commit,
+            table_name=table,
+            column_name=column,
+            schema=schema,
+            dir=dir,
         )
 
         return self.client._request(
             method="post", path=api_path, query_params=query_params, file=path
         )
 
     def delete(
         self,
         path: Union[str, os.PathLike],
         db_commit: Optional[bool] = None,
         table: Optional[str] = None,
         column: Optional[str] = None,
+        schema: Optional[str] = None,
     ) -> dict:
         api_path = f"/{self.tag}/"
         query_params = self._create_input_dict(
-            file_path=path, db_commit=db_commit, table_name=table, column_name=column
+            file_path=path,
+            db_commit=db_commit,
+            table_name=table,
+            column_name=column,
+            schema=schema,
         )
 
         return self.client._request(
             method="delete", path=api_path, query_params=query_params
         )
```

### Comparing `thanosql-0.1.0/thanosql/resources/_query.py` & `thanosql-0.2.0/thanosql/resources/_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import TYPE_CHECKING, List, Optional
 
 from pydantic import TypeAdapter
 
 from thanosql._error import ThanoSQLValueError
 from thanosql._service import ThanoSQLService
 from thanosql.resources._model import BaseModel
+from thanosql.resources._record import Records
 
 if TYPE_CHECKING:
     from thanosql._client import ThanoSQL
 
 
 class QueryLog(BaseModel):
     query_id: Optional[str]
@@ -22,15 +23,15 @@
     query: str
     referer: str
     state: Optional[str]
     destination_table_name: Optional[str]
     destination_schema: Optional[str]
     error_result: Optional[str]
     created_at: Optional[datetime]
-    records: Optional[list] = None
+    records: Optional[Records] = None
 
 
 class QueryType(enum.Enum):
     THANOSQL = "thanosql"
     PSQL = "psql"
```

### Comparing `thanosql-0.1.0/thanosql/resources/_schema.py` & `thanosql-0.2.0/thanosql/resources/_schema.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.1.0/thanosql/resources/_table.py` & `thanosql-0.2.0/thanosql/resources/_table.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
 
+import enum
+import json
 import os
 from datetime import datetime
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional, Union
 
+import pandas as pd
 from pydantic import Field, TypeAdapter
 
 from thanosql._error import ThanoSQLValueError
 from thanosql._service import ThanoSQLService
 from thanosql.resources._model import BaseModel
+from thanosql.resources._record import Records
 
 if TYPE_CHECKING:
     from thanosql._client import ThanoSQL
 
 
 class BaseColumn(BaseModel):
     default: Optional[str] = None
@@ -62,14 +66,20 @@
 
 
 class TableObject(BaseModel):
     columns: Optional[List[BaseColumn]] = None
     constraints: Optional[Constraints] = None
 
 
+class IfExists(enum.Enum):
+    FAIL = "fail"
+    APPEND = "append"
+    REPLACE = "replace"
+
+
 class TableService(ThanoSQLService):
     def __init__(self, client: ThanoSQL) -> None:
         super().__init__(client=client, tag="table")
 
         self.template: TableTemplateService = TableTemplateService(client)
 
     def _parse_table_response(self, raw_response: dict) -> Table:
@@ -138,61 +148,149 @@
         )
 
         return self._parse_table_response(raw_response)
 
     def upload(
         self,
         name: str,
-        file: Union[str, os.PathLike],
+        file: Optional[Union[str, os.PathLike]] = None,
+        df: Optional[pd.DataFrame] = None,
         schema: Optional[str] = None,
         table: Optional[TableObject] = None,
-        if_exists: Optional[str] = None,
+        if_exists: str = "fail",
     ) -> Table:
-        path = f"/{self.tag}/{name}/upload/"
+        try:
+            if_exists_enum = IfExists(if_exists)
+        except Exception as e:
+            raise ThanoSQLValueError(str(e))
 
-        file_extension = Path(file).suffix.lower()
-        if file_extension == ".csv":
-            path = path + "csv"
-        elif file_extension in [
-            ".xls",
-            ".xlsx",
-            ".xlsm",
-            ".xlsb",
-            ".odf",
-            ".ods",
-            ".odt",
-        ]:
-            path = path + "excel"
-        else:
+        if file and df is not None:
             raise ThanoSQLValueError(
-                "Invalid format: only CSV and Excel files possible."
+                "Cannot use both file and DataFrame for upload at the same time."
             )
 
-        query_params = self._create_input_dict(schema=schema, if_exists=if_exists)
-        payload = self._create_input_dict(table=table)
+        if file:
+            path = f"/{self.tag}/{name}/upload/"
 
-        raw_response = self.client._request(
-            method="post",
-            path=path,
-            query_params=query_params,
-            payload=payload,
-            file=file,
-        )
+            file_extension = Path(file).suffix.lower()
+            if file_extension == ".csv":
+                path = path + "csv"
+            elif file_extension in [
+                ".xls",
+                ".xlsx",
+                ".xlsm",
+                ".xlsb",
+                ".odf",
+                ".ods",
+                ".odt",
+            ]:
+                path = path + "excel"
+            else:
+                raise ThanoSQLValueError(
+                    "Invalid format: only CSV and Excel files possible."
+                )
 
-        return self._parse_table_response(raw_response)
+            query_params = self._create_input_dict(
+                schema=schema, if_exists=if_exists_enum.value
+            )
+            payload = self._create_input_dict(table=table)
+
+            raw_response = self.client._request(
+                method="post",
+                path=path,
+                query_params=query_params,
+                payload=payload,
+                file=file,
+            )
+
+            return self._parse_table_response(raw_response)
+
+        elif df is not None:
+            path = f"/{self.tag}/{name}/upload/json"
+
+            df_json = df.to_dict(orient="records")
+            query_params = self._create_input_dict(
+                schema=schema, if_exists=if_exists_enum.value
+            )
+            payload = self._create_input_dict(table=table, data=df_json)
+
+            raw_response = self.client._request(
+                method="post",
+                path=path,
+                query_params=query_params,
+                payload=payload,
+                file=file,
+            )
+
+            return self._parse_table_response(raw_response)
+
+        else:
+            raise ThanoSQLValueError("No file or DataFrame provided for upload")
 
     def delete(self, name: str, schema: Optional[str] = None) -> dict:
         path = f"/{self.tag}/{name}"
         query_params = self._create_input_dict(schema=schema)
 
         return self.client._request(
             method="delete", path=path, query_params=query_params
         )
 
 
+class Table(BaseTable):
+    service: Optional[TableService] = None
+
+    def get_records(
+        self,
+        offset: Optional[int] = None,
+        limit: Optional[int] = None,
+    ) -> Records:
+        path = f"/{self.service.tag}/{self.name}/records"
+
+        query_params = self.service._create_input_dict(
+            schema=self.table_schema,
+            offset=offset,
+            limit=limit,
+        )
+
+        res = self.service.client._request(
+            method="get",
+            path=path,
+            query_params=query_params,
+        )
+        return Records(data=res["records"], total=res["total"])
+
+    def get_records_as_csv(
+        self,
+        timezone_offset: Optional[int] = None,
+    ) -> None:
+        path = f"/{self.service.tag}/{self.name}/records/csv"
+
+        query_params = self.service._create_input_dict(
+            schema=self.table_schema,
+            timezone_offset=timezone_offset,
+        )
+
+        self.service.client._request(
+            method="get", path=path, query_params=query_params, stream=True
+        )
+
+    def insert(
+        self,
+        records: List[dict],
+    ) -> Union[Table, dict]:
+        path = f"/{self.service.tag}/{self.name}/records"
+        query_params = self.service._create_input_dict(schema=self.table_schema)
+
+        raw_response = self.service.client._request(
+            method="post", path=path, query_params=query_params, payload=records
+        )
+
+        return self.service._parse_table_response(raw_response)
+
+
 class TableTemplate(BaseModel):
     name: str
     table_template: TableObject
     version: Optional[str]
     compatibility: Optional[str]
     created_at: Optional[datetime]
 
@@ -266,58 +364,7 @@
     def delete(self, name: str, version: Optional[str] = None) -> dict:
         path = f"/{self.tag}/{name}"
         query_params = self._create_input_dict(version=version)
 
         return self.client._request(
             method="delete", path=path, query_params=query_params
         )
-
-
-class Table(BaseTable):
-    service: Optional[TableService] = None
-
-    def get_records(
-        self,
-        offset: Optional[int] = None,
-        limit: Optional[int] = None,
-    ) -> dict:
-        path = f"/{self.service.tag}/{self.name}/records"
-
-        query_params = self.service._create_input_dict(
-            schema=self.table_schema,
-            offset=offset,
-            limit=limit,
-        )
-
-        return self.service.client._request(
-            method="get",
-            path=path,
-            query_params=query_params,
-        )
-
-    def get_records_as_csv(
-        self,
-        timezone_offset: Optional[int] = None,
-    ) -> None:
-        path = f"/{self.service.tag}/{self.name}/records/csv"
-
-        query_params = self.service._create_input_dict(
-            schema=self.table_schema,
-            timezone_offset=timezone_offset,
-        )
-
-        self.service.client._request(
-            method="get", path=path, query_params=query_params, stream=True
-        )
-
-    def insert(
-        self,
-        records: List[dict],
-    ) -> Union[Table, dict]:
-        path = f"/{self.service.tag}/{self.name}/records"
-        query_params = self.service._create_input_dict(schema=self.table_schema)
-
-        raw_response = self.service.client._request(
-            method="post", path=path, query_params=query_params, payload=records
-        )
-
-        return self.service._parse_table_response(raw_response)
```

### Comparing `thanosql-0.1.0/thanosql/resources/_view.py` & `thanosql-0.2.0/thanosql/resources/_view.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.1.0/thanosql.egg-info/PKG-INFO` & `thanosql-0.2.0/thanosql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: thanosql
-Version: 0.1.0
+Version: 0.2.0
 Summary: ThanoSQL SDK for Python
 Home-page: https://github.com/smartmind-team/thanosql-python
 Author: SmartMind
 Author-email: dev@smartmind.team
 License: MIT
 Keywords: smartmind thanosql sdk
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: urllib3
+Requires-Dist: openpyxl
+Requires-Dist: pandas
 Requires-Dist: pydantic>=2.0
+Requires-Dist: requests
 Requires-Dist: tqdm
+Requires-Dist: urllib3
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
 Requires-Dist: faker; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 Requires-Dist: myst-nb; extra == "dev"
 Requires-Dist: sphinx-autoapi; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Provides-Extra: magic
 Requires-Dist: ipython; extra == "magic"
-Requires-Dist: pandas; extra == "magic"
 Requires-Dist: sqlalchemy; extra == "magic"
-Requires-Dist: numpy; extra == "magic"
 Requires-Dist: matplotlib; extra == "magic"
+Requires-Dist: numpy; extra == "magic"
 Requires-Dist: websocket-client; extra == "magic"
 Requires-Dist: pglast; extra == "magic"
 
 # ThanoSQL Python Library
 
 The ThanoSQL Python library provides convenient access to the ThanoSQL API from any Python 3.8+ application. The library covers all ThanoSQL operations that users can do, such as querying, editing tables, and much more.
```

### Comparing `thanosql-0.1.0/thanosql.egg-info/SOURCES.txt` & `thanosql-0.2.0/thanosql.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -25,10 +25,11 @@
 thanosql/magic/magic.py
 thanosql/magic/parse.py
 thanosql/magic/util.py
 thanosql/resources/__init__.py
 thanosql/resources/_file.py
 thanosql/resources/_model.py
 thanosql/resources/_query.py
+thanosql/resources/_record.py
 thanosql/resources/_schema.py
 thanosql/resources/_table.py
 thanosql/resources/_view.py
```

