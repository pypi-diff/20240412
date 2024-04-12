# Comparing `tmp/pytiqs-1.0.6.tar.gz` & `tmp/pytiqs-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytiqs-1.0.6.tar", last modified: Fri Apr 12 05:30:55 2024, max compression
+gzip compressed data, was "pytiqs-1.0.7.tar", last modified: Fri Apr 12 07:39:14 2024, max compression
```

## Comparing `pytiqs-1.0.6.tar` & `pytiqs-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-12 05:30:55.582163 pytiqs-1.0.6/
--rw-r--r--   0 nitin      (501) staff       (20)     1807 2024-04-12 05:30:55.582063 pytiqs-1.0.6/PKG-INFO
--rw-r--r--   0 nitin      (501) staff       (20)     1304 2024-04-12 04:45:33.000000 pytiqs-1.0.6/README.md
-drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-12 05:30:55.580488 pytiqs-1.0.6/pytiqs/
--rw-r--r--   0 nitin      (501) staff       (20)      172 2024-04-10 04:14:30.000000 pytiqs-1.0.6/pytiqs/__init__.py
--rw-r--r--   0 nitin      (501) staff       (20)      232 2024-04-12 05:30:37.000000 pytiqs-1.0.6/pytiqs/__version__.py
--rw-r--r--   0 nitin      (501) staff       (20)    16952 2024-04-12 04:46:16.000000 pytiqs-1.0.6/pytiqs/connect.py
--rw-r--r--   0 nitin      (501) staff       (20)     2525 2024-04-10 04:14:30.000000 pytiqs-1.0.6/pytiqs/constants.py
--rw-r--r--   0 nitin      (501) staff       (20)      555 2024-04-10 04:14:30.000000 pytiqs-1.0.6/pytiqs/exceptions.py
--rw-r--r--   0 nitin      (501) staff       (20)    19070 2024-04-12 05:28:29.000000 pytiqs-1.0.6/pytiqs/sockets.py
-drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-12 05:30:55.581690 pytiqs-1.0.6/pytiqs.egg-info/
--rw-r--r--   0 nitin      (501) staff       (20)     1807 2024-04-12 05:30:55.000000 pytiqs-1.0.6/pytiqs.egg-info/PKG-INFO
--rw-r--r--   0 nitin      (501) staff       (20)      295 2024-04-12 05:30:55.000000 pytiqs-1.0.6/pytiqs.egg-info/SOURCES.txt
--rw-r--r--   0 nitin      (501) staff       (20)        1 2024-04-12 05:30:55.000000 pytiqs-1.0.6/pytiqs.egg-info/dependency_links.txt
--rw-r--r--   0 nitin      (501) staff       (20)      145 2024-04-12 05:30:55.000000 pytiqs-1.0.6/pytiqs.egg-info/requires.txt
--rw-r--r--   0 nitin      (501) staff       (20)        7 2024-04-12 05:30:55.000000 pytiqs-1.0.6/pytiqs.egg-info/top_level.txt
--rw-r--r--   0 nitin      (501) staff       (20)      290 2024-04-12 05:30:55.582512 pytiqs-1.0.6/setup.cfg
--rw-r--r--   0 nitin      (501) staff       (20)     1192 2024-04-10 04:19:46.000000 pytiqs-1.0.6/setup.py
+drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-12 07:39:14.992782 pytiqs-1.0.7/
+-rw-r--r--   0 nitin      (501) staff       (20)     3284 2024-04-12 07:39:14.992695 pytiqs-1.0.7/PKG-INFO
+-rw-r--r--   0 nitin      (501) staff       (20)     2781 2024-04-12 07:37:57.000000 pytiqs-1.0.7/README.md
+drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-12 07:39:14.990717 pytiqs-1.0.7/pytiqs/
+-rw-r--r--   0 nitin      (501) staff       (20)      172 2024-04-10 04:14:30.000000 pytiqs-1.0.7/pytiqs/__init__.py
+-rw-r--r--   0 nitin      (501) staff       (20)      232 2024-04-12 07:38:20.000000 pytiqs-1.0.7/pytiqs/__version__.py
+-rw-r--r--   0 nitin      (501) staff       (20)    16952 2024-04-12 04:46:16.000000 pytiqs-1.0.7/pytiqs/connect.py
+-rw-r--r--   0 nitin      (501) staff       (20)     2525 2024-04-10 04:14:30.000000 pytiqs-1.0.7/pytiqs/constants.py
+-rw-r--r--   0 nitin      (501) staff       (20)      555 2024-04-10 04:14:30.000000 pytiqs-1.0.7/pytiqs/exceptions.py
+-rw-r--r--   0 nitin      (501) staff       (20)    19070 2024-04-12 05:28:29.000000 pytiqs-1.0.7/pytiqs/sockets.py
+drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-12 07:39:14.992370 pytiqs-1.0.7/pytiqs.egg-info/
+-rw-r--r--   0 nitin      (501) staff       (20)     3284 2024-04-12 07:39:14.000000 pytiqs-1.0.7/pytiqs.egg-info/PKG-INFO
+-rw-r--r--   0 nitin      (501) staff       (20)      295 2024-04-12 07:39:14.000000 pytiqs-1.0.7/pytiqs.egg-info/SOURCES.txt
+-rw-r--r--   0 nitin      (501) staff       (20)        1 2024-04-12 07:39:14.000000 pytiqs-1.0.7/pytiqs.egg-info/dependency_links.txt
+-rw-r--r--   0 nitin      (501) staff       (20)      145 2024-04-12 07:39:14.000000 pytiqs-1.0.7/pytiqs.egg-info/requires.txt
+-rw-r--r--   0 nitin      (501) staff       (20)        7 2024-04-12 07:39:14.000000 pytiqs-1.0.7/pytiqs.egg-info/top_level.txt
+-rw-r--r--   0 nitin      (501) staff       (20)      290 2024-04-12 07:39:14.993334 pytiqs-1.0.7/setup.cfg
+-rw-r--r--   0 nitin      (501) staff       (20)     1192 2024-04-10 04:19:46.000000 pytiqs-1.0.7/setup.py
```

### Comparing `pytiqs-1.0.6/PKG-INFO` & `pytiqs-1.0.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytiqs
-Version: 1.0.6
+Version: 1.0.7
 Summary: The official Python client for the Tiqs trading API
 Home-page: 
 Download-URL: 
 Author: Butterfly Broking Pvt. Ltd.
 Author-email: 
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -14,28 +14,38 @@
 Requires-Dist: six>=1.11.0
 Requires-Dist: pyOpenSSL>=17.5.0
 Requires-Dist: python-dateutil>=2.6.1
 Requires-Dist: autobahn[twisted]==19.11.2
 
 # TIQS API Client
 
