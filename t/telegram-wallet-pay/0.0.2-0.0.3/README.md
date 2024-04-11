# Comparing `tmp/telegram_wallet_pay-0.0.2.tar.gz` & `tmp/telegram_wallet_pay-0.0.3.tar.gz`

## Comparing `telegram_wallet_pay-0.0.2.tar` & `telegram_wallet_pay-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/.editorconfig
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/Makefile
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/examples/00_get_started.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/telegram_wallet_pay/__init__.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/telegram_wallet_pay/client.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/telegram_wallet_pay/tools.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/telegram_wallet_pay/schemas/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/telegram_wallet_pay/schemas/_default.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/telegram_wallet_pay/schemas/money_amount.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/telegram_wallet_pay/schemas/order_new.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/telegram_wallet_pay/schemas/order_preview.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/telegram_wallet_pay/schemas/order_result.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/telegram_wallet_pay/schemas/payment_option.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/telegram_wallet_pay/schemas/update.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/telegram_wallet_pay/schemas/webhook_payload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/tests/test_signature.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/.gitignore
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/README.md
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/.editorconfig
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/Makefile
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/examples/00_get_started.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/__init__.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/client.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/tools.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/_default.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/money_amount.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/order_new.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/order_preview.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/order_result.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/payment_option.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/update.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/webhook_payload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/tests/test_signature.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/.gitignore
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/README.md
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/PKG-INFO
```

### Comparing `telegram_wallet_pay-0.0.2/.pre-commit-config.yaml` & `telegram_wallet_pay-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.2/examples/00_get_started.py` & `telegram_wallet_pay-0.0.3/examples/00_get_started.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.2/telegram_wallet_pay/client.py` & `telegram_wallet_pay-0.0.3/telegram_wallet_pay/client.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.2/telegram_wallet_pay/tools.py` & `telegram_wallet_pay-0.0.3/telegram_wallet_pay/tools.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.2/telegram_wallet_pay/schemas/order_new.py` & `telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/order_new.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.2/telegram_wallet_pay/schemas/order_preview.py` & `telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/order_preview.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.2/telegram_wallet_pay/schemas/webhook_payload.py` & `telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/webhook_payload.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.2/tests/test_signature.py` & `telegram_wallet_pay-0.0.3/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.2/.gitignore` & `telegram_wallet_pay-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.2/pyproject.toml` & `telegram_wallet_pay-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.2/PKG-INFO` & `telegram_wallet_pay-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: telegram-wallet-pay
-Version: 0.0.2
+Version: 0.0.3
 Summary: Async client for Telegram Wallet Pay API
 Project-URL: Repository, https://github.com/Olegt0rr/TelegramWalletPay
 Author-email: Oleg Abramov <oleg@trueweb.app>
 Maintainer-email: Oleg Abramov <oleg@trueweb.app>
 License-Expression: MIT
 Keywords: API,Pay,Telegram,Wallet,async
 Classifier: Development Status :: 3 - Alpha
```

