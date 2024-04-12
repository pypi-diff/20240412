# Comparing `tmp/faxdatasdk-0.0.7.tar.gz` & `tmp/faxdatasdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faxdatasdk-0.0.7.tar", last modified: Mon Apr  8 14:16:10 2024, max compression
+gzip compressed data, was "faxdatasdk-0.0.9.tar", last modified: Tue Apr  9 02:47:20 2024, max compression
```

## Comparing `faxdatasdk-0.0.7.tar` & `faxdatasdk-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 14:16:10.079416 faxdatasdk-0.0.7/
--rw-rw-rw-   0        0        0    11558 2023-07-09 16:17:28.000000 faxdatasdk-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     3484 2024-04-08 14:16:10.079416 faxdatasdk-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2770 2024-01-06 09:53:52.000000 faxdatasdk-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 14:16:10.065395 faxdatasdk-0.0.7/faxdatasdk/
--rw-rw-rw-   0        0        0     1294 2024-04-07 13:47:56.000000 faxdatasdk-0.0.7/faxdatasdk/__init__.py
--rw-rw-rw-   0        0        0    15452 2024-04-08 14:14:14.000000 faxdatasdk-0.0.7/faxdatasdk/api.py
--rw-rw-rw-   0        0        0     9605 2024-04-07 14:10:47.000000 faxdatasdk-0.0.7/faxdatasdk/client.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:16:10.078417 faxdatasdk-0.0.7/faxdatasdk/compat/
--rw-rw-rw-   0        0        0        0 2023-07-09 16:17:28.000000 faxdatasdk-0.0.7/faxdatasdk/compat/__init__.py
--rw-rw-rw-   0        0        0     2187 2023-07-09 16:17:28.000000 faxdatasdk-0.0.7/faxdatasdk/compat/pickle_compat.py
--rw-rw-rw-   0        0        0      175 2023-07-09 16:17:28.000000 faxdatasdk-0.0.7/faxdatasdk/exceptions.py
--rw-rw-rw-   0        0        0     3417 2023-12-29 07:30:25.000000 faxdatasdk-0.0.7/faxdatasdk/logger.py
--rw-rw-rw-   0        0        0     2216 2023-12-30 10:25:49.000000 faxdatasdk-0.0.7/faxdatasdk/request.py
--rw-rw-rw-   0        0        0      811 2024-04-07 14:11:07.000000 faxdatasdk-0.0.7/faxdatasdk/thrift_client.py
--rw-rw-rw-   0        0        0      590 2023-12-30 02:20:26.000000 faxdatasdk-0.0.7/faxdatasdk/utils.py
--rw-rw-rw-   0        0        0      438 2024-04-08 14:16:06.000000 faxdatasdk-0.0.7/faxdatasdk/version.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:16:10.077417 faxdatasdk-0.0.7/faxdatasdk.egg-info/
--rw-rw-rw-   0        0        0     3484 2024-04-08 14:16:10.000000 faxdatasdk-0.0.7/faxdatasdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      493 2024-04-08 14:16:10.000000 faxdatasdk-0.0.7/faxdatasdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 14:16:10.000000 faxdatasdk-0.0.7/faxdatasdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-08 14:16:10.000000 faxdatasdk-0.0.7/faxdatasdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      151 2024-04-08 14:16:10.000000 faxdatasdk-0.0.7/faxdatasdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-08 14:16:10.000000 faxdatasdk-0.0.7/faxdatasdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 14:16:10.079416 faxdatasdk-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1966 2024-04-07 14:26:19.000000 faxdatasdk-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:47:20.079053 faxdatasdk-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2023-07-09 16:17:28.000000 faxdatasdk-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3484 2024-04-09 02:47:20.079053 faxdatasdk-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2770 2024-01-06 09:53:52.000000 faxdatasdk-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 02:47:20.057210 faxdatasdk-0.0.9/faxdatasdk/
+-rw-rw-rw-   0        0        0     1294 2024-04-07 13:47:56.000000 faxdatasdk-0.0.9/faxdatasdk/__init__.py
+-rw-rw-rw-   0        0        0    16317 2024-04-09 02:47:16.000000 faxdatasdk-0.0.9/faxdatasdk/api.py
+-rw-rw-rw-   0        0        0     9605 2024-04-07 14:10:47.000000 faxdatasdk-0.0.9/faxdatasdk/client.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:47:20.078005 faxdatasdk-0.0.9/faxdatasdk/compat/
+-rw-rw-rw-   0        0        0        0 2023-07-09 16:17:28.000000 faxdatasdk-0.0.9/faxdatasdk/compat/__init__.py
+-rw-rw-rw-   0        0        0     2187 2023-07-09 16:17:28.000000 faxdatasdk-0.0.9/faxdatasdk/compat/pickle_compat.py
+-rw-rw-rw-   0        0        0      175 2023-07-09 16:17:28.000000 faxdatasdk-0.0.9/faxdatasdk/exceptions.py
+-rw-rw-rw-   0        0        0     3417 2023-12-29 07:30:25.000000 faxdatasdk-0.0.9/faxdatasdk/logger.py
+-rw-rw-rw-   0        0        0     2216 2023-12-30 10:25:49.000000 faxdatasdk-0.0.9/faxdatasdk/request.py
+-rw-rw-rw-   0        0        0      811 2024-04-07 14:11:07.000000 faxdatasdk-0.0.9/faxdatasdk/thrift_client.py
+-rw-rw-rw-   0        0        0      590 2023-12-30 02:20:26.000000 faxdatasdk-0.0.9/faxdatasdk/utils.py
+-rw-rw-rw-   0        0        0      438 2024-04-09 02:47:16.000000 faxdatasdk-0.0.9/faxdatasdk/version.py
+drwxrwxrwx   0        0        0        0 2024-04-09 02:47:20.073163 faxdatasdk-0.0.9/faxdatasdk.egg-info/
+-rw-rw-rw-   0        0        0     3484 2024-04-09 02:47:19.000000 faxdatasdk-0.0.9/faxdatasdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2024-04-09 02:47:19.000000 faxdatasdk-0.0.9/faxdatasdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 02:47:19.000000 faxdatasdk-0.0.9/faxdatasdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-09 02:47:19.000000 faxdatasdk-0.0.9/faxdatasdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      151 2024-04-09 02:47:19.000000 faxdatasdk-0.0.9/faxdatasdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 02:47:19.000000 faxdatasdk-0.0.9/faxdatasdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 02:47:20.079053 faxdatasdk-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1966 2024-04-07 14:26:19.000000 faxdatasdk-0.0.9/setup.py
```

### Comparing `faxdatasdk-0.0.7/LICENSE` & `faxdatasdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.7/PKG-INFO` & `faxdatasdk-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faxdatasdk
-Version: 0.0.7
+Version: 0.0.9
 Summary: Data SDK for stock analysis.
 Home-page: https://www.faxframework.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 License: Apache License v2
