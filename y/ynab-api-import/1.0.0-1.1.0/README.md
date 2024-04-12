# Comparing `tmp/ynab_api_import-1.0.0.tar.gz` & `tmp/ynab_api_import-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynab_api_import-1.0.0.tar", max compression
+gzip compressed data, was "ynab_api_import-1.1.0.tar", max compression
```

## Comparing `ynab_api_import-1.0.0.tar` & `ynab_api_import-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    35148 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/LICENSE
--rw-r--r--   0        0        0     6098 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/README.md
--rw-r--r--   0        0        0      832 2024-04-04 16:33:53.200009 ynab_api_import-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/__init__.py
--rw-r--r--   0        0        0     1465 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/accountfetcher.py
--rw-r--r--   0        0        0      340 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/memocleaner.py
--rw-r--r--   0        0        0      757 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/models/config.py
--rw-r--r--   0        0        0      223 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/models/exceptions.py
--rw-r--r--   0        0        0     1466 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/models/transaction.py
--rw-r--r--   0        0        0     2913 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/requisitionhandler.py
--rw-r--r--   0        0        0      904 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/transactionfetcher.py
--rw-r--r--   0        0        0     3548 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/ynabapiimport.py
--rw-r--r--   0        0        0      801 2024-04-04 16:33:35.323880 ynab_api_import-1.0.0/ynabapiimport/ynabclient.py
--rw-r--r--   0        0        0     6907 1970-01-01 00:00:00.000000 ynab_api_import-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-12 06:16:15.550381 ynab_api_import-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6516 2024-04-12 06:16:15.550381 ynab_api_import-1.1.0/README.md
+-rw-r--r--   0        0        0      832 2024-04-12 06:16:30.322406 ynab_api_import-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-12 06:16:15.550381 ynab_api_import-1.1.0/ynabapiimport/__init__.py
+-rw-r--r--   0        0        0     1373 2024-04-12 06:16:15.550381 ynab_api_import-1.1.0/ynabapiimport/accountclient.py
+-rw-r--r--   0        0        0     1465 2024-04-12 06:16:15.550381 ynab_api_import-1.1.0/ynabapiimport/accountfetcher.py
+-rw-r--r--   0        0        0       48 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/exceptions.py
+-rw-r--r--   0        0        0      340 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/memocleaner.py
+-rw-r--r--   0        0        0      757 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/models/config.py
+-rw-r--r--   0        0        0      223 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/models/exceptions.py
+-rw-r--r--   0        0        0     1466 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/models/transaction.py
+-rw-r--r--   0        0        0     2913 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/requisitionhandler.py
+-rw-r--r--   0        0        0     5817 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/ynabapiimport.py
+-rw-r--r--   0        0        0     1036 2024-04-12 06:16:15.554381 ynab_api_import-1.1.0/ynabapiimport/ynabclient.py
+-rw-r--r--   0        0        0     7325 1970-01-01 00:00:00.000000 ynab_api_import-1.1.0/PKG-INFO
```

### Comparing `ynab_api_import-1.0.0/LICENSE` & `ynab_api_import-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.0.0/README.md` & `ynab_api_import-1.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -92,14 +92,19 @@
                                 secret_id='<secret_id>', 
                                 secret_key='<secret_key>',
                                 reference='<reference>',
                                 token='<ynab_token>',
                                 budget_id='<budget_id>',
                                 account_id='<account_id>')
 ```
+### Compare balances
+This method will fetch the available [balance variants](https://developer.gocardless.com/bank-account-data/balance) for your account from the API and compare them to the balance in YNAB. It compares the plain balance values as well as the balances minus the sum of still pending transactions. If none of them match it raises a `BalancesDontMatchError`
+```py
+ynab_api_import.compare_balances()
+```
 ### Delete current bank authorization
 By default you can create only one bank authorization per reference. If you need to replace the authorization under 
 your current reference you can explicitly do that by setting the `delete_current_auth` option when creating and auth 
 link.
 ```py
 ynab_api_import.create_auth_link(institution_id='<institution_id>', delete_current_auth=True)
 ```
```

### Comparing `ynab_api_import-1.0.0/pyproject.toml` & `ynab_api_import-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry-core.masonry.api"
 
 [tool.poetry]
 name = "ynab-api-import"
-version = "1.0.0"
+version = "1.1.0"
 authors = ["Daniel Basta <ynab@basta.info>"]
 description = "Library to import bank transactions via API into You Need A Budget (YNAB)"
 readme = "README.md"
 license = 'MIT'
 packages = [{include = 'ynabapiimport'}]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ynab_api_import-1.0.0/ynabapiimport/accountfetcher.py` & `ynab_api_import-1.1.0/ynabapiimport/accountfetcher.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.0.0/ynabapiimport/models/config.py` & `ynab_api_import-1.1.0/ynabapiimport/models/config.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.0.0/ynabapiimport/models/transaction.py` & `ynab_api_import-1.1.0/ynabapiimport/models/transaction.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.0.0/ynabapiimport/requisitionhandler.py` & `ynab_api_import-1.1.0/ynabapiimport/requisitionhandler.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.0.0/ynabapiimport/ynabclient.py` & `ynab_api_import-1.1.0/ynabapiimport/ynabclient.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,7 +19,13 @@
 		common_attributes = {'account_id': self._account_id, 'cleared': 'cleared'}
 		data = {'transactions': [{**t.as_dict(), **common_attributes} for t in transactions]}
 		r = requests.post(f"{YNAB_BASE_URL}/budgets/{self._budget_id}/transactions",
 						  json=data,
 						  headers=self._header)
 		r.raise_for_status()
 		return len(r.json()['data']['transaction_ids'])
+
+	def fetch_balance(self) -> int:
+		r = requests.get(f"{YNAB_BASE_URL}/budgets/{self._budget_id}/accounts/{self._account_id}",
+						 headers=self._header)
+		r.raise_for_status()
+		return r.json()['data']['account']['cleared_balance']
```

### Comparing `ynab_api_import-1.0.0/PKG-INFO` & `ynab_api_import-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynab-api-import
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library to import bank transactions via API into You Need A Budget (YNAB)
 License: MIT
 Author: Daniel Basta
 Author-email: ynab@basta.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -114,14 +114,19 @@
                                 secret_id='<secret_id>', 
                                 secret_key='<secret_key>',
                                 reference='<reference>',
                                 token='<ynab_token>',
                                 budget_id='<budget_id>',
                                 account_id='<account_id>')
 ```
+### Compare balances
+This method will fetch the available [balance variants](https://developer.gocardless.com/bank-account-data/balance) for your account from the API and compare them to the balance in YNAB. It compares the plain balance values as well as the balances minus the sum of still pending transactions. If none of them match it raises a `BalancesDontMatchError`
+```py
+ynab_api_import.compare_balances()
+```
 ### Delete current bank authorization
 By default you can create only one bank authorization per reference. If you need to replace the authorization under 
 your current reference you can explicitly do that by setting the `delete_current_auth` option when creating and auth 
 link.
 ```py
 ynab_api_import.create_auth_link(institution_id='<institution_id>', delete_current_auth=True)
 ```
```

