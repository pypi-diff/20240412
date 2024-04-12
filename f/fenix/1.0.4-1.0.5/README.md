# Comparing `tmp/fenix-1.0.4.tar.gz` & `tmp/fenix-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenix-1.0.4.tar", last modified: Fri Mar 29 10:58:01 2024, max compression
+gzip compressed data, was "fenix-1.0.5.tar", last modified: Fri Apr 12 08:22:28 2024, max compression
```

## Comparing `fenix-1.0.4.tar` & `fenix-1.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 10:58:01.270868 fenix-1.0.4/
--rw-rw-rw-   0        0        0    35823 2023-11-22 17:26:17.000000 fenix-1.0.4/LICENSE
--rw-rw-rw-   0        0        0    51123 2024-03-29 10:58:01.270364 fenix-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     7580 2024-03-29 10:42:52.000000 fenix-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 10:58:01.256472 fenix-1.0.4/fenix/
--rw-rw-rw-   0        0        0     3980 2024-03-29 10:42:02.000000 fenix-1.0.4/fenix/__init__.py
--rw-rw-rw-   0        0        0    88944 2024-03-29 10:52:09.000000 fenix-1.0.4/fenix/aliceblue.py
--rw-rw-rw-   0        0        0    77835 2024-03-29 10:52:24.000000 fenix-1.0.4/fenix/angelone.py
-drwxrwxrwx   0        0        0        0 2024-03-29 10:58:01.265970 fenix-1.0.4/fenix/base/
--rw-rw-rw-   0        0        0      281 2024-03-29 10:41:45.000000 fenix-1.0.4/fenix/base/__init__.py
--rw-rw-rw-   0        0        0    24221 2024-03-29 10:41:50.000000 fenix-1.0.4/fenix/base/broker.py
--rw-rw-rw-   0        0        0     4222 2024-03-29 10:38:05.000000 fenix-1.0.4/fenix/base/constants.py
--rw-rw-rw-   0        0        0      430 2024-03-29 10:38:19.000000 fenix-1.0.4/fenix/base/errors.py
--rw-rw-rw-   0        0        0    69445 2024-03-29 10:52:22.000000 fenix-1.0.4/fenix/choice.py
--rw-rw-rw-   0        0        0    75739 2024-03-29 10:52:21.000000 fenix-1.0.4/fenix/finvasia.py
--rw-rw-rw-   0        0        0    82712 2024-03-29 10:52:18.000000 fenix-1.0.4/fenix/fivepaisa.py
--rw-rw-rw-   0        0        0    75810 2024-03-29 10:09:12.000000 fenix-1.0.4/fenix/fyers.py
--rw-rw-rw-   0        0        0    74476 2024-03-29 10:52:17.000000 fenix-1.0.4/fenix/iifl.py
--rw-rw-rw-   0        0        0    58418 2024-03-29 09:53:47.000000 fenix-1.0.4/fenix/kotak.py
--rw-rw-rw-   0        0        0    75897 2024-03-29 10:52:16.000000 fenix-1.0.4/fenix/kotakneo.py
--rw-rw-rw-   0        0        0      608 2024-03-29 09:37:55.000000 fenix-1.0.4/fenix/kunjee.py
--rw-rw-rw-   0        0        0    80185 2024-03-29 10:52:14.000000 fenix-1.0.4/fenix/mastertrust.py
--rw-rw-rw-   0        0        0      676 2024-03-29 09:24:42.000000 fenix-1.0.4/fenix/motilaloswal.py
--rw-rw-rw-   0        0        0    67682 2024-03-29 09:24:32.000000 fenix-1.0.4/fenix/paper.py
--rw-rw-rw-   0        0        0    72748 2024-03-29 10:52:12.000000 fenix-1.0.4/fenix/symphony.py
--rw-rw-rw-   0        0        0    69927 2024-03-29 08:11:35.000000 fenix-1.0.4/fenix/upstox.py
--rw-rw-rw-   0        0        0      577 2024-03-29 07:53:42.000000 fenix-1.0.4/fenix/vpc.py
--rw-rw-rw-   0        0        0    71966 2024-03-29 10:56:10.000000 fenix-1.0.4/fenix/zerodha.py
-drwxrwxrwx   0        0        0        0 2024-03-29 10:58:01.265970 fenix-1.0.4/fenix.egg-info/
--rw-rw-rw-   0        0        0    51123 2024-03-29 10:58:01.000000 fenix-1.0.4/fenix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2024-03-29 10:58:01.000000 fenix-1.0.4/fenix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 10:58:01.000000 fenix-1.0.4/fenix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      195 2024-03-29 10:58:01.000000 fenix-1.0.4/fenix.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-29 10:58:01.000000 fenix-1.0.4/fenix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2567 2024-03-16 19:25:49.000000 fenix-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 10:58:01.270868 fenix-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2868 2024-03-16 20:06:03.000000 fenix-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:22:28.275020 fenix-1.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-11-22 17:26:17.000000 fenix-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0    51170 2024-04-12 08:22:28.274019 fenix-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7580 2024-03-29 10:42:52.000000 fenix-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 08:22:28.258527 fenix-1.0.5/fenix/
+-rw-rw-rw-   0        0        0     3980 2024-04-12 08:22:01.000000 fenix-1.0.5/fenix/__init__.py
+-rw-rw-rw-   0        0        0    89924 2024-04-04 06:16:08.000000 fenix-1.0.5/fenix/aliceblue.py
+-rw-rw-rw-   0        0        0    77835 2024-03-30 18:18:42.000000 fenix-1.0.5/fenix/angelone.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:22:28.271015 fenix-1.0.5/fenix/base/
+-rw-rw-rw-   0        0        0      281 2024-03-29 10:41:45.000000 fenix-1.0.5/fenix/base/__init__.py
+-rw-rw-rw-   0        0        0    24401 2024-04-04 07:06:08.000000 fenix-1.0.5/fenix/base/broker.py
+-rw-rw-rw-   0        0        0     4222 2024-03-29 10:38:05.000000 fenix-1.0.5/fenix/base/constants.py
+-rw-rw-rw-   0        0        0      430 2024-03-29 10:38:19.000000 fenix-1.0.5/fenix/base/errors.py
+-rw-rw-rw-   0        0        0    69445 2024-03-29 10:52:22.000000 fenix-1.0.5/fenix/choice.py
+-rw-rw-rw-   0        0        0    75904 2024-04-01 07:45:19.000000 fenix-1.0.5/fenix/finvasia.py
+-rw-rw-rw-   0        0        0    83357 2024-04-12 08:06:18.000000 fenix-1.0.5/fenix/fivepaisa.py
+-rw-rw-rw-   0        0        0    76031 2024-04-02 05:50:12.000000 fenix-1.0.5/fenix/fyers.py
+-rw-rw-rw-   0        0        0    74758 2024-04-03 20:04:58.000000 fenix-1.0.5/fenix/iifl.py
+-rw-rw-rw-   0        0        0    58636 2024-04-12 08:07:35.000000 fenix-1.0.5/fenix/kotak.py
+-rw-rw-rw-   0        0        0    75897 2024-03-29 10:52:16.000000 fenix-1.0.5/fenix/kotakneo.py
+-rw-rw-rw-   0        0        0      608 2024-03-29 09:37:55.000000 fenix-1.0.5/fenix/kunjee.py
+-rw-rw-rw-   0        0        0    82611 2024-04-02 13:49:09.000000 fenix-1.0.5/fenix/mastertrust.py
+-rw-rw-rw-   0        0        0      676 2024-03-29 09:24:42.000000 fenix-1.0.5/fenix/motilaloswal.py
+-rw-rw-rw-   0        0        0    67682 2024-03-29 09:24:32.000000 fenix-1.0.5/fenix/paper.py
+-rw-rw-rw-   0        0        0    72748 2024-04-03 20:47:42.000000 fenix-1.0.5/fenix/symphony.py
+-rw-rw-rw-   0        0        0    70092 2024-04-01 05:53:05.000000 fenix-1.0.5/fenix/upstox.py
+-rw-rw-rw-   0        0        0      577 2024-03-29 07:53:42.000000 fenix-1.0.5/fenix/vpc.py
+-rw-rw-rw-   0        0        0    72146 2024-04-12 08:16:54.000000 fenix-1.0.5/fenix/zerodha.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:22:28.272015 fenix-1.0.5/fenix.egg-info/
+-rw-rw-rw-   0        0        0    51170 2024-04-12 08:22:27.000000 fenix-1.0.5/fenix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2024-04-12 08:22:27.000000 fenix-1.0.5/fenix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 08:22:27.000000 fenix-1.0.5/fenix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      226 2024-04-12 08:22:27.000000 fenix-1.0.5/fenix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-12 08:22:27.000000 fenix-1.0.5/fenix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2606 2024-04-12 08:17:37.000000 fenix-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 08:22:28.275020 fenix-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2917 2024-04-12 08:20:56.000000 fenix-1.0.5/setup.py
```

### Comparing `fenix-1.0.4/LICENSE` & `fenix-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fenix-1.0.4/PKG-INFO` & `fenix-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenix
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python library for trading in the Indian Finance Sector with support for multiple broker APIs.
 Home-page: https://fenix.hardeep.tech
 Author: Hardeep Singh
 Author-email: Hardeep Singh <hardeep.hd13@gmail.com>
 Maintainer-email: Hardeep Singh <hardeep.hd13@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -708,14 +708,15 @@
 Requires-Dist: PyJWT>=2.8.0
 Requires-Dist: pyotp>=2.9.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: requests-oauthlib>=1.4.0
 Requires-Dist: selenium>=4.18.1
 Requires-Dist: urllib3>=2.2.1
 Requires-Dist: webdriver-manager>=4.0.1
