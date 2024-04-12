# Comparing `tmp/volstreet-7.1.2.tar.gz` & `tmp/volstreet-7.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-7.1.2.tar", last modified: Wed Apr 10 03:39:04 2024, max compression
+gzip compressed data, was "volstreet-7.1.3.tar", last modified: Fri Apr 12 03:35:49 2024, max compression
```

## Comparing `volstreet-7.1.2.tar` & `volstreet-7.1.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 03:39:04.266067 volstreet-7.1.2/
--rw-rw-rw-   0        0        0     1293 2024-04-10 03:39:04.266067 volstreet-7.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.1.2/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.1.2/pyproject.toml
--rw-rw-rw-   0        0        0     1104 2024-04-10 03:39:04.267495 volstreet-7.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-10 03:39:04.146669 volstreet-7.1.2/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.1.2/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:39:04.169462 volstreet-7.1.2/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.1.2/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.1.2/volstreet/angel_interface/access_rate_handlers.py
--rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     2600 2024-04-03 08:06:51.000000 volstreet-7.1.2/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    13980 2024-04-06 06:31:33.000000 volstreet-7.1.2/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-7.1.2/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    28910 2024-03-28 11:04:55.000000 volstreet-7.1.2/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.1.2/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:39:04.195073 volstreet-7.1.2/volstreet/backtests/
--rw-rw-rw-   0        0        0      187 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0     8882 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/backtests/data_handling.py
--rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.1.2/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    47225 2024-04-06 06:31:33.000000 volstreet-7.1.2/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5397 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.1.2/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15721 2024-03-26 10:23:44.000000 volstreet-7.1.2/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     1628 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    20783 2024-04-09 13:24:35.000000 volstreet-7.1.2/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     6003 2024-04-08 03:36:49.000000 volstreet-7.1.2/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:39:04.211899 volstreet-7.1.2/volstreet/datamodule/
--rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.1.2/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.1.2/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.1.2/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:39:04.211899 volstreet-7.1.2/volstreet/historical_info/
--rw-rw-rw-   0        0        0    18338 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-7.1.2/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:39:04.229263 volstreet-7.1.2/volstreet/strategies/
--rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0     5766 2024-04-09 12:38:37.000000 volstreet-7.1.2/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    27410 2024-04-08 06:26:07.000000 volstreet-7.1.2/volstreet/strategies/execution.py
--rw-rw-rw-   0        0        0    57282 2024-04-09 14:37:19.000000 volstreet-7.1.2/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0    16535 2024-04-09 15:11:43.000000 volstreet-7.1.2/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0    89791 2024-04-08 12:54:07.000000 volstreet-7.1.2/volstreet/strategies/strats.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:39:04.235967 volstreet-7.1.2/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      256 2024-04-03 08:06:51.000000 volstreet-7.1.2/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26301 2024-04-09 05:59:29.000000 volstreet-7.1.2/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0    10006 2024-04-09 12:29:54.000000 volstreet-7.1.2/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    11895 2024-04-09 12:18:28.000000 volstreet-7.1.2/volstreet/trade_interface/order_placement.py
--rw-rw-rw-   0        0        0    20048 2024-04-03 08:06:51.000000 volstreet-7.1.2/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:39:04.252538 volstreet-7.1.2/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-7.1.2/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    13047 2024-03-28 07:00:26.000000 volstreet-7.1.2/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6487 2024-03-14 04:36:05.000000 volstreet-7.1.2/volstreet/vectorized_blackscholes.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:39:04.263466 volstreet-7.1.2/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.1.2/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.1.2/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.1.2/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.1.2/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0      599 2024-03-28 11:16:14.000000 volstreet-7.1.2/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:39:04.264995 volstreet-7.1.2/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1293 2024-04-10 03:39:04.000000 volstreet-7.1.2/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2374 2024-04-10 03:39:04.000000 volstreet-7.1.2/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 03:39:04.000000 volstreet-7.1.2/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      460 2024-04-10 03:39:04.000000 volstreet-7.1.2/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-10 03:39:04.000000 volstreet-7.1.2/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 03:35:49.839087 volstreet-7.1.3/
+-rw-rw-rw-   0        0        0     1293 2024-04-12 03:35:49.839087 volstreet-7.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.1.3/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1104 2024-04-12 03:35:49.840082 volstreet-7.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 03:35:49.767407 volstreet-7.1.3/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.1.3/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 03:35:49.784724 volstreet-7.1.3/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.1.3/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.1.3/volstreet/angel_interface/access_rate_handlers.py
+-rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     2600 2024-04-03 08:06:51.000000 volstreet-7.1.3/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    13980 2024-04-06 06:31:33.000000 volstreet-7.1.3/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-7.1.3/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    29542 2024-04-11 10:12:50.000000 volstreet-7.1.3/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.1.3/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-04-12 03:35:49.798488 volstreet-7.1.3/volstreet/backtests/
+-rw-rw-rw-   0        0        0      187 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0     8882 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/backtests/data_handling.py
+-rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.1.3/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    47225 2024-04-06 06:31:33.000000 volstreet-7.1.3/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5397 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.1.3/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15721 2024-03-26 10:23:44.000000 volstreet-7.1.3/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     1628 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    20783 2024-04-09 13:24:35.000000 volstreet-7.1.3/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     6003 2024-04-08 03:36:49.000000 volstreet-7.1.3/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-04-12 03:35:49.808550 volstreet-7.1.3/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.1.3/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.1.3/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.1.3/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-12 03:35:49.809551 volstreet-7.1.3/volstreet/historical_info/
+-rw-rw-rw-   0        0        0    18338 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-7.1.3/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-04-12 03:35:49.816370 volstreet-7.1.3/volstreet/strategies/
+-rw-rw-rw-   0        0        0      133 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0     5766 2024-04-09 12:38:37.000000 volstreet-7.1.3/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    28004 2024-04-10 08:07:20.000000 volstreet-7.1.3/volstreet/strategies/execution.py
+-rw-rw-rw-   0        0        0    56936 2024-04-12 03:35:04.000000 volstreet-7.1.3/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0    17179 2024-04-10 07:52:35.000000 volstreet-7.1.3/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0    90300 2024-04-10 08:47:06.000000 volstreet-7.1.3/volstreet/strategies/strats.py
+drwxrwxrwx   0        0        0        0 2024-04-12 03:35:49.824403 volstreet-7.1.3/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      256 2024-04-03 08:06:51.000000 volstreet-7.1.3/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26301 2024-04-09 05:59:29.000000 volstreet-7.1.3/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0    10006 2024-04-09 12:29:54.000000 volstreet-7.1.3/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    11895 2024-04-09 12:18:28.000000 volstreet-7.1.3/volstreet/trade_interface/order_placement.py
+-rw-rw-rw-   0        0        0    20048 2024-04-03 08:06:51.000000 volstreet-7.1.3/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-04-12 03:35:49.830133 volstreet-7.1.3/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-7.1.3/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    13047 2024-03-28 07:00:26.000000 volstreet-7.1.3/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6487 2024-03-14 04:36:05.000000 volstreet-7.1.3/volstreet/vectorized_blackscholes.py
+drwxrwxrwx   0        0        0        0 2024-04-12 03:35:49.836480 volstreet-7.1.3/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.1.3/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.1.3/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.1.3/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.1.3/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0      599 2024-03-28 11:16:14.000000 volstreet-7.1.3/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-04-12 03:35:49.838081 volstreet-7.1.3/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1293 2024-04-12 03:35:49.000000 volstreet-7.1.3/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2374 2024-04-12 03:35:49.000000 volstreet-7.1.3/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 03:35:49.000000 volstreet-7.1.3/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      460 2024-04-12 03:35:49.000000 volstreet-7.1.3/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-12 03:35:49.000000 volstreet-7.1.3/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-7.1.2/PKG-INFO` & `volstreet-7.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.1.2
+Version: 7.1.3
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.1.2/setup.cfg` & `volstreet-7.1.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 372e 312e 320d 0a61  rsion = 7.1.2..a
+00000020: 7273 696f 6e20 3d20 372e 312e 330d 0a61  rsion = 7.1.3..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-7.1.2/volstreet/angel_interface/access_rate_handlers.py` & `volstreet-7.1.3/volstreet/angel_interface/access_rate_handlers.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/angel_interface/async_interface.py` & `volstreet-7.1.3/volstreet/angel_interface/async_interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/angel_interface/base_websocket.py` & `volstreet-7.1.3/volstreet/angel_interface/base_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/angel_interface/interface.py` & `volstreet-7.1.3/volstreet/angel_interface/interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/angel_interface/login.py` & `volstreet-7.1.3/volstreet/angel_interface/login.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/angel_interface/order_websocket.py` & `volstreet-7.1.3/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/angel_interface/price_websocket.py` & `volstreet-7.1.3/volstreet/angel_interface/price_websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import struct
 from datetime import datetime, timezone
 import itertools
 from collections import defaultdict
 from time import sleep
 from datetime import timedelta
