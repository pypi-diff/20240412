# Comparing `tmp/ithaca_py-0.2.0.tar.gz` & `tmp/ithaca_py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ithaca_py-0.2.0.tar", max compression
+gzip compressed data, was "ithaca_py-0.2.1.tar", max compression
```

## Comparing `ithaca_py-0.2.0.tar` & `ithaca_py-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      983 2024-04-09 15:18:24.012787 ithaca_py-0.2.0/README.md
--rw-r--r--   0        0        0     5147 2024-04-09 15:18:24.012787 ithaca_py-0.2.0/ithaca/__init__.py
--rw-r--r--   0        0        0     3656 2024-04-09 15:18:24.012787 ithaca_py-0.2.0/ithaca/analytics.py
--rw-r--r--   0        0        0    10809 2024-04-09 15:18:24.012787 ithaca_py-0.2.0/ithaca/auth.py
--rw-r--r--   0        0        0     5589 2024-04-09 15:18:24.012787 ithaca_py-0.2.0/ithaca/calculation.py
--rw-r--r--   0        0        0     2921 2024-04-09 15:18:24.012787 ithaca_py-0.2.0/ithaca/client.py
--rw-r--r--   0        0        0     1846 2024-04-09 15:18:24.012787 ithaca_py-0.2.0/ithaca/constants.py
--rw-r--r--   0        0        0    12592 2024-04-09 15:18:24.012787 ithaca_py-0.2.0/ithaca/fundlock.py
--rw-r--r--   0        0        0      603 2024-04-09 15:18:24.012787 ithaca_py-0.2.0/ithaca/market.py
--rw-r--r--   0        0        0     6650 2024-04-09 15:18:24.012787 ithaca_py-0.2.0/ithaca/orders.py
--rw-r--r--   0        0        0     1373 2024-04-09 15:18:24.012787 ithaca_py-0.2.0/ithaca/protocol.py
--rw-r--r--   0        0        0     2210 2024-04-09 15:18:24.016787 ithaca_py-0.2.0/ithaca/socket.py
--rw-r--r--   0        0        0      929 2024-04-09 15:18:24.016787 ithaca_py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      983 2024-04-12 05:58:28.073315 ithaca_py-0.2.1/README.md
+-rw-r--r--   0        0        0     5147 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/__init__.py
+-rw-r--r--   0        0        0     3656 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/analytics.py
+-rw-r--r--   0        0        0    10809 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/auth.py
+-rw-r--r--   0        0        0     5589 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/calculation.py
+-rw-r--r--   0        0        0     3206 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/client.py
+-rw-r--r--   0        0        0     1846 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/constants.py
+-rw-r--r--   0        0        0    12592 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/fundlock.py
+-rw-r--r--   0        0        0      603 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/market.py
+-rw-r--r--   0        0        0     6650 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/orders.py
+-rw-r--r--   0        0        0     1373 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/protocol.py
+-rw-r--r--   0        0        0     2210 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/socket.py
+-rw-r--r--   0        0        0      929 2024-04-12 05:58:28.081315 ithaca_py-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.2.1/PKG-INFO
```

### Comparing `ithaca_py-0.2.0/README.md` & `ithaca_py-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.0/ithaca/__init__.py` & `ithaca_py-0.2.1/ithaca/__init__.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.0/ithaca/analytics.py` & `ithaca_py-0.2.1/ithaca/analytics.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.0/ithaca/auth.py` & `ithaca_py-0.2.1/ithaca/auth.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.0/ithaca/calculation.py` & `ithaca_py-0.2.1/ithaca/calculation.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.0/ithaca/client.py` & `ithaca_py-0.2.1/ithaca/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -45,18 +45,29 @@
                 )
             ).set_index("contractId")
             return (
                 pd.DataFrame(res.get("payload")).set_index("contractId").join(contracts)
             )
         return res
 
-    def trade_history(self, expiry=None, currency_pair=None):
+    def trade_history(self,
+                      date_from: int = None,
+                      date_to: int = None,
+                      offset: int = None,
+                      limit: int = None):
+
         """Get trade history."""
-        body = {"expiry": expiry, "currencyPair": currency_pair}
-        if expiry or currency_pair:
+        """date_from/to are timestamps in backend"""
+        body = {
+            "from": date_from,
+            "to": date_to,
+            "offset": offset,
+            "limit": limit
+        }
+        if date_from or date_to or offset or limit:
             return self.parent.post("/clientapi/tradeHistory", json=body)
         else:
             return self.parent.post("/clientapi/tradeHistory")
 
     def historical_positions(self, expiry):
         """Get client historical positions."""
         body = {"expiry": expiry}
```

### Comparing `ithaca_py-0.2.0/ithaca/constants.py` & `ithaca_py-0.2.1/ithaca/constants.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.0/ithaca/fundlock.py` & `ithaca_py-0.2.1/ithaca/fundlock.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.0/ithaca/market.py` & `ithaca_py-0.2.1/ithaca/market.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.0/ithaca/orders.py` & `ithaca_py-0.2.1/ithaca/orders.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.0/ithaca/protocol.py` & `ithaca_py-0.2.1/ithaca/protocol.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.0/ithaca/socket.py` & `ithaca_py-0.2.1/ithaca/socket.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.0/pyproject.toml` & `ithaca_py-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ithaca_py"
-version = "0.2.0"
+version = "0.2.1"
 description = "Ithaca Protocol SDK"
 authors = ["nhaga <nhaga5@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ithaca"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ithaca_py-0.2.0/PKG-INFO` & `ithaca_py-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ithaca_py
-Version: 0.2.0
+Version: 0.2.1
 Summary: Ithaca Protocol SDK
 Author: nhaga
 Author-email: nhaga5@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

