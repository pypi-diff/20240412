# Comparing `tmp/saltedge-0.1.2.tar.gz` & `tmp/saltedge-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saltedge-0.1.2.tar", max compression
+gzip compressed data, was "saltedge-0.1.3.tar", max compression
```

## Comparing `saltedge-0.1.2.tar` & `saltedge-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11320 2024-04-12 08:43:48.798088 saltedge-0.1.2/LICENSE
--rw-r--r--   0        0        0     3981 2024-04-12 08:43:48.798088 saltedge-0.1.2/README.md
--rw-r--r--   0        0        0      782 2024-04-12 08:43:48.798088 saltedge-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/__init__.py
--rw-r--r--   0        0        0     2997 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/api/__init__.py
--rw-r--r--   0        0        0     2594 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/api/accounts.py
--rw-r--r--   0        0        0     1731 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/api/attempts.py
--rw-r--r--   0        0        0      993 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/api/connections.py
--rw-r--r--   0        0        0      768 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/api/countries.py
--rw-r--r--   0        0        0      437 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/api/customers.py
--rw-r--r--   0        0        0        0 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/api/lead/__init__.py
--rw-r--r--   0        0        0     1840 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/api/lead/leads.py
--rw-r--r--   0        0        0     5292 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/api/lead/sessions.py
--rw-r--r--   0        0        0     1667 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/api/providers.py
--rw-r--r--   0        0        0     3433 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/api/transactions.py
--rw-r--r--   0        0        0     6383 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/http.py
--rw-r--r--   0        0        0      349 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/logging.py
--rw-r--r--   0        0        0     1267 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/services.py
--rw-r--r--   0        0        0        0 2024-04-12 08:43:48.802089 saltedge-0.1.2/saltedge/tests/__init__.py
--rw-r--r--   0        0        0     4651 1970-01-01 00:00:00.000000 saltedge-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11320 2024-04-12 09:09:31.802199 saltedge-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4032 2024-04-12 09:09:31.802199 saltedge-0.1.3/README.md
+-rw-r--r--   0        0        0      782 2024-04-12 09:09:31.802199 saltedge-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-12 09:09:31.802199 saltedge-0.1.3/saltedge/__init__.py
+-rw-r--r--   0        0        0     2997 2024-04-12 09:09:31.802199 saltedge-0.1.3/saltedge/api/__init__.py
+-rw-r--r--   0        0        0     2594 2024-04-12 09:09:31.806199 saltedge-0.1.3/saltedge/api/accounts.py
+-rw-r--r--   0        0        0     1731 2024-04-12 09:09:31.806199 saltedge-0.1.3/saltedge/api/attempts.py
+-rw-r--r--   0        0        0      993 2024-04-12 09:09:31.806199 saltedge-0.1.3/saltedge/api/connections.py
+-rw-r--r--   0        0        0      768 2024-04-12 09:09:31.806199 saltedge-0.1.3/saltedge/api/countries.py
+-rw-r--r--   0        0        0      437 2024-04-12 09:09:31.806199 saltedge-0.1.3/saltedge/api/customers.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:09:31.806199 saltedge-0.1.3/saltedge/api/lead/__init__.py
+-rw-r--r--   0        0        0     1840 2024-04-12 09:09:31.806199 saltedge-0.1.3/saltedge/api/lead/leads.py
+-rw-r--r--   0        0        0     5292 2024-04-12 09:09:31.806199 saltedge-0.1.3/saltedge/api/lead/sessions.py
+-rw-r--r--   0        0        0     1667 2024-04-12 09:09:31.806199 saltedge-0.1.3/saltedge/api/providers.py
+-rw-r--r--   0        0        0     3433 2024-04-12 09:09:31.806199 saltedge-0.1.3/saltedge/api/transactions.py
+-rw-r--r--   0        0        0     6383 2024-04-12 09:09:31.806199 saltedge-0.1.3/saltedge/http.py
+-rw-r--r--   0        0        0      349 2024-04-12 09:09:31.806199 saltedge-0.1.3/saltedge/logging.py
+-rw-r--r--   0        0        0     1267 2024-04-12 09:09:31.806199 saltedge-0.1.3/saltedge/services.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:09:31.806199 saltedge-0.1.3/saltedge/tests/__init__.py
+-rw-r--r--   0        0        0     4702 1970-01-01 00:00:00.000000 saltedge-0.1.3/PKG-INFO
```

### Comparing `saltedge-0.1.2/LICENSE` & `saltedge-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.2/README.md` & `saltedge-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,22 @@
 A simple python wrapper around [saltedge](https://docs.saltedge.com/general/) api with some utilities.
 
 ## Features
 - Automatic page handling through generators
 - Modular design
 - Dynamic payload with typing support with TypedDict
 
-# Quickstart - Partner Account API (AISP)
+# Quickstart 
+
+## Installation
+```
+pip install saltedge
+```
+
+## Partner API overview (AISP)
 https://docs.saltedge.com/partners/v1/#quick_start
 ```python
 import datetime as dt
 
 from saltedge.api.accounts import AccountDTO
 from saltedge.api.connections import ConnectionDTO
 from saltedge.api.lead.leads import CreateLeadDTO
@@ -92,8 +99,8 @@
 - poetry
 
 ## Dev quickstart
 ```shell
 git clone git@github.com:besil/saltedge.git
 cd saltedge
 poetry install
-```
+```
```

### Comparing `saltedge-0.1.2/pyproject.toml` & `saltedge-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saltedge"
-version = "0.1.2"
+version = "0.1.3"
 description = "A simple python wrapper around saltedge api with some utilities."
 authors = ["besil <silvio.bernardinello@outlook.com>"]
 license = "apache v2"
 readme = "README.md"
 homepage = "https://pypi.org/project/saltedge/"
 repository = "https://github.com/besil/saltedge"
```

### Comparing `saltedge-0.1.2/saltedge/api/__init__.py` & `saltedge-0.1.3/saltedge/api/__init__.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.2/saltedge/api/accounts.py` & `saltedge-0.1.3/saltedge/api/accounts.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.2/saltedge/api/attempts.py` & `saltedge-0.1.3/saltedge/api/attempts.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.2/saltedge/api/connections.py` & `saltedge-0.1.3/saltedge/api/connections.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.2/saltedge/api/countries.py` & `saltedge-0.1.3/saltedge/api/countries.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.2/saltedge/api/lead/leads.py` & `saltedge-0.1.3/saltedge/api/lead/leads.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.2/saltedge/api/lead/sessions.py` & `saltedge-0.1.3/saltedge/api/lead/sessions.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.2/saltedge/api/providers.py` & `saltedge-0.1.3/saltedge/api/providers.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.2/saltedge/api/transactions.py` & `saltedge-0.1.3/saltedge/api/transactions.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.2/saltedge/http.py` & `saltedge-0.1.3/saltedge/http.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.2/saltedge/services.py` & `saltedge-0.1.3/saltedge/services.py`

 * *Files identical despite different names*

### Comparing `saltedge-0.1.2/PKG-INFO` & `saltedge-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saltedge
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple python wrapper around saltedge api with some utilities.
 Home-page: https://pypi.org/project/saltedge/
 License: apache v2
 Author: besil
 Author-email: silvio.bernardinello@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
@@ -20,15 +20,22 @@
 A simple python wrapper around [saltedge](https://docs.saltedge.com/general/) api with some utilities.
 
 ## Features
 - Automatic page handling through generators
 - Modular design
 - Dynamic payload with typing support with TypedDict
 
-# Quickstart - Partner Account API (AISP)
+# Quickstart 
+
+## Installation
+```
+pip install saltedge
+```
+
+## Partner API overview (AISP)
 https://docs.saltedge.com/partners/v1/#quick_start
 ```python
 import datetime as dt
 
 from saltedge.api.accounts import AccountDTO
 from saltedge.api.connections import ConnectionDTO
 from saltedge.api.lead.leads import CreateLeadDTO
@@ -111,7 +118,8 @@
 
 ## Dev quickstart
 ```shell
 git clone git@github.com:besil/saltedge.git
 cd saltedge
 poetry install
 ```
+
```

