# Comparing `tmp/saltedge-0.1.0.tar.gz` & `tmp/saltedge-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saltedge-0.1.0.tar", max compression
+gzip compressed data, was "saltedge-0.1.1.tar", max compression
```

## Comparing `saltedge-0.1.0.tar` & `saltedge-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11320 2024-04-02 08:20:58.242743 saltedge-0.1.0/LICENSE
--rw-r--r--   0        0        0     3981 2024-04-12 08:10:05.980894 saltedge-0.1.0/README.md
--rw-r--r--   0        0        0      667 2024-04-02 08:20:58.243550 saltedge-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 08:20:58.243764 saltedge-0.1.0/saltedge/__init__.py
--rw-r--r--   0        0        0     2997 2024-04-03 12:32:36.985455 saltedge-0.1.0/saltedge/api/__init__.py
--rw-r--r--   0        0        0     2594 2024-04-03 13:05:15.655474 saltedge-0.1.0/saltedge/api/accounts.py
--rw-r--r--   0        0        0     1731 2024-04-03 12:53:43.453297 saltedge-0.1.0/saltedge/api/attempts.py
--rw-r--r--   0        0        0      993 2024-04-03 12:58:14.319443 saltedge-0.1.0/saltedge/api/connections.py
--rw-r--r--   0        0        0      768 2024-04-03 11:56:59.551818 saltedge-0.1.0/saltedge/api/countries.py
--rw-r--r--   0        0        0      437 2024-04-03 12:33:28.394963 saltedge-0.1.0/saltedge/api/customers.py
--rw-r--r--   0        0        0        0 2024-04-03 08:19:30.762648 saltedge-0.1.0/saltedge/api/lead/__init__.py
--rw-r--r--   0        0        0     1840 2024-04-11 15:37:58.951121 saltedge-0.1.0/saltedge/api/lead/leads.py
--rw-r--r--   0        0        0     5292 2024-04-03 12:26:31.321598 saltedge-0.1.0/saltedge/api/lead/sessions.py
--rw-r--r--   0        0        0     1667 2024-04-03 11:54:52.394428 saltedge-0.1.0/saltedge/api/providers.py
--rw-r--r--   0        0        0     3433 2024-04-03 13:30:10.866139 saltedge-0.1.0/saltedge/api/transactions.py
--rw-r--r--   0        0        0     6383 2024-04-11 15:14:12.401723 saltedge-0.1.0/saltedge/http.py
--rw-r--r--   0        0        0      349 2024-04-03 12:25:33.360112 saltedge-0.1.0/saltedge/logging.py
--rw-r--r--   0        0        0     1267 2024-04-11 15:49:27.378213 saltedge-0.1.0/saltedge/services.py
--rw-r--r--   0        0        0        0 2024-04-02 08:20:58.245219 saltedge-0.1.0/saltedge/tests/__init__.py
--rw-r--r--   0        0        0     4525 1970-01-01 00:00:00.000000 saltedge-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11320 2024-04-02 08:20:58.242743 saltedge-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3981 2024-04-12 08:10:05.980894 saltedge-0.1.1/README.md
+-rw-r--r--   0        0        0      828 2024-04-12 08:29:46.902022 saltedge-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 08:20:58.243764 saltedge-0.1.1/saltedge/__init__.py
+-rw-r--r--   0        0        0     2997 2024-04-03 12:32:36.985455 saltedge-0.1.1/saltedge/api/__init__.py
+-rw-r--r--   0        0        0     2594 2024-04-03 13:05:15.655474 saltedge-0.1.1/saltedge/api/accounts.py
+-rw-r--r--   0        0        0     1731 2024-04-03 12:53:43.453297 saltedge-0.1.1/saltedge/api/attempts.py
+-rw-r--r--   0        0        0      993 2024-04-03 12:58:14.319443 saltedge-0.1.1/saltedge/api/connections.py
+-rw-r--r--   0        0        0      768 2024-04-03 11:56:59.551818 saltedge-0.1.1/saltedge/api/countries.py
+-rw-r--r--   0        0        0      437 2024-04-03 12:33:28.394963 saltedge-0.1.1/saltedge/api/customers.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:19:30.762648 saltedge-0.1.1/saltedge/api/lead/__init__.py
+-rw-r--r--   0        0        0     1840 2024-04-11 15:37:58.951121 saltedge-0.1.1/saltedge/api/lead/leads.py
+-rw-r--r--   0        0        0     5292 2024-04-03 12:26:31.321598 saltedge-0.1.1/saltedge/api/lead/sessions.py
+-rw-r--r--   0        0        0     1667 2024-04-03 11:54:52.394428 saltedge-0.1.1/saltedge/api/providers.py
+-rw-r--r--   0        0        0     3433 2024-04-03 13:30:10.866139 saltedge-0.1.1/saltedge/api/transactions.py
+-rw-r--r--   0        0        0     6383 2024-04-11 15:14:12.401723 saltedge-0.1.1/saltedge/http.py
+-rw-r--r--   0        0        0      349 2024-04-03 12:25:33.360112 saltedge-0.1.1/saltedge/logging.py
+-rw-r--r--   0        0        0     1267 2024-04-11 15:49:27.378213 saltedge-0.1.1/saltedge/services.py
+-rw-r--r--   0        0        0        0 2024-04-02 08:20:58.245219 saltedge-0.1.1/saltedge/tests/__init__.py
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 saltedge-0.1.1/PKG-INFO
```

### Comparing `saltedge-0.1.0/LICENSE` & `saltedge-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.0/README.md` & `saltedge-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.0/saltedge/api/__init__.py` & `saltedge-0.1.1/saltedge/api/__init__.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.0/saltedge/api/accounts.py` & `saltedge-0.1.1/saltedge/api/accounts.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.0/saltedge/api/attempts.py` & `saltedge-0.1.1/saltedge/api/attempts.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.0/saltedge/api/connections.py` & `saltedge-0.1.1/saltedge/api/connections.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.0/saltedge/api/countries.py` & `saltedge-0.1.1/saltedge/api/countries.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.0/saltedge/api/lead/leads.py` & `saltedge-0.1.1/saltedge/api/lead/leads.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.0/saltedge/api/lead/sessions.py` & `saltedge-0.1.1/saltedge/api/lead/sessions.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.0/saltedge/api/providers.py` & `saltedge-0.1.1/saltedge/api/providers.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.0/saltedge/api/transactions.py` & `saltedge-0.1.1/saltedge/api/transactions.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.0/saltedge/http.py` & `saltedge-0.1.1/saltedge/http.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.0/saltedge/services.py` & `saltedge-0.1.1/saltedge/services.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.0/PKG-INFO` & `saltedge-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: saltedge
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: A simple python wrapper around saltedge api with some utilities.
+Home-page: https://pypi.org/project/saltedge/
 License: apache v2
 Author: besil
 Author-email: silvio.bernardinello@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: black[d] (>=24.3.0,<25.0.0)
 Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Repository, https://github.com/besil/saltedge
 Description-Content-Type: text/markdown
 
 # Saltedge python sdk
 A simple python wrapper around [saltedge](https://docs.saltedge.com/general/) api with some utilities.
 
 ## Features
 - Automatic page handling through generators
```