-Official Python client for [Tiqs Hummingbird API](https://docs.tiqs.in/documentation/).
+[![PyPI](https://img.shields.io/pypi/v/pytiqs.svg)](https://pypi.python.org/pypi/pytiqs) 
+
+Official Python client for [Tiqs](https://tiqs.in/).
+
+## Documentation
+
+- [Tiqs HTTP API documentation](https://docs.tiqs.in/documentation)
 
 ## Installation
 
 You can install the package using:
-```
+```shell
 python3 -m pip install pytiqs
 ```
 
+update to latest version
+```shell
+python3 -m pip install -U pytiqs
+```
+
 ## API Usage
 
 ```python
 import logging
-import sys
 from pytiqs import Tiqs, constants
 
 
 logging.basicConfig(level=logging.DEBUG,
                     format='%(asctime)s | %(levelname)s | %(name)s:%(lineno)d | %(message)s')
 
 tiqs = Tiqs(app_id="<APP_ID>")
@@ -61,12 +71,74 @@
         amo=False,
         trigger_price=None
     )
     logging.info("order id: {}".format(order_no))
 except Exception as e:
     logging.error("error in order placement: {}".format(e))
     
+# get order by order number
+order = tiqs.get_order("24040200000302")
+
+# delete order
+response = tiqs.delete_order("24040200000302")
+
 # all orders
-tiqs.get_user_orders()
+user_orders = tiqs.get_user_orders()
+
+# all trades
+user_trades = tiqs.get_user_trades()
+
+# user details
+tiqs.user_details()
+
+# positions 
+tiqs.get_positions()
+
+# all instruments
+tiqs.get_instruments()
+
+# market holidays
+holidays = tiqs.holidays()
+
+# index list
+index_list = tiqs.index_list()
 
+# option chain for an underlying asset for a give expiry date
+option_chain = tiqs.option_chain(params={
+    "token": "26009",
+    "exchange": "INDEX",
+    "count": "10",
+    "expiry": "10-APR-2024"
+})
 ```
 
+## Websockets
+
+```python
+import time
+import logging
+from pytiqs import TiqsSocket
+
+
+def on_ticks(ws, ticks):
+    logging.debug("Ticks: {}".format(ticks))
+
+
+def on_connect(ws, response):
+    ws.subscribe([7929])
+    time.sleep(5)
+    ws.set_mode(socketClient.MODE_LTP, [7929])
+
+
+def on_close(ws, code, reason):
+    logging.debug("closed, {}, {}".format(code, reason))
+    ws.stop()
+
+
+socketClient = TiqsSocket(app_id="<APP_ID>", token="<token>")
+socketClient.on_ticks = on_ticks
+socketClient.on_connect = on_connect
+socketClient.on_close = on_close
+
+# if you want to keep this as non-blocking code use socketClient.connect(threaded=True)
+socketClient.connect() 
+```
```

### Comparing `pytiqs-1.0.6/pytiqs/connect.py` & `pytiqs-1.0.7/pytiqs/connect.py`

 * *Files identical despite different names*

### Comparing `pytiqs-1.0.6/pytiqs/constants.py` & `pytiqs-1.0.7/pytiqs/constants.py`

 * *Files identical despite different names*

### Comparing `pytiqs-1.0.6/pytiqs/exceptions.py` & `pytiqs-1.0.7/pytiqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytiqs-1.0.6/pytiqs/sockets.py` & `pytiqs-1.0.7/pytiqs/sockets.py`

 * *Files identical despite different names*

### Comparing `pytiqs-1.0.6/pytiqs.egg-info/PKG-INFO` & `pytiqs-1.0.7/pytiqs.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytiqs
-Version: 1.0.6
+Version: 1.0.7
 Summary: The official Python client for the Tiqs trading API
 Home-page: 
 Download-URL: 
 Author: Butterfly Broking Pvt. Ltd.
 Author-email: 
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -14,28 +14,38 @@
 Requires-Dist: six>=1.11.0
 Requires-Dist: pyOpenSSL>=17.5.0
 Requires-Dist: python-dateutil>=2.6.1
 Requires-Dist: autobahn[twisted]==19.11.2
 
 # TIQS API Client
 
-Official Python client for [Tiqs Hummingbird API](https://docs.tiqs.in/documentation/).
+[![PyPI](https://img.shields.io/pypi/v/pytiqs.svg)](https://pypi.python.org/pypi/pytiqs) 
+
+Official Python client for [Tiqs](https://tiqs.in/).
+
+## Documentation
+
+- [Tiqs HTTP API documentation](https://docs.tiqs.in/documentation)
 
 ## Installation
 
 You can install the package using:
-```
+```shell
 python3 -m pip install pytiqs
 ```
 
+update to latest version
+```shell
+python3 -m pip install -U pytiqs
+```
+
 ## API Usage
 
 ```python
 import logging
-import sys
 from pytiqs import Tiqs, constants
 
 
 logging.basicConfig(level=logging.DEBUG,
                     format='%(asctime)s | %(levelname)s | %(name)s:%(lineno)d | %(message)s')
 
 tiqs = Tiqs(app_id="<APP_ID>")
@@ -61,12 +71,74 @@
         amo=False,
         trigger_price=None
     )
     logging.info("order id: {}".format(order_no))
 except Exception as e:
     logging.error("error in order placement: {}".format(e))
     
+# get order by order number
+order = tiqs.get_order("24040200000302")
+
+# delete order
+response = tiqs.delete_order("24040200000302")
+
 # all orders
-tiqs.get_user_orders()
+user_orders = tiqs.get_user_orders()
+
+# all trades
+user_trades = tiqs.get_user_trades()
+
+# user details
+tiqs.user_details()
+
+# positions 
+tiqs.get_positions()
+
+# all instruments
+tiqs.get_instruments()
+
+# market holidays
+holidays = tiqs.holidays()
+
+# index list
+index_list = tiqs.index_list()
 
+# option chain for an underlying asset for a give expiry date
+option_chain = tiqs.option_chain(params={
+    "token": "26009",
+    "exchange": "INDEX",
+    "count": "10",
+    "expiry": "10-APR-2024"
+})
 ```
 
+## Websockets
+
+```python
+import time
+import logging
+from pytiqs import TiqsSocket
+
+
+def on_ticks(ws, ticks):
+    logging.debug("Ticks: {}".format(ticks))
+
+
+def on_connect(ws, response):
+    ws.subscribe([7929])
+    time.sleep(5)
+    ws.set_mode(socketClient.MODE_LTP, [7929])
+
+
+def on_close(ws, code, reason):
+    logging.debug("closed, {}, {}".format(code, reason))
+    ws.stop()
+
+
+socketClient = TiqsSocket(app_id="<APP_ID>", token="<token>")
+socketClient.on_ticks = on_ticks
+socketClient.on_connect = on_connect
+socketClient.on_close = on_close
+
+# if you want to keep this as non-blocking code use socketClient.connect(threaded=True)
+socketClient.connect() 
+```
```

### Comparing `pytiqs-1.0.6/setup.py` & `pytiqs-1.0.7/setup.py`

 * *Files identical despite different names*

