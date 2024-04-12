# Comparing `tmp/pyqqq-0.7.1.tar.gz` & `tmp/pyqqq-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.7.1.tar", max compression
+gzip compressed data, was "pyqqq-0.7.2.tar", max compression
```

## Comparing `pyqqq-0.7.1.tar` & `pyqqq-0.7.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.7.1/README.md
--rw-r--r--   0        0        0      770 2024-04-11 04:26:19.637148 pyqqq-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.7.1/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.7.1/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.7.1/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    39030 2024-04-04 06:07:52.832635 pyqqq-0.7.1/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.7.1/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24219 2024-04-11 04:25:37.648517 pyqqq-0.7.1/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.7.1/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.7.1/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.7.1/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.7.1/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.7.1/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24359 2024-04-11 03:46:13.044337 pyqqq-0.7.1/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.7.1/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      437 2024-03-25 05:15:17.008929 pyqqq-0.7.1/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.7.1/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.7.1/pyqqq/data/daily.py
--rw-r--r--   0        0        0     6546 2024-04-09 03:46:33.909510 pyqqq-0.7.1/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     7289 2024-04-04 05:56:05.786196 pyqqq-0.7.1/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.7.1/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.878098 pyqqq-0.7.1/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      951 2024-04-09 08:23:47.157710 pyqqq-0.7.1/pyqqq/utils/array.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.7.1/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.7.1/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.7.1/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.7.1/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.7.1/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.7.1/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.7.2/README.md
+-rw-r--r--   0        0        0      770 2024-04-11 10:01:50.723071 pyqqq-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.7.2/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.7.2/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.7.2/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    39223 2024-04-11 09:59:48.694231 pyqqq-0.7.2/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.7.2/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24219 2024-04-11 09:20:58.472842 pyqqq-0.7.2/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.7.2/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.7.2/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.7.2/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.7.2/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.7.2/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24359 2024-04-11 03:46:13.044337 pyqqq-0.7.2/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.7.2/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      437 2024-03-25 05:15:17.008929 pyqqq-0.7.2/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.7.2/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     6546 2024-04-09 03:46:33.909510 pyqqq-0.7.2/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     5939 2024-04-11 09:40:12.485317 pyqqq-0.7.2/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.7.2/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.7.2/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.7.2/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.878098 pyqqq-0.7.2/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.7.2/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.7.2/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.7.2/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.7.2/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.7.2/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.7.2/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.7.2/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.7.2/PKG-INFO
```

### Comparing `pyqqq-0.7.1/README.md` & `pyqqq-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyproject.toml` & `pyqqq-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.7.1"
+version = "0.7.2"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.7.1/pyqqq/__init__.py` & `pyqqq-0.7.2/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.7.2/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pyqqq.brokerage.ebest.oauth import EBestAuth
 from pyqqq.brokerage.ebest.tr_client import (
     EBestTRClient,
     EBestTRWebsocketClient,
     EBestTRWebsocketKeepConnectionStatus,
 )
-from pyqqq.utils.limiter import limit_calls
+from pyqqq.utils.limiter import CallLimiter, limit_calls
 from typing import AsyncGenerator
 import asyncio
 import datetime as dtm
 import json
 import websockets
 
 from pyqqq.utils.market_schedule import get_market_schedule
@@ -23,15 +23,14 @@
         self.auth = auth
         self.corp_data = corp_data
         self.tr_client = EBestTRClient(auth)
 
     def _tr_request(self, *args, **kwargs):
         return self.tr_client.request(*args, **kwargs)
 
-    @limit_calls(scope="ebest/t8436", max_calls=2)
     def get_asset_list(self, market_type: str = "0") -> list:
         """
         ([주식]기타) 주식종목조회 API용 (t8436)
 
         Args:
             market_type (str): 시장유형 (0:전체 1:코스피 2:코스닥)
 
@@ -53,14 +52,16 @@
                 - recprice (int): 기준가
                 - gubun (str): 구분 (1:코스피 2:코스닥)
                 - bu12gubun (str): 12월결산월
                 - spac_gubun (str): 기업인수목적회사여부 (Y:기업인수목적회사)
                 - filler (str): filler
         """
 