+Requires-Dist: undetected-chromedriver>=3.5.5
 
 # Fenix – Indian Broker Trading Library
 
 ![License](https://img.shields.io/badge/License-GPLv3-blue?color=%234ec820)
 
 
 A Python library for trading in the Indian Finance Sector with support for many broker APIs.
```

### Comparing `fenix-1.0.4/README.md` & `fenix-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fenix-1.0.4/fenix/__init__.py` & `fenix-1.0.5/fenix/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #  ------------------------------------------------------------------------------
 
 
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 
 #  ------------------------------------------------------------------------------
 
 from threading import Thread
 
 from fenix.base.broker import Broker  # noqa: F401
```

### Comparing `fenix-1.0.4/fenix/aliceblue.py` & `fenix-1.0.5/fenix/aliceblue.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     # Base URLs
 
     base_urls = {
         "api_doc": "https://v2api.aliceblueonline.com/introduction",
         "token_01": "https://ant.aliceblueonline.com/rest/AliceBlueAPIService",
         "token_02": "https://ant.aliceblueonline.com/",
         "base": "https://ant.aliceblueonline.com/rest/AliceBlueAPIService/api",
-        "market_data": f"https://v2api.aliceblueonline.com/restpy/static/contract_master/{ExchangeCode.NFO}.csv",
+        "market_data": "https://v2api.aliceblueonline.com/restpy/contract_master",
     }
 
     # Access Token Generation URLs
 
     token_urls = {
         "get_enc_key": f"{base_urls['base']}/customer/getAPIEncpkey",
         "session_id": f"{base_urls['base']}/customer/getUserSID",
@@ -243,63 +243,77 @@
         """
         Downlaods NSE & BSE Equity Info for F&O Segment.
         Stores them in the aliceblue.indices Dictionary.
 
         Returns:
             dict: Unified fenix indices format.
         """
-        nse_url = cls.base_urls["market_data"].replace(
-            ExchangeCode.NFO, ExchangeCode.BSE
+        params = {"exch": ExchangeCode.BSE}
+        response = cls.fetch(
+            method="GET",
+            url=cls.base_urls["market_data"],
+            params=params,
         )
-        df_bse = cls.data_reader(link=nse_url, filetype="csv")
+        data = cls._json_parser(response)[ExchangeCode.BSE]
 
-        df_bse = df_bse[(df_bse["Instrument Type"] == "E")]
-        df_bse = df_bse[["Trading Symbol", "Token", "Lot Size", "Tick Size", "Exch"]]
+        df_bse = cls.data_frame(data)
+
+        df_bse = df_bse[(df_bse["instrument_type"] == "E")]
+        df_bse = df_bse[["trading_symbol", "token", "lot_size", "tick_size", "exch"]]
         df_bse.rename(
             {
-                "Trading Symbol": "Symbol",
-                "Tick Size": "TickSize",
-                "Lot Size": "LotSize",
-                "Exch": "Exchange",
+                "trading_symbol": "Symbol",
+                "tick_size": "TickSize",
+                "lot_size": "LotSize",
+                "exch": "Exchange",
+                "token": "Token",
             },
             axis=1,
             inplace=True,
         )
 
         df_bse.set_index(df_bse["Symbol"], inplace=True)
 
         df_bse["TickSize"] = df_bse["TickSize"].astype(float)
         df_bse["LotSize"] = df_bse["LotSize"].astype(int)
+        df_bse["Token"] = df_bse["Token"].astype(int)
 
-        bse_url = cls.base_urls["market_data"].replace(
-            ExchangeCode.NFO, ExchangeCode.NSE
+        params = {"exch": ExchangeCode.NSE}
+        response = cls.fetch(
+            method="GET",
+            url=cls.base_urls["market_data"],
+            params=params,
         )
-        df_nse = cls.data_reader(link=bse_url, filetype="csv")
+        data = cls._json_parser(response)[ExchangeCode.NSE]
+
+        df_nse = cls.data_frame(data)
 
-        df_nse = df_nse[(df_nse["Group Name"] == "EQ")]
+        df_nse = df_nse[(df_nse["group_name"] == "EQ")]
         df_nse = df_nse[
-            ["Symbol", "Trading Symbol", "Token", "Lot Size", "Tick Size", "Exch"]
+            ["symbol", "trading_symbol", "token", "lot_size", "tick_size", "exch"]
         ]
         df_nse.rename(
             {
-                "Symbol": "Index",
-                "Trading Symbol": "Symbol",
-                "Tick Size": "TickSize",
-                "Lot Size": "LotSize",
-                "Exch": "Exchange",
+                "symbol": "Index",
+                "trading_symbol": "Symbol",
+                "tick_size": "TickSize",
+                "lot_size": "LotSize",
+                "exch": "Exchange",
+                "token": "Token",
             },
             axis=1,
             inplace=True,
         )
 
         df_nse.set_index(df_nse["Index"], inplace=True)
         df_nse.drop(columns="Index", inplace=True)
 
         df_nse["TickSize"] = df_nse["TickSize"].astype(float)
         df_nse["LotSize"] = df_nse["LotSize"].astype(int)
+        df_nse["Token"] = df_nse["Token"].astype(int)
 
         cls.eq_tokens[ExchangeCode.NSE] = df_nse.to_dict(orient="index")
         cls.eq_tokens[ExchangeCode.BSE] = df_bse.to_dict(orient="index")
 
         return cls.eq_tokens
 
     @classmethod
@@ -307,25 +321,32 @@
         """
         Downloads all the Broker Indices Token data.
         Stores them in the aliceblue.indices Dictionary.
 
         Returns:
             dict: Unified fenix indices format.
         """
-        indices_url = cls.base_urls["market_data"].replace(ExchangeCode.NFO, "INDICES")
-        df = cls.data_reader(link=indices_url, filetype="csv")
 
-        df.rename(
-            {"symbol": "Symbol", "token": "Token", "exch": "Exchange"},
-            axis=1,
-            inplace=True,
+        params = {"exch": "INDICES"}
+        response = cls.fetch(
+            method="GET",
+            url=cls.base_urls["market_data"],
+            params=params,
         )
-        df.index = df["Symbol"]
+        data = cls._json_parser(response)
 
-        indices = df.to_dict(orient="index")
+        indices = {}
+
+        for exch in [ExchangeCode.NSE, ExchangeCode.BSE, ExchangeCode.MCX]:
+            for token_data in data[exch]:
+                indices[token_data["symbol"]] = {
+                    "Symbol": token_data["symbol"],
+                    "Token": token_data["token"],
+                    "Exchange": exch,
+                }
 
         indices[Root.BNF] = indices["NIFTY BANK"]
         indices[Root.NF] = indices["NIFTY 50"]
         indices[Root.FNF] = indices["NIFTY FIN SERVICE"]
         indices[Root.MIDCPNF] = indices["NIFTY MIDCAP SELECT"]
 
         cls.indices = indices
@@ -338,48 +359,62 @@
         Downloades Token Data for the FNO Segment for the 3 latest Weekly Expiries.
         Stores them in the aliceblue.fno_tokens Dictionary.
 
         Raises:
             TokenDownloadError: Any Error Occured is raised through this Error Type.
         """
         try:
-            df_nfo = cls.data_reader(link=cls.base_urls["market_data"], filetype="csv")
+            params = {"exch": ExchangeCode.NFO}
+            response = cls.fetch(
+                method="GET",
+                url=cls.base_urls["market_data"],
+                params=params,
+            )
+            data = cls._json_parser(response)[ExchangeCode.NFO]
+
+            df_nfo = cls.data_frame(data)
 
             df_nfo = df_nfo[
                 (
-                    (df_nfo["Symbol"] == "BANKNIFTY")
-                    | (df_nfo["Symbol"] == "NIFTY")
-                    | (df_nfo["Symbol"] == "FINNIFTY")
-                    | (df_nfo["Symbol"] == "MIDCPNIFTY")
+                    (df_nfo["symbol"] == "BANKNIFTY")
+                    | (df_nfo["symbol"] == "NIFTY")
+                    | (df_nfo["symbol"] == "FINNIFTY")
+                    | (df_nfo["symbol"] == "MIDCPNIFTY")
                 )
-                & ((df_nfo["Instrument Type"] == "OPTIDX"))
+                & ((df_nfo["instrument_type"] == "OPTIDX"))
             ]
 
-            bfo_url = cls.base_urls["market_data"].replace(
-                ExchangeCode.NFO, ExchangeCode.BFO
+            params = {"exch": ExchangeCode.BFO}
+            response = cls.fetch(
+                method="GET",
+                url=cls.base_urls["market_data"],
+                params=params,
             )
-            df_bfo = cls.data_reader(link=bfo_url, filetype="csv")
+            data = cls._json_parser(response)[ExchangeCode.BFO]
+
+            df_bfo = cls.data_frame(data)
 
             df_bfo = df_bfo[
-                ((df_bfo["Symbol"] == "SENSEX") | (df_bfo["Symbol"] == "BANKEX"))
-                & ((df_bfo["Instrument Type"] == "IO"))
+                ((df_bfo["symbol"] == "SENSEX") | (df_bfo["symbol"] == "BANKEX"))
+                & ((df_bfo["instrument_type"] == "IO"))
             ]
 
             df = cls.concat_df([df_nfo, df_bfo])
 
             df.rename(
                 {
-                    "Option Type": "Option",
-                    "Symbol": "Root",
-                    "Exch": "Exchange",
-                    "Expiry Date": "Expiry",
-                    "Trading Symbol": "Symbol",
-                    "Tick Size": "TickSize",
-                    "Lot Size": "LotSize",
-                    "Strike Price": "StrikePrice",
+                    "option_type": "Option",
+                    "symbol": "Root",
+                    "exch": "Exchange",
+                    "expiry_date": "Expiry",
+                    "trading_symbol": "Symbol",
+                    "tick_size": "TickSize",
+                    "lot_size": "LotSize",
+                    "strike_price": "StrikePrice",
+                    "token": "Token",
                 },
                 axis=1,
                 inplace=True,
             )
             df = df[
                 [
                     "Token",
@@ -391,15 +426,15 @@
                     "Root",
                     "TickSize",
                     "Exchange",
                 ]
             ]
 
             df["StrikePrice"] = df["StrikePrice"].astype(int).astype(str)
-            df["Expiry"] = cls.pd_datetime(df["Expiry"]).dt.date.astype(str)
+            df["Expiry"] = cls.pd_datetime(df["Expiry"], unit="ms").dt.date.astype(str)
             df["Token"] = df["Token"].astype(int)
             df["TickSize"] = df["TickSize"].astype(float)
             df["LotSize"] = df["LotSize"].astype(float)
 
             expiry_data = cls.jsonify_expiry(data_frame=df)
             cls.fno_tokens = expiry_data
```

### Comparing `fenix-1.0.4/fenix/angelone.py` & `fenix-1.0.5/fenix/angelone.py`

 * *Files identical despite different names*

### Comparing `fenix-1.0.4/fenix/base/broker.py` & `fenix-1.0.5/fenix/base/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,17 +309,24 @@
         if filetype == "csv":
             if col_names:
                 return read_csv(
                     link,
                     dtype=dtype,
                     sep=sep,
                     names=col_names,
+                    # sep="|",
                 )
 
-            return read_csv(link, dtype=dtype, sep=sep)
+            return read_csv(
+                link,
+                dtype=dtype,
+                sep=sep,
+                on_bad_lines="skip",
+                encoding_errors="ignore",
+            )
 
         raise InputError(
             f"Wrong Filetype: {filetype}, the possible values are: 'json', 'csv'"
         )
 
     @staticmethod
     def data_frame(data: list) -> DataFrame:
```

### Comparing `fenix-1.0.4/fenix/base/constants.py` & `fenix-1.0.5/fenix/base/constants.py`

 * *Files identical despite different names*

### Comparing `fenix-1.0.4/fenix/choice.py` & `fenix-1.0.5/fenix/choice.py`

 * *Files identical despite different names*

### Comparing `fenix-1.0.4/fenix/finvasia.py` & `fenix-1.0.5/fenix/finvasia.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,17 +76,18 @@
     }
 
     # Request Parameters Dictionaries
 
     req_exchange = {
         ExchangeCode.NSE: "NSE",
         ExchangeCode.NFO: "NFO",
+        ExchangeCode.BSE: "BSE",
+        ExchangeCode.BFO: "BFO",
         ExchangeCode.CDS: "CDS",
         ExchangeCode.MCX: "MCX",
-        ExchangeCode.BSE: "BSE",
     }
 
     req_order_type = {
         OrderType.MARKET: "MKT",
         OrderType.LIMIT: "LMT",
         OrderType.SL: "SL-LMT",
         OrderType.SLM: "SL-MKT",
@@ -207,14 +208,16 @@
 
         indices = df.to_dict(orient="index")
 
         indices[Root.BNF] = indices["NIFTY BANK"]
         indices[Root.NF] = indices["NIFTY INDEX"]
         indices[Root.FNF] = indices["FINNIFTY"]
         indices[Root.MIDCPNF] = indices["MIDCPNIFTY"]
+        indices[Root.SENSEX] = {"Symbol": "SENSEX", "Token": 1}
+        indices[Root.BANKEX] = {"Symbol": "BANKEX", "Token": 12}
 
         cls.indices = indices
 
         return indices
 
     @classmethod
     def create_fno_tokens(cls):
```

### Comparing `fenix-1.0.4/fenix/fivepaisa.py` & `fenix-1.0.5/fenix/fivepaisa.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,14 +217,16 @@
             & (df["ExchangeType"] == "C")
             & (df["Series"] == "EQ")
         ]
 
         df_bse = df_bse[
             ["Symbol", "Token", "TickSize", "LotSize", "Exchange", "ExchangeType"]
         ]
+
+        df_bse["Exchange"] = ExchangeCode.BSE
         df_bse.drop_duplicates(subset=["Symbol"], keep="first", inplace=True)
         df_bse.set_index(df_bse["Symbol"], inplace=True)
 
         df_nse = df[
             (df["CpType"] == "XX")
             & (df["Exchange"] == "N")
             & (df["ExchangeType"] == "C")
@@ -319,14 +321,15 @@
                     "Exch": "Exchange",
                     "ExchType": "ExchangeType",
                 },
                 axis=1,
                 inplace=True,
             )
 
+            df["Exchange"].replace({"B": "BSE", "N": "NSE"}, inplace=True)
             df["Expiry"] = cls.pd_datetime(df["Expiry"]).dt.date.astype(str)
             df["StrikePrice"] = df["StrikePrice"].astype(int).astype(str)
 
             expiry_data = cls.jsonify_expiry(data_frame=df)
 
             cls.fno_tokens = expiry_data
 
@@ -412,14 +415,15 @@
             },
         }
 
         headers = {
             "headers": req_headers,
             "user_key": params["user_key"],
             "client_code": client_code,
+            "access_token": jwt_token,
             "json_data": json_data,
         }
 
         cls._session = cls._create_session()
         return headers
 
     @classmethod
@@ -674,15 +678,17 @@
         if not target:
             json_data = {
                 "head": {
                     "key": headers["user_key"],
                 },
                 "body": {
                     "ScripCode": token_dict["Token"],
-                    "Exchange": cls._key_mapper(cls.req_exchange, token_dict["Exchange"], "exchange"),
+                    "Exchange": cls._key_mapper(
+                        cls.req_exchange, token_dict["Exchange"], "exchange"
+                    ),
                     "ExchangeType": cls._key_mapper(
                         cls.req_exchange_type, token_dict["Exchange"], "exchange"
                     ),
                     "Price": price,
                     "StopLossPrice": trigger,
                     "Qty": quantity,
                     "OrderType": cls._key_mapper(cls.req_side, side),
@@ -706,15 +712,17 @@
         else:
             json_data = {
                 "head": {
                     "key": headers["user_key"],
                 },
                 "body": {
                     "ScripCode": token_dict["Token"],
-                    "Exch": cls._key_mapper(cls.req_exchange, token_dict["Exchange"], "exchange"),
+                    "Exch": cls._key_mapper(
+                        cls.req_exchange, token_dict["Exchange"], "exchange"
+                    ),
                     "ExchType": cls._key_mapper(
                         cls.req_exchange_type, token_dict["Exchange"], "exchange"
                     ),
                     "LimitPriceInitialOrder": price,
                     "TriggerPriceInitialOrder": trigger,
                     "LimitPriceProfitOrder": target,
                     "LimitPriceForSL": stoploss,
@@ -780,15 +788,17 @@
         if not target:
             json_data = {
                 "head": {
                     "key": headers["user_key"],
                 },
                 "body": {
                     "ScripCode": token_dict["Token"],
-                    "Exchange": cls._key_mapper(cls.req_exchange, token_dict["Exchange"], "exchange"),
+                    "Exchange": cls._key_mapper(
+                        cls.req_exchange, token_dict["Exchange"], "exchange"
+                    ),
                     "ExchangeType": cls._key_mapper(
                         cls.req_exchange_type, token_dict["Exchange"], "exchange"
                     ),
                     "Price": 0,
                     "StopLossPrice": 0,
                     "Qty": quantity,
                     "OrderType": cls._key_mapper(cls.req_side, side),
@@ -812,15 +822,17 @@
         else:
             json_data = {
                 "head": {
                     "key": headers["user_key"],
                 },
                 "body": {
                     "ScripCode": token_dict["Token"],
-                    "Exch": cls._key_mapper(cls.req_exchange, token_dict["Exchange"], "exchange"),
+                    "Exch": cls._key_mapper(
+                        cls.req_exchange, token_dict["Exchange"], "exchange"
+                    ),
                     "ExchType": cls._key_mapper(
                         cls.req_exchange_type, token_dict["Exchange"], "exchange"
                     ),
                     "LimitPriceInitialOrder": 0,
                     "TriggerPriceInitialOrder": 0,
                     "LimitPriceProfitOrder": target,
                     "LimitPriceForSL": stoploss,
@@ -888,15 +900,17 @@
         if not target:
             json_data = {
                 "head": {
                     "key": headers["user_key"],
                 },
                 "body": {
                     "ScripCode": token_dict["Token"],
-                    "Exchange": cls._key_mapper(cls.req_exchange, token_dict["Exchange"], "exchange"),
+                    "Exchange": cls._key_mapper(
+                        cls.req_exchange, token_dict["Exchange"], "exchange"
+                    ),
                     "ExchangeType": cls._key_mapper(
                         cls.req_exchange_type, token_dict["Exchange"], "exchange"
                     ),
                     "Price": price,
                     "StopLossPrice": 0,
                     "Qty": quantity,
                     "OrderType": cls._key_mapper(cls.req_side, side),
@@ -920,15 +934,17 @@
         else:
             json_data = {
                 "head": {
                     "key": headers["user_key"],
                 },
                 "body": {
                     "ScripCode": token_dict["Token"],
-                    "Exch": cls._key_mapper(cls.req_exchange, token_dict["Exchange"], "exchange"),
+                    "Exch": cls._key_mapper(
+                        cls.req_exchange, token_dict["Exchange"], "exchange"
+                    ),
                     "ExchType": cls._key_mapper(
                         cls.req_exchange_type, token_dict["Exchange"], "exchange"
                     ),
                     "LimitPriceInitialOrder": price,
                     "TriggerPriceInitialOrder": 0,
                     "LimitPriceProfitOrder": target,
                     "LimitPriceForSL": stoploss,
@@ -998,15 +1014,17 @@
         if not target:
             json_data = {
                 "head": {
                     "key": headers["user_key"],
                 },
                 "body": {
                     "ScripCode": token_dict["Token"],
-                    "Exchange": cls._key_mapper(cls.req_exchange, token_dict["Exchange"], "exchange"),
+                    "Exchange": cls._key_mapper(
+                        cls.req_exchange, token_dict["Exchange"], "exchange"
+                    ),
                     "ExchangeType": cls._key_mapper(
                         cls.req_exchange_type, token_dict["Exchange"], "exchange"
                     ),
                     "Price": price,
                     "StopLossPrice": trigger,
                     "Qty": quantity,
                     "OrderType": cls._key_mapper(cls.req_side, side),
@@ -1030,15 +1048,17 @@
         else:
             json_data = {
                 "head": {
                     "key": headers["user_key"],
                 },
                 "body": {
                     "ScripCode": token_dict["Token"],
-                    "Exch": cls._key_mapper(cls.req_exchange, token_dict["Exchange"], "exchange"),
+                    "Exch": cls._key_mapper(
+                        cls.req_exchange, token_dict["Exchange"], "exchange"
+                    ),
                     "ExchType": cls._key_mapper(
                         cls.req_exchange_type, token_dict["Exchange"], "exchange"
                     ),
                     "LimitPriceInitialOrder": price,
                     "TriggerPriceInitialOrder": trigger,
                     "LimitPriceProfitOrder": target,
                     "LimitPriceForSL": stoploss,
@@ -1106,15 +1126,17 @@
         if not target:
             json_data = {
                 "head": {
                     "key": headers["user_key"],
                 },
                 "body": {
                     "ScripCode": token_dict["Token"],
-                    "Exchange": cls._key_mapper(cls.req_exchange, token_dict["Exchange"], "exchange"),
+                    "Exchange": cls._key_mapper(
+                        cls.req_exchange, token_dict["Exchange"], "exchange"
+                    ),
                     "ExchangeType": cls._key_mapper(
                         cls.req_exchange_type, token_dict["Exchange"], "exchange"
                     ),
                     "Price": 0,
                     "StopLossPrice": trigger,
                     "Qty": quantity,
                     "OrderType": cls._key_mapper(cls.req_side, side),
@@ -1138,15 +1160,17 @@
         else:
             json_data = {
                 "head": {
                     "key": headers["user_key"],
                 },
                 "body": {
                     "ScripCode": token_dict["Token"],
-                    "Exch": cls._key_mapper(cls.req_exchange, token_dict["Exchange"], "exchange"),
+                    "Exch": cls._key_mapper(
+                        cls.req_exchange, token_dict["Exchange"], "exchange"
+                    ),
                     "ExchType": cls._key_mapper(
                         cls.req_exchange_type, token_dict["Exchange"], "exchange"
                     ),
                     "LimitPriceInitialOrder": 0,
                     "TriggerPriceInitialOrder": trigger,
                     "LimitPriceProfitOrder": target,
                     "LimitPriceForSL": stoploss,
```

### Comparing `fenix-1.0.4/fenix/fyers.py` & `fenix-1.0.5/fenix/fyers.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,16 @@
             "Scrip code",
             "Underlying scrip code",
             "Option type",
             "Strike price",
             "Underlying FyToken",
             "NA",
             "NAA",
+            "NAAA",
+            "NAAAA",
         ]
 
         df_bse = cls.data_reader(
             cls.base_urls["market_data"].replace("NSE_FO", "BSE_CM"),
             filetype="csv",
             col_names=col_names,
         )
@@ -305,32 +307,33 @@
             "Scrip code",
             "Underlying scrip code",
             "Option type",
             "Strike price",
             "Underlying FyToken",
             "NA",
             "NAA",
+            "NAAA",
+            "NAAAA",
         ]
 
         df_nse = cls.data_reader(
             cls.base_urls["market_data"].replace("NSE_FO", "NSE_CM"),
             filetype="csv",
             col_names=col_names,
         )
-
         df_bse = cls.data_reader(
             cls.base_urls["market_data"].replace("NSE_FO", "BSE_CM"),
             filetype="csv",
             col_names=col_names,
         )
 
         df = cls.concat_df([df_nse, df_bse])
 
         df = df[df["Symbol ticker"].str.endswith("INDEX")][
-            ["Symbol ticker", "Scrip code"]
+            ["Symbol ticker", "Scrip code", "Exchange", "Segment"]
         ]
         df.rename(
             {"Symbol ticker": "Symbol", "Scrip code": "Token"}, axis=1, inplace=True
         )
 
         df.index = (
             df["Symbol"].str.split(":", expand=True)[1].str.split("-", expand=True)[0]
@@ -375,20 +378,21 @@
                 "Scrip code",
                 "Underlying scrip code",
                 "Option type",
                 "Strike price",
                 "Underlying FyToken",
                 "NA",
                 "NAA",
+                "NAAA",
+                "NAAAA",
             ]
 
             df_nfo = cls.data_reader(
                 cls.base_urls["market_data"], filetype="csv", col_names=col_names
             )
-
             df_nfo = df_nfo[
                 (
                     (df_nfo["Underlying scrip code"] == "BANKNIFTY")
                     | (df_nfo["Underlying scrip code"] == "NIFTY")
                     | (df_nfo["Underlying scrip code"] == "FINNIFTY")
                     | (df_nfo["Underlying scrip code"] == "MIDCPNIFTY")
                 )
@@ -433,14 +437,16 @@
                     "Symbol",
                     "Expiry",
                     "Option",
                     "StrikePrice",
                     "LotSize",
                     "Root",
                     "TickSize",
+                    "Exchange",
+                    "Segment",
                 ]
             ]
 
             df["Expiry"] = cls.pd_datetime(df["Expiry"]).dt.date.astype(str)
             df["StrikePrice"] = df["StrikePrice"].astype(int).astype(str)
 
             expiry_data = cls.jsonify_expiry(data_frame=df)
```

### Comparing `fenix-1.0.4/fenix/iifl.py` & `fenix-1.0.5/fenix/iifl.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,21 +244,31 @@
         response = cls.fetch(
             method="GET",
             url=cls.base_urls["index_data"],
             params=params,
         )
         data_bse = cls._json_parser(response)["result"]["indexList"]
 
-        data_nse.extend(data_bse)
-
         indices = {}
 
         for i in data_nse:
             symbol, token = i.split("_")
-            indices[symbol] = {"Symbol": symbol, "Token": int(token)}
+            indices[symbol] = {
+                "Symbol": symbol,
+                "Token": int(token),
+                "Exchange": "NSECM",
+            }
+
+        for i in data_bse:
+            symbol, token = i.split("_")
+            indices[symbol] = {
+                "Symbol": symbol,
+                "Token": int(token),
+                "Exchange": "BSECM",
+            }
 
         indices[Root.BNF] = indices["NIFTY BANK"]
         indices[Root.NF] = indices["NIFTY 50"]
         indices[Root.FNF] = indices["NIFTY FIN SERVICE"]
         indices[Root.MIDCPNF] = indices["NIFTY MID SELECT"]
 
         cls.indices = indices
```

### Comparing `fenix-1.0.4/fenix/kotak.py` & `fenix-1.0.5/fenix/kotak.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     eq_tokens = {}
     fno_tokens = {}
     token_params = [
         "user_id",
         "password",
         "consumer_key",
         "access_token",
+        "consumer_secret",
     ]
     id = "kotak"
     _session = Broker._create_session()
 
     # Base URLs
 
     base_urls = {
@@ -158,15 +159,14 @@
         Stores them in the kotak.indices Dictionary.
 
         Returns:
             dict: Unified fenix indices format.
         """
         date_obj = cls.data_datetime()
         link = f"{cls.base_urls['market_data']}/TradeApiInstruments_Cash_{date_obj}.txt"
-
         df = cls.data_reader(link, filetype="csv", sep="|")
 
         df = df[df["instrumentType"] == "EQ"]
         df = df[
             [
                 "exchange",
                 "instrumentName",
@@ -189,14 +189,15 @@
         )
 
         df_bse = df[df["Exchange"] == ExchangeCode.BSE]
         df_bse.drop_duplicates(subset=["Symbol"], keep="first", inplace=True)
         df_bse.set_index(df_bse["Symbol"], inplace=True)
 
         df_nse = df[df["Exchange"] == ExchangeCode.NSE]
+        df_nse.drop_duplicates(subset=["Symbol"], keep="first", inplace=True)
         df_nse.set_index(df_nse["Symbol"], inplace=True)
 
         cls.eq_tokens[ExchangeCode.NSE] = df_nse.to_dict(orient="index")
         cls.eq_tokens[ExchangeCode.BSE] = df_bse.to_dict(orient="index")
 
         return cls.eq_tokens
 
@@ -377,15 +378,17 @@
             "headers": {
                 "Accept": "application/json",
                 "Content-Type": "application/json",
                 "User-Agent": "KSTradeApi-python/1.0.0/python",
                 "consumerKey": params["consumer_key"],
                 "sessionToken": info02["success"]["sessionToken"],
                 "Authorization": f"Bearer {params['access_token']}",
-            }
+            },
+            "consumer_key": params["consumer_key"],
+            "consumer_secret": params["consumer_secret"],
         }
 
         cls._session = cls._create_session()
 
         return headers
 
     @classmethod
```

### Comparing `fenix-1.0.4/fenix/kotakneo.py` & `fenix-1.0.5/fenix/kotakneo.py`

 * *Files identical despite different names*

### Comparing `fenix-1.0.4/fenix/kunjee.py` & `fenix-1.0.5/fenix/kunjee.py`

 * *Files identical despite different names*

### Comparing `fenix-1.0.4/fenix/mastertrust.py` & `fenix-1.0.5/fenix/mastertrust.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from typing import Any
 
 import re
+import io
+import zipfile
 from requests_oauthlib import OAuth2Session
 
 from fenix.base.broker import Broker
 
 from fenix.base.constants import Side
 from fenix.base.constants import OrderType
 from fenix.base.constants import ExchangeCode
@@ -54,14 +56,15 @@
     # Base URLs
 
     base_urls = {
         "api_doc": "http://139.180.212.2/mastertrust",
         "marketdata_doc": " http://139.180.212.2/ray-websocket",
         "base": "https://masterswift-beta.mastertrust.co.in/api/v1",
         "market_data": "https://masterswift.mastertrust.co.in/api/v2/contracts.json",
+        "bfo_data": "https://masterswift-beta.mastertrust.co.in/api/v1/contract/Compact",
     }
 
     # Access Token Generation URLs
 
     token_urls = {
         "auth": "https://masterswift-beta.mastertrust.co.in/oauth2/auth",
         "auth_token": "https://masterswift-beta.mastertrust.co.in/oauth2/token",
@@ -235,19 +238,40 @@
         response = cls.fetch(
             method="GET",
             url=cls.base_urls["market_data"],
             params=params,
         )
         data = cls._json_parser(response)["NSE-IND"]
 
-        df = cls.data_frame(data)
+        df_nse = cls.data_frame(data)
+
+        params = {"exchanges": "BSE"}
+        response = cls.fetch(
+            method="GET",
+            url=cls.base_urls["market_data"],
+            params=params,
+        )
+        data = cls._json_parser(response)["BSE-IND"]
 
-        df = df[["trading_symbol", "code"]]
-        df.rename({"trading_symbol": "Symbol", "code": "Token"}, axis=1, inplace=True)
+        df_bse = cls.data_frame(data)
+
+        df = cls.concat_df([df_nse, df_bse])
+
+        df = df[["trading_symbol", "code", "exchange"]]
+        df.rename(
+            {
+                "trading_symbol": "Symbol",
+                "code": "Token",
+                "exchange": "Exchange",
+            },
+            axis=1,
+            inplace=True,
+        )
         df.index = df["Symbol"]
+        df["Token"] = df["Token"].astype(int)
 
         indices = df.to_dict(orient="index")
 
         indices[Root.BNF] = indices["Nifty Bank"]
         indices[Root.NF] = indices["Nifty 50"]
         indices[Root.FNF] = indices["Nifty Fin Service"]
         indices[Root.MIDCPNF] = indices["NIFTY MID SELECT"]
@@ -269,55 +293,110 @@
             params = {"exchanges": "NFO"}
             response = cls.fetch(
                 method="GET",
                 url=cls.base_urls["market_data"],
                 params=params,
             )
             data = cls._json_parser(response)["NSE-OPT"]
-            df = cls.data_frame(data)
 
-            df = df[
-                df["symbol"].str.startswith(
+            df_nfo = cls.data_frame(data)
+
+            df_nfo = df_nfo[
+                df_nfo["symbol"].str.startswith(
                     ("BANKNIFTY", "NIFTY", "FINNIFTY", "MIDCPNIFTY")
                 )
             ]
 
-            df["Root"] = df["symbol"].str.split(" ", expand=True)[0]
-            dfx = df["symbol"].str.rsplit(pat=" ", n=3, expand=True)
+            df_nfo["Root"] = df_nfo["symbol"].str.split(" ", expand=True)[0]
 
-            df.rename(
+            sp_op = df_nfo["symbol"].str.rsplit(pat=" ", n=3, expand=True)
+            df_nfo["StrikePrice"] = sp_op[2]
+            df_nfo["Option"] = sp_op[3]
+            df_nfo["expiry"] = cls.pd_datetime(
+                df_nfo["expiry"], unit="s"
+            ).dt.date.astype(str)
+
+            df_nfo.rename(
                 {
                     "code": "Token",
                     "expiry": "Expiry",
                     "trading_symbol": "Symbol",
                     "lotSize": "LotSize",
                     "exchange": "Exchange",
                 },
                 axis=1,
                 inplace=True,
             )
 
-            df["StrikePrice"] = dfx[2]
-            df["Option"] = dfx[3]
+            df_nfo = df_nfo[
+                [
+                    "Token",
+                    "Symbol",
+                    "Expiry",
+                    "Option",
+                    "StrikePrice",
+                    "LotSize",
+                    "Root",
+                    "Exchange",
+                ]
+            ]
+
+            params = {
+                "info": "download",
+                "exchanges": "BFO",
+            }
+            response = cls.fetch(
+                method="GET",
+                url=cls.base_urls["bfo_data"],
+                params=params,
+            )
+
+            zip_data = zipfile.ZipFile(io.BytesIO(response.content))
+            bfo_file = zip_data.namelist()[0]
+            with zip_data.open(bfo_file) as data:
+                df_bfo = cls.data_reader(data, filetype="csv")
+
+            df_bfo.rename(
+                {
+                    "exchange_token": "Token",
+                    "expiry": "Expiry",
+                    "trading_symbol": "Symbol",
+                    "lot_size": "LotSize",
+                    "exchange": "Exchange",
+                    "option_type": "Option",
+                    "strike": "StrikePrice",
+                    "company_name": "Root",
+                },
+                axis=1,
+                inplace=True,
+            )
+
+            df_bfo = df_bfo[
+                ((df_bfo["Root"] == Root.SENSEX) | (df_bfo["Root"] == Root.BANKEX))
+                & (df_bfo["instrument_name"] == "IO")
+            ]
 
-            df = df[
+            df_bfo = df_bfo[
                 [
                     "Token",
                     "Symbol",
                     "Expiry",
                     "Option",
                     "StrikePrice",
                     "LotSize",
                     "Root",
                     "Exchange",
                 ]
             ]
 
+            df_bfo["Expiry"] = cls.pd_datetime(df_bfo["Expiry"]).dt.date.astype(str)
+
+            df = cls.concat_df([df_nfo, df_bfo])
+
             df["StrikePrice"] = df["StrikePrice"].astype(float).astype(int).astype(str)
-            df["Expiry"] = cls.pd_datetime(df["Expiry"], unit="s").dt.date.astype(str)
             df["Token"] = df["Token"].astype(int)
             df["LotSize"] = df["LotSize"].astype(int)
 
             expiry_data = cls.jsonify_expiry(data_frame=df)
             cls.nfo_tokens = expiry_data
 
             return expiry_data
```

### Comparing `fenix-1.0.4/fenix/motilaloswal.py` & `fenix-1.0.5/fenix/motilaloswal.py`

 * *Files identical despite different names*

### Comparing `fenix-1.0.4/fenix/paper.py` & `fenix-1.0.5/fenix/paper.py`

 * *Files identical despite different names*

### Comparing `fenix-1.0.4/fenix/symphony.py` & `fenix-1.0.5/fenix/symphony.py`

 * *Files identical despite different names*

### Comparing `fenix-1.0.4/fenix/upstox.py` & `fenix-1.0.5/fenix/upstox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from typing import Any
 
 import time
 from selenium import webdriver
-from webdriver_manager.chrome import ChromeDriverManager
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.chrome.service import Service as ChromeService
+import undetected_chromedriver as uc
 
 from fenix.base.broker import Broker
 
 from fenix.base.constants import Side
 from fenix.base.constants import OrderType
 from fenix.base.constants import ExchangeCode
 from fenix.base.constants import Product
@@ -184,27 +183,32 @@
         df.rename(
             {
                 "tradingsymbol": "Symbol",
                 "instrument_key": "Token",
                 "exchange_token": "ExchangeToken",
                 "tick_size": "TickSize",
                 "lot_size": "LotSize",
+                "exchange": "Exchange",
             },
             axis=1,
             inplace=True,
         )
 
-        df_bse = df[df["exchange"] == "BSE_EQ"]
-        df_bse = df_bse[["Symbol", "Token", "ExchangeToken", "TickSize", "LotSize"]]
+        df_bse = df[df["Exchange"] == "BSE_EQ"]
+        df_bse = df_bse[
+            ["Symbol", "Token", "ExchangeToken", "TickSize", "LotSize", "Exchange"]
+        ]
         df_bse["ExchangeToken"] = df_bse["ExchangeToken"].astype(int)
         df_bse.set_index(df_bse["Symbol"], inplace=True)
         df_bse.drop_duplicates(subset=["Symbol"], keep="first", inplace=True)
 
-        df_nse = df[df["exchange"] == "NSE_EQ"]
-        df_nse = df_nse[["Symbol", "Token", "ExchangeToken", "TickSize", "LotSize"]]
+        df_nse = df[df["Exchange"] == "NSE_EQ"]
+        df_nse = df_nse[
+            ["Symbol", "Token", "ExchangeToken", "TickSize", "LotSize", "Exchange"]
+        ]
         df_nse["ExchangeToken"] = df_nse["ExchangeToken"].astype(int)
         df_nse.set_index(df_nse["Symbol"], inplace=True)
         df_nse.drop_duplicates(subset=["Symbol"], keep="first", inplace=True)
 
         cls.eq_tokens[ExchangeCode.NSE] = df_nse.to_dict(orient="index")
         cls.eq_tokens[ExchangeCode.BSE] = df_bse.to_dict(orient="index")
 
@@ -218,24 +222,28 @@
 
         Returns:
             dict: Unified fenix indices format.
         """
         df = cls.data_reader(link=cls.base_urls["market_data"], filetype="csv")
 
         df = df[((df["exchange"] == "NSE_INDEX") | (df["exchange"] == "BSE_INDEX"))][
-            ["name", "instrument_key", "exchange_token"]
+            ["name", "instrument_key", "exchange"]
         ]
 
         df.rename(
-            {"instrument_key": "Symbol", "exchange_token": "Token"},
+            {
+                "instrument_key": "Token",
+                "name": "Symbol",
+                "exchange": "Exchange",
+            },
             axis=1,
             inplace=True,
         )
-        df.index = df["name"]
-        del df["name"]
+        df.index = df["Symbol"]
+        # del df["Symbol"]
         indices = df.to_dict(orient="index")
 
         indices[Root.BNF] = indices["Nifty Bank"]
         indices[Root.NF] = indices["Nifty 50"]
         indices[Root.FNF] = indices["Nifty Fin Service"]
         indices[Root.MIDCPNF] = indices["NIFTY MID SELECT"]
 
@@ -269,30 +277,31 @@
                     "instrument_key": "Token",
                     "expiry": "Expiry",
                     "tradingsymbol": "Symbol",
                     "tick_size": "TickSize",
                     "lot_size": "LotSize",
                     "strike": "StrikePrice",
                     "exchange_token": "ExchangeToken",
+                    "exchange": "Exchange",
                 },
                 axis=1,
                 inplace=True,
             )
-
             df = df[
                 [
                     "Token",
                     "Symbol",
                     "ExchangeToken",
                     "Expiry",
                     "Option",
                     "StrikePrice",
                     "LotSize",
                     "Root",
                     "TickSize",
+                    "Exchange",
                 ]
             ]
 
             df["StrikePrice"] = df["StrikePrice"].astype(int).astype(str)
             df["ExchangeToken"] = df["ExchangeToken"].astype(int)
             df["Expiry"] = cls.pd_datetime(df["Expiry"]).dt.date.astype(str)
 
@@ -338,25 +347,24 @@
 
         options = webdriver.ChromeOptions()
         options.add_argument("--headless")
         options.add_argument(
             "user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/79.0.3945.79 Safari/537.36"
         )
 
-        driver = webdriver.Chrome(
-            service=ChromeService(ChromeDriverManager().install()), options=options
-        )
+        driver = driver = uc.Chrome()
 
         driver.get(dialog_url)
 
         elem = driver.find_element(By.ID, "mobileNum")
         elem.clear()
         elem.send_keys(params["mobile_no"])
 
         c1 = driver.find_element(By.ID, "getOtp")
+        driver.execute_script("arguments[0].removeAttribute('disabled');", c1)
         c1.click()
 
         totp = cls.totp_creator(params["totpstr"])
         elem = WebDriverWait(driver, 5).until(
             EC.presence_of_element_located((By.ID, "otpNum"))
         )
         elem.clear()
```

### Comparing `fenix-1.0.4/fenix/vpc.py` & `fenix-1.0.5/fenix/vpc.py`

 * *Files identical despite different names*

### Comparing `fenix-1.0.4/fenix/zerodha.py` & `fenix-1.0.5/fenix/zerodha.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,21 @@
     """
 
     # Market Data Dictonaries
 
     indices = {}
     eq_tokens = {}
     nfo_tokens = {}
-    token_params = ["user_id", "password", "totpstr", "api_key", "api_secret"]
+    token_params = [
+        "user_id",
+        "password",
+        "totpstr",
+        "api_key",
+        "api_secret",
+    ]
     id = "zerodha"
     _session = Broker._create_session()
 
     # Base URLs
 
     base_urls = {
         "api_doc": "https://kite.trade/docs/connect/v3",
@@ -201,17 +207,23 @@
         Stores them in the zerodha.indices Dictionary.
 
         Returns:
             dict: Unified fenix indices format.
         """
         df = cls.data_reader(cls.base_urls["market_data"], filetype="csv")
 
-        df = df[(df["segment"] == "INDICES")][["tradingsymbol", "instrument_token"]]
+        df = df[(df["segment"] == "INDICES")][
+            ["tradingsymbol", "instrument_token", "exchange"]
+        ]
         df.rename(
-            {"tradingsymbol": "Symbol", "instrument_token": "Token"},
+            {
+                "tradingsymbol": "Symbol",
+                "instrument_token": "Token",
+                "exchange": "Exchange",
+            },
             axis=1,
             inplace=True,
         )
         df.index = df["Symbol"]
 
         indices = df.to_dict(orient="index")
```

### Comparing `fenix-1.0.4/fenix.egg-info/PKG-INFO` & `fenix-1.0.5/fenix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenix
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python library for trading in the Indian Finance Sector with support for multiple broker APIs.
 Home-page: https://fenix.hardeep.tech
 Author: Hardeep Singh
 Author-email: Hardeep Singh <hardeep.hd13@gmail.com>
 Maintainer-email: Hardeep Singh <hardeep.hd13@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -708,14 +708,15 @@
 Requires-Dist: PyJWT>=2.8.0
 Requires-Dist: pyotp>=2.9.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: requests-oauthlib>=1.4.0
 Requires-Dist: selenium>=4.18.1
 Requires-Dist: urllib3>=2.2.1
 Requires-Dist: webdriver-manager>=4.0.1
+Requires-Dist: undetected-chromedriver>=3.5.5
 
 # Fenix – Indian Broker Trading Library
 
 ![License](https://img.shields.io/badge/License-GPLv3-blue?color=%234ec820)
 
 
 A Python library for trading in the Indian Finance Sector with support for many broker APIs.
```

### Comparing `fenix-1.0.4/fenix.egg-info/SOURCES.txt` & `fenix-1.0.5/fenix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenix-1.0.4/pyproject.toml` & `fenix-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "PyJWT>=2.8.0",
     "pyotp>=2.9.0",
     "requests>=2.31.0",
     "requests-oauthlib>=1.4.0",
     "selenium>=4.18.1",
     "urllib3>=2.2.1",
     "webdriver-manager>=4.0.1",
+    "undetected-chromedriver>=3.5.5",
 ]
 requires-python = ">=3.8"
 authors = [
     {name = "Hardeep Singh", email = "hardeep.hd13@gmail.com"}
 ]
 maintainers = [
     {name = "Hardeep Singh", email = "hardeep.hd13@gmail.com"}
```

### Comparing `fenix-1.0.4/setup.py` & `fenix-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import setuptools
 import codecs
 import os.path
 
+
 def read(rel_path):
     here = os.path.abspath(os.path.dirname(__file__))
     with codecs.open(os.path.join(here, rel_path), 'r') as fp:
         return fp.read()
 
+
 def get_version(rel_path):
     for line in read(rel_path).splitlines():
         if line.startswith('__version__'):
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
+
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="fenix",
     version=get_version("fenix/__init__.py"),
     keywords="fenix, aliceblue, angelone, choice, finvasia, fivepaisa, fyers, iifl, kotak, kotakneo, kunjee, mastertrust, motilaloswal, paper, symphony, upstox, vpc, zerodha, finance, broker, trader, XTS, kite, algorithmic, algotrading, api, arbitrage, real-time, realtime, backtest, backtesting, etc, framework, invest, investing, investor, library, market, market data, ohlcv, order, orderbook, order book, strategy, ticker, tickers, toolkit, trade, trader, trading, volume, websocket, websockets, web socket, web sockets, ws",
@@ -39,14 +42,15 @@
         "PyJWT>=2.8.0",
         "pyotp>=2.9.0",
         "requests>=2.31.0",
         "requests-oauthlib>=1.4.0",
         "selenium>=4.18.1",
         "urllib3>=2.2.1",
         "webdriver-manager>=4.0.1",
+        "undetected-chromedriver>=3.5.5",
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Financial and Insurance Industry",
         "Intended Audience :: Information Technology",
         "Topic :: Software Development :: Build Tools",
```

