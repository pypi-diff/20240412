# Comparing `tmp/telegram_wallet_pay-0.0.3.tar.gz` & `tmp/telegram_wallet_pay-0.0.4.tar.gz`

## Comparing `telegram_wallet_pay-0.0.3.tar` & `telegram_wallet_pay-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/.editorconfig
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/Makefile
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/examples/00_get_started.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/__init__.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/client.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/tools.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/_default.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/money_amount.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/order_new.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/order_preview.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/order_result.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/payment_option.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/update.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/webhook_payload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/tests/test_signature.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/.gitignore
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/README.md
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/.editorconfig
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/Makefile
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/examples/00_get_started.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/__init__.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/client.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/tools.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/_default.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/money_amount.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/order_new.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/order_preview.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/order_result.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/payment_option.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/update.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/webhook_payload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/tests/test_signature.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/README.md
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.0.4/PKG-INFO
```

### Comparing `telegram_wallet_pay-0.0.3/.pre-commit-config.yaml` & `telegram_wallet_pay-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.3/examples/00_get_started.py` & `telegram_wallet_pay-0.0.4/examples/00_get_started.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.3/telegram_wallet_pay/client.py` & `telegram_wallet_pay-0.0.4/telegram_wallet_pay/client.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.3/telegram_wallet_pay/tools.py` & `telegram_wallet_pay-0.0.4/telegram_wallet_pay/tools.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/order_new.py` & `telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/order_new.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/order_preview.py` & `telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/order_preview.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.3/telegram_wallet_pay/schemas/webhook_payload.py` & `telegram_wallet_pay-0.0.4/telegram_wallet_pay/schemas/webhook_payload.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.3/tests/test_signature.py` & `telegram_wallet_pay-0.0.4/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.3/.gitignore` & `telegram_wallet_pay-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.0.3/pyproject.toml` & `telegram_wallet_pay-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "telegram-wallet-pay"
 dynamic = ["version"]
 description = "Async client for Telegram Wallet Pay API"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 license = "MIT"
 authors = [
     { name = "Oleg Abramov", email = "oleg@trueweb.app" },
 ]
 maintainers = [
     { name = "Oleg Abramov", email = "oleg@trueweb.app" },
 ]
@@ -24,39 +24,40 @@
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Framework :: AsyncIO",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "aiohttp>=3.8.5,<3.10.0",
-    "pydantic>=2.4",
+    "aiohttp>=3.8.5,<3.10",
+    "pydantic>=2.4,<3",
 ]
 
 [project.optional-dependencies]
 dev = [
     "ruff>=0",
     "mypy>=1",
     "pre-commit>=3",
 ]
 test = [
     "coverage>=7",
-    "pytest>=7",
+    "pytest>=8",
     "pytest-asyncio>=0",
-    "pytest-cov>=4",
+    "pytest-cov>=5",
 ]
 
 
 
 [project.urls]
 Repository = "https://github.com/Olegt0rr/TelegramWalletPay"
 
@@ -79,22 +80,22 @@
 
 [tool.hatch.envs.default.scripts]
 lint = [
     "ruff check telegram_wallet_pay --fix",
 ]
 
 [tool.hatch.envs.dev]
-python = "3.9"
+python = "3.8"
 features = [
     "dev",
     "test",
 ]
 
 [[tool.hatch.envs.test.matrix]]
-python = ["3.9", "310", "311", "312"]
+python = ["3.8", "3.9", "310", "311", "312"]
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 testpaths = [
     "tests",
 ]
 
@@ -161,16 +162,16 @@
 
 # Same as Black.
 line-length = 88
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-# Assume Python 3.9
-target-version = "py39"
+# Assume minimal Python version
+target-version = "py38"
 
 [tool.ruff.mccabe]
 max-complexity = 10
 
 [tool.ruff.flake8-type-checking]
 runtime-evaluated-base-classes = ["pydantic.BaseModel", "telegram_wallet_pay.schemas._default.DefaultModel"]
```