+import threading
 from volstreet.config import token_symbol_dict, logger, token_exchange_dict
 from volstreet.utils import (
     current_time,
     get_symbol_token,
     strike_range_different,
     log_error,
 )
@@ -52,14 +53,15 @@
         correlation_id="default",
         webhook_url=None,
         default_strike_range=7,
     ):
         self.correlation_id = correlation_id
         self.webhook_url = webhook_url
         self.default_strike_range = default_strike_range
+        self.request_dict_lock = threading.Lock()
 
         super().__init__(auth_token, api_key, client_code, feed_token, manager)
 
         self.command_queue = manager.Queue()
         self.input_request_dict = manager.dict()
         self.underlying_options_subscribed = manager.dict()
         self.subscribed_to_options = False
@@ -69,17 +71,21 @@
     @staticmethod
     def processing_subscriptions(
         func,
     ):  # This decorator is used to avoid updating strike range while
         # subscription processes are running
         def wrapper(self, *args, **kwargs):
             self._processing_subscriptions = True
-            result = func(self, *args, **kwargs)
-            self._processing_subscriptions = False
-            return result
+            try:
+                self.request_dict_lock.acquire()
+                result = func(self, *args, **kwargs)
+                return result
+            finally:
+                self.request_dict_lock.release()
+                self._processing_subscriptions = False
 
         return wrapper
 
     @property
     def root_uri(self):
         return "wss://smartapisocket.angelone.in/smart-stream"
 
