# Comparing `tmp/pytiqs-1.0.5.tar.gz` & `tmp/pytiqs-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytiqs-1.0.5.tar", last modified: Fri Apr 12 05:19:29 2024, max compression
+gzip compressed data, was "pytiqs-1.0.6.tar", last modified: Fri Apr 12 05:30:55 2024, max compression
```

## Comparing `pytiqs-1.0.5.tar` & `pytiqs-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-12 05:19:29.915569 pytiqs-1.0.5/
--rw-r--r--   0 nitin      (501) staff       (20)     1807 2024-04-12 05:19:29.915473 pytiqs-1.0.5/PKG-INFO
--rw-r--r--   0 nitin      (501) staff       (20)     1304 2024-04-12 04:45:33.000000 pytiqs-1.0.5/README.md
-drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-12 05:19:29.912678 pytiqs-1.0.5/pytiqs/
--rw-r--r--   0 nitin      (501) staff       (20)      172 2024-04-10 04:14:30.000000 pytiqs-1.0.5/pytiqs/__init__.py
--rw-r--r--   0 nitin      (501) staff       (20)      232 2024-04-12 05:18:54.000000 pytiqs-1.0.5/pytiqs/__version__.py
--rw-r--r--   0 nitin      (501) staff       (20)    16952 2024-04-12 04:46:16.000000 pytiqs-1.0.5/pytiqs/connect.py
--rw-r--r--   0 nitin      (501) staff       (20)     2525 2024-04-10 04:14:30.000000 pytiqs-1.0.5/pytiqs/constants.py
--rw-r--r--   0 nitin      (501) staff       (20)      555 2024-04-10 04:14:30.000000 pytiqs-1.0.5/pytiqs/exceptions.py
--rw-r--r--   0 nitin      (501) staff       (20)    19070 2024-04-12 05:18:43.000000 pytiqs-1.0.5/pytiqs/sockets.py
-drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-12 05:19:29.915137 pytiqs-1.0.5/pytiqs.egg-info/
--rw-r--r--   0 nitin      (501) staff       (20)     1807 2024-04-12 05:19:29.000000 pytiqs-1.0.5/pytiqs.egg-info/PKG-INFO
--rw-r--r--   0 nitin      (501) staff       (20)      295 2024-04-12 05:19:29.000000 pytiqs-1.0.5/pytiqs.egg-info/SOURCES.txt
--rw-r--r--   0 nitin      (501) staff       (20)        1 2024-04-12 05:19:29.000000 pytiqs-1.0.5/pytiqs.egg-info/dependency_links.txt
--rw-r--r--   0 nitin      (501) staff       (20)      145 2024-04-12 05:19:29.000000 pytiqs-1.0.5/pytiqs.egg-info/requires.txt
--rw-r--r--   0 nitin      (501) staff       (20)        7 2024-04-12 05:19:29.000000 pytiqs-1.0.5/pytiqs.egg-info/top_level.txt
--rw-r--r--   0 nitin      (501) staff       (20)      290 2024-04-12 05:19:29.915909 pytiqs-1.0.5/setup.cfg
--rw-r--r--   0 nitin      (501) staff       (20)     1192 2024-04-10 04:19:46.000000 pytiqs-1.0.5/setup.py
+drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-12 05:30:55.582163 pytiqs-1.0.6/
+-rw-r--r--   0 nitin      (501) staff       (20)     1807 2024-04-12 05:30:55.582063 pytiqs-1.0.6/PKG-INFO
+-rw-r--r--   0 nitin      (501) staff       (20)     1304 2024-04-12 04:45:33.000000 pytiqs-1.0.6/README.md
+drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-12 05:30:55.580488 pytiqs-1.0.6/pytiqs/
+-rw-r--r--   0 nitin      (501) staff       (20)      172 2024-04-10 04:14:30.000000 pytiqs-1.0.6/pytiqs/__init__.py
+-rw-r--r--   0 nitin      (501) staff       (20)      232 2024-04-12 05:30:37.000000 pytiqs-1.0.6/pytiqs/__version__.py
+-rw-r--r--   0 nitin      (501) staff       (20)    16952 2024-04-12 04:46:16.000000 pytiqs-1.0.6/pytiqs/connect.py
+-rw-r--r--   0 nitin      (501) staff       (20)     2525 2024-04-10 04:14:30.000000 pytiqs-1.0.6/pytiqs/constants.py
+-rw-r--r--   0 nitin      (501) staff       (20)      555 2024-04-10 04:14:30.000000 pytiqs-1.0.6/pytiqs/exceptions.py
+-rw-r--r--   0 nitin      (501) staff       (20)    19070 2024-04-12 05:28:29.000000 pytiqs-1.0.6/pytiqs/sockets.py
+drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-12 05:30:55.581690 pytiqs-1.0.6/pytiqs.egg-info/
+-rw-r--r--   0 nitin      (501) staff       (20)     1807 2024-04-12 05:30:55.000000 pytiqs-1.0.6/pytiqs.egg-info/PKG-INFO
+-rw-r--r--   0 nitin      (501) staff       (20)      295 2024-04-12 05:30:55.000000 pytiqs-1.0.6/pytiqs.egg-info/SOURCES.txt
+-rw-r--r--   0 nitin      (501) staff       (20)        1 2024-04-12 05:30:55.000000 pytiqs-1.0.6/pytiqs.egg-info/dependency_links.txt
+-rw-r--r--   0 nitin      (501) staff       (20)      145 2024-04-12 05:30:55.000000 pytiqs-1.0.6/pytiqs.egg-info/requires.txt
+-rw-r--r--   0 nitin      (501) staff       (20)        7 2024-04-12 05:30:55.000000 pytiqs-1.0.6/pytiqs.egg-info/top_level.txt
+-rw-r--r--   0 nitin      (501) staff       (20)      290 2024-04-12 05:30:55.582512 pytiqs-1.0.6/setup.cfg
+-rw-r--r--   0 nitin      (501) staff       (20)     1192 2024-04-10 04:19:46.000000 pytiqs-1.0.6/setup.py
```

### Comparing `pytiqs-1.0.5/PKG-INFO` & `pytiqs-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytiqs
-Version: 1.0.5
+Version: 1.0.6
 Summary: The official Python client for the Tiqs trading API
 Home-page: 
 Download-URL: 
 Author: Butterfly Broking Pvt. Ltd.
 Author-email: 
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pytiqs-1.0.5/README.md` & `pytiqs-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pytiqs-1.0.5/pytiqs/connect.py` & `pytiqs-1.0.6/pytiqs/connect.py`

 * *Files identical despite different names*

### Comparing `pytiqs-1.0.5/pytiqs/constants.py` & `pytiqs-1.0.6/pytiqs/constants.py`

 * *Files identical despite different names*

### Comparing `pytiqs-1.0.5/pytiqs/exceptions.py` & `pytiqs-1.0.6/pytiqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytiqs-1.0.5/pytiqs/sockets.py` & `pytiqs-1.0.6/pytiqs/sockets.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,29 +409,29 @@
         if data.get("type") == "error":
             self._on_error(ws, code=0, reason=data.get("data"))
 
     def _parse_binary(self, data: bytes) -> Dict[str, Any]:
         tick = {}  # type: Dict[str, Any]
         if self.debug:
             log.debug("Parsing binary, len: {}".format(len(data)))
