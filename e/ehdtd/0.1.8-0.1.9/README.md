# Comparing `tmp/ehdtd-0.1.8.tar.gz` & `tmp/ehdtd-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdtd-0.1.8.tar", max compression
+gzip compressed data, was "ehdtd-0.1.9.tar", max compression
```

## Comparing `ehdtd-0.1.8.tar` & `ehdtd-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1105 2023-11-23 05:07:16.141066 ehdtd-0.1.8/LICENSE
--rw-r--r--   0        0        0     2530 2024-02-29 07:50:34.714293 ehdtd-0.1.8/README.md
--rw-r--r--   0        0        0      921 2023-11-28 02:30:35.236883 ehdtd-0.1.8/ehdtd/__init__.py
--rw-r--r--   0        0        0    23764 2024-04-07 11:48:58.674464 ehdtd-0.1.8/ehdtd/binance.py
--rw-r--r--   0        0        0   105876 2024-04-07 04:00:06.936458 ehdtd-0.1.8/ehdtd/ehdtd.py
--rw-r--r--   0        0        0     6539 2024-04-07 09:34:20.505668 ehdtd-0.1.8/ehdtd/ehdtd_common_functions.py
--rw-r--r--   0        0        0      683 2024-04-07 11:47:09.162698 ehdtd-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 ehdtd-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-11-23 05:07:16.141066 ehdtd-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2530 2024-02-29 07:50:34.714293 ehdtd-0.1.9/README.md
+-rw-r--r--   0        0        0      921 2023-11-28 02:30:35.236883 ehdtd-0.1.9/ehdtd/__init__.py
+-rw-r--r--   0        0        0    23764 2024-04-07 11:48:58.674464 ehdtd-0.1.9/ehdtd/binance.py
+-rw-r--r--   0        0        0   106667 2024-04-12 03:18:14.984434 ehdtd-0.1.9/ehdtd/ehdtd.py
+-rw-r--r--   0        0        0     6539 2024-04-07 09:34:20.505668 ehdtd-0.1.9/ehdtd/ehdtd_common_functions.py
+-rw-r--r--   0        0        0      683 2024-04-12 03:26:24.972254 ehdtd-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 ehdtd-0.1.9/PKG-INFO
```

### Comparing `ehdtd-0.1.8/LICENSE` & `ehdtd-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.8/README.md` & `ehdtd-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.8/ehdtd/__init__.py` & `ehdtd-0.1.9/ehdtd/__init__.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.8/ehdtd/binance.py` & `ehdtd-0.1.9/ehdtd/binance.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.8/ehdtd/ehdtd.py` & `ehdtd-0.1.9/ehdtd/ehdtd.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,25 +178,32 @@
 
         self.__not_partition_intervals = ['1d', '3d', '1w', '1mo']
 
         self.__db_type = None
         self.__db_name = None
         self.__exchange = None
         self.__fetch_data = None
-        self.__trading_type = trading_type
+        self.__trading_type = None
 
         self.__lock_thread_get_file = threading.Lock()
         self.__lock_schedule = threading.Lock()
 
         self.__cache_table_name = 'ehdtd_cache_data'
 
+        if trading_type is not None\
+            and isinstance(trading_type, str)\
+            and trading_type in Ehdtd.get_supported_trading_types():
+            self.__trading_type = trading_type
+        else:
+            raise ValueError(f'The trading type {trading_type} is not supported.')
+
         if exchange in Ehdtd.get_supported_exchanges():
             self.__exchange = exchange
         else:
-            raise ValueError('The exchange ' + str(exchange) + ' is not supported.')
+            raise ValueError(f'The exchange {exchange} is not supported.')
 
         self.__exchange_aux_class = EhdtdExchangeConfig.exchange_classes[self.__exchange]()
 
         self.__chk_db_all_symbols_thd = {}
 
         self.__db_uri = None
         self.__db_engine = None
@@ -344,15 +351,17 @@
             and __limit_counter <= __limit_time:
             __limit_counter = __limit_counter + 1
             time.sleep(1)
 
         self.__db_conn.close()
 
     def __get_table_name(self, symbol, interval):
-        result = self.__exchange + '__' + symbol.replace('/','_').lower() + '__' + interval
+        result = f"{self.__exchange}__"
+        result += f"{self.__trading_type.replace('/','_').replace('-','_').lower()}"
+        result += f"__{symbol.replace('/','_').lower()}__{interval}"
         return result
 
     def __create_cache_table(self):
         result = False
         try:
             if self.__db_metadata is not None:
 
@@ -2452,14 +2461,28 @@
         __result = (
             EhdtdExchangeConfig.exchange_classes[exchange]().get_exchange_connectivity()
         )
 
         return __result
 
     @classmethod
+    def get_supported_trading_types(cls):
+        """
+        get_supported_trading_types.
+        ============================
+            This method return a list of supported trading_types.
+                :param cls: Ehdtd Class.
+
+                :return: list of supported trading_types.
+        """
+        __suported_trading_types = ['SPOT']
+
+        return __suported_trading_types
+
+    @classmethod
     def get_supported_intervals(cls, exchange='binance'):
         """
         get_supported_intervals.
         ========================
             This method return a list of supported intervals.
                 :param cls: Ehdtd Class.
                 :param exchange: str.
```

### Comparing `ehdtd-0.1.8/ehdtd/ehdtd_common_functions.py` & `ehdtd-0.1.9/ehdtd/ehdtd_common_functions.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.8/pyproject.toml` & `ehdtd-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ehdtd"
-version = "0.1.8"
+version = "0.1.9"
 description = "Ehdtd - cryptoCurrency Exchange history data to database"
 authors = ["Ricardo Marcelo Alvarez <rmalvarezkai@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/rmalvarezkai/ehdtd"
 
 [tool.poetry.dependencies]
```

### Comparing `ehdtd-0.1.8/PKG-INFO` & `ehdtd-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdtd
-Version: 0.1.8
+Version: 0.1.9
 Summary: Ehdtd - cryptoCurrency Exchange history data to database
 Home-page: https://github.com/rmalvarezkai/ehdtd
 License: MIT
 Author: Ricardo Marcelo Alvarez
 Author-email: rmalvarezkai@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