@@ -167,20 +173,23 @@
         payload = self._create_payload(tokens)
         self._subscribe(self.correlation_id, mode, payload)
 
     def unsubscribe(self, tokens: list, mode: int = 1):
         payload = self._create_payload(tokens)
         self._unsubscribe(self.correlation_id, mode, payload)
 
-    def get_current_usage(self):
-        return sum(
-            len(tokens) * mode
-            for mode, val in self.input_request_dict.items()
-            for _, tokens in val.items()
-        )
+    def get_current_usage(
+        self,
+    ):  # Our usage should be capped at 1000 (weighted) tokens.
+        with self.request_dict_lock:
+            return sum(
+                len(tokens) * mode
+                for mode, val in self.input_request_dict.items()
+                for _, tokens in val.items()
+            )
 
     def close_connection(self):
         self.intentionally_closed.value = True
         self.RESUBSCRIBE_FLAG = False
         if self.wsapp:
             self.wsapp.close()
             logger.info(f"{self.websocket_type} wsapp closed")
@@ -627,15 +636,20 @@
 
     def update_strike_range(self):
         for underlying in self.underlying_options_subscribed.keys():
             refreshed_strike_range = self.get_active_strike_range(underlying)
             current_strike_range = self.underlying_options_subscribed[underlying]
 
             if not strike_range_different(refreshed_strike_range, current_strike_range):
-                logger.info(f"Strike range for {underlying.name} is unchanged.")
+                current_usage = self.get_current_usage()
+                logger.info(
+                    f"Strike range for {underlying.name} is unchanged. Current usage is {current_usage}."
+                    f"Subscribed strike range: {current_strike_range}. "
+                    f"Refreshed strike range: {refreshed_strike_range}."
+                )
                 continue
 
             new_strikes = set(refreshed_strike_range) - set(current_strike_range)
             obsolete_strikes = set(current_strike_range) - set(refreshed_strike_range)
             if len(new_strikes) >= 0.4 * len(current_strike_range):  # Hardcoded 40%
                 logger.info(
                     f"New strike range for {underlying.name}: {refreshed_strike_range}. "
@@ -664,15 +678,15 @@
                 )
                 all_symbols_subscribed = [
                     token_symbol_dict[token] for token in all_tokens_subscribed
                 ]
                 all_symbols_unsubscribed = [
                     token_symbol_dict[token] for token in all_tokens_unsubscribed
                 ]