+        CallLimiter().wait_limit_rate(2, scope="ebest/t8436")
+
         assert market_type in ["0", "1", "2"], "Invalid market type"
 
         tr_code = "t8436"
         req_body = {f"{tr_code}InBlock": {"gubun": market_type}}
 
         res_body, _ = self._tr_request("/stock/etc", tr_code, body=req_body)
 
@@ -68,15 +69,14 @@
             "rsp_cd": res_body["rsp_cd"],
             "rsp_msg": res_body["rsp_msg"],
             "output": res_body.get("t8436OutBlock", []),
         }
 
         return result
 
-    @limit_calls(scope="ebest/t1102", max_calls=3)
     def get_price(self, asset_code: str) -> dict:
         """
         ([주식]시세) 주식현재가(시세)조회 (t1102)
 
         Args:
             asset_code (str): 종목 코드
 
@@ -85,27 +85,28 @@
 
             - rsp_cd (str): 응답코드
             - rsp_msg (str): 응답메시지
             - output (list): 종목의 현재가 정보
         """
         assert len(asset_code) == 6, "Invalid asset code"
 
+        CallLimiter().wait_limit_rate(3, scope="ebest/t1102")
+
         tr_code = "t1102"
         req_body = {f"{tr_code}InBlock": {"shcode": asset_code}}
         res_body, _ = self._tr_request("/stock/market-data", tr_code, body=req_body)
 
         result = {
             "rsp_cd": res_body["rsp_cd"],
             "rsp_msg": res_body["rsp_msg"],
             "output": res_body.get("t1102OutBlock", []),
         }
 
         return result
 