```

### Comparing `faxdatasdk-0.0.7/README.md` & `faxdatasdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.7/faxdatasdk/__init__.py` & `faxdatasdk-0.0.9/faxdatasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.7/faxdatasdk/api.py` & `faxdatasdk-0.0.9/faxdatasdk/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 # coding=utf-8
 from .client import FaxDataClient
 from .utils import *
+from typing import Union, List
 
 
 @assert_auth
-def get_factor(sec_code: str = None,
+def get_factor(sec_code: Union[None, str, List[str]] = None,
+               factor: Union[None, str, List[str]] = None,
                sec_code_list: list = None,
-               factor_list=None,
+               factor_list: list = None,
                factor_group_list: list = None,
                trade_date: str = None,
                start_date: str = None,
                end_date: str = None,
                start_datetime: str = None,
                end_datetime: str = None,
                stock_pool: list = None,
-               dividend_type='front',
+               dividend_type: str = 'front',
                unit: str = '1d',
                expect_df: bool = True,
                count: int = None):
     """
     查询因子库数据.
 
-    :param sec_code: 股票代码
+
+    :param sec_code: 股票代码，支持字符串或者字符串数组. 为数组的时候等价于sec_code_list
+    :param factor: 因子名称, 支持字符串或者字符串数组，为数组的时候，等价于factor_list
     :param sec_code_list: 股票代码列表
     :param factor_list: 因子列表，因子可能来源于不同的因子分组
     :param factor_group_list: 限定因子分组
     :param trade_date: 限定交易日
     :param start_date: 开始交易日
     :param end_date: 结束交易日
     :param start_datetime: 当unit='1m'时有效，格式：2023-03-29 14:57:00
     :param end_datetime: 当unit='1m'时有效，格式：2023-03-29 14:57:00
-    :param stock_pool: 指数列表，仅加载指数成分股
-    :param dividend_type: 复权选项
+    :param stock_pool: 指数列表，仅加载指数成分股。
+                       选出了历史中出现在指数中所有成分，此时有未来函数，等于把低价股票提前选入了沪深300的股票池中。
+                       数据分析中需要结合crud.get_index_members_lst()一起使用，过滤掉未来函数的股票。
+    :param dividend_type: 复权选项(对股票/基金的价格字段、成交量字段及factor字段生效)
                 'front'
                 : 前复权, 默认是前复权
                 none
                 : 不复权, 返回实际价格
                 'back'
                 : 后复权
     :param unit: 单位时间长度，支持1d、1m，默认为1d
@@ -101,25 +107,25 @@
                 stock_pool: list = None,
                 expect_df=True,
                 skip_paused=False,
                 dividend_type='front'):
     """
     获取历史数据，可查询多个标的单个数据字段，返回数据格式为 DataFrame 或 Dict(字典)
 
-    :param stock_pool: 股票池
-    :param start_date: 开始日期
-    :param end_date: 结束日期
+    :param stock_pool:
+    :param start_date:
+    :param end_date:
     :param count: 数量, 返回的结果集的行数
     :param unit: 单位时间长度, 几天或者几分钟, 现在支持'1d','1m'
     :param start_datetime: 当unit='1m'时有效，格式：2023-03-29 14:57:00
     :param end_datetime: 当unit='1m'时有效，格式：2023-03-29 14:57:00
     :param field: 要获取的数据字段
     :param security_list: 要获取数据的股票列表
-    :param expect_df: df=True: [pandas.DataFrame]对象, 行索引是[datetime.datetime]对象, 列索引是股票代号
-               df=False: dict, key是股票代码, value是一个numpy数组[numpy.ndarray]
+    :param expect_df: expect_df=True: [pandas.DataFrame]对象, 行索引是[datetime.datetime]对象, 列索引是股票代号
+               expect_df=False: dict, key是股票代码, value是一个numpy数组[numpy.ndarray]
     :param skip_paused: 是否跳过不交易日期(包括停牌, 未上市或者退市后的日期)
     :param dividend_type: 复权选项(对股票/基金的价格字段、成交量字段及factor字段生效)
                 'front'
                 : 前复权, 默认是前复权
                 none
                 : 不复权, 返回实际价格
                 'back'
@@ -382,19 +388,26 @@
     :param stock_lst:
     :param suspend_type: 停牌：S，复牌：R
     :return:
     """
     return FaxDataClient.instance().get_suspend_info(**locals())
 
 
+@assert_auth
 def get_stock_name_his(sec_code: str, trade_date: str):
     """
     获取股票代码的历史名称
     :param trade_date:
     :param sec_code:
     :return: {'sec_code': '000001.SZ', 'name': '平安银行', 'start_date': '2012-08-02', 'end_date': '2099-12-30'}
     """
     return FaxDataClient.instance().get_stock_name_his(**locals())
 
 
-__all__ = []
+@assert_auth
+def is_open_trade_date(date: str):
+    """检查是否为交易日"""
+    return FaxDataClient.instance().is_open_trade_date(**locals())
+
+
+__all__ = ["is_open_trade_date"]
 __all__.extend([name for name in globals().keys() if name.startswith("get")])
```

### Comparing `faxdatasdk-0.0.7/faxdatasdk/client.py` & `faxdatasdk-0.0.9/faxdatasdk/client.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.7/faxdatasdk/compat/pickle_compat.py` & `faxdatasdk-0.0.9/faxdatasdk/compat/pickle_compat.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.7/faxdatasdk/logger.py` & `faxdatasdk-0.0.9/faxdatasdk/logger.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.7/faxdatasdk/request.py` & `faxdatasdk-0.0.9/faxdatasdk/request.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.7/faxdatasdk/thrift_client.py` & `faxdatasdk-0.0.9/faxdatasdk/thrift_client.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.7/faxdatasdk/utils.py` & `faxdatasdk-0.0.9/faxdatasdk/utils.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.7/faxdatasdk.egg-info/PKG-INFO` & `faxdatasdk-0.0.9/faxdatasdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faxdatasdk
-Version: 0.0.7
+Version: 0.0.9
 Summary: Data SDK for stock analysis.
 Home-page: https://www.faxframework.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 License: Apache License v2
```

### Comparing `faxdatasdk-0.0.7/setup.py` & `faxdatasdk-0.0.9/setup.py`

 * *Files identical despite different names*

