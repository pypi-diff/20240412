# Comparing `tmp/telegram_wallet_pay-0.0.4.tar.gz` & `tmp/telegram_wallet_pay-0.0.5.tar.gz`

## Comparing `telegram_wallet_pay-0.0.4.tar` & `telegram_wallet_pay-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/.editorconfig
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/Makefile
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/examples/00_get_started.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/__init__.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/client.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/tools.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/_default.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/money_amount.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/order_new.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/order_preview.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/order_result.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/payment_option.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/update.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/webhook_payload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/tests/test_signature.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/.gitignore
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/README.md
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/.editorconfig
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/Makefile
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/examples/00_get_started.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/telegram_wallet_pay/__init__.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/telegram_wallet_pay/client.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/telegram_wallet_pay/tools.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/telegram_wallet_pay/schemas/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/telegram_wallet_pay/schemas/_default.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/telegram_wallet_pay/schemas/money_amount.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/telegram_wallet_pay/schemas/order_new.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/telegram_wallet_pay/schemas/order_preview.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/telegram_wallet_pay/schemas/order_result.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/telegram_wallet_pay/schemas/payment_option.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/telegram_wallet_pay/schemas/update.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/telegram_wallet_pay/schemas/webhook_payload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/tests/test_signature.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/README.md
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.5/PKG-INFO
```

### Comparing `telegram_wallet_pay-0.0.4/.pre-commit-config.yaml` & `telegram_wallet_pay-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.4/examples/00_get_started.py` & `telegram_wallet_pay-0.0.5/examples/00_get_started.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.4/telegram_wallet_pay/client.py` & `telegram_wallet_pay-0.0.5/telegram_wallet_pay/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 import logging
 import ssl
-from collections.abc import Mapping
 from contextlib import asynccontextmanager
 from decimal import Decimal
-from typing import Literal, Optional, Union
+from typing import Literal, Optional, Union, Mapping
 
 from aiohttp import ClientResponse, ClientSession, TCPConnector
 
 from telegram_wallet_pay.schemas import MoneyAmount, OrderNew, OrderResult
 
 AUTH_HEADER = "Wpay-Store-Api-Key"
 DEFAULT_API_HOST = "https://pay.wallet.tg"
```

### Comparing `telegram_wallet_pay-0.0.4/telegram_wallet_pay/tools.py` & `telegram_wallet_pay-0.0.5/telegram_wallet_pay/tools.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/order_new.py` & `telegram_wallet_pay-0.0.5/telegram_wallet_pay/schemas/order_new.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/order_preview.py` & `telegram_wallet_pay-0.0.5/telegram_wallet_pay/schemas/order_preview.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/update.py` & `telegram_wallet_pay-0.0.5/telegram_wallet_pay/schemas/update.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from collections.abc import Iterator
 from datetime import datetime
-from typing import List, Literal
+from typing import List, Literal, Iterator
 
 from pydantic import Field
 
 from ._default import DefaultModel, DefaultRootModel
 from .webhook_payload import WebhookPayload
```

### Comparing `telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/webhook_payload.py` & `telegram_wallet_pay-0.0.5/telegram_wallet_pay/schemas/webhook_payload.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.4/tests/test_signature.py` & `telegram_wallet_pay-0.0.5/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.4/.gitignore` & `telegram_wallet_pay-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.4/README.md` & `telegram_wallet_pay-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.4/pyproject.toml` & `telegram_wallet_pay-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.4/PKG-INFO` & `telegram_wallet_pay-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: telegram-wallet-pay
-Version: 0.0.4
+Version: 0.0.5
 Summary: Async client for Telegram Wallet Pay API
 Project-URL: Repository, https://github.com/Olegt0rr/TelegramWalletPay
 Author-email: Oleg Abramov <oleg@trueweb.app>
 Maintainer-email: Oleg Abramov <oleg@trueweb.app>
 License-Expression: MIT
 Keywords: API,Pay,Telegram,Wallet,async
 Classifier: Development Status :: 3 - Alpha
```