-        if len(data) == 13:
+        if len(data) >= 13:
             tick['token'] = int.from_bytes(data[0:4])
             tick['ltp'] = int.from_bytes(data[4:8])
             tick['mode'] = self.MODE_LTP
-        if len(data) == 17:
+        if len(data) >= 17:
             tick['close'] = int.from_bytes(data[13:17])
             tick['netChange'] = round(((tick['ltp'] - tick['close']) / tick['close']) * 100 + 1e-9, 2) or 0.00
             if tick['ltp'] > tick['close']:
                 tick['changeFlag'] = 43  # ascii code for '+'
             elif tick['ltp'] < tick['close']:
                 tick['changeFlag'] = 45  # ascii code for '-'
             else:
                 tick['changeFlag'] = 32  # no change
             tick['mode'] = self.MODE_LTPC
-        if len(data) == 69:
+        if len(data) >= 69:
             tick['ltq'] = int.from_bytes(data[13:17])
             tick['avgPrice'] = int.from_bytes(data[17:21])
             tick['totalBuyQuantity'] = int.from_bytes(data[21:25])
             tick['totalSellQuantity'] = int.from_bytes(data[25:29])
             tick['open'] = int.from_bytes(data[29:33])
             tick['high'] = int.from_bytes(data[33:37])
             tick['close'] = int.from_bytes(data[37:41])
@@ -445,15 +445,15 @@
             if tick['ltp'] > tick['close']:
                 tick['changeFlag'] = 43  # ascii code for '+'
             elif tick['ltp'] < tick['close']:
                 tick['changeFlag'] = 45  # ascii code for '-'
             else:
                 tick['changeFlag'] = 32  # no change
             tick['mode'] = self.MODE_QUOTE
-        if len(data) == 197:
+        if len(data) >= 197:
             tick['ltt'] = int.from_bytes(data[49:53])
             tick['lowerLimit'] = int.from_bytes(data[69:73])
             tick['upperLimit'] = int.from_bytes(data[73:77])
             bids = []
             asks = []
             for i in range(10):
                 quantity = int.from_bytes(data[77 + i * 12:81 + i * 12])
```

### Comparing `pytiqs-1.0.5/pytiqs.egg-info/PKG-INFO` & `pytiqs-1.0.6/pytiqs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytiqs
-Version: 1.0.5
+Version: 1.0.6
 Summary: The official Python client for the Tiqs trading API
 Home-page: 
 Download-URL: 
 Author: Butterfly Broking Pvt. Ltd.
 Author-email: 
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pytiqs-1.0.5/setup.py` & `pytiqs-1.0.6/setup.py`

 * *Files identical despite different names*