-                logger.debug(
+                logger.info(
                     f"{underlying.name} subscribed to: {all_symbols_subscribed} "
                     f"and unsubscribed from: {all_symbols_unsubscribed}"
                 )
 
     def periodically_execute_command_queue(self):
         while True and not self.intentionally_closed.value:
             try:
```

### Comparing `volstreet-7.1.2/volstreet/angel_interface/smart_connect.py` & `volstreet-7.1.3/volstreet/angel_interface/smart_connect.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/backtests/data_handling.py` & `volstreet-7.1.3/volstreet/backtests/data_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/backtests/database.py` & `volstreet-7.1.3/volstreet/backtests/database.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/backtests/delta_hedging.py` & `volstreet-7.1.3/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/backtests/delta_optimizer.py` & `volstreet-7.1.3/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/backtests/framework.py` & `volstreet-7.1.3/volstreet/backtests/framework.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-7.1.3/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/backtests/tools.py` & `volstreet-7.1.3/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/backtests/trend.py` & `volstreet-7.1.3/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/backtests/underlying_info.py` & `volstreet-7.1.3/volstreet/backtests/underlying_info.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/blackscholes.py` & `volstreet-7.1.3/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/config.py` & `volstreet-7.1.3/volstreet/config.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/database_connection.py` & `volstreet-7.1.3/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/datamodule/analysis.py` & `volstreet-7.1.3/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/datamodule/archive.py` & `volstreet-7.1.3/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/datamodule/eod_client.py` & `volstreet-7.1.3/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/datamodule/gambling.py` & `volstreet-7.1.3/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/datamodule/intraday_data.py` & `volstreet-7.1.3/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/datamodule/stockmock.py` & `volstreet-7.1.3/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/datamodule/trading_assistance.py` & `volstreet-7.1.3/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/dealingroom.py` & `volstreet-7.1.3/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/decorators.py` & `volstreet-7.1.3/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/discord_bot.py` & `volstreet-7.1.3/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/exceptions.py` & `volstreet-7.1.3/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/historical_info/index_expiries.pkl` & `volstreet-7.1.3/volstreet/historical_info/index_expiries.pkl`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/parallelization.py` & `volstreet-7.1.3/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/performance_tracking.py` & `volstreet-7.1.3/volstreet/performance_tracking.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/strategies/error_handling.py` & `volstreet-7.1.3/volstreet/strategies/error_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/strategies/execution.py` & `volstreet-7.1.3/volstreet/strategies/execution.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,27 @@
     @property
     @abstractmethod
     def to_divide_exposure(self) -> bool:
         pass
 
     @abstractmethod
     def initialize_indices(self, indices: Optional[list] = None) -> list[Index]:
-        pass
+        if indices:
+            notifier(
+                f"Trading {self.__class__.__name__} on {', '.join([index.name for index in indices])}.",
+                self.client_data.get("webhook_url"),
+                "INFO",
+            )
+        else:
+            notifier(
+                f"No indices to trade for {self.__class__.__name__}.",
+                self.client_data.get("webhook_url"),
+                "INFO",
+            )
+        return indices
 
     @abstractmethod
     def set_strategy_tags(
         self, strategy_tags: Optional[list[str] | str] = None
     ) -> list[str]:
         pass
 
@@ -189,15 +201,15 @@
                     final_parameters[index.name][tag].update(special_param)
         logger.info(
             f"Initializing {self.__class__.__name__} with parameters: {final_parameters}"
         )
         return final_parameters
 
     def run(self):
-        """This function will run the strategy and IMPORTANTLY block until all threads are finished."""
+        """This function will run the strategy. IMPORTANT: it will block until all threads are finished."""
 
         # Moved initialization methods here
         self.strategy_tags = self.set_strategy_tags(self._strategy_tags)
         self.indices_to_trade = self.initialize_indices(self._indices)
         self.parameters, self.special_parameters = self.set_parameters(
             self._parameters, self._special_parameters
         )
@@ -267,23 +279,26 @@
 class QuickStrangle(BaseStrategy):
     @property
     def strats(self):
         return [quick_strangle]
 
     @property
     def to_divide_exposure(self) -> bool:
-        return False
+        return True
 
     def set_strategy_tags(self, strategy_tags: Optional[list[str]] = None) -> list[str]:
         return strategy_tags or ["Quick Strangle"]
 
     def initialize_indices(self, indices: Optional[list] = None) -> list[Index]:
         indices = indices or ["NIFTY", "BANKNIFTY", "FINNIFTY", "MIDCPNIFTY", "SENSEX"]
         indices = [Index(index) for index in indices]
         indices: list[Index] | [] = get_strangle_indices_to_trade(*indices)
+        indices = super().initialize_indices(
+            indices
+        )  # This will notify about what indices are being traded
         return indices
 
 
 class IntradayStrangle(BaseStrategy):
     @property
     def strats(self):
         return [intraday_strangle]
@@ -295,20 +310,17 @@
     def set_strategy_tags(self, strategy_tags: Optional[list[str]] = None) -> list[str]:
         return strategy_tags or ["Intraday strangle"]
 
     def initialize_indices(self, indices: Optional[list] = None) -> list[Index]:
         indices = indices or ["NIFTY", "BANKNIFTY", "FINNIFTY", "MIDCPNIFTY", "SENSEX"]
         indices = [Index(index) for index in indices]
         indices: list[Index] | [] = get_strangle_indices_to_trade(*indices)
-        if indices:
-            notifier(
-                f"Trading strangle on {', '.join([index.name for index in indices])}.",
-                self.client_data.get("webhook_url"),
-                "INFO",
-            )
+        indices = super().initialize_indices(
+            indices
+        )  # This will notify about what indices are being traded
         return indices
 
 
 class IntradayTrend(BaseStrategy):
     @property
     def strats(self):
         return [intraday_trend]
@@ -320,15 +332,19 @@
     def set_strategy_tags(
         self, strategy_tags: Optional[list[str] | str] = None
     ) -> list[str]:
         return strategy_tags or ["Intraday trend"]
 
     def initialize_indices(self, indices: Optional[list] = None) -> list[Index]:
         indices = indices or ["NIFTY", "BANKNIFTY", "FINNIFTY"]
-        return [Index(index) for index in indices]
+        indices = [Index(index) for index in indices]
+        indices = super().initialize_indices(
+            indices
+        )  # This will notify about what indices are being traded
+        return indices
 
 
 class DeltaHedgedStrangle(BaseStrategy):
     @property
     def strats(self):
         return [delta_hedged_strangle]
 
@@ -338,32 +354,20 @@
 
     def set_strategy_tags(
         self, strategy_tags: Optional[list[str] | str] = None
     ) -> list[str]:
         return strategy_tags or ["Delta hedged strangle"]
 
     def initialize_indices(self, indices: Optional[list] = None) -> list[Index]:
-        if indices:
-            indices = [Index(index) for index in indices]
-        else:
-            indices = ["NIFTY", "BANKNIFTY", "FINNIFTY", "MIDCPNIFTY", "SENSEX"]
-            indices = [Index(index) for index in indices]
-            indices: list[Index] | [] = get_strangle_indices_to_trade(*indices)
-        if indices:
-            notifier(
-                f"Trading {self.__class__.__name__} on {', '.join([index.name for index in indices])}.",
-                self.client_data.get("webhook_url"),
-                "INFO",
-            )
-        else:
-            notifier(
-                f"No indices to trade for {self.__class__.__name__}.",
-                self.client_data.get("webhook_url"),
-                "INFO",
-            )
+        indices = indices or ["NIFTY", "BANKNIFTY", "FINNIFTY", "MIDCPNIFTY", "SENSEX"]
+        indices = [Index(index) for index in indices]
+        indices: list[Index] | [] = get_strangle_indices_to_trade(*indices)
+        indices = super().initialize_indices(
+            indices
+        )  # This will notify about what indices are being traded
         return indices
 
 
 class OvernightStraddle(BaseStrategy):
     """Since the overnight straddle is a combination of two strategies (main and hedge),
     the parameters should be a list of two dictionaries. The first dictionary will be used
     for the main strategy and the second dictionary will be used for the hedge strategy.
@@ -383,16 +387,20 @@
 
     def set_strategy_tags(
         self, strategy_tags: Optional[list[str] | str] = None
     ) -> list[str]:
         return strategy_tags or ["Weekly hedge", "Overnight short straddle"]
 
     def initialize_indices(self, indices: Optional[list] = None) -> list[Index]:
-        indices = indices or ["NIFTY"]
-        return [Index(index) for index in indices]
+        indices = indices or ["NIFTY", "BANKNIFTY"]
+        indices = [Index(index) for index in indices]
+        indices = super().initialize_indices(
+            indices
+        )  # This will notify about what indices are being traded
+        return indices
 
 
 class BiweeklyStraddle(BaseStrategy):
     """Since the biweekly straddle is a combination of two strategies (main and hedge),
     the parameters should be a list of two dictionaries. The first dictionary will be used
     for the main strategy and the second dictionary will be used for the hedge strategy.
 
@@ -412,15 +420,19 @@
     def set_strategy_tags(
         self, strategy_tags: Optional[list[str] | str] = None
     ) -> list[str]:
         return strategy_tags or ["Biweekly hedge", "Biweekly straddle"]
 
     def initialize_indices(self, indices: Optional[list] = None) -> list[Index]:
         indices = indices or ["NIFTY"]
-        return [Index(index) for index in indices]
+        indices = [Index(index) for index in indices]
+        indices = super().initialize_indices(
+            indices
+        )  # This will notify about what indices are being traded
+        return indices
 
 
 class Client:
     config_file = "client_config.json"
     strategy_function_map = {
         "quick_strangle": QuickStrangle,
         "intraday_strangle": IntradayStrangle,
```

### Comparing `volstreet-7.1.2/volstreet/strategies/helpers.py` & `volstreet-7.1.3/volstreet/strategies/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,27 +467,15 @@
             option.recommended_qty = 0
 
     def identify_prospective_options(
         self,
         range_of_strikes: int,
         options_with_cache: bool,
     ) -> tuple[list[ActiveOption], list[ActiveOption]]:
-        if (
-            LiveFeeds.price_feed_connected()
-            and self.underlying
-            in LiveFeeds.price_feed.underlying_options_subscribed.keys()
-        ):
-            logger.info(
-                f"{self.underlying.name} fetched prospective strikes from live feed"
-            )
-            strikes = LiveFeeds.price_feed.underlying_options_subscribed[
-                self.underlying
-            ]
-        else:
-            strikes = self.underlying.get_active_strikes(range_of_strikes)
+        strikes = self.underlying.get_active_strikes(range_of_strikes)
 
         self.cached_strikes = strikes
 
         return (
             [
                 ActiveOption(
                     strike=strike,
@@ -785,15 +773,15 @@
             )
 
         if not success_calls or not success_puts:
             self.set_recommended_qty_backup(
                 target_delta=target_delta + 0.1, attempt_no=attempt_no + 1
             )
 
-    def set_optimized_recommended_qty(self):
+    def set_optimized_recommended_qty(self, optimize_gamma: bool):
         self.reset_options()
         ivs = self.get_option_ivs(self.prospective_calls + self.prospective_puts)
         median_iv = np.nanmedian(ivs)
         logger.info(f"Using median IV {median_iv} for optimization")
         call_greeks = self.prepare_greek_frame_with_options(
             self.prospective_calls, True
         )
@@ -802,15 +790,15 @@
         # At this point all_greeks has the following columns:
         # [strike, ltp, delta, gamma, theta, vega, option]
 
         # Solving the optimization problem
 
         prob, weights = delta_neutral_optimization_lp(
             all_greeks[:, 2:6],
-            scale_gamma=True,
+            optimize_gamma=optimize_gamma,
             spot=self.underlying.fetch_ltp(),
             time_to_expiry=time_to_expiry(self.expiry),
             r=self.underlying.get_basis_for_expiry(self.expiry),
             iv=median_iv,
         )  # Using delta, gamma, theta, vega
 
         if prob.status != 1:
@@ -822,18 +810,20 @@
 
         # noinspection PyUnboundLocalVariable
         for option, weight in zip(all_greeks[:, -1], weights):
             option.recommended_qty = round_shares_to_lot_size(
                 weight * self.base_exposure_qty, option.lot_size
             )
 
-    def set_recommended_qty(self, target_delta: float, optimized: bool) -> None:
+    def set_recommended_qty(
+        self, target_delta: float, optimized: bool, optimize_gamma: bool
+    ) -> None:
         if optimized:
             try:
-                self.set_optimized_recommended_qty()
+                self.set_optimized_recommended_qty(optimize_gamma=optimize_gamma)
             except Exception as e:
                 notifier(
                     f"{self.underlying.name} Error while setting optimized recommended qty: {e}\n"
                     f"Using backup implementation\n"
                     f"Traceback: {e.__traceback__}",
                     self.notifier_url,
                     "ERROR",
```

### Comparing `volstreet-7.1.2/volstreet/strategies/optimization.py` & `volstreet-7.1.3/volstreet/strategies/optimization.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,20 @@
     gamma_value = gamma(spot, strike, time_to_expiry, r, iv)
     return gamma_value
 
 
 def generate_base_problem(
     greeks: np.ndarray, scale_gamma: bool = True
 ) -> tuple[LpProblem, dict]:
+    """
+    The base problem defines the weights for the options and variables.
+    Only quantity constraints are defined here.
+    """
+
+    g_scaler = 1
 
     if scale_gamma:
         # Gamma scaling
         # Minimum of the ratios of absolute-theta/gamma. Dividing by 4 just to keep it in check.
         # Preliminary study shows dividing does not matter all that much
         g_scaler = min(abs(greeks[:, 2]) / greeks[:, 1]) / 4
         logger.info(
@@ -114,94 +120,105 @@
             "deltas": put_deltas,
             "gammas": put_gammas,
             "thetas": put_thetas,
             "total_delta": put_total_delta,
             "total_theta": put_total_theta,
             "total_gamma": put_total_gamma,
         },
+        "gamma_scaler": g_scaler,
     }
 
     return prob, vars_dict
 
 
 def delta_neutral_optimization_lp(
-    greeks: np.ndarray, scale_gamma: bool = True, **simulation_inputs
+    greeks: np.ndarray, optimize_gamma: bool = True, **simulation_inputs
 ) -> tuple[LpProblem, np.ndarray]:
     """Required simulation inputs:
     spot: float
     iv: float
     time_to_expiry: float
     r: float
-    flag: str
-    target_delta: float
+    flag: str Optional
+    target_delta: float: Optional
     """
     # Check if all arguments to pass to the simulation function are present. Excluding the default ones
     simulation_args = signature(simulate_gamma_with_delta).parameters.keys()
     non_default_args = set(simulation_args) - {"flag", "target_delta"}
     if not non_default_args.issubset(set(simulation_inputs.keys())):
         raise ValueError(
             f"Simulation inputs are missing. Required inputs are: {non_default_args}"
         )
 
     logger.info(f"Starting delta neutral optimization for greeks: {greeks}")
 
+    scale_gamma = optimize_gamma
+
     prob, vars_dict = generate_base_problem(greeks, scale_gamma)
 
     call_total_delta = vars_dict["call"]["total_delta"]
     call_total_theta = vars_dict["call"]["total_theta"]
     call_total_gamma = vars_dict["call"]["total_gamma"]
 
     put_total_delta = vars_dict["put"]["total_delta"]
     put_total_theta = vars_dict["put"]["total_theta"]
     put_total_gamma = vars_dict["put"]["total_gamma"]
 
     # Set objective function
-    prob += lpSum(
-        [(call_total_theta + put_total_theta), (call_total_gamma + put_total_gamma)]
-    )
+    if optimize_gamma:
+        logger.info("Optimizing theta and gamma.")
+        prob += lpSum(
+            [(call_total_theta + put_total_theta), (call_total_gamma + put_total_gamma)]
+        )
+    else:
+        logger.info("Optimizing only theta.")
+        prob += lpSum([call_total_theta, put_total_theta])
 
     # Add constraints
 
     # DELTA CONSTRAINTS
     prob += lpSum([call_total_delta, put_total_delta]) <= 0.005  # Delta constraint
     prob += lpSum([call_total_delta, put_total_delta]) >= -0.005  # Delta constraint
 
     # THETA POSITIVE AND GAMMA NEGATIVE
     prob += lpSum([call_total_theta, put_total_theta]) >= 0  # Theta constraint
     prob += lpSum([call_total_gamma, put_total_gamma]) <= 0  # Gamma constraint
 
     # GAMMA THRESHOLD PERFORMANCE
-
+    g_scaler = vars_dict["gamma_scaler"]
     gamma_threshold = simulate_gamma_with_delta(**simulation_inputs)
     # Negative because we want to mimic a short position
     # And double because we would sell call and put
     total_threshold = gamma_threshold * -2
     logger.info(
-        f"Using single side gamma threshold: {gamma_threshold} as performance target. "
-        f"Total threshold: {total_threshold}"
+        f"Using single side gamma threshold: {gamma_threshold} as performance target (before scaling). "
+        f"Total threshold: {total_threshold}. "
+        f"Scaled gamma threshold: {total_threshold * g_scaler} "
     )
 
-    # We should try to outperform the 25th percentile gamma
-    prob += lpSum([call_total_gamma, put_total_gamma]) >= total_threshold
+    # We should try to outperform the gamma threshold
+    prob += lpSum([call_total_gamma, put_total_gamma]) >= (total_threshold * g_scaler)
 
     # Solve the problem
     prob.solve()
 
     call_weights = np.array([v.varValue for v in vars_dict["call"]["weights"]])
     put_weights = np.array([v.varValue for v in vars_dict["put"]["weights"]])
 
     combined_weights = np.concatenate([call_weights, put_weights])
 
     logger.info(
         f"Status of optimization: {LpStatus[prob.status]}, "
         f"Objective value: {value(prob.objective)}. "
-        f"Call Delta, Theta, Gamma: {value(call_total_delta)}, {value(call_total_theta)}, {value(call_total_gamma)}. "
-        f"Put Delta, Theta, Gamma: {value(put_total_delta)}, {value(put_total_theta)}, {value(put_total_gamma)}. "
+        f"Call Delta, Theta, Gamma: "
+        f"{value(call_total_delta)}, {value(call_total_theta)}, {value(call_total_gamma)/g_scaler}. "
+        f"Put Delta, Theta, Gamma: "
+        f"{value(put_total_delta)}, {value(put_total_theta)}, {value(put_total_gamma)/g_scaler}. "
         f"Total Delta, Theta, Gamma: {value(call_total_delta + put_total_delta)}, "
-        f"{value(call_total_theta + put_total_theta)}, {value(call_total_gamma + put_total_gamma)}"
+        f"{value(call_total_theta + put_total_theta)}, {value(call_total_gamma + put_total_gamma)/g_scaler}"
     )
 
     return prob, combined_weights
 
 
 def generate_constraints(
     deltas: np.ndarray,
```

### Comparing `volstreet-7.1.2/volstreet/strategies/strats.py` & `volstreet-7.1.3/volstreet/strategies/strats.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,25 +281,29 @@
 
 @exit_on_error
 @increase_robustness
 def delta_hedged_strangle(
     underlying: Index | Stock,
     exposure: int | float,
     tracking_strikes: int,
-    target_delta: float,
+    target_delta: float = 0.1,
     optimized: bool = False,
+    optimize_gamma: bool = False,
+    theta_time_jump_hours: float = 1,  # In hours
     delta_interval_minutes: int | float = 1,
-    delta_threshold_pct: float = 0.02,
+    delta_threshold_pct: float = 0.04,
     hedge_margin: float | None = None,  # eg 0.2
     exit_time: Optional[tuple] = (15, 29),
     use_cache: Optional[bool] = True,
     notification_url: Optional[str] = None,
     strategy_tag: Optional[str] = "Delta hedged strangle",
 ):
-    """Strangle with continuous delta hedging."""
+    """Theta time jump is defined in hours. Delta interval is in minutes. Delta threshold is in percentage terms
+    eg: 0.02 for 2%
+    """
 
     # Setting the exposure
     start_time = current_time()
     if hedge_margin is None:
         base_exposure = exposure
     else:
         base_exposure = exposure / (1 + hedge_margin)
@@ -333,29 +337,30 @@
         f"delta threshold: {delta_threshold}. "
     )
     notifier(starting_message, notification_url, "INFO")
 
     delta_position: DeltaPosition = DeltaPosition(
         underlying=underlying,
         base_exposure_qty=base_qty_shares,
+        greek_settings={"theta_time_jump": theta_time_jump_hours / (365 * 24)},
         order_tag=strategy_tag,
         notifier_url=notification_url,
     )
     while current_time().time() < time(*exit_time):
         if delta_position.cached_strikes is None or strike_range_different(
             underlying.get_active_strikes(tracking_strikes),
             delta_position.cached_strikes,
         ):
             delta_position.update_prospective_options(tracking_strikes, use_cache)
             logger.info(
                 f"{current_time()} {underlying.name} set active options and set "
                 f"{len(delta_position.all_options)} prospective options"
             )
         delta_position.update_underlying()
-        delta_position.set_recommended_qty(target_delta, optimized)
+        delta_position.set_recommended_qty(target_delta, optimized, optimize_gamma)
         delta_position.adjust_recommended_qty()
         delta_position.enter_positions()
         delta_position.reset_trigger_flags()
 
         def interruption_condition():
             # Hard coded 7% of base qty shares as the threshold for interruption
             condition_1 = (
@@ -1941,25 +1946,29 @@
                         "quantity_in_lots": quantity_in_lots,
                         "order_tag": strategy_tag,
                     }
                 }
             )
             call_avg_price, put_avg_price = execution_details[position.instrument]
 
-            logger.info(
-                f"Entered {underlying.name} {position.instrument} with avg price {call_avg_price + put_avg_price}"
+            notifier(
+                f"Entered {underlying.name} {strategy_tag} on {position.instrument} "
+                f"with avg price {call_avg_price + put_avg_price}",
+                notification_url,
+                "INFO",
             )
             position.initiating_price = call_avg_price + put_avg_price
             break
 
         sleep(0.1)
 
     if not position.position_active:
-        logger.info(
+        notifier(
             f"{underlying.name} {strategy_tag} not triggered. Exiting.",
+            notification_url,
         )
         return
 
     if position.position_active:
         position.profit_threshold = position.initiating_price * (
             1 + (take_profit * action.num_value)
         )
@@ -1972,21 +1981,23 @@
             )
             total_current_price = current_call_price + current_put_price
             logger.info(
                 f"{underlying.name} {strategy_tag} Current price: {total_current_price} "
                 f"Target price: {position.profit_threshold} Stop loss price: {position.stop_loss_threshold}"
             )
             if profit_condition():
-                logger.info(
-                    f"{underlying.name} {strategy_tag} profit triggered. Exiting."
+                notifier(
+                    f"{underlying.name} {strategy_tag} profit triggered. Exiting.",
+                    notification_url,
                 )
                 break
             if stop_loss_condition():
-                logger.info(
-                    f"{underlying.name} {strategy_tag} stop loss triggered. Exiting."
+                notifier(
+                    f"{underlying.name} {strategy_tag} stop loss triggered. Exiting.",
+                    notification_url,
                 )
                 break
 
             sleep(0.1)
 
         # noinspection PyUnboundLocalVariable
         execution_details = execute_instructions(
@@ -1997,16 +2008,17 @@
                     "order_tag": strategy_tag,
                 }
             }
         )
         call_exit_price, put_exit_price = execution_details[position.instrument]
         exit_price = call_exit_price + put_exit_price
         profit_points = (exit_price - position.initiating_price) * action.num_value
-        logger.info(
+        notifier(
             f"Exited {underlying.name} {strategy_tag} with profit points {profit_points}",
+            notification_url,
         )
 
 
 @exit_on_error
 @increase_robustness
 def intraday_trend(
     underlying: Index | Stock,
```

### Comparing `volstreet-7.1.2/volstreet/trade_interface/instruments.py` & `volstreet-7.1.3/volstreet/trade_interface/instruments.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/trade_interface/order_execution.py` & `volstreet-7.1.3/volstreet/trade_interface/order_execution.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/trade_interface/order_placement.py` & `volstreet-7.1.3/volstreet/trade_interface/order_placement.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/trade_interface/underlyings.py` & `volstreet-7.1.3/volstreet/trade_interface/underlyings.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/utils/change_config.py` & `volstreet-7.1.3/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/utils/communication.py` & `volstreet-7.1.3/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/utils/core.py` & `volstreet-7.1.3/volstreet/utils/core.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/utils/data_io.py` & `volstreet-7.1.3/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/utils/scrip_processing.py` & `volstreet-7.1.3/volstreet/utils/scrip_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/vectorized_blackscholes.py` & `volstreet-7.1.3/volstreet/vectorized_blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/vslogging/formatters.py` & `volstreet-7.1.3/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/vslogging/logging_config.json` & `volstreet-7.1.3/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/vslogging/logging_setup.py` & `volstreet-7.1.3/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet/vslogging/parsing.py` & `volstreet-7.1.3/volstreet/vslogging/parsing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.2/volstreet.egg-info/PKG-INFO` & `volstreet-7.1.3/volstreet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.1.2
+Version: 7.1.3
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.1.2/volstreet.egg-info/SOURCES.txt` & `volstreet-7.1.3/volstreet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

