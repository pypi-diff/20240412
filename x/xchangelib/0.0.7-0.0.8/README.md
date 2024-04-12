# Comparing `tmp/xchangelib-0.0.7.tar.gz` & `tmp/xchangelib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchangelib-0.0.7.tar", last modified: Thu Apr 11 08:41:50 2024, max compression
+gzip compressed data, was "xchangelib-0.0.8.tar", last modified: Fri Apr 12 03:12:19 2024, max compression
```

## Comparing `xchangelib-0.0.7.tar` & `xchangelib-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:50.234673 xchangelib-0.0.7/
--rw-r--r--   0 rohanv     (501) staff       (20)     1070 2024-04-11 08:41:35.000000 xchangelib-0.0.7/LICENSE
--rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-04-11 08:41:50.233536 xchangelib-0.0.7/PKG-INFO
--rw-r--r--   0 rohanv     (501) staff       (20)      140 2024-04-11 08:41:35.000000 xchangelib-0.0.7/README.md
--rw-r--r--   0 rohanv     (501) staff       (20)      650 2024-04-11 08:41:35.000000 xchangelib-0.0.7/pyproject.toml
--rw-r--r--   0 rohanv     (501) staff       (20)       38 2024-04-11 08:41:50.234868 xchangelib-0.0.7/setup.cfg
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:50.224705 xchangelib-0.0.7/src/
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:50.229849 xchangelib-0.0.7/src/xchangelib/
--rw-r--r--   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:35.000000 xchangelib-0.0.7/src/xchangelib/__init__.py
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:50.225042 xchangelib-0.0.7/src/xchangelib/docs/
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:50.231921 xchangelib-0.0.7/src/xchangelib/docs/source/
--rw-r--r--   0 rohanv     (501) staff       (20)     2246 2024-04-11 08:41:35.000000 xchangelib-0.0.7/src/xchangelib/docs/source/conf.py
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:50.232424 xchangelib-0.0.7/src/xchangelib/examples/
--rw-r--r--   0 rohanv     (501) staff       (20)     3683 2024-04-11 08:41:35.000000 xchangelib-0.0.7/src/xchangelib/examples/example_bot.py
--rw-r--r--   0 rohanv     (501) staff       (20)    12187 2024-04-11 08:41:35.000000 xchangelib-0.0.7/src/xchangelib/service_pb2.py
--rw-r--r--   0 rohanv     (501) staff       (20)     8437 2024-04-11 08:41:35.000000 xchangelib-0.0.7/src/xchangelib/service_pb2_grpc.py
--rw-r--r--   0 rohanv     (501) staff       (20)      398 2024-04-11 08:41:35.000000 xchangelib-0.0.7/src/xchangelib/setup.py
--rw-r--r--   0 rohanv     (501) staff       (20)    15346 2024-04-11 08:41:35.000000 xchangelib-0.0.7/src/xchangelib/xchange_client.py
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-11 08:41:50.232982 xchangelib-0.0.7/src/xchangelib.egg-info/
--rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-04-11 08:41:50.000000 xchangelib-0.0.7/src/xchangelib.egg-info/PKG-INFO
--rw-r--r--   0 rohanv     (501) staff       (20)      444 2024-04-11 08:41:50.000000 xchangelib-0.0.7/src/xchangelib.egg-info/SOURCES.txt
--rw-r--r--   0 rohanv     (501) staff       (20)        1 2024-04-11 08:41:50.000000 xchangelib-0.0.7/src/xchangelib.egg-info/dependency_links.txt
--rw-r--r--   0 rohanv     (501) staff       (20)       49 2024-04-11 08:41:50.000000 xchangelib-0.0.7/src/xchangelib.egg-info/requires.txt
--rw-r--r--   0 rohanv     (501) staff       (20)       11 2024-04-11 08:41:50.000000 xchangelib-0.0.7/src/xchangelib.egg-info/top_level.txt
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-12 03:12:19.933633 xchangelib-0.0.8/
+-rw-r--r--   0 rohanv     (501) staff       (20)     1070 2024-04-12 03:12:01.000000 xchangelib-0.0.8/LICENSE
+-rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-04-12 03:12:19.933036 xchangelib-0.0.8/PKG-INFO
+-rw-r--r--   0 rohanv     (501) staff       (20)      140 2024-04-12 03:12:01.000000 xchangelib-0.0.8/README.md
+-rw-r--r--   0 rohanv     (501) staff       (20)      650 2024-04-12 03:12:01.000000 xchangelib-0.0.8/pyproject.toml
+-rw-r--r--   0 rohanv     (501) staff       (20)       38 2024-04-12 03:12:19.933775 xchangelib-0.0.8/setup.cfg
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-12 03:12:19.925155 xchangelib-0.0.8/src/
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-12 03:12:19.928494 xchangelib-0.0.8/src/xchangelib/
+-rw-r--r--   0 rohanv     (501) staff       (20)        0 2024-04-12 03:12:01.000000 xchangelib-0.0.8/src/xchangelib/__init__.py
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-12 03:12:19.925509 xchangelib-0.0.8/src/xchangelib/docs/
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-12 03:12:19.931303 xchangelib-0.0.8/src/xchangelib/docs/source/
+-rw-r--r--   0 rohanv     (501) staff       (20)     2246 2024-04-12 03:12:01.000000 xchangelib-0.0.8/src/xchangelib/docs/source/conf.py
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-12 03:12:19.931789 xchangelib-0.0.8/src/xchangelib/examples/
+-rw-r--r--   0 rohanv     (501) staff       (20)     3683 2024-04-12 03:12:01.000000 xchangelib-0.0.8/src/xchangelib/examples/example_bot.py
+-rw-r--r--   0 rohanv     (501) staff       (20)    12187 2024-04-12 03:12:01.000000 xchangelib-0.0.8/src/xchangelib/service_pb2.py
+-rw-r--r--   0 rohanv     (501) staff       (20)     8437 2024-04-12 03:12:01.000000 xchangelib-0.0.8/src/xchangelib/service_pb2_grpc.py
+-rw-r--r--   0 rohanv     (501) staff       (20)      398 2024-04-12 03:12:01.000000 xchangelib-0.0.8/src/xchangelib/setup.py
+-rw-r--r--   0 rohanv     (501) staff       (20)    15498 2024-04-12 03:12:01.000000 xchangelib-0.0.8/src/xchangelib/xchange_client.py
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-12 03:12:19.932306 xchangelib-0.0.8/src/xchangelib.egg-info/
+-rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-04-12 03:12:19.000000 xchangelib-0.0.8/src/xchangelib.egg-info/PKG-INFO
+-rw-r--r--   0 rohanv     (501) staff       (20)      444 2024-04-12 03:12:19.000000 xchangelib-0.0.8/src/xchangelib.egg-info/SOURCES.txt
+-rw-r--r--   0 rohanv     (501) staff       (20)        1 2024-04-12 03:12:19.000000 xchangelib-0.0.8/src/xchangelib.egg-info/dependency_links.txt
+-rw-r--r--   0 rohanv     (501) staff       (20)       49 2024-04-12 03:12:19.000000 xchangelib-0.0.8/src/xchangelib.egg-info/requires.txt
+-rw-r--r--   0 rohanv     (501) staff       (20)       11 2024-04-12 03:12:19.000000 xchangelib-0.0.8/src/xchangelib.egg-info/top_level.txt
```

### Comparing `xchangelib-0.0.7/LICENSE` & `xchangelib-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.7/PKG-INFO` & `xchangelib-0.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchangelib
-Version: 0.0.7
+Version: 0.0.8
 Summary: A client library for interacting with xchange-v3
 Author-email: Rohan Voddhi <rohan.voddhi@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/UChicagoFM/xchangelib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xchangelib-0.0.7/pyproject.toml` & `xchangelib-0.0.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xchangelib"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     { name="Rohan Voddhi", email="rohan.voddhi@gmail.com" },
 ]
 description = "A client library for interacting with xchange-v3"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ['setuptools>=69.0','protobuf==5.26.0', 'grpcio==1.62.1']
