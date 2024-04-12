# Comparing `tmp/ops-py-azure-key-vault-report-4.0.0.tar.gz` & `tmp/ops-py-azure-key-vault-report-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-py-azure-key-vault-report-4.0.0.tar", last modified: Thu Apr 11 12:26:14 2024, max compression
+gzip compressed data, was "ops-py-azure-key-vault-report-4.0.1.tar", last modified: Fri Apr 12 13:14:34 2024, max compression
```

## Comparing `ops-py-azure-key-vault-report-4.0.0.tar` & `ops-py-azure-key-vault-report-4.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:26:14.679647 ops-py-azure-key-vault-report-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-11 12:26:12.000000 ops-py-azure-key-vault-report-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-11 12:26:14.679647 ops-py-azure-key-vault-report-4.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:26:14.679647 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/
--rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/az_cmd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17664 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/azure_key_vault_report.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1346 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/html_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1219 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/markdown.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/ms_teams_json.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      949 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/set_timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:26:14.679647 ops-py-azure-key-vault-report-4.0.0/ops_py_azure_key_vault_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-11 12:26:14.000000 ops-py-azure-key-vault-report-4.0.0/ops_py_azure_key_vault_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-11 12:26:14.000000 ops-py-azure-key-vault-report-4.0.0/ops_py_azure_key_vault_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:26:14.000000 ops-py-azure-key-vault-report-4.0.0/ops_py_azure_key_vault_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 12:26:14.000000 ops-py-azure-key-vault-report-4.0.0/ops_py_azure_key_vault_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-11 12:26:12.000000 ops-py-azure-key-vault-report-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-11 12:26:12.000000 ops-py-azure-key-vault-report-4.0.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:26:14.679647 ops-py-azure-key-vault-report-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 12:26:12.000000 ops-py-azure-key-vault-report-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:14:34.949968 ops-py-azure-key-vault-report-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 13:14:33.000000 ops-py-azure-key-vault-report-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-12 13:14:34.949968 ops-py-azure-key-vault-report-4.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:14:34.949968 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/az_cmd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17634 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/azure_key_vault_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1346 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/html_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1219 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/markdown.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/ms_teams_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      949 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/set_timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:14:34.949968 ops-py-azure-key-vault-report-4.0.1/ops_py_azure_key_vault_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-12 13:14:34.000000 ops-py-azure-key-vault-report-4.0.1/ops_py_azure_key_vault_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-12 13:14:34.000000 ops-py-azure-key-vault-report-4.0.1/ops_py_azure_key_vault_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:14:34.000000 ops-py-azure-key-vault-report-4.0.1/ops_py_azure_key_vault_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 13:14:34.000000 ops-py-azure-key-vault-report-4.0.1/ops_py_azure_key_vault_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 13:14:33.000000 ops-py-azure-key-vault-report-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-12 13:14:33.000000 ops-py-azure-key-vault-report-4.0.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:14:34.949968 ops-py-azure-key-vault-report-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 13:14:33.000000 ops-py-azure-key-vault-report-4.0.1/setup.py
```

### Comparing `ops-py-azure-key-vault-report-4.0.0/LICENSE` & `ops-py-azure-key-vault-report-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-4.0.0/PKG-INFO` & `ops-py-azure-key-vault-report-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-report
-Version: 4.0.0
+Version: 4.0.1
 Summary: Output a Key Vault Secrets report
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/az_cmd.py` & `ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/az_cmd.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/azure_key_vault_report.py` & `ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/azure_key_vault_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,16 +96,16 @@
         self.report = []
         self.summary = {}
         self.summary_md = ""
         self.summary_values = config.get("summary")
         self.report_values = config.get("report")
         self.report_full = {
             "created_at": datetime.datetime.utcnow().isoformat(),
-            "summary": {"rows": []},
-            "report": {"rows": []}
+            "summary": {},
+            "report": {}
         }
 
     def sort_items(self, expired_days=7, will_expire_days=14):
         """Sort the list of dict items by days to expiration
 
         If no parameters provided, this method will return a sorted list of all the records.
         The list will be sorted from top and down, by the oldest 'Expiration' date and then followed
@@ -229,15 +229,15 @@
                     text = v.get("text")
                     rows.append([text, value])
                     self.summary[text] = value
 
         md = Markdown(rows)
         md.set_widths()
         self.summary_md = md.get_output(1)
-        self.report_full["summary"]["rows"].append(self.summary)
+        self.report_full["summary"]["rows"] = [self.summary]
 
     def add_report(self, expire_threshold=None, ignore_no_expiration=True, include_all=False, teams_json=False):
         """creates a plain text report and initiates ms team report generation if specified.
         returns the plain text report.
 
         Parameters
         ----------
@@ -357,15 +357,15 @@
             # Then finally add the row to the rows (The ones that will be reported)
             rows.append(row)
 
             # If a html_table is created, then also add the row to the html table. Used in MS Teams payload
             if self.html_table:
                 self.html_table.add_html_row(*row)
 
-        self.report_full["report"]["rows"].append(self.create_kv_rows(rows_all))
+        self.report_full["report"]["rows"] = self.create_kv_rows(rows_all)
 
         if include_all:
             rows = rows_all
 
         if not rows:
             logging.error("No report generated.")
             return
```

### Comparing `ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/config.py` & `ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/config.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/html_table.py` & `ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/html_table.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/markdown.py` & `ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/markdown.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/ms_teams_json.py` & `ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/ms_teams_json.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/set_timestamp.py` & `ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/set_timestamp.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-4.0.0/ops_py_azure_key_vault_report.egg-info/PKG-INFO` & `ops-py-azure-key-vault-report-4.0.1/ops_py_azure_key_vault_report.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-report
-Version: 4.0.0
+Version: 4.0.1
 Summary: Output a Key Vault Secrets report
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ops-py-azure-key-vault-report-4.0.0/ops_py_azure_key_vault_report.egg-info/SOURCES.txt` & `ops-py-azure-key-vault-report-4.0.1/ops_py_azure_key_vault_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-4.0.0/readme.md` & `ops-py-azure-key-vault-report-4.0.1/readme.md`

 * *Files identical despite different names*