-    @limit_calls(scope="ebest/t1301", max_calls=2)
     def get_stock_time_conclude(
         self,
         asset_code: str,
         cvolume: int,
         start_time: dtm.time,
         end_time: dtm.time,
         cts_time: str = "",
@@ -127,14 +128,16 @@
             - rsp_cd (str): 응답코드
             - rsp_msg (str): 응답메시지
             - tr_cont (str): 연속조회여부
             - tr_cont_key (str): 연속조회키
             - output (list): 주식 시간대별 체결 정보
         """
 
+        CallLimiter().wait_limit_rate(2, scope="ebest/t1301")
+
         assert len(asset_code) == 6, "Invalid asset code"
 
         tr_code = "t1301"
         tr_cont = "Y" if cts_time else "N"
 
         req_body = {
             f"{tr_code}InBlock": {
@@ -160,15 +163,14 @@
             "tr_cont": res_header.get("tr_cont", ""),
             "tr_cont_key": res_header.get("tr_cont_key", ""),
             "output": res_body.get("t1301OutBlock", []),
         }
 
         return result
 
-    @limit_calls(scope="ebest/t1302", max_calls=1)
     def get_stock_minute_prices(
         self,
         shcode: str,
         gubun: str,
         cnt=900,
         cts_time: str = "",
         tr_cont_key: str = "",
@@ -190,14 +192,16 @@
             - rsp_msg (str): 응답메시지
             - tr_cont (str): 연속조회여부
             - tr_cont_key (str): 연속조회키
             - output1 (dict): 연속 조회를 위한 cts_time 필드를 포함
             - output2 (list): 주식 분별 주가 정보
         """
 
+        CallLimiter().wait_limit_rate(1, scope="ebest/t1302")
+
         assert len(shcode) == 6, "Invalid asset code"
         assert gubun in ["1", "2", "3", "4", "5", "6"], "Invalid gubun"
 
         tr_code = "t1302"
         tr_cont = "Y" if cts_time else "N"
 
         req_body = {
@@ -224,15 +228,14 @@
             "tr_cont_key": res_header.get("tr_cont_key", ""),
             "output1": res_body.get("t1302OutBlock", {}),
             "output2": res_body.get("t1302OutBlock1", []),
         }
 
         return result
 
-    @limit_calls(scope="ebest/t1310", max_calls=1)
     def get_stock_tick_data_today_yesterday(
         self,
         daygb: int,
         timegb: int,
         shcode: str,
         endtime: dtm.time,
         cts_time: str = "",
@@ -255,14 +258,16 @@
             - rsp_cd (str): 응답코드
             - rsp_msg (str): 응답메시지
             - tr_cont (str): 연속조회여부
             - tr_cont_key (str): 연속조회키
             - output1 (dict): 연속 조회를 위한 cts_time 필드를 포함
             - output2 (list): 분틱 정보
         """
+        CallLimiter().wait_limit_rate(1, scope="ebest/t1310")
+
         assert daygb in [0, 1], "Invalid daygb"
         assert timegb in [0, 1], "Invalid timegb"
         assert len(shcode) >= 6, "Invalid asset code"
         assert isinstance(endtime, dtm.time), "Invalid endtime"
 
         tr_code = "t1310"
         req_body = {
@@ -292,15 +297,14 @@
             "tr_cont_key": res_header.get("tr_cont_key", ""),
             "output1": res_body.get("t1310OutBlock", {}),
             "output2": res_body.get("t1310OutBlock1", []),
         }
 
         return result
 
-    @limit_calls(scope="ebest/t8410", max_calls=1)
     def get_stock_chart_dwmy(
         self,
         shcode: str,
         gubun: str,
         edate: dtm.date,
         sdate: dtm.date = None,
         qrycnt: int = 500,
@@ -330,14 +334,16 @@
             - rsp_msg (str): 응답메시지
             - tr_cont (str): 연속조회여부
             - tr_cont_key (str): 연속조회키
             - output1 (dict): 전일/당일 시세 정보
             - output2 (list): 주기별 시세 정보
         """
 
+        CallLimiter().wait_limit_rate(1, scope="ebest/t8410")
+
         assert len(shcode) == 6, "Invalid asset code"
         assert gubun.lower() in ["d", "w", "m", "y"], "Invalid gubun"
 
         tr_code = "t8410"
         tr_cont = "Y" if cts_date else "N"
 
         req_body = {
@@ -368,15 +374,14 @@
             "rsp_msg": res_body["rsp_msg"],
             "output1": res_body.get("t8410OutBlock", {}),
             "output2": res_body.get("t8410OutBlock1", []),
         }
 
         return result
 
-    @limit_calls(scope="ebest/t8412", max_calls=1)
     def get_stock_chart_minutes(
         self,
         shcode: str,
         ncnt: int,
         qrycnt: int,
         nday: int,
         edate: dtm.date,
@@ -408,14 +413,16 @@
             - rsp_msg (str): 응답메시지
             - tr_cont (str): 연속조회여부
             - tr_cont_key (str): 연속조회키
             - output1 (dict): 전일/당일 시세 정보
             - output2 (list): 단위 별 주식 차트 정보
         """
 
+        CallLimiter().wait_limit_rate(1, scope="ebest/t8412")
+
         tr_code = "t8412"
         tr_cont = "Y" if cts_date else "N"
 
         req_body = {
             f"{tr_code}InBlock": {
                 "shcode": shcode,
                 "ncnt": ncnt,
@@ -444,43 +451,43 @@
             "rsp_msg": res_body["rsp_msg"],
             "output1": res_body.get("t8412OutBlock", {}),
             "output2": res_body.get("t8412OutBlock1", []),
         }
 
         return result
 
-    @limit_calls(scope="ebest/CSPAQ12200", max_calls=1)
     def get_account_deposit_orderable_total_evaluation(self) -> dict:
         """
         ([주식]계좌) 현물계좌예수금 주문가능금액 총평가 조회 (CSPAQ12200)
 
         Returns:
             dict: 주문가능금액 총평가 정보
 
             - rsp_cd (str): 응답코드
             - rsp_msg (str): 응답메시지
             - output1 (dict): 계좌기본정보
             - output2 (dict): 주문가능금액 총평가 정보
         """
 
+        CallLimiter().wait_limit_rate(1, scope="ebest/CSPAQ12200")
+
         tr_code = "CSPAQ12200"
         req_body = {f"{tr_code}InBlock1": {"BalCreTp": "0"}}
 
         res_body, _ = self._tr_request("/stock/accno", tr_code, body=req_body)
 
         result = {
             "rsp_cd": res_body["rsp_cd"],
             "rsp_msg": res_body["rsp_msg"],
             "output1": res_body.get("CSPAQ12200OutBlock1", {}),
             "output2": res_body.get("CSPAQ12200OutBlock2", {}),
         }
 
         return result
 
-    @limit_calls(scope="ebest/CSPBQ00200", max_calls=1)
     def get_account_orderable_quantity(
         self,
         bns_tp_code: int,
         isu_no: str,
         ord_prc: int,
     ) -> dict:
         """
@@ -495,14 +502,17 @@
             dict: 주문가능수량 정보
 
             - rsp_cd (str): 응답코드
             - rsp_msg (str): 응답메시지
             - output1 (dict): 요청 정보
             - output2 (dict): 계좌 및 증거금률 별 주문가능수량 정보
         """
+
+        CallLimiter().wait_limit_rate(1, scope="ebest/CSPBQ00200")
+
         assert bns_tp_code in [1, 2], "Invalid bns_tp_code"
         assert len(isu_no) == 6 or (
             len(isu_no) == 7 and isu_no[0] == "A"
         ), "Invalid isu_no"
 
         tr_code = "CSPBQ00200"
         req_body = {
@@ -520,15 +530,14 @@
             "rsp_msg": res_body["rsp_msg"],
             "output1": res_body.get("CSPBQ00200OutBlock1", {}),
             "output2": res_body.get("CSPBQ00200OutBlock2", {}),
         }
 
         return result
 
-    @limit_calls(scope="ebest/t0424", max_calls=1)
     def get_stock_balance(
         self,
         prcgb: int = 1,
         chegb: int = 0,
         dangb: int = 0,
         charge: int = 0,
         cts_expcode: str = "",
@@ -551,14 +560,16 @@
             - rsp_msg (str): 응답메시지
             - tr_cont (str): 연속조회여부
             - tr_cont_key (str): 연속조회키
             - output1 (dict): 계좌 정보
             - output2 (list): 종목 별 잔고 정보
         """
 
+        CallLimiter().wait_limit_rate(1, scope="ebest/t0424")
+
         assert prcgb in [1, 2], "Invalid prcgb"
         assert chegb in [0, 2], "Invalid chegb"
         assert dangb in [0, 1], "Invalid dangb"
         assert charge in [0, 1], "Invalid charge"
 
         tr_code = "t0424"
         tr_cont = "Y" if cts_expcode else "N"
@@ -588,29 +599,30 @@
             "rsp_msg": res_body["rsp_msg"],
             "output1": res_body.get("t0424OutBlock", []),
             "output2": res_body.get("t0424OutBlock1", []),
         }
 
         return result
 
-    @limit_calls(scope="ebest/CSPAQ13700", max_calls=1)
     def get_deposit_order_list(
         self,
         isu_no: str = "",
         ord_mkt_code: str = "00",
         bns_tp_code: str = "0",
         exec_yn: str = "0",
         ord_dt: str = None,
         srt_ord_no2: str = "999999999",
         bkseq_tp_code: str = "0",
         ord_ptn_code: str = "00",
     ) -> dict:
         """
         ([주식]계좌) 현물계좌 주문체결내역 조회(API) (CSPAQ13700)
         """
+        CallLimiter().wait_limit_rate(1, scope="ebest/CSPAQ13700")
+
         tr_code = "CSPAQ13700"
         if ord_dt is None:
             ord_dt = dtm.date.today().strftime("%Y%m%d")
 
         req_body = {
             f"{tr_code}InBlock1": {
                 "IsuNo": isu_no,
@@ -634,15 +646,14 @@
             "output1": res_body.get("CSPAQ13700OutBlock1", {}),
             "output2": res_body.get("CSPAQ13700OutBlock2", {}),
             "output3": res_body.get("CSPAQ13700OutBlock3", {}),
         }
 
         return result
 
-    @limit_calls(scope="ebest/t0425", max_calls=1)
     def get_order_list(
         self,
         chegb: int = 0,
         medosu: int = 0,
         sortgb: int = 2,
         expcode: str = "",
         cts_ordno: str = "",
@@ -665,14 +676,16 @@
             - rsp_cd (str): 응답코드
             - rsp_msg (str): 응답메시지
             - tr_cont (str): 연속조회여부
             - tr_cont_key (str): 연속조회키
             - output1 (dict): 총 주문/체결 정보
             - output2 (list): 주문 별 정보
         """
+        CallLimiter().wait_limit_rate(1, scope="ebest/t0425")
+
         tr_code = "t0425"
         tr_cont = "Y" if cts_ordno else "N"
 
         req_body = {
             f"{tr_code}InBlock": {
                 "chegb": str(chegb),
                 "medosu": str(medosu),
@@ -720,15 +733,14 @@
             "tr_cont_key": res_header.get("tr_cont_key", ""),
             "output1": res_body["t0425OutBlock"],
             "output2": res_body["t0425OutBlock1"],
         }
 
         return result
 
-    @limit_calls(scope="ebest/CSPAT00601", max_calls=10)
     def create_order(
         self,
         isu_no: str,
         ord_qty: int,
         ord_prc: int,
         bns_tp_code: int,
         ord_prc_ptn_code: str,
@@ -779,14 +791,16 @@
             dict: 주문 결과
 
             - rsp_cd (str): 응답코드
             - rsp_msg (str): 응답메시지
             - output1 (dict): 주문 결과
             - output2 (dict): 주문 결과
         """
+        CallLimiter().wait_limit_rate(10, scope="ebest/CSPAT00601")
+
         tr_cd = "CSPAT00601"
         req_body = {
             f"{tr_cd}InBlock1": {
                 "IsuNo": isu_no,
                 "OrdQty": ord_qty,
                 "OrdPrc": ord_prc,
                 "BnsTpCode": str(bns_tp_code),
@@ -804,15 +818,14 @@
             "rsp_msg": res_body["rsp_msg"],
             "output1": res_body.get(f"{tr_cd}OutBlock1", {}),
             "output2": res_body.get(f"{tr_cd}OutBlock2", {}),
         }
 
         return result
 
-    @limit_calls(scope="ebest/CSPAT00701", max_calls=3)
     def update_order(
         self,
         org_ord_no: str,
         isu_no: str,
         ord_qty: int,
         ord_prc_ptn_code: str,
         ord_cndi_tp_code: int = 0,
@@ -844,14 +857,16 @@
 
             - rsp_cd (str): 응답코드
             - rsp_msg (str): 응답메시지
             - output1 (dict): 원 주문 정보
             - output2 (dict): 정정 주문 정보
         """
 
+        CallLimiter().wait_limit_rate(3, scope="ebest/CSPAT00701")
+
         tr_cd = "CSPAT00701"
         req_body = {
             f"{tr_cd}InBlock1": {
                 "OrgOrdNo": int(org_ord_no),
                 "IsuNo": isu_no,
                 "OrdQty": ord_qty,
                 "OrdprcPtnCode": ord_prc_ptn_code,
@@ -867,15 +882,14 @@
             "rsp_msg": res_body["rsp_msg"],
             "output1": res_body.get(f"{tr_cd}OutBlock1", {}),
             "output2": res_body.get(f"{tr_cd}OutBlock2", {}),
         }
 
         return result
 
-    @limit_calls(scope="ebest/CSPAT00801", max_calls=3)
     def cancel_order(self, org_ord_no: str, isu_no: str, ord_qty: int) -> dict:
         """
         ([주식]주문) 현물취소주문 (CSPAT00801)
 
         Args:
             org_ord_no (str): 원주문번호
             isu_no (str): 종목번호
@@ -886,14 +900,15 @@
 
             - rsp_cd (str): 응답코드
             - rsp_msg (str): 응답메시지
             - output1 (dict): 원 주문 정보
             - output2 (dict): 취소 주문 정보
 
         """
+        CallLimiter().wait_limit_rate(3, scope="ebest/CSPAT00801")
 
         tr_cd = "CSPAT00801"
         req_body = {
             f"{tr_cd}InBlock1": {
                 "OrgOrdNo": int(org_ord_no),
                 "IsuNo": isu_no,
                 "OrdQty": ord_qty,
```

### Comparing `pyqqq-0.7.1/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.7.2/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.7.2/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.7.2/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.7.2/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.7.2/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.7.2/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.7.2/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.7.2/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/data/daily.py` & `pyqqq-0.7.2/pyqqq/data/ticks.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/data/domestic.py` & `pyqqq-0.7.2/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/data/realtime.py` & `pyqqq-0.7.2/pyqqq/data/minutes.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,58 +2,15 @@
 import datetime as dtm
 import pandas as pd
 import pyqqq
 import pyqqq.config as c
 import pytz
 import requests
 
-logger = get_logger("realtime")
-
-
-def get_all_last_trades():
-    """
-    모든 종목의 최근 체결 정보를 반환합니다.
-
-    Returns:
-        list:
-        - dict:
-            - chetime (str): 체결시간
-            - sign (str): 전일대비구분
-            - change (int): 전일대비가격
-            - drate (float): 전일대비등락율
-            - price (int): 체결가
-            - opentime (str): 시가시간
-            - open (int): 시가
-            - hightime (str): 고가시간
-            - high (int): 고가
-            - lowtime (str): 저가시간
-            - low (int): 저가
-            - cgubun (str): 체결구분
-            - cvolume (int): 체결량
-            - value (int): 누적거래대금
-            - mdvolume (int): 매도체결수량
-            - mdchecnt (int): 매도체결건수
-            - msvolume (int): 매수체결수량
-            - mschecnt (int): 매수체결건수
-            - cpower (float): 체결강도
-            - offerho (int): 매도호가
-            - bidho (int): 매수호가
-            - status (str): 장정보
-            - jnilvolume (int): 전일거래량
-            - shcode (str): 종목코드
-
-    """
-
-    r = requests.get(f"{c.PYQQQ_API_URL}/domestic-stock/trades")
-    r.raise_for_status()
-
-    data = r.json()
-    result = [data[k] for k in data.keys()]
-
-    return result
+logger = get_logger("minutes")
 
 
 def get_all_minute_data(
     time: dtm.datetime, include_empty: bool = False
 ) -> pd.DataFrame:
     """
     모든 종목의 분봉 데이터를 반환합니다.
```

### Comparing `pyqqq-0.7.1/pyqqq/datatypes.py` & `pyqqq-0.7.2/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/utils/array.py` & `pyqqq-0.7.2/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/utils/display.py` & `pyqqq-0.7.2/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/utils/kvstore.py` & `pyqqq-0.7.2/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/utils/limiter.py` & `pyqqq-0.7.2/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/utils/logger.py` & `pyqqq-0.7.2/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/utils/market_schedule.py` & `pyqqq-0.7.2/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/pyqqq/utils/retry.py` & `pyqqq-0.7.2/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.1/PKG-INFO` & `pyqqq-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.7.1
+Version: 0.7.2
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