```

### Comparing `xchangelib-0.0.7/src/xchangelib/docs/source/conf.py` & `xchangelib-0.0.8/src/xchangelib/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 project = 'xchangelib'
 copyright = '2024, UChicagoFM'
 author = 'UChicagoFM'
 
 
 # The full version, including alpha/beta/rc tags
-release = '0.0.0'
+release = '0.0.8'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `xchangelib-0.0.7/src/xchangelib/examples/example_bot.py` & `xchangelib-0.0.8/src/xchangelib/examples/example_bot.py`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.7/src/xchangelib/service_pb2.py` & `xchangelib-0.0.8/src/xchangelib/service_pb2.py`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.7/src/xchangelib/service_pb2_grpc.py` & `xchangelib-0.0.8/src/xchangelib/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.7/src/xchangelib/xchange_client.py` & `xchangelib-0.0.8/src/xchangelib/xchange_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging
 from dataclasses import dataclass, field
 from collections import defaultdict
 from typing import Optional
 import time
 
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 logging.basicConfig(level=logging.INFO)
 _LOGGER = logging.getLogger("xchange-client")
 _LOGGER.setLevel(logging.INFO)
 
 
 @dataclass
@@ -115,17 +115,17 @@
         else:
             limit_order_msg = utc_bot_pb2.LimitOrder(qty=qty, px=px)
             order_request = utc_bot_pb2.NewOrderRequest(symbol=symbol, id=str(self.order_id), limit=limit_order_msg,
                                                         side=side)
         request = utc_bot_pb2.ClientMessageToExchange(new_order=order_request)
         key = str(self.order_id)
         self.order_id += 1
+        self.open_orders[key] = [order_request, qty, is_market]
         async with self.request_lock:
             await self.call.write(request)
-        self.open_orders[key] = [order_request, qty, is_market]
         return key
     async def place_swap_order(self, swap: str, qty: int) -> None:
         """
         Places a swap request with the exchange.
         :param swap: Name of the swap
         :param qty: Quantity of swaps to execute
         :return:
@@ -151,14 +151,16 @@
 
     async def handle_order_fill(self, msg) -> None:
         """
         Updates the positions based on the order fill. Then calls the bot specific code.
         :param msg: OrderFillMessage from exchange
         :return:
         """
+        if msg.id not in self.open_orders:
+            return
         order_info: list = self.open_orders[msg.id]
         symbol: str = order_info[0].symbol
         fill_qty: int = msg.qty
         fill_price: int = msg.px
         is_buy = order_info[0].side == utc_bot_pb2.NewOrderRequest.Side.BUY
         self.positions[symbol] += fill_qty * (1 if is_buy else -1)
         self.positions['cash'] += fill_qty * fill_price * (-1 if is_buy else 1)
@@ -175,27 +177,29 @@
 
     async def handle_order_rejected(self, msg) -> None:
         """
         Calls the users order rejection handler and then removes it from the open orders.
         :param msg: Order Rejected Message
         """
         await self.bot_handle_order_rejected(msg.id, msg.reason)
-        self.open_orders.pop(msg.id)
+        if msg.id in self.open_orders:
+            self.open_orders.pop(msg.id)
 
     async def handle_cancel_response(self, msg):
         """
         Processes a cancel order response and calls the users handler.
         :param msg:
         :return:
         """
         result_type = msg.WhichOneof('result')
         if result_type == 'ok':
             _LOGGER.info("Cancel order %s successful.", msg.id)
             await self.bot_handle_cancel_response(msg.id, True, None)
-            self.open_orders.pop(msg.id)
+            if msg.id in self.open_orders:
+                self.open_orders.pop(msg.id)
         else:
             _LOGGER.info("Failed to cancel order %s.", msg.id)
             await self.bot_handle_cancel_response(msg.id, False, msg.error)
 
     async def handle_swap_response(self, msg) -> None:
         """
         Updates positions if swap was successful.
```

### Comparing `xchangelib-0.0.7/src/xchangelib.egg-info/PKG-INFO` & `xchangelib-0.0.8/src/xchangelib.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchangelib
-Version: 0.0.7
+Version: 0.0.8
 Summary: A client library for interacting with xchange-v3
 Author-email: Rohan Voddhi <rohan.voddhi@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/UChicagoFM/xchangelib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

