# Comparing `tmp/finazon_grpc_python-1.0.141.tar.gz` & `tmp/finazon_grpc_python-1.0.146.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finazon_grpc_python-1.0.141.tar", max compression
+gzip compressed data, was "finazon_grpc_python-1.0.146.tar", max compression
```

## Comparing `finazon_grpc_python-1.0.141.tar` & `finazon_grpc_python-1.0.146.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1064 2024-02-13 20:32:42.949886 finazon_grpc_python-1.0.141/LICENSE.txt
--rw-r--r--   0        0        0    10159 2024-03-04 14:48:33.533986 finazon_grpc_python-1.0.141/README.md
--rw-r--r--   0        0        0        0 2024-02-28 07:42:52.990282 finazon_grpc_python-1.0.141/finazon_grpc_python/__init__.py
--rw-r--r--   0        0        0     1997 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/api_usage_pb2.py
--rw-r--r--   0        0        0     2977 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/api_usage_pb2.pyi
--rw-r--r--   0        0        0     2715 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/api_usage_pb2_grpc.py
--rw-r--r--   0        0        0      504 2024-04-01 10:30:58.049306 finazon_grpc_python-1.0.141/finazon_grpc_python/api_usage_service.py
--rw-r--r--   0        0        0     9699 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_pb2.py
--rw-r--r--   0        0        0    27137 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_pb2.pyi
--rw-r--r--   0        0        0     7871 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_pb2_grpc.py
--rw-r--r--   0        0        0     1175 2024-04-01 10:30:57.909306 finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_service.py
--rw-r--r--   0        0        0     2456 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/binance_pb2.py
--rw-r--r--   0        0        0     4188 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/binance_pb2.pyi
--rw-r--r--   0        0        0     2769 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/binance_pb2_grpc.py
--rw-r--r--   0        0        0      537 2024-04-01 10:30:58.029306 finazon_grpc_python-1.0.141/finazon_grpc_python/binance_service.py
--rw-r--r--   0        0        0        0 2024-02-27 14:37:50.723171 finazon_grpc_python-1.0.141/finazon_grpc_python/common/__init__.py
--rw-r--r--   0        0        0     1786 2024-02-28 12:02:26.373203 finazon_grpc_python-1.0.141/finazon_grpc_python/common/client.py
--rw-r--r--   0        0        0      496 2024-02-28 12:00:04.869646 finazon_grpc_python-1.0.141/finazon_grpc_python/common/errors.py
--rw-r--r--   0        0        0      177 2024-04-01 10:30:50.613342 finazon_grpc_python-1.0.141/finazon_grpc_python/common/settings.py
--rw-r--r--   0        0        0     1966 2024-03-04 14:05:10.294573 finazon_grpc_python-1.0.141/finazon_grpc_python/common/utils.py
--rw-r--r--   0        0        0     2225 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_pb2.py
--rw-r--r--   0        0        0     3411 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_pb2.pyi
--rw-r--r--   0        0        0     2737 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_pb2_grpc.py
--rw-r--r--   0        0        0      528 2024-04-01 10:30:58.041306 finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_service.py
--rw-r--r--   0        0        0     1787 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/datasets_pb2.py
--rw-r--r--   0        0        0     2208 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/datasets_pb2.pyi
--rw-r--r--   0        0        0     2718 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/datasets_pb2_grpc.py
--rw-r--r--   0        0        0      501 2024-04-01 10:30:58.053305 finazon_grpc_python-1.0.141/finazon_grpc_python/datasets_service.py
--rw-r--r--   0        0        0        0 2024-02-13 20:32:42.949886 finazon_grpc_python-1.0.141/finazon_grpc_python/examples/__init__.py
--rw-r--r--   0        0        0      627 2024-03-04 14:34:47.300646 finazon_grpc_python-1.0.141/finazon_grpc_python/examples/indicator_atr.py
--rw-r--r--   0        0        0      598 2024-03-04 14:22:48.014704 finazon_grpc_python-1.0.141/finazon_grpc_python/examples/indicator_ma.py
--rw-r--r--   0        0        0      689 2024-03-04 14:25:40.473576 finazon_grpc_python-1.0.141/finazon_grpc_python/examples/indicator_ma_pandas.py
--rw-r--r--   0        0        0      489 2024-02-28 13:49:10.731115 finazon_grpc_python-1.0.141/finazon_grpc_python/examples/tickers.py
--rw-r--r--   0        0        0      635 2024-03-04 14:29:59.652016 finazon_grpc_python-1.0.141/finazon_grpc_python/examples/time_series.py
--rw-r--r--   0        0        0      619 2024-03-04 14:14:13.758535 finazon_grpc_python-1.0.141/finazon_grpc_python/examples/time_series_pandas.py
--rw-r--r--   0        0        0     2790 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_pb2.py
--rw-r--r--   0        0        0     4502 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_pb2.pyi
--rw-r--r--   0        0        0     4553 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_pb2_grpc.py
--rw-r--r--   0        0        0      771 2024-04-01 10:30:57.949306 finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_service.py
--rw-r--r--   0        0        0     2181 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/forex_pb2.py
--rw-r--r--   0        0        0     3276 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/forex_pb2.pyi
--rw-r--r--   0        0        0     2713 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/forex_pb2_grpc.py
--rw-r--r--   0        0        0      519 2024-04-01 10:30:57.893306 finazon_grpc_python-1.0.141/finazon_grpc_python/forex_service.py
--rw-r--r--   0        0        0     1805 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_pb2.py
--rw-r--r--   0        0        0     2230 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_pb2.pyi
--rw-r--r--   0        0        0     2778 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_pb2_grpc.py
--rw-r--r--   0        0        0      520 2024-04-01 10:30:58.061306 finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_service.py
--rw-r--r--   0        0        0     2634 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/sec_pb2.py
--rw-r--r--   0        0        0     5228 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/sec_pb2.pyi
--rw-r--r--   0        0        0     2711 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/sec_pb2_grpc.py
--rw-r--r--   0        0        0      486 2024-04-01 10:30:58.037306 finazon_grpc_python-1.0.141/finazon_grpc_python/sec_service.py
--rw-r--r--   0        0        0     3172 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/sip_pb2.py
--rw-r--r--   0        0        0     6003 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/sip_pb2.pyi
--rw-r--r--   0        0        0     4372 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/sip_pb2_grpc.py
--rw-r--r--   0        0        0      716 2024-04-01 10:30:57.921306 finazon_grpc_python-1.0.141/finazon_grpc_python/sip_service.py
--rw-r--r--   0        0        0     3629 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/snapshot_pb2.py
--rw-r--r--   0        0        0     7809 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/snapshot_pb2.pyi
--rw-r--r--   0        0        0     2822 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/snapshot_pb2_grpc.py
--rw-r--r--   0        0        0      501 2024-04-01 10:30:58.025306 finazon_grpc_python-1.0.141/finazon_grpc_python/snapshot_service.py
--rw-r--r--   0        0        0     5421 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_pb2.py
--rw-r--r--   0        0        0    11952 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_pb2.pyi
--rw-r--r--   0        0        0     8214 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_pb2_grpc.py
--rw-r--r--   0        0        0     1223 2024-04-01 10:30:57.937306 finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_service.py
--rw-r--r--   0        0        0    11776 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_pb2.py
--rw-r--r--   0        0        0    28018 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_pb2.pyi
--rw-r--r--   0        0        0    19109 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_pb2_grpc.py
--rw-r--r--   0        0        0     2765 2024-04-01 10:30:58.017306 finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_service.py
--rw-r--r--   0        0        0     2382 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/trade_pb2.py
--rw-r--r--   0        0        0     4295 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/trade_pb2.pyi
--rw-r--r--   0        0        0     2630 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/trade_pb2_grpc.py
--rw-r--r--   0        0        0      474 2024-04-01 10:30:57.953306 finazon_grpc_python-1.0.141/finazon_grpc_python/trade_service.py
--rw-r--r--   0        0        0      813 2024-04-01 10:30:50.609342 finazon_grpc_python-1.0.141/pyproject.toml
--rw-r--r--   0        0        0      443 2024-03-04 13:57:04.928973 finazon_grpc_python-1.0.141/requirements.txt
--rw-r--r--   0        0        0    11039 1970-01-01 00:00:00.000000 finazon_grpc_python-1.0.141/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-12 09:26:00.781227 finazon_grpc_python-1.0.146/LICENSE.txt
+-rw-r--r--   0        0        0    13306 2024-04-12 09:26:01.001277 finazon_grpc_python-1.0.146/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 09:26:00.781227 finazon_grpc_python-1.0.146/finazon_grpc_python/__init__.py
+-rw-r--r--   0        0        0     2030 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/api_usage_pb2.py
+-rw-r--r--   0        0        0     2776 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/api_usage_pb2.pyi
+-rw-r--r--   0        0        0     2715 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/api_usage_pb2_grpc.py
+-rw-r--r--   0        0        0      504 2024-04-12 09:27:56.559063 finazon_grpc_python-1.0.146/finazon_grpc_python/api_usage_service.py
+-rw-r--r--   0        0        0     9732 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_pb2.py
+-rw-r--r--   0        0        0    26705 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_pb2.pyi
+-rw-r--r--   0        0        0     7871 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_pb2_grpc.py
+-rw-r--r--   0        0        0     1175 2024-04-12 09:27:56.399119 finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_service.py
+-rw-r--r--   0        0        0     2485 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/binance_pb2.py
+-rw-r--r--   0        0        0     3890 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/binance_pb2.pyi
+-rw-r--r--   0        0        0     2769 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/binance_pb2_grpc.py
+-rw-r--r--   0        0        0      537 2024-04-12 09:27:56.539070 finazon_grpc_python-1.0.146/finazon_grpc_python/binance_service.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/common/__init__.py
+-rw-r--r--   0        0        0     1786 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/common/client.py
+-rw-r--r--   0        0        0      496 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/common/errors.py
+-rw-r--r--   0        0        0      177 2024-04-12 09:26:01.037285 finazon_grpc_python-1.0.146/finazon_grpc_python/common/settings.py
+-rw-r--r--   0        0        0     1966 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/common/utils.py
+-rw-r--r--   0        0        0     2254 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_pb2.py
+-rw-r--r--   0        0        0     3113 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_pb2.pyi
+-rw-r--r--   0        0        0     2737 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_pb2_grpc.py
+-rw-r--r--   0        0        0      528 2024-04-12 09:27:56.551066 finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_service.py
+-rw-r--r--   0        0        0     1820 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/datasets_pb2.py
+-rw-r--r--   0        0        0     2040 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/datasets_pb2.pyi
+-rw-r--r--   0        0        0     2718 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/datasets_pb2_grpc.py
+-rw-r--r--   0        0        0      501 2024-04-12 09:27:56.563061 finazon_grpc_python-1.0.146/finazon_grpc_python/datasets_service.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/examples/__init__.py
+-rw-r--r--   0        0        0      627 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/examples/indicator_atr.py
+-rw-r--r--   0        0        0      598 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/examples/indicator_ma.py
+-rw-r--r--   0        0        0      689 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/examples/indicator_ma_pandas.py
+-rw-r--r--   0        0        0      489 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/examples/tickers.py
+-rw-r--r--   0        0        0      635 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/examples/time_series.py
+-rw-r--r--   0        0        0      619 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/examples/time_series_pandas.py
+-rw-r--r--   0        0        0     2823 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_pb2.py
+-rw-r--r--   0        0        0     4268 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_pb2.pyi
+-rw-r--r--   0        0        0     4553 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_pb2_grpc.py
+-rw-r--r--   0        0        0      771 2024-04-12 09:27:56.451100 finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_service.py
+-rw-r--r--   0        0        0     2210 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/forex_pb2.py
+-rw-r--r--   0        0        0     2978 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/forex_pb2.pyi
+-rw-r--r--   0        0        0     2713 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/forex_pb2_grpc.py
+-rw-r--r--   0        0        0      519 2024-04-12 09:27:56.375127 finazon_grpc_python-1.0.146/finazon_grpc_python/forex_service.py
+-rw-r--r--   0        0        0     1838 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_pb2.py
+-rw-r--r--   0        0        0     2062 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_pb2.pyi
+-rw-r--r--   0        0        0     2778 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_pb2_grpc.py
+-rw-r--r--   0        0        0      520 2024-04-12 09:27:56.571058 finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_service.py
+-rw-r--r--   0        0        0     2667 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/sec_pb2.py
+-rw-r--r--   0        0        0     5038 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/sec_pb2.pyi
+-rw-r--r--   0        0        0     2711 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/sec_pb2_grpc.py
+-rw-r--r--   0        0        0      486 2024-04-12 09:27:56.543068 finazon_grpc_python-1.0.146/finazon_grpc_python/sec_service.py
+-rw-r--r--   0        0        0     3205 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/sip_pb2.py
+-rw-r--r--   0        0        0     5780 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/sip_pb2.pyi
+-rw-r--r--   0        0        0     4372 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/sip_pb2_grpc.py
+-rw-r--r--   0        0        0      716 2024-04-12 09:27:56.411115 finazon_grpc_python-1.0.146/finazon_grpc_python/sip_service.py
+-rw-r--r--   0        0        0     3662 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/snapshot_pb2.py
+-rw-r--r--   0        0        0     7564 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/snapshot_pb2.pyi
+-rw-r--r--   0        0        0     2822 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/snapshot_pb2_grpc.py
+-rw-r--r--   0        0        0      501 2024-04-12 09:27:56.531072 finazon_grpc_python-1.0.146/finazon_grpc_python/snapshot_service.py
+-rw-r--r--   0        0        0     5454 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_pb2.py
+-rw-r--r--   0        0        0    11586 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_pb2.pyi
+-rw-r--r--   0        0        0     8214 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_pb2_grpc.py
+-rw-r--r--   0        0        0     1223 2024-04-12 09:27:56.439105 finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_service.py
+-rw-r--r--   0        0        0    11805 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_pb2.py
+-rw-r--r--   0        0        0    27027 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_pb2.pyi
+-rw-r--r--   0        0        0    19109 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_pb2_grpc.py
+-rw-r--r--   0        0        0     2765 2024-04-12 09:27:56.527074 finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_service.py
+-rw-r--r--   0        0        0     2415 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/trade_pb2.py
+-rw-r--r--   0        0        0     4127 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/trade_pb2.pyi
+-rw-r--r--   0        0        0     2630 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/trade_pb2_grpc.py
+-rw-r--r--   0        0        0      474 2024-04-12 09:27:56.459098 finazon_grpc_python-1.0.146/finazon_grpc_python/trade_service.py
+-rw-r--r--   0        0        0      815 2024-04-12 09:26:01.037285 finazon_grpc_python-1.0.146/pyproject.toml
+-rw-r--r--   0        0        0      443 2024-04-12 09:26:00.789229 finazon_grpc_python-1.0.146/requirements.txt
+-rw-r--r--   0        0        0    14200 1970-01-01 00:00:00.000000 finazon_grpc_python-1.0.146/PKG-INFO
```

### Comparing `finazon_grpc_python-1.0.141/LICENSE.txt` & `finazon_grpc_python-1.0.146/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/README.md` & `finazon_grpc_python-1.0.146/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 - Lists of datasets, publishers, markets, and tickers.
 - Market data: ticker snapshots, time series, trades, and technical indicators.
 - Data from specific datasets such as Benzinga, Binance, Crypto, Forex, SEC, and SIP.
 
 🔑 **API key** is essential. If you haven't got one yet, [sign up here](https://finazon.io/).
 
 ## Requirements
-Ensure you have Python 3.9 or later. 
+Ensure you have Python 3.9 or later.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Finazon Python gRPC Client library:
 ```shell
 pip install finazon-grpc-python
 ```
@@ -146,53 +146,51 @@
     print(response.result)
 except FinazonGrpcRequestError as e:
     print(f'Received error, code: {e.code}, message: {e.message}')
 ```
 
 👀 Check the full example and other examples [here](https://github.com/finazon-io/finazon-grpc-python/tree/main/finazon_grpc_python/examples)
 
-
 ## RPC support
 
 The following table outlines the supported rpc calls:
-<!--rpc_table_boundary-->
-| Service              | rpc                       | Description                                        |
-|----------------------|---------------------------|----------------------------------------------------|
-| ApiUsageService      | get_api_usage             | Get a list of products with quota limit/usage      |
-| BenzingaService      | get_dividents_calendar    | Returns the dividends calendar from Benzinga       |
-| BenzingaService      | get_earnings_calendar     | Returns the earnings calendar from Benzinga        |
-| BenzingaService      | get_news                  | Returns the news articles from Benzinga            |
-| BenzingaService      | get_ipo                   | Returns IPO data from Benzinga                     |
-| BinanceService       | get_time_series           | Get time series data without technical indicators  |
-| CryptoService        | get_time_series           | Get time series data for any given ticker          |
-| DatasetsService      | get_datasets              | Get a list of all datasets available at Finazon    |
-| ExchangeService      | get_markets_crypto        | Returns a list of supported crypto markets         |
-| ExchangeService      | get_markets_stocks        | Returns a list of supported stock markets          |
-| ForexService         | get_time_series           | Get time series data for any given ticker          |
-| PublisherService     | get_publishers            | Get a list of all publishers available at Finazon  |
-| SecService           | get_filings               | Real-time and historical access to all forms, filings, and exhibits directly from the SEC's EDGAR system |
-| SipService           | get_trades                | Returns detailed information on trades executed through the Securities Information Processor (SIP) |
-| SipService           | get_market_center         | Returns a list of market centers                   |
-| SnapshotService      | get_snapshot              | This endpoint returns a combination of different data points, such as daily performance, last quote, last trade, minute data, and previous day performance |
-| TickersService       | find_tickers_stocks       | This API call returns an array of stocks tickers available at Finazon Data API. This list is updated daily |
-| TickersService       | find_tickers_crypto       | This API call returns an array of crypto tickers available at Finazon Data API. This list is updated daily |
-| TickersService       | find_tickers_forex        | This API call returns an array of forex tickers available at Finazon Data API. This list is updated daily |
-| TickersService       | find_ticker_us            | This API call returns an array of US tickers available at Finazon Data API. This list is updated daily |
-| TimeSeriesService    | get_time_series           | Get time series data without technical indicators  |
-| TimeSeriesService    | get_time_series_atr       | Get time series data for ATR technical indicator   |
-| TimeSeriesService    | get_time_series_b_bands   | Get time series data for BBands technical indicator |
-| TimeSeriesService    | get_time_series_ichimoku  | Get time series data for Ichimoku technical indicator |
-| TimeSeriesService    | get_time_series_ma        | Get time series data for Ma technical indicator    |
-| TimeSeriesService    | get_time_series_macd      | Get time series data for Macd technical indicator  |
-| TimeSeriesService    | get_time_series_obv       | Get time series data for Obv technical indicator   |
-| TimeSeriesService    | get_time_series_rsi       | Get time series data for Rsi technical indicator   |
-| TimeSeriesService    | get_time_series_sar       | Get time series data for Sar technical indicator   |
-| TimeSeriesService    | get_time_series_stoch     | Get time series data for Stoch technical indicator |
-| TradeService         | get_trades                | Returns general information on executed trades     |
-<!--rpc_table_boundary-->
+|Service                |rpc                        |Description                                                                                                                                                      |
+|-----------------------|---------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| ApiUsageService       | getApiUsage               | Get a list of products with quota limit/usage                                                                                                                   |
+| BenzingaService       | getDividentsCalendar      | Returns the dividends calendar from Benzinga                                                                                                                    |
+| BenzingaService       | getEarningsCalendar       | Returns the earnings calendar from Benzinga                                                                                                                     |
+| BenzingaService       | getNews                   | Returns the news articles from Benzinga                                                                                                                         |
+| BenzingaService       | getIPO                    | Returns IPO data from Benzinga                                                                                                                                  |
+| BinanceService        | getTimeSeries             | Get time series data without technical indicators                                                                                                               |
+| CryptoService         | getTimeSeries             | Get time series data for any given ticker                                                                                                                       |
+| DatasetsService       | getDatasets               | Get a list of all datasets available at Finazon.                                                                                                                |
+| ExchangeService       | getMarketsCrypto          | Returns a list of supported crypto markets                                                                                                                      |
+| ExchangeService       | getMarketsStocks          | Returns a list of supported stock markets                                                                                                                       |
+| ForexService          | getTimeSeries             | Get time series data for any given ticker                                                                                                                       |
+| PublisherService      | getPublishers             | Get a list of all publishers available at Finazon.                                                                                                              |
+| SecService            | getFilings                | Real-time and historical access to all forms, filings, and exhibits directly from the SEC's EDGAR system.                                                       |
+| SipService            | getTrades                 | Returns detailed information on trades executed through the Securities Information Processor (SIP)                                                              |
+| SipService            | getMarketCenter           | Returns a list of market centers                                                                                                                                |
+| SnapshotService       | getSnapshot               | This endpoint returns a combination of different data points, such as daily performance, last quote, last trade, minute data, and previous day performance.     |
+| TickersService        | findTickersStocks         | This API call returns an array of stocks tickers available at Finazon Data API. This list is updated daily.                                                     |
+| TickersService        | findTickersCrypto         | This API call returns an array of crypto tickers available at Finazon Data API. This list is updated daily.                                                     |
+| TickersService        | findTickersForex          | This API call returns an array of forex tickers available at Finazon Data API. This list is updated daily.                                                      |
+| TickersService        | findTickerUS              | This API call returns an array of US tickers available at Finazon Data API. This list is updated daily.                                                         |
+| TimeSeriesService     | getTimeSeries             | Get time series data without technical indicators                                                                                                               |
+| TimeSeriesService     | getTimeSeriesAtr          | Get time series data for ATR technical indicator.                                                                                                               |
+| TimeSeriesService     | getTimeSeriesBBands       | Get time series data for BBands technical indicator.                                                                                                            |
+| TimeSeriesService     | getTimeSeriesIchimoku     | Get time series data for Ichimoku technical indicator.                                                                                                          |
+| TimeSeriesService     | getTimeSeriesMa           | Get time series data for Ma technical indicator.                                                                                                                |
+| TimeSeriesService     | getTimeSeriesMacd         | Get time series data for Macd technical indicator.                                                                                                              |
+| TimeSeriesService     | getTimeSeriesObv          | Get time series data for Obv technical indicator.                                                                                                               |
+| TimeSeriesService     | getTimeSeriesRsi          | Get time series data for Rsi technical indicator.                                                                                                               |
+| TimeSeriesService     | getTimeSeriesSar          | Get time series data for Sar technical indicator.                                                                                                               |
+| TimeSeriesService     | getTimeSeriesStoch        | Get time series data for Stoch technical indicator.                                                                                                             |
+| TradeService          | getTrades                 | Returns general information on executed trades                                                                                                                  |
+
 Here's how you can import `service` and `request` objects:
 
 ```python
 from finazon_grpc_python.service_name_service import ServiceNameService, RpcNameRequest
 
 # ...
 
@@ -221,8 +219,8 @@
 3. Commit changes and test.
 4. Push your branch and open a pull request with a comprehensive description.
 
 For more guidance on contributing, see the [GitHub Docs](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) on GitHub.
 
 ## License
 
-This project is licensed under the MIT License. See the `LICENSE.txt` file in this repository for more details.
+This project is licensed under the MIT License. See the `LICENSE.txt` file in this repository for more details.
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/api_usage_pb2.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/api_usage_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: finazon_grpc_python/api_usage.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,15 +16,14 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#finazon_grpc_python/api_usage.proto\x12\x07\x66inazon\"s\n\x0c\x41piUsageItem\x12\x0f\n\x07product\x18\x01 \x01(\t\x12#\n\x08\x61piCalls\x18\x02 \x01(\x0b\x32\x11.finazon.ApiCalls\x12-\n\x12historicalApiCalls\x18\x03 \x01(\x0b\x32\x11.finazon.ApiCalls\"(\n\x08\x41piCalls\x12\r\n\x05limit\x18\x01 \x01(\x05\x12\r\n\x05usage\x18\x02 \x01(\x05\"%\n\x12GetApiUsageRequest\x12\x0f\n\x07product\x18\x01 \x01(\t\"<\n\x13GetApiUsageResponse\x12%\n\x06result\x18\x01 \x03(\x0b\x32\x15.finazon.ApiUsageItem2]\n\x0f\x41piUsageService\x12J\n\x0bGetApiUsage\x12\x1b.finazon.GetApiUsageRequest\x1a\x1c.finazon.GetApiUsageResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.api_usage_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_APIUSAGEITEM']._serialized_start=48
   _globals['_APIUSAGEITEM']._serialized_end=163
   _globals['_APICALLS']._serialized_start=165
   _globals['_APICALLS']._serialized_end=205
   _globals['_GETAPIUSAGEREQUEST']._serialized_start=207
   _globals['_GETAPIUSAGEREQUEST']._serialized_end=244
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/api_usage_pb2.pyi` & `finazon_grpc_python-1.0.146/finazon_grpc_python/api_usage_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class ApiUsageItem(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PRODUCT_FIELD_NUMBER: builtins.int
     APICALLS_FIELD_NUMBER: builtins.int
     HISTORICALAPICALLS_FIELD_NUMBER: builtins.int
     product: builtins.str
@@ -31,60 +27,60 @@
     def __init__(
         self,
         *,
         product: builtins.str = ...,
         apiCalls: global___ApiCalls | None = ...,
         historicalApiCalls: global___ApiCalls | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["apiCalls", b"apiCalls", "historicalApiCalls", b"historicalApiCalls"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["apiCalls", b"apiCalls", "historicalApiCalls", b"historicalApiCalls", "product", b"product"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["apiCalls", b"apiCalls", "historicalApiCalls", b"historicalApiCalls"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["apiCalls", b"apiCalls", "historicalApiCalls", b"historicalApiCalls", "product", b"product"]) -> None: ...
 
 global___ApiUsageItem = ApiUsageItem
 
-@typing_extensions.final
+@typing.final
 class ApiCalls(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LIMIT_FIELD_NUMBER: builtins.int
     USAGE_FIELD_NUMBER: builtins.int
     limit: builtins.int
     usage: builtins.int
     def __init__(
         self,
         *,
         limit: builtins.int = ...,
         usage: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["limit", b"limit", "usage", b"usage"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["limit", b"limit", "usage", b"usage"]) -> None: ...
 
 global___ApiCalls = ApiCalls
 
-@typing_extensions.final
+@typing.final
 class GetApiUsageRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PRODUCT_FIELD_NUMBER: builtins.int
     product: builtins.str
     def __init__(
         self,
         *,
         product: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["product", b"product"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["product", b"product"]) -> None: ...
 
 global___GetApiUsageRequest = GetApiUsageRequest
 
-@typing_extensions.final
+@typing.final
 class GetApiUsageResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApiUsageItem]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___ApiUsageItem] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetApiUsageResponse = GetApiUsageResponse
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/api_usage_pb2_grpc.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/api_usage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_pb2.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: finazon_grpc_python/benzinga.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -16,15 +17,14 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"finazon_grpc_python/benzinga.proto\x12\x07\x66inazon\x1a\x1fgoogle/protobuf/timestamp.proto\"\xfd\x01\n\x1bGetDividentsCalendarRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x02 \x01(\t\x12\x10\n\x08start_at\x18\x03 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x04 \x01(\x03\x12\x0c\n\x04page\x18\x05 \x01(\x05\x12\x11\n\tpage_size\x18\x06 \x01(\x05\x12\r\n\x05order\x18\x07 \x01(\t\x12\x0b\n\x03\x63qs\x18\x08 \x01(\t\x12\x0b\n\x03\x63ik\x18\t \x01(\t\x12\r\n\x05\x63usip\x18\n \x01(\t\x12\x0c\n\x04isin\x18\x0b \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\x0c \x01(\t\x12\x12\n\nshare_figi\x18\r \x01(\t\x12\x0b\n\x03lei\x18\x0e \x01(\t\"N\n\x1cGetDividentsCalendarResponse\x12.\n\x06result\x18\x01 \x03(\x0b\x32\x1e.finazon.DividentsCalendarItem\"\x84\x03\n\x15\x44ividentsCalendarItem\x12\x11\n\trecord_id\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0b\n\x03mic\x18\x04 \x01(\t\x12\x10\n\x08\x63urrency\x18\x05 \x01(\t\x12\x18\n\x10\x65x_dividend_date\x18\x06 \x01(\t\x12\x15\n\rdividend_type\x18\x07 \x01(\t\x12\x10\n\x08\x64ividend\x18\x08 \x01(\x01\x12\x16\n\x0e\x64ividend_yield\x18\t \x01(\x01\x12\x16\n\x0e\x64ividend_prior\x18\n \x01(\t\x12\x18\n\x10\x64\x65\x63laration_date\x18\x0b \x01(\t\x12\x14\n\x0cpayable_date\x18\x0c \x01(\t\x12\x13\n\x0brecord_date\x18\r \x01(\t\x12\x1c\n\x14\x65nd_regular_dividend\x18\x0e \x01(\x08\x12\x11\n\tfrequency\x18\x0f \x01(\x05\x12\x12\n\nimportance\x18\x10 \x01(\x05\x12\r\n\x05notes\x18\x11 \x01(\t\x12\x0f\n\x07updated\x18\x12 \x01(\x03\"\xfc\x01\n\x1aGetEarningsCalendarRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x02 \x01(\t\x12\x10\n\x08start_at\x18\x03 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x04 \x01(\x03\x12\x0c\n\x04page\x18\x05 \x01(\x05\x12\x11\n\tpage_size\x18\x06 \x01(\x05\x12\r\n\x05order\x18\x07 \x01(\t\x12\x0b\n\x03\x63qs\x18\x08 \x01(\t\x12\x0b\n\x03\x63ik\x18\t \x01(\t\x12\r\n\x05\x63usip\x18\n \x01(\t\x12\x0c\n\x04isin\x18\x0b \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\x0c \x01(\t\x12\x12\n\nshare_figi\x18\r \x01(\t\x12\x0b\n\x03lei\x18\x0e \x01(\t\"L\n\x1bGetEarningsCalendarResponse\x12-\n\x06result\x18\x01 \x03(\x0b\x32\x1d.finazon.EarningsCalendarItem\"\xc9\x04\n\x14\x45\x61rningsCalendarItem\x12\x10\n\x08\x63urrency\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x02 \x01(\t\x12\x16\n\x0e\x64\x61te_confirmed\x18\x03 \x01(\x08\x12.\n\x03\x65ps\x18\x04 \x01(\x0b\x32!.finazon.EarningsCalendarItem.Eps\x12\x12\n\nimportance\x18\x05 \x01(\x05\x12\x0b\n\x03mic\x18\x06 \x01(\t\x12\x0c\n\x04name\x18\x07 \x01(\t\x12\r\n\x05notes\x18\x08 \x01(\t\x12\x0e\n\x06period\x18\t \x01(\t\x12\x13\n\x0bperiod_year\x18\n \x01(\x05\x12\x11\n\trecord_id\x18\x0b \x01(\t\x12\x36\n\x07revenue\x18\x0c \x01(\x0b\x32%.finazon.EarningsCalendarItem.Revenue\x12\x0e\n\x06ticker\x18\r \x01(\t\x12\x0c\n\x04time\x18\x0e \x01(\t\x12\x0f\n\x07updated\x18\x0f \x01(\x03\x1as\n\x03\x45ps\x12\x11\n\testimated\x18\x01 \x01(\x01\x12\r\n\x05prior\x18\x02 \x01(\x01\x12\x10\n\x08reported\x18\x03 \x01(\x01\x12\x10\n\x08surprise\x18\x04 \x01(\x01\x12\x18\n\x10surprise_percent\x18\x05 \x01(\x01\x12\x0c\n\x04type\x18\x06 \x01(\t\x1aw\n\x07Revenue\x12\x11\n\testimated\x18\x01 \x01(\x01\x12\r\n\x05prior\x18\x02 \x01(\x01\x12\x10\n\x08reported\x18\x03 \x01(\x01\x12\x10\n\x08surprise\x18\x04 \x01(\x01\x12\x18\n\x10surprise_percent\x18\x05 \x01(\x01\x12\x0c\n\x04type\x18\x06 \x01(\t\"\xf0\x01\n\x0eGetNewsRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x02 \x01(\t\x12\x10\n\x08start_at\x18\x03 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x04 \x01(\x03\x12\x0c\n\x04page\x18\x05 \x01(\x05\x12\x11\n\tpage_size\x18\x06 \x01(\x05\x12\r\n\x05order\x18\x07 \x01(\t\x12\x0b\n\x03\x63qs\x18\x08 \x01(\t\x12\x0b\n\x03\x63ik\x18\t \x01(\t\x12\r\n\x05\x63usip\x18\n \x01(\t\x12\x0c\n\x04isin\x18\x0b \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\x0c \x01(\t\x12\x12\n\nshare_figi\x18\r \x01(\t\x12\x0b\n\x03lei\x18\x0e \x01(\t\"4\n\x0fGetNewsResponse\x12!\n\x06result\x18\x01 \x03(\x0b\x32\x11.finazon.NewsItem\"\xea\x01\n\x08NewsItem\x12\x0e\n\x06\x61uthor\x18\x01 \x01(\t\x12\x10\n\x08\x63hannels\x18\x02 \x03(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06images\x18\x04 \x03(\t\x12\x11\n\trecord_id\x18\x05 \x01(\x05\x12\x0c\n\x04tags\x18\x06 \x03(\t\x12\x0f\n\x07tickers\x18\x07 \x03(\t\x12\r\n\x05title\x18\x08 \x01(\t\x12.\n\nupdated_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03url\x18\n \x01(\t\"s\n\rGetIPORequest\x12\x10\n\x08start_at\x18\x03 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x04 \x01(\x03\x12\x0c\n\x04page\x18\x05 \x01(\x05\x12\x11\n\tpage_size\x18\x06 \x01(\x05\x12\r\n\x05order\x18\x07 \x01(\t\x12\x10\n\x08\x65xchange\x18\x0f \x01(\t\"0\n\x0eGetIPOResponse\x12\x1e\n\x04ipos\x18\x01 \x03(\x0b\x32\x10.finazon.IPOItem\"\xc3\x07\n\x07IPOItem\x12\x11\n\trecord_id\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0b\n\x03mic\x18\x04 \x01(\t\x12\x10\n\x08\x63urrency\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x06 \x01(\t\x12\x1a\n\x12open_date_verified\x18\x07 \x01(\x08\x12\x0c\n\x04time\x18\x08 \x01(\t\x12\x11\n\tprice_max\x18\t \x01(\x01\x12\x11\n\tprice_min\x18\n \x01(\x01\x12\x12\n\nprice_open\x18\x0b \x01(\x01\x12\x1d\n\x15price_public_offering\x18\x0c \x01(\x01\x12\x17\n\x0foffering_shares\x18\r \x01(\x01\x12\x1f\n\x17offering_shares_ord_adr\x18\x0e \x01(\x01\x12\x16\n\x0eoffering_value\x18\x0f \x01(\x01\x12\"\n\x1aord_shares_out_after_offer\x18\x10 \x01(\x01\x12\x1b\n\x13market_cap_at_offer\x18\x11 \x01(\x01\x12\x13\n\x0b\x64\x65\x61l_status\x18\x12 \x01(\t\x12\x1b\n\x13initial_filing_date\x18\x13 \x01(\t\x12\x1b\n\x13insider_lockup_date\x18\x14 \x01(\t\x12\x1b\n\x13insider_lockup_days\x18\x15 \x01(\x05\x12\x10\n\x08ipo_type\x18\x16 \x01(\t\x12\x16\n\x0elast_yr_income\x18\x17 \x01(\x01\x12\x1b\n\x13last_yr_income_year\x18\x18 \x01(\x01\x12\x17\n\x0flast_yr_revenue\x18\x19 \x01(\x01\x12\x1c\n\x14last_yr_revenue_year\x18\x1a \x01(\x01\x12\x19\n\x11lead_underwriters\x18\x1b \x03(\t\x12\x1a\n\x12other_underwriters\x18\x1c \x03(\t\x12\r\n\x05notes\x18\x1d \x01(\t\x12\x14\n\x0cpricing_date\x18\x1e \x01(\t\x12\x1c\n\x14sec_accession_number\x18\x1f \x01(\t\x12\x16\n\x0esec_filing_url\x18  \x01(\t\x12\x1a\n\x12shares_outstanding\x18! \x01(\x01\x12\x0b\n\x03sic\x18\" \x01(\x01\x12 \n\x18spac_converted_to_target\x18# \x01(\x08\x12\x16\n\x0estate_location\x18$ \x01(\t\x12)\n!underwriter_quiet_expiration_date\x18% \x01(\t\x12)\n!underwriter_quiet_expiration_days\x18& \x01(\x05\x12\x0f\n\x07updated\x18\' \x01(\x03\x32\xd9\x02\n\x0f\x42\x65nzingaService\x12\x65\n\x14GetDividentsCalendar\x12$.finazon.GetDividentsCalendarRequest\x1a%.finazon.GetDividentsCalendarResponse\"\x00\x12\x62\n\x13GetEarningsCalendar\x12#.finazon.GetEarningsCalendarRequest\x1a$.finazon.GetEarningsCalendarResponse\"\x00\x12>\n\x07GetNews\x12\x17.finazon.GetNewsRequest\x1a\x18.finazon.GetNewsResponse\"\x00\x12;\n\x06GetIPO\x12\x16.finazon.GetIPORequest\x1a\x17.finazon.GetIPOResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.benzinga_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_GETDIVIDENTSCALENDARREQUEST']._serialized_start=81
   _globals['_GETDIVIDENTSCALENDARREQUEST']._serialized_end=334
   _globals['_GETDIVIDENTSCALENDARRESPONSE']._serialized_start=336
   _globals['_GETDIVIDENTSCALENDARRESPONSE']._serialized_end=414
   _globals['_DIVIDENTSCALENDARITEM']._serialized_start=417
   _globals['_DIVIDENTSCALENDARITEM']._serialized_end=805
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_pb2.pyi` & `finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import google.protobuf.timestamp_pb2
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class GetDividentsCalendarRequest(google.protobuf.message.Message):
     """DividentsCalendar"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
     DATE_FIELD_NUMBER: builtins.int
@@ -65,35 +61,35 @@
         cik: builtins.str = ...,
         cusip: builtins.str = ...,
         isin: builtins.str = ...,
         composite_figi: builtins.str = ...,
         share_figi: builtins.str = ...,
         lei: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "composite_figi", b"composite_figi", "cqs", b"cqs", "cusip", b"cusip", "date", b"date", "end_at", b"end_at", "isin", b"isin", "lei", b"lei", "order", b"order", "page", b"page", "page_size", b"page_size", "share_figi", b"share_figi", "start_at", b"start_at", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cik", b"cik", "composite_figi", b"composite_figi", "cqs", b"cqs", "cusip", b"cusip", "date", b"date", "end_at", b"end_at", "isin", b"isin", "lei", b"lei", "order", b"order", "page", b"page", "page_size", b"page_size", "share_figi", b"share_figi", "start_at", b"start_at", "ticker", b"ticker"]) -> None: ...
 
 global___GetDividentsCalendarRequest = GetDividentsCalendarRequest
 
-@typing_extensions.final
+@typing.final
 class GetDividentsCalendarResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DividentsCalendarItem]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___DividentsCalendarItem] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetDividentsCalendarResponse = GetDividentsCalendarResponse
 
-@typing_extensions.final
+@typing.final
 class DividentsCalendarItem(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RECORD_ID_FIELD_NUMBER: builtins.int
     TICKER_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     MIC_FIELD_NUMBER: builtins.int
@@ -147,19 +143,19 @@
         record_date: builtins.str = ...,
         end_regular_dividend: builtins.bool = ...,
         frequency: builtins.int = ...,
         importance: builtins.int = ...,
         notes: builtins.str = ...,
         updated: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["currency", b"currency", "declaration_date", b"declaration_date", "dividend", b"dividend", "dividend_prior", b"dividend_prior", "dividend_type", b"dividend_type", "dividend_yield", b"dividend_yield", "end_regular_dividend", b"end_regular_dividend", "ex_dividend_date", b"ex_dividend_date", "frequency", b"frequency", "importance", b"importance", "mic", b"mic", "name", b"name", "notes", b"notes", "payable_date", b"payable_date", "record_date", b"record_date", "record_id", b"record_id", "ticker", b"ticker", "updated", b"updated"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["currency", b"currency", "declaration_date", b"declaration_date", "dividend", b"dividend", "dividend_prior", b"dividend_prior", "dividend_type", b"dividend_type", "dividend_yield", b"dividend_yield", "end_regular_dividend", b"end_regular_dividend", "ex_dividend_date", b"ex_dividend_date", "frequency", b"frequency", "importance", b"importance", "mic", b"mic", "name", b"name", "notes", b"notes", "payable_date", b"payable_date", "record_date", b"record_date", "record_id", b"record_id", "ticker", b"ticker", "updated", b"updated"]) -> None: ...
 
 global___DividentsCalendarItem = DividentsCalendarItem
 
-@typing_extensions.final
+@typing.final
 class GetEarningsCalendarRequest(google.protobuf.message.Message):
     """EarningsCalendar"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
     DATE_FIELD_NUMBER: builtins.int
@@ -203,39 +199,39 @@
         cik: builtins.str = ...,
         cusip: builtins.str = ...,
         isin: builtins.str = ...,
         composite_figi: builtins.str = ...,
         share_figi: builtins.str = ...,
         lei: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "composite_figi", b"composite_figi", "cqs", b"cqs", "cusip", b"cusip", "date", b"date", "end_at", b"end_at", "isin", b"isin", "lei", b"lei", "order", b"order", "page", b"page", "page_size", b"page_size", "share_figi", b"share_figi", "start_at", b"start_at", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cik", b"cik", "composite_figi", b"composite_figi", "cqs", b"cqs", "cusip", b"cusip", "date", b"date", "end_at", b"end_at", "isin", b"isin", "lei", b"lei", "order", b"order", "page", b"page", "page_size", b"page_size", "share_figi", b"share_figi", "start_at", b"start_at", "ticker", b"ticker"]) -> None: ...
 
 global___GetEarningsCalendarRequest = GetEarningsCalendarRequest
 
-@typing_extensions.final
+@typing.final
 class GetEarningsCalendarResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___EarningsCalendarItem]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___EarningsCalendarItem] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetEarningsCalendarResponse = GetEarningsCalendarResponse
 
-@typing_extensions.final
+@typing.final
 class EarningsCalendarItem(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Eps(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         ESTIMATED_FIELD_NUMBER: builtins.int
         PRIOR_FIELD_NUMBER: builtins.int
         REPORTED_FIELD_NUMBER: builtins.int
         SURPRISE_FIELD_NUMBER: builtins.int
@@ -253,17 +249,17 @@
             estimated: builtins.float = ...,
             prior: builtins.float = ...,
             reported: builtins.float = ...,
             surprise: builtins.float = ...,
             surprise_percent: builtins.float = ...,
             type: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["estimated", b"estimated", "prior", b"prior", "reported", b"reported", "surprise", b"surprise", "surprise_percent", b"surprise_percent", "type", b"type"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["estimated", b"estimated", "prior", b"prior", "reported", b"reported", "surprise", b"surprise", "surprise_percent", b"surprise_percent", "type", b"type"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class Revenue(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         ESTIMATED_FIELD_NUMBER: builtins.int
         PRIOR_FIELD_NUMBER: builtins.int
         REPORTED_FIELD_NUMBER: builtins.int
         SURPRISE_FIELD_NUMBER: builtins.int
@@ -281,15 +277,15 @@
             estimated: builtins.float = ...,
             prior: builtins.float = ...,
             reported: builtins.float = ...,
             surprise: builtins.float = ...,
             surprise_percent: builtins.float = ...,
             type: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["estimated", b"estimated", "prior", b"prior", "reported", b"reported", "surprise", b"surprise", "surprise_percent", b"surprise_percent", "type", b"type"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["estimated", b"estimated", "prior", b"prior", "reported", b"reported", "surprise", b"surprise", "surprise_percent", b"surprise_percent", "type", b"type"]) -> None: ...
 
     CURRENCY_FIELD_NUMBER: builtins.int
     DATE_FIELD_NUMBER: builtins.int
     DATE_CONFIRMED_FIELD_NUMBER: builtins.int
     EPS_FIELD_NUMBER: builtins.int
     IMPORTANCE_FIELD_NUMBER: builtins.int
     MIC_FIELD_NUMBER: builtins.int
@@ -301,28 +297,28 @@
     REVENUE_FIELD_NUMBER: builtins.int
     TICKER_FIELD_NUMBER: builtins.int
     TIME_FIELD_NUMBER: builtins.int
     UPDATED_FIELD_NUMBER: builtins.int
     currency: builtins.str
     date: builtins.str
     date_confirmed: builtins.bool
-    @property
-    def eps(self) -> global___EarningsCalendarItem.Eps: ...
     importance: builtins.int
     mic: builtins.str
     name: builtins.str
     notes: builtins.str
     period: builtins.str
     period_year: builtins.int
     record_id: builtins.str
-    @property
-    def revenue(self) -> global___EarningsCalendarItem.Revenue: ...
     ticker: builtins.str
     time: builtins.str
     updated: builtins.int
+    @property
+    def eps(self) -> global___EarningsCalendarItem.Eps: ...
+    @property
+    def revenue(self) -> global___EarningsCalendarItem.Revenue: ...
     def __init__(
         self,
         *,
         currency: builtins.str = ...,
         date: builtins.str = ...,
         date_confirmed: builtins.bool = ...,
         eps: global___EarningsCalendarItem.Eps | None = ...,
@@ -334,20 +330,20 @@
         period_year: builtins.int = ...,
         record_id: builtins.str = ...,
         revenue: global___EarningsCalendarItem.Revenue | None = ...,
         ticker: builtins.str = ...,
         time: builtins.str = ...,
         updated: builtins.int = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["eps", b"eps", "revenue", b"revenue"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["currency", b"currency", "date", b"date", "date_confirmed", b"date_confirmed", "eps", b"eps", "importance", b"importance", "mic", b"mic", "name", b"name", "notes", b"notes", "period", b"period", "period_year", b"period_year", "record_id", b"record_id", "revenue", b"revenue", "ticker", b"ticker", "time", b"time", "updated", b"updated"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["eps", b"eps", "revenue", b"revenue"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["currency", b"currency", "date", b"date", "date_confirmed", b"date_confirmed", "eps", b"eps", "importance", b"importance", "mic", b"mic", "name", b"name", "notes", b"notes", "period", b"period", "period_year", b"period_year", "record_id", b"record_id", "revenue", b"revenue", "ticker", b"ticker", "time", b"time", "updated", b"updated"]) -> None: ...
 
 global___EarningsCalendarItem = EarningsCalendarItem
 
-@typing_extensions.final
+@typing.final
 class GetNewsRequest(google.protobuf.message.Message):
     """News"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
     DATE_FIELD_NUMBER: builtins.int
@@ -391,84 +387,84 @@
         cik: builtins.str = ...,
         cusip: builtins.str = ...,
         isin: builtins.str = ...,
         composite_figi: builtins.str = ...,
         share_figi: builtins.str = ...,
         lei: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "composite_figi", b"composite_figi", "cqs", b"cqs", "cusip", b"cusip", "date", b"date", "end_at", b"end_at", "isin", b"isin", "lei", b"lei", "order", b"order", "page", b"page", "page_size", b"page_size", "share_figi", b"share_figi", "start_at", b"start_at", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cik", b"cik", "composite_figi", b"composite_figi", "cqs", b"cqs", "cusip", b"cusip", "date", b"date", "end_at", b"end_at", "isin", b"isin", "lei", b"lei", "order", b"order", "page", b"page", "page_size", b"page_size", "share_figi", b"share_figi", "start_at", b"start_at", "ticker", b"ticker"]) -> None: ...
 
 global___GetNewsRequest = GetNewsRequest
 
-@typing_extensions.final
+@typing.final
 class GetNewsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___NewsItem]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___NewsItem] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetNewsResponse = GetNewsResponse
 
-@typing_extensions.final
+@typing.final
 class NewsItem(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AUTHOR_FIELD_NUMBER: builtins.int
     CHANNELS_FIELD_NUMBER: builtins.int
     CREATED_AT_FIELD_NUMBER: builtins.int
     IMAGES_FIELD_NUMBER: builtins.int
     RECORD_ID_FIELD_NUMBER: builtins.int
     TAGS_FIELD_NUMBER: builtins.int
     TICKERS_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
     UPDATED_AT_FIELD_NUMBER: builtins.int
     URL_FIELD_NUMBER: builtins.int
     author: builtins.str
+    record_id: builtins.int
+    title: builtins.str
+    url: builtins.str
     @property
     def channels(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     @property
     def created_at(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     @property
     def images(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    record_id: builtins.int
     @property
     def tags(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     @property
     def tickers(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    title: builtins.str
     @property
     def updated_at(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
-    url: builtins.str
     def __init__(
         self,
         *,
         author: builtins.str = ...,
         channels: collections.abc.Iterable[builtins.str] | None = ...,
         created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         images: collections.abc.Iterable[builtins.str] | None = ...,
         record_id: builtins.int = ...,
         tags: collections.abc.Iterable[builtins.str] | None = ...,
         tickers: collections.abc.Iterable[builtins.str] | None = ...,
         title: builtins.str = ...,
         updated_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         url: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "updated_at", b"updated_at"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["author", b"author", "channels", b"channels", "created_at", b"created_at", "images", b"images", "record_id", b"record_id", "tags", b"tags", "tickers", b"tickers", "title", b"title", "updated_at", b"updated_at", "url", b"url"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["created_at", b"created_at", "updated_at", b"updated_at"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["author", b"author", "channels", b"channels", "created_at", b"created_at", "images", b"images", "record_id", b"record_id", "tags", b"tags", "tickers", b"tickers", "title", b"title", "updated_at", b"updated_at", "url", b"url"]) -> None: ...
 
 global___NewsItem = NewsItem
 
-@typing_extensions.final
+@typing.final
 class GetIPORequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     START_AT_FIELD_NUMBER: builtins.int
     END_AT_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
     PAGE_SIZE_FIELD_NUMBER: builtins.int
@@ -486,35 +482,35 @@
         start_at: builtins.int = ...,
         end_at: builtins.int = ...,
         page: builtins.int = ...,
         page_size: builtins.int = ...,
         order: builtins.str = ...,
         exchange: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["end_at", b"end_at", "exchange", b"exchange", "order", b"order", "page", b"page", "page_size", b"page_size", "start_at", b"start_at"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["end_at", b"end_at", "exchange", b"exchange", "order", b"order", "page", b"page", "page_size", b"page_size", "start_at", b"start_at"]) -> None: ...
 
 global___GetIPORequest = GetIPORequest
 
-@typing_extensions.final
+@typing.final
 class GetIPOResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     IPOS_FIELD_NUMBER: builtins.int
     @property
     def ipos(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___IPOItem]: ...
     def __init__(
         self,
         *,
         ipos: collections.abc.Iterable[global___IPOItem] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["ipos", b"ipos"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["ipos", b"ipos"]) -> None: ...
 
 global___GetIPOResponse = GetIPOResponse
 
-@typing_extensions.final
+@typing.final
 class IPOItem(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RECORD_ID_FIELD_NUMBER: builtins.int
     TICKER_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     MIC_FIELD_NUMBER: builtins.int
@@ -575,29 +571,29 @@
     insider_lockup_date: builtins.str
     insider_lockup_days: builtins.int
     ipo_type: builtins.str
     last_yr_income: builtins.float
     last_yr_income_year: builtins.float
     last_yr_revenue: builtins.float
     last_yr_revenue_year: builtins.float
-    @property
-    def lead_underwriters(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    @property
-    def other_underwriters(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     notes: builtins.str
     pricing_date: builtins.str
     sec_accession_number: builtins.str
     sec_filing_url: builtins.str
     shares_outstanding: builtins.float
     sic: builtins.float
     spac_converted_to_target: builtins.bool
     state_location: builtins.str
     underwriter_quiet_expiration_date: builtins.str
     underwriter_quiet_expiration_days: builtins.int
     updated: builtins.int
+    @property
+    def lead_underwriters(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    @property
+    def other_underwriters(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     def __init__(
         self,
         *,
         record_id: builtins.str = ...,
         ticker: builtins.str = ...,
         name: builtins.str = ...,
         mic: builtins.str = ...,
@@ -633,10 +629,10 @@
         sic: builtins.float = ...,
         spac_converted_to_target: builtins.bool = ...,
         state_location: builtins.str = ...,
         underwriter_quiet_expiration_date: builtins.str = ...,
         underwriter_quiet_expiration_days: builtins.int = ...,
         updated: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["currency", b"currency", "date", b"date", "deal_status", b"deal_status", "initial_filing_date", b"initial_filing_date", "insider_lockup_date", b"insider_lockup_date", "insider_lockup_days", b"insider_lockup_days", "ipo_type", b"ipo_type", "last_yr_income", b"last_yr_income", "last_yr_income_year", b"last_yr_income_year", "last_yr_revenue", b"last_yr_revenue", "last_yr_revenue_year", b"last_yr_revenue_year", "lead_underwriters", b"lead_underwriters", "market_cap_at_offer", b"market_cap_at_offer", "mic", b"mic", "name", b"name", "notes", b"notes", "offering_shares", b"offering_shares", "offering_shares_ord_adr", b"offering_shares_ord_adr", "offering_value", b"offering_value", "open_date_verified", b"open_date_verified", "ord_shares_out_after_offer", b"ord_shares_out_after_offer", "other_underwriters", b"other_underwriters", "price_max", b"price_max", "price_min", b"price_min", "price_open", b"price_open", "price_public_offering", b"price_public_offering", "pricing_date", b"pricing_date", "record_id", b"record_id", "sec_accession_number", b"sec_accession_number", "sec_filing_url", b"sec_filing_url", "shares_outstanding", b"shares_outstanding", "sic", b"sic", "spac_converted_to_target", b"spac_converted_to_target", "state_location", b"state_location", "ticker", b"ticker", "time", b"time", "underwriter_quiet_expiration_date", b"underwriter_quiet_expiration_date", "underwriter_quiet_expiration_days", b"underwriter_quiet_expiration_days", "updated", b"updated"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["currency", b"currency", "date", b"date", "deal_status", b"deal_status", "initial_filing_date", b"initial_filing_date", "insider_lockup_date", b"insider_lockup_date", "insider_lockup_days", b"insider_lockup_days", "ipo_type", b"ipo_type", "last_yr_income", b"last_yr_income", "last_yr_income_year", b"last_yr_income_year", "last_yr_revenue", b"last_yr_revenue", "last_yr_revenue_year", b"last_yr_revenue_year", "lead_underwriters", b"lead_underwriters", "market_cap_at_offer", b"market_cap_at_offer", "mic", b"mic", "name", b"name", "notes", b"notes", "offering_shares", b"offering_shares", "offering_shares_ord_adr", b"offering_shares_ord_adr", "offering_value", b"offering_value", "open_date_verified", b"open_date_verified", "ord_shares_out_after_offer", b"ord_shares_out_after_offer", "other_underwriters", b"other_underwriters", "price_max", b"price_max", "price_min", b"price_min", "price_open", b"price_open", "price_public_offering", b"price_public_offering", "pricing_date", b"pricing_date", "record_id", b"record_id", "sec_accession_number", b"sec_accession_number", "sec_filing_url", b"sec_filing_url", "shares_outstanding", b"shares_outstanding", "sic", b"sic", "spac_converted_to_target", b"spac_converted_to_target", "state_location", b"state_location", "ticker", b"ticker", "time", b"time", "underwriter_quiet_expiration_date", b"underwriter_quiet_expiration_date", "underwriter_quiet_expiration_days", b"underwriter_quiet_expiration_days", "updated", b"updated"]) -> None: ...
 
 global___IPOItem = IPOItem
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_pb2_grpc.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_service.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/binance_pb2.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/binance_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: finazon_grpc_python/binance.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!finazon_grpc_python/binance.proto\x12\x07\x66inazon\"\xe4\x01\n\x11\x42inanceTimeSeries\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0c\n\x04open\x18\x02 \x01(\x01\x12\r\n\x05\x63lose\x18\x03 \x01(\x01\x12\x0c\n\x04high\x18\x04 \x01(\x01\x12\x0b\n\x03low\x18\x05 \x01(\x01\x12\x0e\n\x06trades\x18\x06 \x01(\x01\x12\x13\n\x0b\x62\x61se_volume\x18\x07 \x01(\x01\x12\x14\n\x0cquote_volume\x18\x08 \x01(\x01\x12#\n\x1btaker_buy_base_asset_volume\x18\t \x01(\x01\x12$\n\x1ctaker_buy_quote_asset_volume\x18\n \x01(\x01\"\xaf\x01\n\x1bGetBinanceTimeSeriesRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x10\n\x08timezone\x18\x02 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08start_at\x18\x05 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x06 \x01(\x03\x12\x0c\n\x04page\x18\x07 \x01(\x05\x12\x11\n\tpage_size\x18\x08 \x01(\x05\x12\r\n\x05order\x18\t \x01(\tJ\x04\x08\x04\x10\x05R\x04\x64\x61te\"J\n\x1cGetBinanceTimeSeriesResponse\x12*\n\x06result\x18\x01 \x03(\x0b\x32\x1a.finazon.BinanceTimeSeries2p\n\x0e\x42inanceService\x12^\n\rGetTimeSeries\x12$.finazon.GetBinanceTimeSeriesRequest\x1a%.finazon.GetBinanceTimeSeriesResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!finazon_grpc_python/binance.proto\x12\x07\x66inazon\"\xe4\x01\n\x11\x42inanceTimeSeries\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0c\n\x04open\x18\x02 \x01(\x01\x12\r\n\x05\x63lose\x18\x03 \x01(\x01\x12\x0c\n\x04high\x18\x04 \x01(\x01\x12\x0b\n\x03low\x18\x05 \x01(\x01\x12\x0e\n\x06trades\x18\x06 \x01(\x01\x12\x13\n\x0b\x62\x61se_volume\x18\x07 \x01(\x01\x12\x14\n\x0cquote_volume\x18\x08 \x01(\x01\x12#\n\x1btaker_buy_base_asset_volume\x18\t \x01(\x01\x12$\n\x1ctaker_buy_quote_asset_volume\x18\n \x01(\x01\"\xad\x01\n\x1bGetBinanceTimeSeriesRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08start_at\x18\x05 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x06 \x01(\x03\x12\x0c\n\x04page\x18\x07 \x01(\x05\x12\x11\n\tpage_size\x18\x08 \x01(\x05\x12\r\n\x05order\x18\t \x01(\tJ\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05R\x08timezoneR\x04\x64\x61te\"J\n\x1cGetBinanceTimeSeriesResponse\x12*\n\x06result\x18\x01 \x03(\x0b\x32\x1a.finazon.BinanceTimeSeries2p\n\x0e\x42inanceService\x12^\n\rGetTimeSeries\x12$.finazon.GetBinanceTimeSeriesRequest\x1a%.finazon.GetBinanceTimeSeriesResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.binance_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_BINANCETIMESERIES']._serialized_start=47
   _globals['_BINANCETIMESERIES']._serialized_end=275
   _globals['_GETBINANCETIMESERIESREQUEST']._serialized_start=278
-  _globals['_GETBINANCETIMESERIESREQUEST']._serialized_end=453
-  _globals['_GETBINANCETIMESERIESRESPONSE']._serialized_start=455
-  _globals['_GETBINANCETIMESERIESRESPONSE']._serialized_end=529
-  _globals['_BINANCESERVICE']._serialized_start=531
-  _globals['_BINANCESERVICE']._serialized_end=643
+  _globals['_GETBINANCETIMESERIESREQUEST']._serialized_end=451
+  _globals['_GETBINANCETIMESERIESRESPONSE']._serialized_start=453
+  _globals['_GETBINANCETIMESERIESRESPONSE']._serialized_end=527
+  _globals['_BINANCESERVICE']._serialized_start=529
+  _globals['_BINANCESERVICE']._serialized_end=641
 # @@protoc_insertion_point(module_scope)
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/binance_pb2.pyi` & `finazon_grpc_python-1.0.146/finazon_grpc_python/binance_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class BinanceTimeSeries(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TIMESTAMP_FIELD_NUMBER: builtins.int
     OPEN_FIELD_NUMBER: builtins.int
     CLOSE_FIELD_NUMBER: builtins.int
     HIGH_FIELD_NUMBER: builtins.int
@@ -50,62 +46,59 @@
         low: builtins.float = ...,
         trades: builtins.float = ...,
         base_volume: builtins.float = ...,
         quote_volume: builtins.float = ...,
         taker_buy_base_asset_volume: builtins.float = ...,
         taker_buy_quote_asset_volume: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["base_volume", b"base_volume", "close", b"close", "high", b"high", "low", b"low", "open", b"open", "quote_volume", b"quote_volume", "taker_buy_base_asset_volume", b"taker_buy_base_asset_volume", "taker_buy_quote_asset_volume", b"taker_buy_quote_asset_volume", "timestamp", b"timestamp", "trades", b"trades"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["base_volume", b"base_volume", "close", b"close", "high", b"high", "low", b"low", "open", b"open", "quote_volume", b"quote_volume", "taker_buy_base_asset_volume", b"taker_buy_base_asset_volume", "taker_buy_quote_asset_volume", b"taker_buy_quote_asset_volume", "timestamp", b"timestamp", "trades", b"trades"]) -> None: ...
 
 global___BinanceTimeSeries = BinanceTimeSeries
 
-@typing_extensions.final
+@typing.final
 class GetBinanceTimeSeriesRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
-    TIMEZONE_FIELD_NUMBER: builtins.int
     INTERVAL_FIELD_NUMBER: builtins.int
     START_AT_FIELD_NUMBER: builtins.int
     END_AT_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
     PAGE_SIZE_FIELD_NUMBER: builtins.int
     ORDER_FIELD_NUMBER: builtins.int
     ticker: builtins.str
-    timezone: builtins.str
     interval: builtins.str
     start_at: builtins.int
     end_at: builtins.int
     page: builtins.int
     page_size: builtins.int
     order: builtins.str
     def __init__(
         self,
         *,
         ticker: builtins.str = ...,
-        timezone: builtins.str = ...,
         interval: builtins.str = ...,
         start_at: builtins.int = ...,
         end_at: builtins.int = ...,
         page: builtins.int = ...,
         page_size: builtins.int = ...,
         order: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["end_at", b"end_at", "interval", b"interval", "order", b"order", "page", b"page", "page_size", b"page_size", "start_at", b"start_at", "ticker", b"ticker", "timezone", b"timezone"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["end_at", b"end_at", "interval", b"interval", "order", b"order", "page", b"page", "page_size", b"page_size", "start_at", b"start_at", "ticker", b"ticker"]) -> None: ...
 
 global___GetBinanceTimeSeriesRequest = GetBinanceTimeSeriesRequest
 
-@typing_extensions.final
+@typing.final
 class GetBinanceTimeSeriesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___BinanceTimeSeries]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___BinanceTimeSeries] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetBinanceTimeSeriesResponse = GetBinanceTimeSeriesResponse
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/binance_pb2_grpc.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/binance_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/binance_service.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/binance_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/common/client.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/common/client.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/common/utils.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/common/utils.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_pb2.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: finazon_grpc_python/crypto.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n finazon_grpc_python/crypto.proto\x12\x07\x66inazon\"m\n\x10\x43ryptoTimeSeries\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0c\n\x04open\x18\x02 \x01(\x01\x12\r\n\x05\x63lose\x18\x03 \x01(\x01\x12\x0c\n\x04high\x18\x04 \x01(\x01\x12\x0b\n\x03low\x18\x05 \x01(\x01\x12\x0e\n\x06volume\x18\x06 \x01(\x01\"\xae\x01\n\x1aGetCryptoTimeSeriesRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x10\n\x08timezone\x18\x02 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08start_at\x18\x05 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x06 \x01(\x03\x12\x0c\n\x04page\x18\x07 \x01(\x05\x12\x11\n\tpage_size\x18\x08 \x01(\x05\x12\r\n\x05order\x18\t \x01(\tJ\x04\x08\x04\x10\x05R\x04\x64\x61te\"H\n\x1bGetCryptoTimeSeriesResponse\x12)\n\x06result\x18\x01 \x03(\x0b\x32\x19.finazon.CryptoTimeSeries2m\n\rCryptoService\x12\\\n\rGetTimeSeries\x12#.finazon.GetCryptoTimeSeriesRequest\x1a$.finazon.GetCryptoTimeSeriesResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n finazon_grpc_python/crypto.proto\x12\x07\x66inazon\"m\n\x10\x43ryptoTimeSeries\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0c\n\x04open\x18\x02 \x01(\x01\x12\r\n\x05\x63lose\x18\x03 \x01(\x01\x12\x0c\n\x04high\x18\x04 \x01(\x01\x12\x0b\n\x03low\x18\x05 \x01(\x01\x12\x0e\n\x06volume\x18\x06 \x01(\x01\"\xac\x01\n\x1aGetCryptoTimeSeriesRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08start_at\x18\x05 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x06 \x01(\x03\x12\x0c\n\x04page\x18\x07 \x01(\x05\x12\x11\n\tpage_size\x18\x08 \x01(\x05\x12\r\n\x05order\x18\t \x01(\tJ\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05R\x08timezoneR\x04\x64\x61te\"H\n\x1bGetCryptoTimeSeriesResponse\x12)\n\x06result\x18\x01 \x03(\x0b\x32\x19.finazon.CryptoTimeSeries2m\n\rCryptoService\x12\\\n\rGetTimeSeries\x12#.finazon.GetCryptoTimeSeriesRequest\x1a$.finazon.GetCryptoTimeSeriesResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.crypto_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_CRYPTOTIMESERIES']._serialized_start=45
   _globals['_CRYPTOTIMESERIES']._serialized_end=154
   _globals['_GETCRYPTOTIMESERIESREQUEST']._serialized_start=157
-  _globals['_GETCRYPTOTIMESERIESREQUEST']._serialized_end=331
-  _globals['_GETCRYPTOTIMESERIESRESPONSE']._serialized_start=333
-  _globals['_GETCRYPTOTIMESERIESRESPONSE']._serialized_end=405
-  _globals['_CRYPTOSERVICE']._serialized_start=407
-  _globals['_CRYPTOSERVICE']._serialized_end=516
+  _globals['_GETCRYPTOTIMESERIESREQUEST']._serialized_end=329
+  _globals['_GETCRYPTOTIMESERIESRESPONSE']._serialized_start=331
+  _globals['_GETCRYPTOTIMESERIESRESPONSE']._serialized_end=403
+  _globals['_CRYPTOSERVICE']._serialized_start=405
+  _globals['_CRYPTOSERVICE']._serialized_end=514
 # @@protoc_insertion_point(module_scope)
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_pb2.pyi` & `finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class CryptoTimeSeries(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TIMESTAMP_FIELD_NUMBER: builtins.int
     OPEN_FIELD_NUMBER: builtins.int
     CLOSE_FIELD_NUMBER: builtins.int
     HIGH_FIELD_NUMBER: builtins.int
@@ -38,62 +34,59 @@
         timestamp: builtins.int = ...,
         open: builtins.float = ...,
         close: builtins.float = ...,
         high: builtins.float = ...,
         low: builtins.float = ...,
         volume: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["close", b"close", "high", b"high", "low", b"low", "open", b"open", "timestamp", b"timestamp", "volume", b"volume"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["close", b"close", "high", b"high", "low", b"low", "open", b"open", "timestamp", b"timestamp", "volume", b"volume"]) -> None: ...
 
 global___CryptoTimeSeries = CryptoTimeSeries
 
-@typing_extensions.final
+@typing.final
 class GetCryptoTimeSeriesRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
-    TIMEZONE_FIELD_NUMBER: builtins.int
     INTERVAL_FIELD_NUMBER: builtins.int
     START_AT_FIELD_NUMBER: builtins.int
     END_AT_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
     PAGE_SIZE_FIELD_NUMBER: builtins.int
     ORDER_FIELD_NUMBER: builtins.int
     ticker: builtins.str
-    timezone: builtins.str
     interval: builtins.str
     start_at: builtins.int
     end_at: builtins.int
     page: builtins.int
     page_size: builtins.int
     order: builtins.str
     def __init__(
         self,
         *,
         ticker: builtins.str = ...,
-        timezone: builtins.str = ...,
         interval: builtins.str = ...,
         start_at: builtins.int = ...,
         end_at: builtins.int = ...,
         page: builtins.int = ...,
         page_size: builtins.int = ...,
         order: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["end_at", b"end_at", "interval", b"interval", "order", b"order", "page", b"page", "page_size", b"page_size", "start_at", b"start_at", "ticker", b"ticker", "timezone", b"timezone"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["end_at", b"end_at", "interval", b"interval", "order", b"order", "page", b"page", "page_size", b"page_size", "start_at", b"start_at", "ticker", b"ticker"]) -> None: ...
 
 global___GetCryptoTimeSeriesRequest = GetCryptoTimeSeriesRequest
 
-@typing_extensions.final
+@typing.final
 class GetCryptoTimeSeriesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CryptoTimeSeries]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___CryptoTimeSeries] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetCryptoTimeSeriesResponse = GetCryptoTimeSeriesResponse
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_pb2_grpc.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_service.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/datasets_pb2.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/datasets_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: finazon_grpc_python/datasets.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,15 +16,14 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"finazon_grpc_python/datasets.proto\x12\x07\x66inazon\")\n\x0b\x44\x61tasetItem\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"C\n\x12GetDatasetsRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\";\n\x13GetDatasetsResponse\x12$\n\x06result\x18\x01 \x03(\x0b\x32\x14.finazon.DatasetItem2]\n\x0f\x44\x61tasetsService\x12J\n\x0bGetDatasets\x12\x1b.finazon.GetDatasetsRequest\x1a\x1c.finazon.GetDatasetsResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.datasets_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_DATASETITEM']._serialized_start=47
   _globals['_DATASETITEM']._serialized_end=88
   _globals['_GETDATASETSREQUEST']._serialized_start=90
   _globals['_GETDATASETSREQUEST']._serialized_end=157
   _globals['_GETDATASETSRESPONSE']._serialized_start=159
   _globals['_GETDATASETSRESPONSE']._serialized_end=218
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/datasets_pb2.pyi` & `finazon_grpc_python-1.0.146/finazon_grpc_python/datasets_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class DatasetItem(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CODE_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     code: builtins.str
     name: builtins.str
     def __init__(
         self,
         *,
         code: builtins.str = ...,
         name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "name", b"name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["code", b"code", "name", b"name"]) -> None: ...
 
 global___DatasetItem = DatasetItem
 
-@typing_extensions.final
+@typing.final
 class GetDatasetsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CODE_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
     PAGE_SIZE_FIELD_NUMBER: builtins.int
     code: builtins.str
@@ -47,26 +43,26 @@
     def __init__(
         self,
         *,
         code: builtins.str = ...,
         page: builtins.int = ...,
         page_size: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "page", b"page", "page_size", b"page_size"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["code", b"code", "page", b"page", "page_size", b"page_size"]) -> None: ...
 
 global___GetDatasetsRequest = GetDatasetsRequest
 
-@typing_extensions.final
+@typing.final
 class GetDatasetsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DatasetItem]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___DatasetItem] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetDatasetsResponse = GetDatasetsResponse
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/datasets_pb2_grpc.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/datasets_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/examples/indicator_atr.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/examples/indicator_atr.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/examples/indicator_ma.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/examples/indicator_ma.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/examples/indicator_ma_pandas.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/examples/indicator_ma_pandas.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/examples/time_series.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/examples/time_series.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/examples/time_series_pandas.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/examples/time_series_pandas.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_pb2.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: finazon_grpc_python/exchange.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,15 +16,14 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"finazon_grpc_python/exchange.proto\x12\x07\x66inazon\":\n\x17GetMarketsCryptoRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\"7\n\x19MarketsCryptoResponseItem\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"N\n\x18GetMarketsCryptoResponse\x12\x32\n\x06result\x18\x01 \x03(\x0b\x32\".finazon.MarketsCryptoResponseItem\"g\n\x17GetMarketsStocksRequest\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\x05\x12\x11\n\tpage_size\x18\x05 \x01(\x05\"G\n\x19MarketsStocksResponseItem\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\t\x12\x0b\n\x03mic\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\"N\n\x18GetMarketsStocksResponse\x12\x32\n\x06result\x18\x01 \x03(\x0b\x32\".finazon.MarketsStocksResponseItem2\xc7\x01\n\x0f\x45xchangeService\x12Y\n\x10GetMarketsCrypto\x12 .finazon.GetMarketsCryptoRequest\x1a!.finazon.GetMarketsCryptoResponse\"\x00\x12Y\n\x10GetMarketsStocks\x12 .finazon.GetMarketsStocksRequest\x1a!.finazon.GetMarketsStocksResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.exchange_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_GETMARKETSCRYPTOREQUEST']._serialized_start=47
   _globals['_GETMARKETSCRYPTOREQUEST']._serialized_end=105
   _globals['_MARKETSCRYPTORESPONSEITEM']._serialized_start=107
   _globals['_MARKETSCRYPTORESPONSEITEM']._serialized_end=162
   _globals['_GETMARKETSCRYPTORESPONSE']._serialized_start=164
   _globals['_GETMARKETSCRYPTORESPONSE']._serialized_end=242
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_pb2.pyi` & `finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class GetMarketsCryptoRequest(google.protobuf.message.Message):
     """Crypto"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PAGE_FIELD_NUMBER: builtins.int
     PAGE_SIZE_FIELD_NUMBER: builtins.int
@@ -28,53 +24,53 @@
     page_size: builtins.int
     def __init__(
         self,
         *,
         page: builtins.int = ...,
         page_size: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["page", b"page", "page_size", b"page_size"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["page", b"page", "page_size", b"page_size"]) -> None: ...
 
 global___GetMarketsCryptoRequest = GetMarketsCryptoRequest
 
-@typing_extensions.final
+@typing.final
 class MarketsCryptoResponseItem(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CODE_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     code: builtins.str
     name: builtins.str
     def __init__(
         self,
         *,
         code: builtins.str = ...,
         name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "name", b"name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["code", b"code", "name", b"name"]) -> None: ...
 
 global___MarketsCryptoResponseItem = MarketsCryptoResponseItem
 
-@typing_extensions.final
+@typing.final
 class GetMarketsCryptoResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MarketsCryptoResponseItem]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___MarketsCryptoResponseItem] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetMarketsCryptoResponse = GetMarketsCryptoResponse
 
-@typing_extensions.final
+@typing.final
 class GetMarketsStocksRequest(google.protobuf.message.Message):
     """Stocks"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COUNTRY_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
@@ -91,19 +87,19 @@
         *,
         country: builtins.str = ...,
         name: builtins.str = ...,
         code: builtins.str = ...,
         page: builtins.int = ...,
         page_size: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "country", b"country", "name", b"name", "page", b"page", "page_size", b"page_size"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["code", b"code", "country", b"country", "name", b"name", "page", b"page", "page_size", b"page_size"]) -> None: ...
 
 global___GetMarketsStocksRequest = GetMarketsStocksRequest
 
-@typing_extensions.final
+@typing.final
 class MarketsStocksResponseItem(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COUNTRY_FIELD_NUMBER: builtins.int
     MIC_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     country: builtins.str
@@ -112,26 +108,26 @@
     def __init__(
         self,
         *,
         country: builtins.str = ...,
         mic: builtins.str = ...,
         name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["country", b"country", "mic", b"mic", "name", b"name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["country", b"country", "mic", b"mic", "name", b"name"]) -> None: ...
 
 global___MarketsStocksResponseItem = MarketsStocksResponseItem
 
-@typing_extensions.final
+@typing.final
 class GetMarketsStocksResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MarketsStocksResponseItem]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___MarketsStocksResponseItem] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetMarketsStocksResponse = GetMarketsStocksResponse
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_pb2_grpc.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_service.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/forex_pb2.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/forex_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: finazon_grpc_python/forex.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66inazon_grpc_python/forex.proto\x12\x07\x66inazon\"\\\n\x0f\x46orexTimeSeries\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0c\n\x04open\x18\x02 \x01(\x01\x12\r\n\x05\x63lose\x18\x03 \x01(\x01\x12\x0c\n\x04high\x18\x04 \x01(\x01\x12\x0b\n\x03low\x18\x05 \x01(\x01\"\xad\x01\n\x19GetForexTimeSeriesRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x10\n\x08timezone\x18\x02 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08start_at\x18\x05 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x06 \x01(\x03\x12\x0c\n\x04page\x18\x07 \x01(\x05\x12\x11\n\tpage_size\x18\x08 \x01(\x05\x12\r\n\x05order\x18\t \x01(\tJ\x04\x08\x04\x10\x05R\x04\x64\x61te\"F\n\x1aGetForexTimeSeriesResponse\x12(\n\x06result\x18\x01 \x03(\x0b\x32\x18.finazon.ForexTimeSeries2j\n\x0c\x46orexService\x12Z\n\rGetTimeSeries\x12\".finazon.GetForexTimeSeriesRequest\x1a#.finazon.GetForexTimeSeriesResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66inazon_grpc_python/forex.proto\x12\x07\x66inazon\"\\\n\x0f\x46orexTimeSeries\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0c\n\x04open\x18\x02 \x01(\x01\x12\r\n\x05\x63lose\x18\x03 \x01(\x01\x12\x0c\n\x04high\x18\x04 \x01(\x01\x12\x0b\n\x03low\x18\x05 \x01(\x01\"\xab\x01\n\x19GetForexTimeSeriesRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08start_at\x18\x05 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x06 \x01(\x03\x12\x0c\n\x04page\x18\x07 \x01(\x05\x12\x11\n\tpage_size\x18\x08 \x01(\x05\x12\r\n\x05order\x18\t \x01(\tJ\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05R\x08timezoneR\x04\x64\x61te\"F\n\x1aGetForexTimeSeriesResponse\x12(\n\x06result\x18\x01 \x03(\x0b\x32\x18.finazon.ForexTimeSeries2j\n\x0c\x46orexService\x12Z\n\rGetTimeSeries\x12\".finazon.GetForexTimeSeriesRequest\x1a#.finazon.GetForexTimeSeriesResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.forex_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_FOREXTIMESERIES']._serialized_start=44
   _globals['_FOREXTIMESERIES']._serialized_end=136
   _globals['_GETFOREXTIMESERIESREQUEST']._serialized_start=139
-  _globals['_GETFOREXTIMESERIESREQUEST']._serialized_end=312
-  _globals['_GETFOREXTIMESERIESRESPONSE']._serialized_start=314
-  _globals['_GETFOREXTIMESERIESRESPONSE']._serialized_end=384
-  _globals['_FOREXSERVICE']._serialized_start=386
-  _globals['_FOREXSERVICE']._serialized_end=492
+  _globals['_GETFOREXTIMESERIESREQUEST']._serialized_end=310
+  _globals['_GETFOREXTIMESERIESRESPONSE']._serialized_start=312
+  _globals['_GETFOREXTIMESERIESRESPONSE']._serialized_end=382
+  _globals['_FOREXSERVICE']._serialized_start=384
+  _globals['_FOREXSERVICE']._serialized_end=490
 # @@protoc_insertion_point(module_scope)
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/forex_pb2.pyi` & `finazon_grpc_python-1.0.146/finazon_grpc_python/forex_pb2.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class ForexTimeSeries(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TIMESTAMP_FIELD_NUMBER: builtins.int
     OPEN_FIELD_NUMBER: builtins.int
     CLOSE_FIELD_NUMBER: builtins.int
     HIGH_FIELD_NUMBER: builtins.int
@@ -35,62 +31,59 @@
         *,
         timestamp: builtins.int = ...,
         open: builtins.float = ...,
         close: builtins.float = ...,
         high: builtins.float = ...,
         low: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["close", b"close", "high", b"high", "low", b"low", "open", b"open", "timestamp", b"timestamp"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["close", b"close", "high", b"high", "low", b"low", "open", b"open", "timestamp", b"timestamp"]) -> None: ...
 
 global___ForexTimeSeries = ForexTimeSeries
 
-@typing_extensions.final
+@typing.final
 class GetForexTimeSeriesRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
-    TIMEZONE_FIELD_NUMBER: builtins.int
     INTERVAL_FIELD_NUMBER: builtins.int
     START_AT_FIELD_NUMBER: builtins.int
     END_AT_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
     PAGE_SIZE_FIELD_NUMBER: builtins.int
     ORDER_FIELD_NUMBER: builtins.int
     ticker: builtins.str
-    timezone: builtins.str
     interval: builtins.str
     start_at: builtins.int
     end_at: builtins.int
     page: builtins.int
     page_size: builtins.int
     order: builtins.str
     def __init__(
         self,
         *,
         ticker: builtins.str = ...,
-        timezone: builtins.str = ...,
         interval: builtins.str = ...,
         start_at: builtins.int = ...,
         end_at: builtins.int = ...,
         page: builtins.int = ...,
         page_size: builtins.int = ...,
         order: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["end_at", b"end_at", "interval", b"interval", "order", b"order", "page", b"page", "page_size", b"page_size", "start_at", b"start_at", "ticker", b"ticker", "timezone", b"timezone"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["end_at", b"end_at", "interval", b"interval", "order", b"order", "page", b"page", "page_size", b"page_size", "start_at", b"start_at", "ticker", b"ticker"]) -> None: ...
 
 global___GetForexTimeSeriesRequest = GetForexTimeSeriesRequest
 
-@typing_extensions.final
+@typing.final
 class GetForexTimeSeriesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ForexTimeSeries]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___ForexTimeSeries] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetForexTimeSeriesResponse = GetForexTimeSeriesResponse
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/forex_pb2_grpc.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/forex_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/forex_service.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/forex_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_pb2.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: finazon_grpc_python/publishers.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,15 +16,14 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$finazon_grpc_python/publishers.proto\x12\x07\x66inazon\"+\n\rPublisherItem\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"E\n\x14GetPublishersRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\"?\n\x15GetPublishersResponse\x12&\n\x06result\x18\x01 \x03(\x0b\x32\x16.finazon.PublisherItem2d\n\x10PublisherService\x12P\n\rGetPublishers\x12\x1d.finazon.GetPublishersRequest\x1a\x1e.finazon.GetPublishersResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.publishers_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_PUBLISHERITEM']._serialized_start=49
   _globals['_PUBLISHERITEM']._serialized_end=92
   _globals['_GETPUBLISHERSREQUEST']._serialized_start=94
   _globals['_GETPUBLISHERSREQUEST']._serialized_end=163
   _globals['_GETPUBLISHERSRESPONSE']._serialized_start=165
   _globals['_GETPUBLISHERSRESPONSE']._serialized_end=228
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_pb2.pyi` & `finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_pb2.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class PublisherItem(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CODE_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     code: builtins.str
     name: builtins.str
     def __init__(
         self,
         *,
         code: builtins.str = ...,
         name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "name", b"name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["code", b"code", "name", b"name"]) -> None: ...
 
 global___PublisherItem = PublisherItem
 
-@typing_extensions.final
+@typing.final
 class GetPublishersRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CODE_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
     PAGE_SIZE_FIELD_NUMBER: builtins.int
     code: builtins.str
@@ -47,26 +43,26 @@
     def __init__(
         self,
         *,
         code: builtins.str = ...,
         page: builtins.int = ...,
         page_size: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "page", b"page", "page_size", b"page_size"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["code", b"code", "page", b"page", "page_size", b"page_size"]) -> None: ...
 
 global___GetPublishersRequest = GetPublishersRequest
 
-@typing_extensions.final
+@typing.final
 class GetPublishersResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___PublisherItem]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___PublisherItem] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetPublishersResponse = GetPublishersResponse
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_pb2_grpc.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_service.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/sec_pb2.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/sec_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: finazon_grpc_python/sec.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,15 +16,14 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x66inazon_grpc_python/sec.proto\x12\x07\x66inazon\"\xf9\x01\n\x15GetSecFillingsRequest\x12\x0b\n\x03\x63ik\x18\x01 \x01(\x03\x12\x0e\n\x06ticker\x18\x03 \x01(\t\x12\x11\n\tform_type\x18\x04 \x03(\t\x12\x16\n\x0e\x66illed_from_ts\x18\x05 \x01(\x03\x12\x14\n\x0c\x66illed_to_ts\x18\x06 \x01(\x03\x12\x0c\n\x04page\x18\x07 \x01(\x05\x12\x11\n\tpage_size\x18\x08 \x01(\x05\x12\x0b\n\x03\x63qs\x18\t \x01(\t\x12\r\n\x05\x63usip\x18\n \x01(\t\x12\x0c\n\x04isin\x18\x0b \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\x0c \x01(\t\x12\x12\n\nshare_figi\x18\r \x01(\t\x12\x0b\n\x03lei\x18\x0e \x01(\t\"B\n\x16GetSecFillingsResponse\x12(\n\x06result\x18\x01 \x03(\x0b\x32\x18.finazon.SecFillingsItem\"\x8e\x01\n\x0fSecFillingsItem\x12\x0e\n\x06ticker\x18\x01 \x03(\t\x12\x0b\n\x03\x63ik\x18\x02 \x01(\x03\x12\x11\n\tform_type\x18\x03 \x01(\t\x12\x10\n\x08\x66iled_at\x18\x04 \x01(\x03\x12\x12\n\nfiling_url\x18\x05 \x01(\t\x12%\n\x05\x66iles\x18\x06 \x03(\x0b\x32\x16.finazon.SecFilingFile\"F\n\rSecFilingFile\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04size\x18\x02 \x01(\x05\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0b\n\x03url\x18\x04 \x01(\t2]\n\nSecService\x12O\n\nGetFilings\x12\x1e.finazon.GetSecFillingsRequest\x1a\x1f.finazon.GetSecFillingsResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.sec_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_GETSECFILLINGSREQUEST']._serialized_start=43
   _globals['_GETSECFILLINGSREQUEST']._serialized_end=292
   _globals['_GETSECFILLINGSRESPONSE']._serialized_start=294
   _globals['_GETSECFILLINGSRESPONSE']._serialized_end=360
   _globals['_SECFILLINGSITEM']._serialized_start=363
   _globals['_SECFILLINGSITEM']._serialized_end=505
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/sec_pb2.pyi` & `finazon_grpc_python-1.0.146/finazon_grpc_python/sec_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class GetSecFillingsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CIK_FIELD_NUMBER: builtins.int
     TICKER_FIELD_NUMBER: builtins.int
     FORM_TYPE_FIELD_NUMBER: builtins.int
     FILLED_FROM_TS_FIELD_NUMBER: builtins.int
@@ -31,26 +27,26 @@
     CUSIP_FIELD_NUMBER: builtins.int
     ISIN_FIELD_NUMBER: builtins.int
     COMPOSITE_FIGI_FIELD_NUMBER: builtins.int
     SHARE_FIGI_FIELD_NUMBER: builtins.int
     LEI_FIELD_NUMBER: builtins.int
     cik: builtins.int
     ticker: builtins.str
-    @property
-    def form_type(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     filled_from_ts: builtins.int
     filled_to_ts: builtins.int
     page: builtins.int
     page_size: builtins.int
     cqs: builtins.str
     cusip: builtins.str
     isin: builtins.str
     composite_figi: builtins.str
     share_figi: builtins.str
     lei: builtins.str
+    @property
+    def form_type(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     def __init__(
         self,
         *,
         cik: builtins.int = ...,
         ticker: builtins.str = ...,
         form_type: collections.abc.Iterable[builtins.str] | None = ...,
         filled_from_ts: builtins.int = ...,
@@ -60,67 +56,67 @@
         cqs: builtins.str = ...,
         cusip: builtins.str = ...,
         isin: builtins.str = ...,
         composite_figi: builtins.str = ...,
         share_figi: builtins.str = ...,
         lei: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "composite_figi", b"composite_figi", "cqs", b"cqs", "cusip", b"cusip", "filled_from_ts", b"filled_from_ts", "filled_to_ts", b"filled_to_ts", "form_type", b"form_type", "isin", b"isin", "lei", b"lei", "page", b"page", "page_size", b"page_size", "share_figi", b"share_figi", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cik", b"cik", "composite_figi", b"composite_figi", "cqs", b"cqs", "cusip", b"cusip", "filled_from_ts", b"filled_from_ts", "filled_to_ts", b"filled_to_ts", "form_type", b"form_type", "isin", b"isin", "lei", b"lei", "page", b"page", "page_size", b"page_size", "share_figi", b"share_figi", "ticker", b"ticker"]) -> None: ...
 
 global___GetSecFillingsRequest = GetSecFillingsRequest
 
-@typing_extensions.final
+@typing.final
 class GetSecFillingsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SecFillingsItem]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___SecFillingsItem] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetSecFillingsResponse = GetSecFillingsResponse
 
-@typing_extensions.final
+@typing.final
 class SecFillingsItem(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
     CIK_FIELD_NUMBER: builtins.int
     FORM_TYPE_FIELD_NUMBER: builtins.int
     FILED_AT_FIELD_NUMBER: builtins.int
     FILING_URL_FIELD_NUMBER: builtins.int
     FILES_FIELD_NUMBER: builtins.int
-    @property
-    def ticker(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     cik: builtins.int
     form_type: builtins.str
     filed_at: builtins.int
     filing_url: builtins.str
     @property
+    def ticker(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    @property
     def files(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SecFilingFile]: ...
     def __init__(
         self,
         *,
         ticker: collections.abc.Iterable[builtins.str] | None = ...,
         cik: builtins.int = ...,
         form_type: builtins.str = ...,
         filed_at: builtins.int = ...,
         filing_url: builtins.str = ...,
         files: collections.abc.Iterable[global___SecFilingFile] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "filed_at", b"filed_at", "files", b"files", "filing_url", b"filing_url", "form_type", b"form_type", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cik", b"cik", "filed_at", b"filed_at", "files", b"files", "filing_url", b"filing_url", "form_type", b"form_type", "ticker", b"ticker"]) -> None: ...
 
 global___SecFillingsItem = SecFillingsItem
 
-@typing_extensions.final
+@typing.final
 class SecFilingFile(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     SIZE_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     URL_FIELD_NUMBER: builtins.int
@@ -132,10 +128,10 @@
         self,
         *,
         name: builtins.str = ...,
         size: builtins.int = ...,
         type: builtins.str = ...,
         url: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "size", b"size", "type", b"type", "url", b"url"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "size", b"size", "type", b"type", "url", b"url"]) -> None: ...
 
 global___SecFilingFile = SecFilingFile
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/sec_pb2_grpc.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/sec_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/sip_pb2.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/sip_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: finazon_grpc_python/sip.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,15 +16,14 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x66inazon_grpc_python/sip.proto\x12\x07\x66inazon\"\x84\x01\n\rSipTradesItem\x12\x12\n\ntrade_date\x18\x01 \x01(\x03\x12\x15\n\rmarket_center\x18\x02 \x01(\t\x12\r\n\x05topic\x18\x03 \x01(\t\x12\r\n\x05price\x18\x04 \x01(\x01\x12\x10\n\x08quantity\x18\x05 \x01(\x03\x12\x18\n\x10sales_conditions\x18\x06 \x01(\t\"\xa3\x02\n\x13GetSipTradesRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x0b\n\x03mic\x18\x02 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x03 \x01(\t\x12\x0e\n\x06market\x18\x04 \x01(\t\x12\x10\n\x08start_at\x18\x05 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x06 \x01(\x03\x12\x0c\n\x04tape\x18\x07 \x01(\t\x12\x0c\n\x04page\x18\x08 \x01(\x05\x12\x11\n\tpage_size\x18\t \x01(\x05\x12\r\n\x05order\x18\n \x01(\t\x12\x0b\n\x03\x63qs\x18\x0b \x01(\t\x12\x0b\n\x03\x63ik\x18\x0c \x01(\t\x12\r\n\x05\x63usip\x18\r \x01(\t\x12\x0c\n\x04isin\x18\x0e \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\x0f \x01(\t\x12\x12\n\nshare_figi\x18\x10 \x01(\t\x12\x0b\n\x03lei\x18\x11 \x01(\t\">\n\x14GetSipTradesResponse\x12&\n\x06result\x18\x01 \x03(\x0b\x32\x16.finazon.SipTradesItem\"\x1b\n\x19GetSipMarketCenterRequest\"1\n\x13SipMarketCenterItem\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\"J\n\x1aGetSipMarketCenterResponse\x12,\n\x06result\x18\x01 \x03(\x0b\x32\x1c.finazon.SipMarketCenterItem2\xb6\x01\n\nSipService\x12J\n\tGetTrades\x12\x1c.finazon.GetSipTradesRequest\x1a\x1d.finazon.GetSipTradesResponse\"\x00\x12\\\n\x0fGetMarketCenter\x12\".finazon.GetSipMarketCenterRequest\x1a#.finazon.GetSipMarketCenterResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.sip_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_SIPTRADESITEM']._serialized_start=43
   _globals['_SIPTRADESITEM']._serialized_end=175
   _globals['_GETSIPTRADESREQUEST']._serialized_start=178
   _globals['_GETSIPTRADESREQUEST']._serialized_end=469
   _globals['_GETSIPTRADESRESPONSE']._serialized_start=471
   _globals['_GETSIPTRADESRESPONSE']._serialized_end=533
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/sip_pb2.pyi` & `finazon_grpc_python-1.0.146/finazon_grpc_python/sip_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class SipTradesItem(google.protobuf.message.Message):
     """trades"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TRADE_DATE_FIELD_NUMBER: builtins.int
     MARKET_CENTER_FIELD_NUMBER: builtins.int
@@ -40,19 +36,19 @@
         trade_date: builtins.int = ...,
         market_center: builtins.str = ...,
         topic: builtins.str = ...,
         price: builtins.float = ...,
         quantity: builtins.int = ...,
         sales_conditions: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["market_center", b"market_center", "price", b"price", "quantity", b"quantity", "sales_conditions", b"sales_conditions", "topic", b"topic", "trade_date", b"trade_date"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["market_center", b"market_center", "price", b"price", "quantity", b"quantity", "sales_conditions", b"sales_conditions", "topic", b"topic", "trade_date", b"trade_date"]) -> None: ...
 
 global___SipTradesItem = SipTradesItem
 
-@typing_extensions.final
+@typing.final
 class GetSipTradesRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
     MIC_FIELD_NUMBER: builtins.int
     COUNTRY_FIELD_NUMBER: builtins.int
     MARKET_FIELD_NUMBER: builtins.int
@@ -103,72 +99,72 @@
         cik: builtins.str = ...,
         cusip: builtins.str = ...,
         isin: builtins.str = ...,
         composite_figi: builtins.str = ...,
         share_figi: builtins.str = ...,
         lei: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "end_at", b"end_at", "isin", b"isin", "lei", b"lei", "market", b"market", "mic", b"mic", "order", b"order", "page", b"page", "page_size", b"page_size", "share_figi", b"share_figi", "start_at", b"start_at", "tape", b"tape", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "end_at", b"end_at", "isin", b"isin", "lei", b"lei", "market", b"market", "mic", b"mic", "order", b"order", "page", b"page", "page_size", b"page_size", "share_figi", b"share_figi", "start_at", b"start_at", "tape", b"tape", "ticker", b"ticker"]) -> None: ...
 
 global___GetSipTradesRequest = GetSipTradesRequest
 
-@typing_extensions.final
+@typing.final
 class GetSipTradesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SipTradesItem]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___SipTradesItem] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetSipTradesResponse = GetSipTradesResponse
 
-@typing_extensions.final
+@typing.final
 class GetSipMarketCenterRequest(google.protobuf.message.Message):
     """market center"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___GetSipMarketCenterRequest = GetSipMarketCenterRequest
 
-@typing_extensions.final
+@typing.final
 class SipMarketCenterItem(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     CODE_FIELD_NUMBER: builtins.int
     name: builtins.str
     code: builtins.str
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         code: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "name", b"name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["code", b"code", "name", b"name"]) -> None: ...
 
 global___SipMarketCenterItem = SipMarketCenterItem
 
-@typing_extensions.final
+@typing.final
 class GetSipMarketCenterResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SipMarketCenterItem]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___SipMarketCenterItem] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetSipMarketCenterResponse = GetSipMarketCenterResponse
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/sip_pb2_grpc.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/sip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/sip_service.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/sip_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/snapshot_pb2.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/snapshot_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: finazon_grpc_python/snapshot.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,15 +16,14 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"finazon_grpc_python/snapshot.proto\x12\x07\x66inazon\"\xe6\x01\n\x12GetSnapshotRequest\x12\x11\n\tpublisher\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x0e\n\x06market\x18\x03 \x01(\t\x12\x0b\n\x03mic\x18\x04 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x05 \x01(\t\x12\x0b\n\x03\x63qs\x18\x06 \x01(\t\x12\x0b\n\x03\x63ik\x18\x07 \x01(\t\x12\r\n\x05\x63usip\x18\x08 \x01(\t\x12\x0c\n\x04isin\x18\t \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\n \x01(\t\x12\x12\n\nshare_figi\x18\x0b \x01(\t\x12\x0b\n\x03lei\x18\x0c \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\r \x01(\t\"W\n\rSnapshotOhlcv\x12\x0c\n\x04open\x18\x01 \x01(\x01\x12\x0c\n\x04high\x18\x02 \x01(\x01\x12\x0b\n\x03low\x18\x03 \x01(\x01\x12\r\n\x05\x63lose\x18\x04 \x01(\x01\x12\x0e\n\x06volume\x18\x05 \x01(\x01\"D\n\x11SnapshotLastTrade\x12\x10\n\x08\x65vent_at\x18\x01 \x01(\x03\x12\r\n\x05price\x18\x02 \x01(\x01\x12\x0e\n\x06shares\x18\x03 \x01(\x03\"\x96\x01\n\x18SnapshotLastFiftyTwoWeek\x12\x0c\n\x04high\x18\x01 \x01(\x01\x12\x0f\n\x07high_at\x18\x02 \x01(\x03\x12\x0b\n\x03low\x18\x03 \x01(\x01\x12\x0e\n\x06low_at\x18\x04 \x01(\x03\x12\x0e\n\x06\x63hange\x18\x05 \x01(\x01\x12\x16\n\x0e\x63hange_percent\x18\x06 \x01(\x01\x12\x16\n\x0e\x61verage_volume\x18\x07 \x01(\x03\"g\n\x0eSnapshotChange\x12\x1a\n\x12\x64\x61y_change_percent\x18\x01 \x01(\x01\x12\x1b\n\x13week_change_percent\x18\x02 \x01(\x01\x12\x1c\n\x14month_change_percent\x18\x03 \x01(\x01\"\xb2\x02\n\x13GetSnapshotResponse\x12(\n\x08last_day\x18\x01 \x01(\x0b\x32\x16.finazon.SnapshotOhlcv\x12*\n\nlast_month\x18\x02 \x01(\x0b\x32\x16.finazon.SnapshotOhlcv\x12.\n\nlast_trade\x18\x03 \x01(\x0b\x32\x1a.finazon.SnapshotLastTrade\x12,\n\x0cprevious_day\x18\x04 \x01(\x0b\x32\x16.finazon.SnapshotOhlcv\x12>\n\x13last_fifty_two_week\x18\x05 \x01(\x0b\x32!.finazon.SnapshotLastFiftyTwoWeek\x12\'\n\x06\x63hange\x18\x06 \x01(\x0b\x32\x17.finazon.SnapshotChange2]\n\x0fSnapshotService\x12J\n\x0bGetSnapshot\x12\x1b.finazon.GetSnapshotRequest\x1a\x1c.finazon.GetSnapshotResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.snapshot_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_GETSNAPSHOTREQUEST']._serialized_start=48
   _globals['_GETSNAPSHOTREQUEST']._serialized_end=278
   _globals['_SNAPSHOTOHLCV']._serialized_start=280
   _globals['_SNAPSHOTOHLCV']._serialized_end=367
   _globals['_SNAPSHOTLASTTRADE']._serialized_start=369
   _globals['_SNAPSHOTLASTTRADE']._serialized_end=437
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/snapshot_pb2.pyi` & `finazon_grpc_python-1.0.146/finazon_grpc_python/snapshot_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class GetSnapshotRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PUBLISHER_FIELD_NUMBER: builtins.int
     TICKER_FIELD_NUMBER: builtins.int
     MARKET_FIELD_NUMBER: builtins.int
     MIC_FIELD_NUMBER: builtins.int
@@ -57,19 +53,19 @@
         cusip: builtins.str = ...,
         isin: builtins.str = ...,
         composite_figi: builtins.str = ...,
         share_figi: builtins.str = ...,
         lei: builtins.str = ...,
         dataset: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "dataset", b"dataset", "isin", b"isin", "lei", b"lei", "market", b"market", "mic", b"mic", "publisher", b"publisher", "share_figi", b"share_figi", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "dataset", b"dataset", "isin", b"isin", "lei", b"lei", "market", b"market", "mic", b"mic", "publisher", b"publisher", "share_figi", b"share_figi", "ticker", b"ticker"]) -> None: ...
 
 global___GetSnapshotRequest = GetSnapshotRequest
 
-@typing_extensions.final
+@typing.final
 class SnapshotOhlcv(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OPEN_FIELD_NUMBER: builtins.int
     HIGH_FIELD_NUMBER: builtins.int
     LOW_FIELD_NUMBER: builtins.int
     CLOSE_FIELD_NUMBER: builtins.int
@@ -84,19 +80,19 @@
         *,
         open: builtins.float = ...,
         high: builtins.float = ...,
         low: builtins.float = ...,
         close: builtins.float = ...,
         volume: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["close", b"close", "high", b"high", "low", b"low", "open", b"open", "volume", b"volume"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["close", b"close", "high", b"high", "low", b"low", "open", b"open", "volume", b"volume"]) -> None: ...
 
 global___SnapshotOhlcv = SnapshotOhlcv
 
-@typing_extensions.final
+@typing.final
 class SnapshotLastTrade(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EVENT_AT_FIELD_NUMBER: builtins.int
     PRICE_FIELD_NUMBER: builtins.int
     SHARES_FIELD_NUMBER: builtins.int
     event_at: builtins.int
@@ -105,19 +101,19 @@
     def __init__(
         self,
         *,
         event_at: builtins.int = ...,
         price: builtins.float = ...,
         shares: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["event_at", b"event_at", "price", b"price", "shares", b"shares"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["event_at", b"event_at", "price", b"price", "shares", b"shares"]) -> None: ...
 
 global___SnapshotLastTrade = SnapshotLastTrade
 
-@typing_extensions.final
+@typing.final
 class SnapshotLastFiftyTwoWeek(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HIGH_FIELD_NUMBER: builtins.int
     HIGH_AT_FIELD_NUMBER: builtins.int
     LOW_FIELD_NUMBER: builtins.int
     LOW_AT_FIELD_NUMBER: builtins.int
@@ -138,19 +134,19 @@
         high_at: builtins.int = ...,
         low: builtins.float = ...,
         low_at: builtins.int = ...,
         change: builtins.float = ...,
         change_percent: builtins.float = ...,
         average_volume: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["average_volume", b"average_volume", "change", b"change", "change_percent", b"change_percent", "high", b"high", "high_at", b"high_at", "low", b"low", "low_at", b"low_at"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["average_volume", b"average_volume", "change", b"change", "change_percent", b"change_percent", "high", b"high", "high_at", b"high_at", "low", b"low", "low_at", b"low_at"]) -> None: ...
 
 global___SnapshotLastFiftyTwoWeek = SnapshotLastFiftyTwoWeek
 
-@typing_extensions.final
+@typing.final
 class SnapshotChange(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DAY_CHANGE_PERCENT_FIELD_NUMBER: builtins.int
     WEEK_CHANGE_PERCENT_FIELD_NUMBER: builtins.int
     MONTH_CHANGE_PERCENT_FIELD_NUMBER: builtins.int
     day_change_percent: builtins.float
@@ -159,19 +155,19 @@
     def __init__(
         self,
         *,
         day_change_percent: builtins.float = ...,
         week_change_percent: builtins.float = ...,
         month_change_percent: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["day_change_percent", b"day_change_percent", "month_change_percent", b"month_change_percent", "week_change_percent", b"week_change_percent"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["day_change_percent", b"day_change_percent", "month_change_percent", b"month_change_percent", "week_change_percent", b"week_change_percent"]) -> None: ...
 
 global___SnapshotChange = SnapshotChange
 
-@typing_extensions.final
+@typing.final
 class GetSnapshotResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LAST_DAY_FIELD_NUMBER: builtins.int
     LAST_MONTH_FIELD_NUMBER: builtins.int
     LAST_TRADE_FIELD_NUMBER: builtins.int
     PREVIOUS_DAY_FIELD_NUMBER: builtins.int
@@ -195,11 +191,11 @@
         last_day: global___SnapshotOhlcv | None = ...,
         last_month: global___SnapshotOhlcv | None = ...,
         last_trade: global___SnapshotLastTrade | None = ...,
         previous_day: global___SnapshotOhlcv | None = ...,
         last_fifty_two_week: global___SnapshotLastFiftyTwoWeek | None = ...,
         change: global___SnapshotChange | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["change", b"change", "last_day", b"last_day", "last_fifty_two_week", b"last_fifty_two_week", "last_month", b"last_month", "last_trade", b"last_trade", "previous_day", b"previous_day"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["change", b"change", "last_day", b"last_day", "last_fifty_two_week", b"last_fifty_two_week", "last_month", b"last_month", "last_trade", b"last_trade", "previous_day", b"previous_day"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["change", b"change", "last_day", b"last_day", "last_fifty_two_week", b"last_fifty_two_week", "last_month", b"last_month", "last_trade", b"last_trade", "previous_day", b"previous_day"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["change", b"change", "last_day", b"last_day", "last_fifty_two_week", b"last_fifty_two_week", "last_month", b"last_month", "last_trade", b"last_trade", "previous_day", b"previous_day"]) -> None: ...
 
 global___GetSnapshotResponse = GetSnapshotResponse
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/snapshot_pb2_grpc.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/snapshot_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_pb2.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: finazon_grpc_python/tickers.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,15 +16,14 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!finazon_grpc_python/tickers.proto\x12\x07\x66inazon\"p\n\x10TickerStocksInfo\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x02 \x01(\t\x12\x10\n\x08\x63urrency\x18\x03 \x01(\t\x12\x11\n\tpublisher\x18\x04 \x01(\t\x12\x16\n\x0epublisher_name\x18\x05 \x01(\t\"\xfd\x01\n\x18\x46indTickersStocksRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x11\n\tpublisher\x18\x02 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x03 \x01(\t\x12\x0b\n\x03mic\x18\x04 \x01(\t\x12\x0c\n\x04page\x18\x05 \x01(\x05\x12\x11\n\tpage_size\x18\x06 \x01(\x05\x12\x0b\n\x03\x63qs\x18\x0b \x01(\t\x12\x0b\n\x03\x63ik\x18\x0c \x01(\t\x12\r\n\x05\x63usip\x18\r \x01(\t\x12\x0c\n\x04isin\x18\x0e \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\x0f \x01(\t\x12\x12\n\nshare_figi\x18\x10 \x01(\t\x12\x0b\n\x03lei\x18\x11 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x12 \x01(\t\"E\n\x18\x46indTickerStocksResponse\x12)\n\x06result\x18\x01 \x03(\x0b\x32\x19.finazon.TickerStocksInfo\"M\n\x10TickerCryptoInfo\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x11\n\tpublisher\x18\x02 \x01(\t\x12\x16\n\x0epublisher_name\x18\x03 \x01(\t\"n\n\x18\x46indTickersCryptoRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x11\n\tpublisher\x18\x02 \x01(\t\x12\x0e\n\x06market\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\x05\x12\x11\n\tpage_size\x18\x05 \x01(\x05\"E\n\x18\x46indTickerCryptoResponse\x12)\n\x06result\x18\x01 \x03(\x0b\x32\x19.finazon.TickerCryptoInfo\"!\n\x0fTickerForexInfo\x12\x0e\n\x06ticker\x18\x01 \x01(\t\"J\n\x17\x46indTickersForexRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\"C\n\x17\x46indTickerForexResponse\x12(\n\x06result\x18\x01 \x03(\x0b\x32\x18.finazon.TickerForexInfo\"\xa9\x01\n\x0cTickerUSInfo\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x10\n\x08\x63urrency\x18\x02 \x01(\t\x12\x10\n\x08security\x18\x03 \x01(\t\x12\x0b\n\x03mic\x18\x04 \x01(\t\x12\x12\n\nasset_type\x18\x05 \x01(\t\x12\x0b\n\x03\x63ik\x18\x07 \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\n \x01(\t\x12\x12\n\nshare_figi\x18\x0b \x01(\t\x12\x0b\n\x03lei\x18\x0c \x01(\t\"\xc3\x01\n\x13\x46indTickerUSRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x0b\n\x03mic\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\x05\x12\x11\n\tpage_size\x18\x04 \x01(\x05\x12\x0b\n\x03\x63qs\x18\x05 \x01(\t\x12\x0b\n\x03\x63ik\x18\x06 \x01(\t\x12\r\n\x05\x63usip\x18\x07 \x01(\t\x12\x0c\n\x04isin\x18\x08 \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\t \x01(\t\x12\x12\n\nshare_figi\x18\n \x01(\t\x12\x0b\n\x03lei\x18\x0b \x01(\t\"=\n\x14\x46indTickerUSResponse\x12%\n\x06result\x18\x01 \x03(\x0b\x32\x15.finazon.TickerUSInfo2\xf3\x02\n\x0eTickersService\x12[\n\x11\x46indTickersStocks\x12!.finazon.FindTickersStocksRequest\x1a!.finazon.FindTickerStocksResponse\"\x00\x12[\n\x11\x46indTickersCrypto\x12!.finazon.FindTickersCryptoRequest\x1a!.finazon.FindTickerCryptoResponse\"\x00\x12X\n\x10\x46indTickersForex\x12 .finazon.FindTickersForexRequest\x1a .finazon.FindTickerForexResponse\"\x00\x12M\n\x0c\x46indTickerUS\x12\x1c.finazon.FindTickerUSRequest\x1a\x1d.finazon.FindTickerUSResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.tickers_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_TICKERSTOCKSINFO']._serialized_start=46
   _globals['_TICKERSTOCKSINFO']._serialized_end=158
   _globals['_FINDTICKERSSTOCKSREQUEST']._serialized_start=161
   _globals['_FINDTICKERSSTOCKSREQUEST']._serialized_end=414
   _globals['_FINDTICKERSTOCKSRESPONSE']._serialized_start=416
   _globals['_FINDTICKERSTOCKSRESPONSE']._serialized_end=485
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_pb2.pyi` & `finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class TickerStocksInfo(google.protobuf.message.Message):
     """Stocks"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
     COUNTRY_FIELD_NUMBER: builtins.int
@@ -38,19 +34,19 @@
         *,
         ticker: builtins.str = ...,
         country: builtins.str = ...,
         currency: builtins.str = ...,
         publisher: builtins.str = ...,
         publisher_name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["country", b"country", "currency", b"currency", "publisher", b"publisher", "publisher_name", b"publisher_name", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["country", b"country", "currency", b"currency", "publisher", b"publisher", "publisher_name", b"publisher_name", "ticker", b"ticker"]) -> None: ...
 
 global___TickerStocksInfo = TickerStocksInfo
 
-@typing_extensions.final
+@typing.final
 class FindTickersStocksRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
     PUBLISHER_FIELD_NUMBER: builtins.int
     COUNTRY_FIELD_NUMBER: builtins.int
     MIC_FIELD_NUMBER: builtins.int
@@ -92,35 +88,35 @@
         cusip: builtins.str = ...,
         isin: builtins.str = ...,
         composite_figi: builtins.str = ...,
         share_figi: builtins.str = ...,
         lei: builtins.str = ...,
         dataset: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "dataset", b"dataset", "isin", b"isin", "lei", b"lei", "mic", b"mic", "page", b"page", "page_size", b"page_size", "publisher", b"publisher", "share_figi", b"share_figi", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "dataset", b"dataset", "isin", b"isin", "lei", b"lei", "mic", b"mic", "page", b"page", "page_size", b"page_size", "publisher", b"publisher", "share_figi", b"share_figi", "ticker", b"ticker"]) -> None: ...
 
 global___FindTickersStocksRequest = FindTickersStocksRequest
 
-@typing_extensions.final
+@typing.final
 class FindTickerStocksResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TickerStocksInfo]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___TickerStocksInfo] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___FindTickerStocksResponse = FindTickerStocksResponse
 
-@typing_extensions.final
+@typing.final
 class TickerCryptoInfo(google.protobuf.message.Message):
     """Crypto"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
     PUBLISHER_FIELD_NUMBER: builtins.int
@@ -131,19 +127,19 @@
     def __init__(
         self,
         *,
         ticker: builtins.str = ...,
         publisher: builtins.str = ...,
         publisher_name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["publisher", b"publisher", "publisher_name", b"publisher_name", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["publisher", b"publisher", "publisher_name", b"publisher_name", "ticker", b"ticker"]) -> None: ...
 
 global___TickerCryptoInfo = TickerCryptoInfo
 
-@typing_extensions.final
+@typing.final
 class FindTickersCryptoRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
     PUBLISHER_FIELD_NUMBER: builtins.int
     MARKET_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
@@ -158,52 +154,52 @@
         *,
         ticker: builtins.str = ...,
         publisher: builtins.str = ...,
         market: builtins.str = ...,
         page: builtins.int = ...,
         page_size: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["market", b"market", "page", b"page", "page_size", b"page_size", "publisher", b"publisher", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["market", b"market", "page", b"page", "page_size", b"page_size", "publisher", b"publisher", "ticker", b"ticker"]) -> None: ...
 
 global___FindTickersCryptoRequest = FindTickersCryptoRequest
 
-@typing_extensions.final
+@typing.final
 class FindTickerCryptoResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TickerCryptoInfo]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___TickerCryptoInfo] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___FindTickerCryptoResponse = FindTickerCryptoResponse
 
-@typing_extensions.final
+@typing.final
 class TickerForexInfo(google.protobuf.message.Message):
     """Forex"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
     ticker: builtins.str
     def __init__(
         self,
         *,
         ticker: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["ticker", b"ticker"]) -> None: ...
 
 global___TickerForexInfo = TickerForexInfo
 
-@typing_extensions.final
+@typing.final
 class FindTickersForexRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
     PAGE_SIZE_FIELD_NUMBER: builtins.int
     ticker: builtins.str
@@ -212,35 +208,35 @@
     def __init__(
         self,
         *,
         ticker: builtins.str = ...,
         page: builtins.int = ...,
         page_size: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["page", b"page", "page_size", b"page_size", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["page", b"page", "page_size", b"page_size", "ticker", b"ticker"]) -> None: ...
 
 global___FindTickersForexRequest = FindTickersForexRequest
 
-@typing_extensions.final
+@typing.final
 class FindTickerForexResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TickerForexInfo]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___TickerForexInfo] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___FindTickerForexResponse = FindTickerForexResponse
 
-@typing_extensions.final
+@typing.final
 class TickerUSInfo(google.protobuf.message.Message):
     """US tickers"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
     CURRENCY_FIELD_NUMBER: builtins.int
@@ -269,19 +265,19 @@
         mic: builtins.str = ...,
         asset_type: builtins.str = ...,
         cik: builtins.str = ...,
         composite_figi: builtins.str = ...,
         share_figi: builtins.str = ...,
         lei: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["asset_type", b"asset_type", "cik", b"cik", "composite_figi", b"composite_figi", "currency", b"currency", "lei", b"lei", "mic", b"mic", "security", b"security", "share_figi", b"share_figi", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["asset_type", b"asset_type", "cik", b"cik", "composite_figi", b"composite_figi", "currency", b"currency", "lei", b"lei", "mic", b"mic", "security", b"security", "share_figi", b"share_figi", "ticker", b"ticker"]) -> None: ...
 
 global___TickerUSInfo = TickerUSInfo
 
-@typing_extensions.final
+@typing.final
 class FindTickerUSRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TICKER_FIELD_NUMBER: builtins.int
     MIC_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
     PAGE_SIZE_FIELD_NUMBER: builtins.int
@@ -314,26 +310,26 @@
         cik: builtins.str = ...,
         cusip: builtins.str = ...,
         isin: builtins.str = ...,
         composite_figi: builtins.str = ...,
         share_figi: builtins.str = ...,
         lei: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "composite_figi", b"composite_figi", "cqs", b"cqs", "cusip", b"cusip", "isin", b"isin", "lei", b"lei", "mic", b"mic", "page", b"page", "page_size", b"page_size", "share_figi", b"share_figi", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cik", b"cik", "composite_figi", b"composite_figi", "cqs", b"cqs", "cusip", b"cusip", "isin", b"isin", "lei", b"lei", "mic", b"mic", "page", b"page", "page_size", b"page_size", "share_figi", b"share_figi", "ticker", b"ticker"]) -> None: ...
 
 global___FindTickerUSRequest = FindTickerUSRequest
 
-@typing_extensions.final
+@typing.final
 class FindTickerUSResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TickerUSInfo]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___TickerUSInfo] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___FindTickerUSResponse = FindTickerUSResponse
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_pb2_grpc.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_service.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_pb2.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,86 +1,86 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: finazon_grpc_python/time_series.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%finazon_grpc_python/time_series.proto\x12\x07\x66inazon\"g\n\nTimeSeries\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0c\n\x04open\x18\x02 \x01(\x01\x12\r\n\x05\x63lose\x18\x03 \x01(\x01\x12\x0c\n\x04high\x18\x04 \x01(\x01\x12\x0b\n\x03low\x18\x05 \x01(\x01\x12\x0e\n\x06volume\x18\x06 \x01(\x01\"\xb6\x03\n\x14GetTimeSeriesRequest\x12\x11\n\tpublisher\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x10\n\x08\x65xchange\x18\x03 \x01(\t\x12\x0b\n\x03mic\x18\x04 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x05 \x01(\t\x12\x17\n\x0finstrument_type\x18\x06 \x01(\t\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12\x10\n\x08interval\x18\x08 \x01(\t\x12\x10\n\x08start_at\x18\n \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x0b \x01(\x03\x12\x0c\n\x04page\x18\x0c \x01(\x05\x12\x11\n\tpage_size\x18\r \x01(\x05\x12\r\n\x05order\x18\x0e \x01(\t\x12\x0f\n\x07prepost\x18\x0f \x01(\x08\x12\x0e\n\x06market\x18\x10 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x11 \x01(\t\x12\x0b\n\x03\x63qs\x18\x12 \x01(\t\x12\x0b\n\x03\x63ik\x18\x13 \x01(\t\x12\r\n\x05\x63usip\x18\x14 \x01(\t\x12\x0c\n\x04isin\x18\x15 \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\x16 \x01(\t\x12\x12\n\nshare_figi\x18\x17 \x01(\t\x12\x0b\n\x03lei\x18\x18 \x01(\t\x12\x0e\n\x06\x61\x64just\x18\x19 \x01(\tJ\x04\x08\t\x10\nR\x04\x64\x61te\"<\n\x15GetTimeSeriesResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.finazon.TimeSeries\"b\n\x17GetTimeSeriesAtrRequest\x12\x13\n\x0btime_period\x18\x01 \x01(\x05\x12\x32\n\x0btime_series\x18\x02 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"x\n\x18GetTimeSeriesAtrResponse\x12\x35\n\x06result\x18\x01 \x03(\x0b\x32%.finazon.GetTimeSeriesAtrResponse.Atr\x1a%\n\x03\x41tr\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0b\n\x03\x61tr\x18\x02 \x01(\t\"\x97\x01\n\x1aGetTimeSeriesBBandsRequest\x12\x13\n\x0btime_period\x18\x01 \x01(\x05\x12\x13\n\x0bseries_type\x18\x02 \x01(\t\x12\n\n\x02sd\x18\x03 \x01(\x01\x12\x0f\n\x07ma_type\x18\x04 \x01(\t\x12\x32\n\x0btime_series\x18\x05 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"\xb4\x01\n\x1bGetTimeSeriesBBandsResponse\x12;\n\x06result\x18\x01 \x03(\x0b\x32+.finazon.GetTimeSeriesBBandsResponse.BBands\x1aX\n\x06\x42\x42\x61nds\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x12\n\nupper_band\x18\x02 \x01(\t\x12\x13\n\x0bmiddle_band\x18\x03 \x01(\t\x12\x12\n\nlower_band\x18\x04 \x01(\t\"\xeb\x01\n\x1cGetTimeSeriesIchimokuRequest\x12\x1e\n\x16\x63onversion_line_period\x18\x01 \x01(\x05\x12\x18\n\x10\x62\x61se_line_period\x18\x02 \x01(\x05\x12\x1d\n\x15leading_span_b_period\x18\x03 \x01(\x05\x12\x1b\n\x13lagging_span_period\x18\x04 \x01(\x05\x12!\n\x19include_ahead_span_period\x18\x05 \x01(\x08\x12\x32\n\x0btime_series\x18\x06 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"\xea\x01\n\x1dGetTimeSeriesIchimokuResponse\x12?\n\x06result\x18\x01 \x03(\x0b\x32/.finazon.GetTimeSeriesIchimokuResponse.Ichimoku\x1a\x87\x01\n\x08Ichimoku\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x12\n\ntenkan_sen\x18\x02 \x01(\t\x12\x11\n\tkijun_sen\x18\x03 \x01(\t\x12\x15\n\rsenkou_span_a\x18\x04 \x01(\t\x12\x15\n\rsenkou_span_b\x18\x05 \x01(\t\x12\x13\n\x0b\x63hikou_span\x18\x06 \x01(\t\"\x87\x01\n\x16GetTimeSeriesMaRequest\x12\x13\n\x0btime_period\x18\x01 \x01(\x05\x12\x13\n\x0bseries_type\x18\x02 \x01(\t\x12\x0f\n\x07ma_type\x18\x03 \x01(\t\x12\x32\n\x0btime_series\x18\x04 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"s\n\x17GetTimeSeriesMaResponse\x12\x33\n\x06result\x18\x01 \x03(\x0b\x32#.finazon.GetTimeSeriesMaResponse.Ma\x1a#\n\x02Ma\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\n\n\x02ma\x18\x02 \x01(\t\"\xa4\x01\n\x18GetTimeSeriesMacdRequest\x12\x13\n\x0bseries_type\x18\x01 \x01(\t\x12\x13\n\x0b\x66\x61st_period\x18\x02 \x01(\x05\x12\x13\n\x0bslow_period\x18\x03 \x01(\x05\x12\x15\n\rsignal_period\x18\x04 \x01(\x05\x12\x32\n\x0btime_series\x18\x05 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"\xa5\x01\n\x19GetTimeSeriesMacdResponse\x12\x37\n\x06result\x18\x01 \x03(\x0b\x32\'.finazon.GetTimeSeriesMacdResponse.Macd\x1aO\n\x04Macd\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0c\n\x04macd\x18\x02 \x01(\t\x12\x13\n\x0bmacd_signal\x18\x03 \x01(\t\x12\x11\n\tmacd_hist\x18\x04 \x01(\t\"b\n\x17GetTimeSeriesObvRequest\x12\x13\n\x0bseries_type\x18\x01 \x01(\t\x12\x32\n\x0btime_series\x18\x02 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"x\n\x18GetTimeSeriesObvResponse\x12\x35\n\x06result\x18\x01 \x03(\x0b\x32%.finazon.GetTimeSeriesObvResponse.Obv\x1a%\n\x03Obv\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0b\n\x03obv\x18\x02 \x01(\t\"w\n\x17GetTimeSeriesRsiRequest\x12\x13\n\x0btime_period\x18\x01 \x01(\x05\x12\x13\n\x0bseries_type\x18\x02 \x01(\t\x12\x32\n\x0btime_series\x18\x03 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"x\n\x18GetTimeSeriesRsiResponse\x12\x35\n\x06result\x18\x01 \x03(\x0b\x32%.finazon.GetTimeSeriesRsiResponse.Rsi\x1a%\n\x03Rsi\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0b\n\x03rsi\x18\x02 \x01(\t\"t\n\x17GetTimeSeriesSarRequest\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\x01 \x01(\x01\x12\x0f\n\x07maximum\x18\x02 \x01(\x01\x12\x32\n\x0btime_series\x18\x03 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"x\n\x18GetTimeSeriesSarResponse\x12\x35\n\x06result\x18\x01 \x03(\x0b\x32%.finazon.GetTimeSeriesSarResponse.Sar\x1a%\n\x03Sar\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0b\n\x03sar\x18\x02 \x01(\t\"\xc2\x01\n\x19GetTimeSeriesStochRequest\x12\x15\n\rfast_k_period\x18\x01 \x01(\x05\x12\x15\n\rslow_k_period\x18\x02 \x01(\x05\x12\x15\n\rslow_d_period\x18\x03 \x01(\x05\x12\x15\n\rslow_kma_type\x18\x04 \x01(\t\x12\x15\n\rslow_dma_type\x18\x05 \x01(\t\x12\x32\n\x0btime_series\x18\x06 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"\x93\x01\n\x1aGetTimeSeriesStochResponse\x12\x39\n\x06result\x18\x01 \x03(\x0b\x32).finazon.GetTimeSeriesStochResponse.Stoch\x1a:\n\x05Stoch\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0e\n\x06slow_k\x18\x02 \x01(\t\x12\x0e\n\x06slow_d\x18\x03 \x01(\t2\xb6\x07\n\x11TimeSeriesService\x12P\n\rGetTimeSeries\x12\x1d.finazon.GetTimeSeriesRequest\x1a\x1e.finazon.GetTimeSeriesResponse\"\x00\x12Y\n\x10GetTimeSeriesAtr\x12 .finazon.GetTimeSeriesAtrRequest\x1a!.finazon.GetTimeSeriesAtrResponse\"\x00\x12\x62\n\x13GetTimeSeriesBBands\x12#.finazon.GetTimeSeriesBBandsRequest\x1a$.finazon.GetTimeSeriesBBandsResponse\"\x00\x12h\n\x15GetTimeSeriesIchimoku\x12%.finazon.GetTimeSeriesIchimokuRequest\x1a&.finazon.GetTimeSeriesIchimokuResponse\"\x00\x12V\n\x0fGetTimeSeriesMa\x12\x1f.finazon.GetTimeSeriesMaRequest\x1a .finazon.GetTimeSeriesMaResponse\"\x00\x12\\\n\x11GetTimeSeriesMacd\x12!.finazon.GetTimeSeriesMacdRequest\x1a\".finazon.GetTimeSeriesMacdResponse\"\x00\x12Y\n\x10GetTimeSeriesObv\x12 .finazon.GetTimeSeriesObvRequest\x1a!.finazon.GetTimeSeriesObvResponse\"\x00\x12Y\n\x10GetTimeSeriesRsi\x12 .finazon.GetTimeSeriesRsiRequest\x1a!.finazon.GetTimeSeriesRsiResponse\"\x00\x12Y\n\x10GetTimeSeriesSar\x12 .finazon.GetTimeSeriesSarRequest\x1a!.finazon.GetTimeSeriesSarResponse\"\x00\x12_\n\x12GetTimeSeriesStoch\x12\".finazon.GetTimeSeriesStochRequest\x1a#.finazon.GetTimeSeriesStochResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%finazon_grpc_python/time_series.proto\x12\x07\x66inazon\"g\n\nTimeSeries\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0c\n\x04open\x18\x02 \x01(\x01\x12\r\n\x05\x63lose\x18\x03 \x01(\x01\x12\x0c\n\x04high\x18\x04 \x01(\x01\x12\x0b\n\x03low\x18\x05 \x01(\x01\x12\x0e\n\x06volume\x18\x06 \x01(\x01\"\xb4\x03\n\x14GetTimeSeriesRequest\x12\x11\n\tpublisher\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x10\n\x08\x65xchange\x18\x03 \x01(\t\x12\x0b\n\x03mic\x18\x04 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x05 \x01(\t\x12\x17\n\x0finstrument_type\x18\x06 \x01(\t\x12\x10\n\x08interval\x18\x08 \x01(\t\x12\x10\n\x08start_at\x18\n \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x0b \x01(\x03\x12\x0c\n\x04page\x18\x0c \x01(\x05\x12\x11\n\tpage_size\x18\r \x01(\x05\x12\r\n\x05order\x18\x0e \x01(\t\x12\x0f\n\x07prepost\x18\x0f \x01(\x08\x12\x0e\n\x06market\x18\x10 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x11 \x01(\t\x12\x0b\n\x03\x63qs\x18\x12 \x01(\t\x12\x0b\n\x03\x63ik\x18\x13 \x01(\t\x12\r\n\x05\x63usip\x18\x14 \x01(\t\x12\x0c\n\x04isin\x18\x15 \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\x16 \x01(\t\x12\x12\n\nshare_figi\x18\x17 \x01(\t\x12\x0b\n\x03lei\x18\x18 \x01(\t\x12\x0e\n\x06\x61\x64just\x18\x19 \x01(\tJ\x04\x08\x07\x10\x08J\x04\x08\t\x10\nR\x08timezoneR\x04\x64\x61te\"<\n\x15GetTimeSeriesResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.finazon.TimeSeries\"b\n\x17GetTimeSeriesAtrRequest\x12\x13\n\x0btime_period\x18\x01 \x01(\x05\x12\x32\n\x0btime_series\x18\x02 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"x\n\x18GetTimeSeriesAtrResponse\x12\x35\n\x06result\x18\x01 \x03(\x0b\x32%.finazon.GetTimeSeriesAtrResponse.Atr\x1a%\n\x03\x41tr\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0b\n\x03\x61tr\x18\x02 \x01(\t\"\x97\x01\n\x1aGetTimeSeriesBBandsRequest\x12\x13\n\x0btime_period\x18\x01 \x01(\x05\x12\x13\n\x0bseries_type\x18\x02 \x01(\t\x12\n\n\x02sd\x18\x03 \x01(\x01\x12\x0f\n\x07ma_type\x18\x04 \x01(\t\x12\x32\n\x0btime_series\x18\x05 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"\xb4\x01\n\x1bGetTimeSeriesBBandsResponse\x12;\n\x06result\x18\x01 \x03(\x0b\x32+.finazon.GetTimeSeriesBBandsResponse.BBands\x1aX\n\x06\x42\x42\x61nds\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x12\n\nupper_band\x18\x02 \x01(\t\x12\x13\n\x0bmiddle_band\x18\x03 \x01(\t\x12\x12\n\nlower_band\x18\x04 \x01(\t\"\xeb\x01\n\x1cGetTimeSeriesIchimokuRequest\x12\x1e\n\x16\x63onversion_line_period\x18\x01 \x01(\x05\x12\x18\n\x10\x62\x61se_line_period\x18\x02 \x01(\x05\x12\x1d\n\x15leading_span_b_period\x18\x03 \x01(\x05\x12\x1b\n\x13lagging_span_period\x18\x04 \x01(\x05\x12!\n\x19include_ahead_span_period\x18\x05 \x01(\x08\x12\x32\n\x0btime_series\x18\x06 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"\xea\x01\n\x1dGetTimeSeriesIchimokuResponse\x12?\n\x06result\x18\x01 \x03(\x0b\x32/.finazon.GetTimeSeriesIchimokuResponse.Ichimoku\x1a\x87\x01\n\x08Ichimoku\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x12\n\ntenkan_sen\x18\x02 \x01(\t\x12\x11\n\tkijun_sen\x18\x03 \x01(\t\x12\x15\n\rsenkou_span_a\x18\x04 \x01(\t\x12\x15\n\rsenkou_span_b\x18\x05 \x01(\t\x12\x13\n\x0b\x63hikou_span\x18\x06 \x01(\t\"\x87\x01\n\x16GetTimeSeriesMaRequest\x12\x13\n\x0btime_period\x18\x01 \x01(\x05\x12\x13\n\x0bseries_type\x18\x02 \x01(\t\x12\x0f\n\x07ma_type\x18\x03 \x01(\t\x12\x32\n\x0btime_series\x18\x04 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"s\n\x17GetTimeSeriesMaResponse\x12\x33\n\x06result\x18\x01 \x03(\x0b\x32#.finazon.GetTimeSeriesMaResponse.Ma\x1a#\n\x02Ma\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\n\n\x02ma\x18\x02 \x01(\t\"\xa4\x01\n\x18GetTimeSeriesMacdRequest\x12\x13\n\x0bseries_type\x18\x01 \x01(\t\x12\x13\n\x0b\x66\x61st_period\x18\x02 \x01(\x05\x12\x13\n\x0bslow_period\x18\x03 \x01(\x05\x12\x15\n\rsignal_period\x18\x04 \x01(\x05\x12\x32\n\x0btime_series\x18\x05 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"\xa5\x01\n\x19GetTimeSeriesMacdResponse\x12\x37\n\x06result\x18\x01 \x03(\x0b\x32\'.finazon.GetTimeSeriesMacdResponse.Macd\x1aO\n\x04Macd\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0c\n\x04macd\x18\x02 \x01(\t\x12\x13\n\x0bmacd_signal\x18\x03 \x01(\t\x12\x11\n\tmacd_hist\x18\x04 \x01(\t\"b\n\x17GetTimeSeriesObvRequest\x12\x13\n\x0bseries_type\x18\x01 \x01(\t\x12\x32\n\x0btime_series\x18\x02 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"x\n\x18GetTimeSeriesObvResponse\x12\x35\n\x06result\x18\x01 \x03(\x0b\x32%.finazon.GetTimeSeriesObvResponse.Obv\x1a%\n\x03Obv\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0b\n\x03obv\x18\x02 \x01(\t\"w\n\x17GetTimeSeriesRsiRequest\x12\x13\n\x0btime_period\x18\x01 \x01(\x05\x12\x13\n\x0bseries_type\x18\x02 \x01(\t\x12\x32\n\x0btime_series\x18\x03 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"x\n\x18GetTimeSeriesRsiResponse\x12\x35\n\x06result\x18\x01 \x03(\x0b\x32%.finazon.GetTimeSeriesRsiResponse.Rsi\x1a%\n\x03Rsi\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0b\n\x03rsi\x18\x02 \x01(\t\"t\n\x17GetTimeSeriesSarRequest\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\x01 \x01(\x01\x12\x0f\n\x07maximum\x18\x02 \x01(\x01\x12\x32\n\x0btime_series\x18\x03 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"x\n\x18GetTimeSeriesSarResponse\x12\x35\n\x06result\x18\x01 \x03(\x0b\x32%.finazon.GetTimeSeriesSarResponse.Sar\x1a%\n\x03Sar\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0b\n\x03sar\x18\x02 \x01(\t\"\xc2\x01\n\x19GetTimeSeriesStochRequest\x12\x15\n\rfast_k_period\x18\x01 \x01(\x05\x12\x15\n\rslow_k_period\x18\x02 \x01(\x05\x12\x15\n\rslow_d_period\x18\x03 \x01(\x05\x12\x15\n\rslow_kma_type\x18\x04 \x01(\t\x12\x15\n\rslow_dma_type\x18\x05 \x01(\t\x12\x32\n\x0btime_series\x18\x06 \x01(\x0b\x32\x1d.finazon.GetTimeSeriesRequest\"\x93\x01\n\x1aGetTimeSeriesStochResponse\x12\x39\n\x06result\x18\x01 \x03(\x0b\x32).finazon.GetTimeSeriesStochResponse.Stoch\x1a:\n\x05Stoch\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0e\n\x06slow_k\x18\x02 \x01(\t\x12\x0e\n\x06slow_d\x18\x03 \x01(\t2\xb6\x07\n\x11TimeSeriesService\x12P\n\rGetTimeSeries\x12\x1d.finazon.GetTimeSeriesRequest\x1a\x1e.finazon.GetTimeSeriesResponse\"\x00\x12Y\n\x10GetTimeSeriesAtr\x12 .finazon.GetTimeSeriesAtrRequest\x1a!.finazon.GetTimeSeriesAtrResponse\"\x00\x12\x62\n\x13GetTimeSeriesBBands\x12#.finazon.GetTimeSeriesBBandsRequest\x1a$.finazon.GetTimeSeriesBBandsResponse\"\x00\x12h\n\x15GetTimeSeriesIchimoku\x12%.finazon.GetTimeSeriesIchimokuRequest\x1a&.finazon.GetTimeSeriesIchimokuResponse\"\x00\x12V\n\x0fGetTimeSeriesMa\x12\x1f.finazon.GetTimeSeriesMaRequest\x1a .finazon.GetTimeSeriesMaResponse\"\x00\x12\\\n\x11GetTimeSeriesMacd\x12!.finazon.GetTimeSeriesMacdRequest\x1a\".finazon.GetTimeSeriesMacdResponse\"\x00\x12Y\n\x10GetTimeSeriesObv\x12 .finazon.GetTimeSeriesObvRequest\x1a!.finazon.GetTimeSeriesObvResponse\"\x00\x12Y\n\x10GetTimeSeriesRsi\x12 .finazon.GetTimeSeriesRsiRequest\x1a!.finazon.GetTimeSeriesRsiResponse\"\x00\x12Y\n\x10GetTimeSeriesSar\x12 .finazon.GetTimeSeriesSarRequest\x1a!.finazon.GetTimeSeriesSarResponse\"\x00\x12_\n\x12GetTimeSeriesStoch\x12\".finazon.GetTimeSeriesStochRequest\x1a#.finazon.GetTimeSeriesStochResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.time_series_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_TIMESERIES']._serialized_start=50
   _globals['_TIMESERIES']._serialized_end=153
   _globals['_GETTIMESERIESREQUEST']._serialized_start=156
-  _globals['_GETTIMESERIESREQUEST']._serialized_end=594
-  _globals['_GETTIMESERIESRESPONSE']._serialized_start=596
-  _globals['_GETTIMESERIESRESPONSE']._serialized_end=656
-  _globals['_GETTIMESERIESATRREQUEST']._serialized_start=658
-  _globals['_GETTIMESERIESATRREQUEST']._serialized_end=756
-  _globals['_GETTIMESERIESATRRESPONSE']._serialized_start=758
-  _globals['_GETTIMESERIESATRRESPONSE']._serialized_end=878
-  _globals['_GETTIMESERIESATRRESPONSE_ATR']._serialized_start=841
-  _globals['_GETTIMESERIESATRRESPONSE_ATR']._serialized_end=878
-  _globals['_GETTIMESERIESBBANDSREQUEST']._serialized_start=881
-  _globals['_GETTIMESERIESBBANDSREQUEST']._serialized_end=1032
-  _globals['_GETTIMESERIESBBANDSRESPONSE']._serialized_start=1035
-  _globals['_GETTIMESERIESBBANDSRESPONSE']._serialized_end=1215
-  _globals['_GETTIMESERIESBBANDSRESPONSE_BBANDS']._serialized_start=1127
-  _globals['_GETTIMESERIESBBANDSRESPONSE_BBANDS']._serialized_end=1215
-  _globals['_GETTIMESERIESICHIMOKUREQUEST']._serialized_start=1218
-  _globals['_GETTIMESERIESICHIMOKUREQUEST']._serialized_end=1453
-  _globals['_GETTIMESERIESICHIMOKURESPONSE']._serialized_start=1456
-  _globals['_GETTIMESERIESICHIMOKURESPONSE']._serialized_end=1690
-  _globals['_GETTIMESERIESICHIMOKURESPONSE_ICHIMOKU']._serialized_start=1555
-  _globals['_GETTIMESERIESICHIMOKURESPONSE_ICHIMOKU']._serialized_end=1690
-  _globals['_GETTIMESERIESMAREQUEST']._serialized_start=1693
-  _globals['_GETTIMESERIESMAREQUEST']._serialized_end=1828
-  _globals['_GETTIMESERIESMARESPONSE']._serialized_start=1830
-  _globals['_GETTIMESERIESMARESPONSE']._serialized_end=1945
-  _globals['_GETTIMESERIESMARESPONSE_MA']._serialized_start=1910
-  _globals['_GETTIMESERIESMARESPONSE_MA']._serialized_end=1945
-  _globals['_GETTIMESERIESMACDREQUEST']._serialized_start=1948
-  _globals['_GETTIMESERIESMACDREQUEST']._serialized_end=2112
-  _globals['_GETTIMESERIESMACDRESPONSE']._serialized_start=2115
-  _globals['_GETTIMESERIESMACDRESPONSE']._serialized_end=2280
-  _globals['_GETTIMESERIESMACDRESPONSE_MACD']._serialized_start=2201
-  _globals['_GETTIMESERIESMACDRESPONSE_MACD']._serialized_end=2280
-  _globals['_GETTIMESERIESOBVREQUEST']._serialized_start=2282
-  _globals['_GETTIMESERIESOBVREQUEST']._serialized_end=2380
-  _globals['_GETTIMESERIESOBVRESPONSE']._serialized_start=2382
-  _globals['_GETTIMESERIESOBVRESPONSE']._serialized_end=2502
-  _globals['_GETTIMESERIESOBVRESPONSE_OBV']._serialized_start=2465
-  _globals['_GETTIMESERIESOBVRESPONSE_OBV']._serialized_end=2502
-  _globals['_GETTIMESERIESRSIREQUEST']._serialized_start=2504
-  _globals['_GETTIMESERIESRSIREQUEST']._serialized_end=2623
-  _globals['_GETTIMESERIESRSIRESPONSE']._serialized_start=2625
-  _globals['_GETTIMESERIESRSIRESPONSE']._serialized_end=2745
-  _globals['_GETTIMESERIESRSIRESPONSE_RSI']._serialized_start=2708
-  _globals['_GETTIMESERIESRSIRESPONSE_RSI']._serialized_end=2745
-  _globals['_GETTIMESERIESSARREQUEST']._serialized_start=2747
-  _globals['_GETTIMESERIESSARREQUEST']._serialized_end=2863
-  _globals['_GETTIMESERIESSARRESPONSE']._serialized_start=2865
-  _globals['_GETTIMESERIESSARRESPONSE']._serialized_end=2985
-  _globals['_GETTIMESERIESSARRESPONSE_SAR']._serialized_start=2948
-  _globals['_GETTIMESERIESSARRESPONSE_SAR']._serialized_end=2985
-  _globals['_GETTIMESERIESSTOCHREQUEST']._serialized_start=2988
-  _globals['_GETTIMESERIESSTOCHREQUEST']._serialized_end=3182
-  _globals['_GETTIMESERIESSTOCHRESPONSE']._serialized_start=3185
-  _globals['_GETTIMESERIESSTOCHRESPONSE']._serialized_end=3332
-  _globals['_GETTIMESERIESSTOCHRESPONSE_STOCH']._serialized_start=3274
-  _globals['_GETTIMESERIESSTOCHRESPONSE_STOCH']._serialized_end=3332
-  _globals['_TIMESERIESSERVICE']._serialized_start=3335
-  _globals['_TIMESERIESSERVICE']._serialized_end=4285
+  _globals['_GETTIMESERIESREQUEST']._serialized_end=592
+  _globals['_GETTIMESERIESRESPONSE']._serialized_start=594
+  _globals['_GETTIMESERIESRESPONSE']._serialized_end=654
+  _globals['_GETTIMESERIESATRREQUEST']._serialized_start=656
+  _globals['_GETTIMESERIESATRREQUEST']._serialized_end=754
+  _globals['_GETTIMESERIESATRRESPONSE']._serialized_start=756
+  _globals['_GETTIMESERIESATRRESPONSE']._serialized_end=876
+  _globals['_GETTIMESERIESATRRESPONSE_ATR']._serialized_start=839
+  _globals['_GETTIMESERIESATRRESPONSE_ATR']._serialized_end=876
+  _globals['_GETTIMESERIESBBANDSREQUEST']._serialized_start=879
+  _globals['_GETTIMESERIESBBANDSREQUEST']._serialized_end=1030
+  _globals['_GETTIMESERIESBBANDSRESPONSE']._serialized_start=1033
+  _globals['_GETTIMESERIESBBANDSRESPONSE']._serialized_end=1213
+  _globals['_GETTIMESERIESBBANDSRESPONSE_BBANDS']._serialized_start=1125
+  _globals['_GETTIMESERIESBBANDSRESPONSE_BBANDS']._serialized_end=1213
+  _globals['_GETTIMESERIESICHIMOKUREQUEST']._serialized_start=1216
+  _globals['_GETTIMESERIESICHIMOKUREQUEST']._serialized_end=1451
+  _globals['_GETTIMESERIESICHIMOKURESPONSE']._serialized_start=1454
+  _globals['_GETTIMESERIESICHIMOKURESPONSE']._serialized_end=1688
+  _globals['_GETTIMESERIESICHIMOKURESPONSE_ICHIMOKU']._serialized_start=1553
+  _globals['_GETTIMESERIESICHIMOKURESPONSE_ICHIMOKU']._serialized_end=1688
+  _globals['_GETTIMESERIESMAREQUEST']._serialized_start=1691
+  _globals['_GETTIMESERIESMAREQUEST']._serialized_end=1826
+  _globals['_GETTIMESERIESMARESPONSE']._serialized_start=1828
+  _globals['_GETTIMESERIESMARESPONSE']._serialized_end=1943
+  _globals['_GETTIMESERIESMARESPONSE_MA']._serialized_start=1908
+  _globals['_GETTIMESERIESMARESPONSE_MA']._serialized_end=1943
+  _globals['_GETTIMESERIESMACDREQUEST']._serialized_start=1946
+  _globals['_GETTIMESERIESMACDREQUEST']._serialized_end=2110
+  _globals['_GETTIMESERIESMACDRESPONSE']._serialized_start=2113
+  _globals['_GETTIMESERIESMACDRESPONSE']._serialized_end=2278
+  _globals['_GETTIMESERIESMACDRESPONSE_MACD']._serialized_start=2199
+  _globals['_GETTIMESERIESMACDRESPONSE_MACD']._serialized_end=2278
+  _globals['_GETTIMESERIESOBVREQUEST']._serialized_start=2280
+  _globals['_GETTIMESERIESOBVREQUEST']._serialized_end=2378
+  _globals['_GETTIMESERIESOBVRESPONSE']._serialized_start=2380
+  _globals['_GETTIMESERIESOBVRESPONSE']._serialized_end=2500
+  _globals['_GETTIMESERIESOBVRESPONSE_OBV']._serialized_start=2463
+  _globals['_GETTIMESERIESOBVRESPONSE_OBV']._serialized_end=2500
+  _globals['_GETTIMESERIESRSIREQUEST']._serialized_start=2502
+  _globals['_GETTIMESERIESRSIREQUEST']._serialized_end=2621
+  _globals['_GETTIMESERIESRSIRESPONSE']._serialized_start=2623
+  _globals['_GETTIMESERIESRSIRESPONSE']._serialized_end=2743
+  _globals['_GETTIMESERIESRSIRESPONSE_RSI']._serialized_start=2706
+  _globals['_GETTIMESERIESRSIRESPONSE_RSI']._serialized_end=2743
+  _globals['_GETTIMESERIESSARREQUEST']._serialized_start=2745
+  _globals['_GETTIMESERIESSARREQUEST']._serialized_end=2861
+  _globals['_GETTIMESERIESSARRESPONSE']._serialized_start=2863
+  _globals['_GETTIMESERIESSARRESPONSE']._serialized_end=2983
+  _globals['_GETTIMESERIESSARRESPONSE_SAR']._serialized_start=2946
+  _globals['_GETTIMESERIESSARRESPONSE_SAR']._serialized_end=2983
+  _globals['_GETTIMESERIESSTOCHREQUEST']._serialized_start=2986
+  _globals['_GETTIMESERIESSTOCHREQUEST']._serialized_end=3180
+  _globals['_GETTIMESERIESSTOCHRESPONSE']._serialized_start=3183
+  _globals['_GETTIMESERIESSTOCHRESPONSE']._serialized_end=3330
+  _globals['_GETTIMESERIESSTOCHRESPONSE_STOCH']._serialized_start=3272
+  _globals['_GETTIMESERIESSTOCHRESPONSE_STOCH']._serialized_end=3330
+  _globals['_TIMESERIESSERVICE']._serialized_start=3333
+  _globals['_TIMESERIESSERVICE']._serialized_end=4283
 # @@protoc_insertion_point(module_scope)
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_pb2.pyi` & `finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class TimeSeries(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TIMESTAMP_FIELD_NUMBER: builtins.int
     OPEN_FIELD_NUMBER: builtins.int
     CLOSE_FIELD_NUMBER: builtins.int
     HIGH_FIELD_NUMBER: builtins.int
@@ -38,29 +34,28 @@
         timestamp: builtins.int = ...,
         open: builtins.float = ...,
         close: builtins.float = ...,
         high: builtins.float = ...,
         low: builtins.float = ...,
         volume: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["close", b"close", "high", b"high", "low", b"low", "open", b"open", "timestamp", b"timestamp", "volume", b"volume"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["close", b"close", "high", b"high", "low", b"low", "open", b"open", "timestamp", b"timestamp", "volume", b"volume"]) -> None: ...
 
 global___TimeSeries = TimeSeries
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PUBLISHER_FIELD_NUMBER: builtins.int
     TICKER_FIELD_NUMBER: builtins.int
     EXCHANGE_FIELD_NUMBER: builtins.int
     MIC_FIELD_NUMBER: builtins.int
     COUNTRY_FIELD_NUMBER: builtins.int
     INSTRUMENT_TYPE_FIELD_NUMBER: builtins.int
-    TIMEZONE_FIELD_NUMBER: builtins.int
     INTERVAL_FIELD_NUMBER: builtins.int
     START_AT_FIELD_NUMBER: builtins.int
     END_AT_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
     PAGE_SIZE_FIELD_NUMBER: builtins.int
     ORDER_FIELD_NUMBER: builtins.int
     PREPOST_FIELD_NUMBER: builtins.int
@@ -76,15 +71,14 @@
     ADJUST_FIELD_NUMBER: builtins.int
     publisher: builtins.str
     ticker: builtins.str
     exchange: builtins.str
     mic: builtins.str
     country: builtins.str
     instrument_type: builtins.str
-    timezone: builtins.str
     interval: builtins.str
     start_at: builtins.int
     end_at: builtins.int
     page: builtins.int
     page_size: builtins.int
     order: builtins.str
     prepost: builtins.bool
@@ -103,15 +97,14 @@
         *,
         publisher: builtins.str = ...,
         ticker: builtins.str = ...,
         exchange: builtins.str = ...,
         mic: builtins.str = ...,
         country: builtins.str = ...,
         instrument_type: builtins.str = ...,
-        timezone: builtins.str = ...,
         interval: builtins.str = ...,
         start_at: builtins.int = ...,
         end_at: builtins.int = ...,
         page: builtins.int = ...,
         page_size: builtins.int = ...,
         order: builtins.str = ...,
         prepost: builtins.bool = ...,
@@ -122,87 +115,87 @@
         cusip: builtins.str = ...,
         isin: builtins.str = ...,
         composite_figi: builtins.str = ...,
         share_figi: builtins.str = ...,
         lei: builtins.str = ...,
         adjust: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["adjust", b"adjust", "cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "dataset", b"dataset", "end_at", b"end_at", "exchange", b"exchange", "instrument_type", b"instrument_type", "interval", b"interval", "isin", b"isin", "lei", b"lei", "market", b"market", "mic", b"mic", "order", b"order", "page", b"page", "page_size", b"page_size", "prepost", b"prepost", "publisher", b"publisher", "share_figi", b"share_figi", "start_at", b"start_at", "ticker", b"ticker", "timezone", b"timezone"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["adjust", b"adjust", "cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "dataset", b"dataset", "end_at", b"end_at", "exchange", b"exchange", "instrument_type", b"instrument_type", "interval", b"interval", "isin", b"isin", "lei", b"lei", "market", b"market", "mic", b"mic", "order", b"order", "page", b"page", "page_size", b"page_size", "prepost", b"prepost", "publisher", b"publisher", "share_figi", b"share_figi", "start_at", b"start_at", "ticker", b"ticker"]) -> None: ...
 
 global___GetTimeSeriesRequest = GetTimeSeriesRequest
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TimeSeries]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___TimeSeries] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetTimeSeriesResponse = GetTimeSeriesResponse
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesAtrRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TIME_PERIOD_FIELD_NUMBER: builtins.int
     TIME_SERIES_FIELD_NUMBER: builtins.int
     time_period: builtins.int
     @property
     def time_series(self) -> global___GetTimeSeriesRequest: ...
     def __init__(
         self,
         *,
         time_period: builtins.int = ...,
         time_series: global___GetTimeSeriesRequest | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["time_series", b"time_series"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["time_period", b"time_period", "time_series", b"time_series"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["time_series", b"time_series"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["time_period", b"time_period", "time_series", b"time_series"]) -> None: ...
 
 global___GetTimeSeriesAtrRequest = GetTimeSeriesAtrRequest
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesAtrResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Atr(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         TIMESTAMP_FIELD_NUMBER: builtins.int
         ATR_FIELD_NUMBER: builtins.int
         timestamp: builtins.int
         atr: builtins.str
         def __init__(
             self,
             *,
             timestamp: builtins.int = ...,
             atr: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["atr", b"atr", "timestamp", b"timestamp"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["atr", b"atr", "timestamp", b"timestamp"]) -> None: ...
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GetTimeSeriesAtrResponse.Atr]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___GetTimeSeriesAtrResponse.Atr] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetTimeSeriesAtrResponse = GetTimeSeriesAtrResponse
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesBBandsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TIME_PERIOD_FIELD_NUMBER: builtins.int
     SERIES_TYPE_FIELD_NUMBER: builtins.int
     SD_FIELD_NUMBER: builtins.int
     MA_TYPE_FIELD_NUMBER: builtins.int
@@ -218,24 +211,24 @@
         *,
         time_period: builtins.int = ...,
         series_type: builtins.str = ...,
         sd: builtins.float = ...,
         ma_type: builtins.str = ...,
         time_series: global___GetTimeSeriesRequest | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["time_series", b"time_series"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["ma_type", b"ma_type", "sd", b"sd", "series_type", b"series_type", "time_period", b"time_period", "time_series", b"time_series"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["time_series", b"time_series"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["ma_type", b"ma_type", "sd", b"sd", "series_type", b"series_type", "time_period", b"time_period", "time_series", b"time_series"]) -> None: ...
 
 global___GetTimeSeriesBBandsRequest = GetTimeSeriesBBandsRequest
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesBBandsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class BBands(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         TIMESTAMP_FIELD_NUMBER: builtins.int
         UPPER_BAND_FIELD_NUMBER: builtins.int
         MIDDLE_BAND_FIELD_NUMBER: builtins.int
         LOWER_BAND_FIELD_NUMBER: builtins.int
@@ -247,29 +240,29 @@
             self,
             *,
             timestamp: builtins.int = ...,
             upper_band: builtins.str = ...,
             middle_band: builtins.str = ...,
             lower_band: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["lower_band", b"lower_band", "middle_band", b"middle_band", "timestamp", b"timestamp", "upper_band", b"upper_band"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["lower_band", b"lower_band", "middle_band", b"middle_band", "timestamp", b"timestamp", "upper_band", b"upper_band"]) -> None: ...
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GetTimeSeriesBBandsResponse.BBands]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___GetTimeSeriesBBandsResponse.BBands] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetTimeSeriesBBandsResponse = GetTimeSeriesBBandsResponse
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesIchimokuRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONVERSION_LINE_PERIOD_FIELD_NUMBER: builtins.int
     BASE_LINE_PERIOD_FIELD_NUMBER: builtins.int
     LEADING_SPAN_B_PERIOD_FIELD_NUMBER: builtins.int
     LAGGING_SPAN_PERIOD_FIELD_NUMBER: builtins.int
@@ -288,24 +281,24 @@
         conversion_line_period: builtins.int = ...,
         base_line_period: builtins.int = ...,
         leading_span_b_period: builtins.int = ...,
         lagging_span_period: builtins.int = ...,
         include_ahead_span_period: builtins.bool = ...,
         time_series: global___GetTimeSeriesRequest | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["time_series", b"time_series"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["base_line_period", b"base_line_period", "conversion_line_period", b"conversion_line_period", "include_ahead_span_period", b"include_ahead_span_period", "lagging_span_period", b"lagging_span_period", "leading_span_b_period", b"leading_span_b_period", "time_series", b"time_series"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["time_series", b"time_series"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["base_line_period", b"base_line_period", "conversion_line_period", b"conversion_line_period", "include_ahead_span_period", b"include_ahead_span_period", "lagging_span_period", b"lagging_span_period", "leading_span_b_period", b"leading_span_b_period", "time_series", b"time_series"]) -> None: ...
 
 global___GetTimeSeriesIchimokuRequest = GetTimeSeriesIchimokuRequest
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesIchimokuResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Ichimoku(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         TIMESTAMP_FIELD_NUMBER: builtins.int
         TENKAN_SEN_FIELD_NUMBER: builtins.int
         KIJUN_SEN_FIELD_NUMBER: builtins.int
         SENKOU_SPAN_A_FIELD_NUMBER: builtins.int
@@ -323,29 +316,29 @@
             timestamp: builtins.int = ...,
             tenkan_sen: builtins.str = ...,
             kijun_sen: builtins.str = ...,
             senkou_span_a: builtins.str = ...,
             senkou_span_b: builtins.str = ...,
             chikou_span: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["chikou_span", b"chikou_span", "kijun_sen", b"kijun_sen", "senkou_span_a", b"senkou_span_a", "senkou_span_b", b"senkou_span_b", "tenkan_sen", b"tenkan_sen", "timestamp", b"timestamp"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["chikou_span", b"chikou_span", "kijun_sen", b"kijun_sen", "senkou_span_a", b"senkou_span_a", "senkou_span_b", b"senkou_span_b", "tenkan_sen", b"tenkan_sen", "timestamp", b"timestamp"]) -> None: ...
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GetTimeSeriesIchimokuResponse.Ichimoku]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___GetTimeSeriesIchimokuResponse.Ichimoku] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetTimeSeriesIchimokuResponse = GetTimeSeriesIchimokuResponse
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesMaRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TIME_PERIOD_FIELD_NUMBER: builtins.int
     SERIES_TYPE_FIELD_NUMBER: builtins.int
     MA_TYPE_FIELD_NUMBER: builtins.int
     TIME_SERIES_FIELD_NUMBER: builtins.int
@@ -358,52 +351,52 @@
         self,
         *,
         time_period: builtins.int = ...,
         series_type: builtins.str = ...,
         ma_type: builtins.str = ...,
         time_series: global___GetTimeSeriesRequest | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["time_series", b"time_series"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["ma_type", b"ma_type", "series_type", b"series_type", "time_period", b"time_period", "time_series", b"time_series"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["time_series", b"time_series"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["ma_type", b"ma_type", "series_type", b"series_type", "time_period", b"time_period", "time_series", b"time_series"]) -> None: ...
 
 global___GetTimeSeriesMaRequest = GetTimeSeriesMaRequest
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesMaResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Ma(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         TIMESTAMP_FIELD_NUMBER: builtins.int
         MA_FIELD_NUMBER: builtins.int
         timestamp: builtins.int
         ma: builtins.str
         def __init__(
             self,
             *,
             timestamp: builtins.int = ...,
             ma: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["ma", b"ma", "timestamp", b"timestamp"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["ma", b"ma", "timestamp", b"timestamp"]) -> None: ...
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GetTimeSeriesMaResponse.Ma]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___GetTimeSeriesMaResponse.Ma] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetTimeSeriesMaResponse = GetTimeSeriesMaResponse
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesMacdRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SERIES_TYPE_FIELD_NUMBER: builtins.int
     FAST_PERIOD_FIELD_NUMBER: builtins.int
     SLOW_PERIOD_FIELD_NUMBER: builtins.int
     SIGNAL_PERIOD_FIELD_NUMBER: builtins.int
@@ -419,24 +412,24 @@
         *,
         series_type: builtins.str = ...,
         fast_period: builtins.int = ...,
         slow_period: builtins.int = ...,
         signal_period: builtins.int = ...,
         time_series: global___GetTimeSeriesRequest | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["time_series", b"time_series"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["fast_period", b"fast_period", "series_type", b"series_type", "signal_period", b"signal_period", "slow_period", b"slow_period", "time_series", b"time_series"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["time_series", b"time_series"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["fast_period", b"fast_period", "series_type", b"series_type", "signal_period", b"signal_period", "slow_period", b"slow_period", "time_series", b"time_series"]) -> None: ...
 
 global___GetTimeSeriesMacdRequest = GetTimeSeriesMacdRequest
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesMacdResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Macd(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         TIMESTAMP_FIELD_NUMBER: builtins.int
         MACD_FIELD_NUMBER: builtins.int
         MACD_SIGNAL_FIELD_NUMBER: builtins.int
         MACD_HIST_FIELD_NUMBER: builtins.int
@@ -448,81 +441,81 @@
             self,
             *,
             timestamp: builtins.int = ...,
             macd: builtins.str = ...,
             macd_signal: builtins.str = ...,
             macd_hist: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["macd", b"macd", "macd_hist", b"macd_hist", "macd_signal", b"macd_signal", "timestamp", b"timestamp"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["macd", b"macd", "macd_hist", b"macd_hist", "macd_signal", b"macd_signal", "timestamp", b"timestamp"]) -> None: ...
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GetTimeSeriesMacdResponse.Macd]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___GetTimeSeriesMacdResponse.Macd] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetTimeSeriesMacdResponse = GetTimeSeriesMacdResponse
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesObvRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SERIES_TYPE_FIELD_NUMBER: builtins.int
     TIME_SERIES_FIELD_NUMBER: builtins.int
     series_type: builtins.str
     @property
     def time_series(self) -> global___GetTimeSeriesRequest: ...
     def __init__(
         self,
         *,
         series_type: builtins.str = ...,
         time_series: global___GetTimeSeriesRequest | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["time_series", b"time_series"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["series_type", b"series_type", "time_series", b"time_series"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["time_series", b"time_series"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["series_type", b"series_type", "time_series", b"time_series"]) -> None: ...
 
 global___GetTimeSeriesObvRequest = GetTimeSeriesObvRequest
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesObvResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Obv(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         TIMESTAMP_FIELD_NUMBER: builtins.int
         OBV_FIELD_NUMBER: builtins.int
         timestamp: builtins.int
         obv: builtins.str
         def __init__(
             self,
             *,
             timestamp: builtins.int = ...,
             obv: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["obv", b"obv", "timestamp", b"timestamp"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["obv", b"obv", "timestamp", b"timestamp"]) -> None: ...
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GetTimeSeriesObvResponse.Obv]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___GetTimeSeriesObvResponse.Obv] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetTimeSeriesObvResponse = GetTimeSeriesObvResponse
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesRsiRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TIME_PERIOD_FIELD_NUMBER: builtins.int
     SERIES_TYPE_FIELD_NUMBER: builtins.int
     TIME_SERIES_FIELD_NUMBER: builtins.int
     time_period: builtins.int
@@ -532,52 +525,52 @@
     def __init__(
         self,
         *,
         time_period: builtins.int = ...,
         series_type: builtins.str = ...,
         time_series: global___GetTimeSeriesRequest | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["time_series", b"time_series"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["series_type", b"series_type", "time_period", b"time_period", "time_series", b"time_series"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["time_series", b"time_series"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["series_type", b"series_type", "time_period", b"time_period", "time_series", b"time_series"]) -> None: ...
 
 global___GetTimeSeriesRsiRequest = GetTimeSeriesRsiRequest
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesRsiResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Rsi(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         TIMESTAMP_FIELD_NUMBER: builtins.int
         RSI_FIELD_NUMBER: builtins.int
         timestamp: builtins.int
         rsi: builtins.str
         def __init__(
             self,
             *,
             timestamp: builtins.int = ...,
             rsi: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["rsi", b"rsi", "timestamp", b"timestamp"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["rsi", b"rsi", "timestamp", b"timestamp"]) -> None: ...
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GetTimeSeriesRsiResponse.Rsi]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___GetTimeSeriesRsiResponse.Rsi] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetTimeSeriesRsiResponse = GetTimeSeriesRsiResponse
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesSarRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ACCELERATION_FIELD_NUMBER: builtins.int
     MAXIMUM_FIELD_NUMBER: builtins.int
     TIME_SERIES_FIELD_NUMBER: builtins.int
     acceleration: builtins.float
@@ -587,52 +580,52 @@
     def __init__(
         self,
         *,
         acceleration: builtins.float = ...,
         maximum: builtins.float = ...,
         time_series: global___GetTimeSeriesRequest | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["time_series", b"time_series"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["acceleration", b"acceleration", "maximum", b"maximum", "time_series", b"time_series"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["time_series", b"time_series"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["acceleration", b"acceleration", "maximum", b"maximum", "time_series", b"time_series"]) -> None: ...
 
 global___GetTimeSeriesSarRequest = GetTimeSeriesSarRequest
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesSarResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Sar(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         TIMESTAMP_FIELD_NUMBER: builtins.int
         SAR_FIELD_NUMBER: builtins.int
         timestamp: builtins.int
         sar: builtins.str
         def __init__(
             self,
             *,
             timestamp: builtins.int = ...,
             sar: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["sar", b"sar", "timestamp", b"timestamp"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["sar", b"sar", "timestamp", b"timestamp"]) -> None: ...
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GetTimeSeriesSarResponse.Sar]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___GetTimeSeriesSarResponse.Sar] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetTimeSeriesSarResponse = GetTimeSeriesSarResponse
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesStochRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FAST_K_PERIOD_FIELD_NUMBER: builtins.int
     SLOW_K_PERIOD_FIELD_NUMBER: builtins.int
     SLOW_D_PERIOD_FIELD_NUMBER: builtins.int
     SLOW_KMA_TYPE_FIELD_NUMBER: builtins.int
@@ -651,24 +644,24 @@
         fast_k_period: builtins.int = ...,
         slow_k_period: builtins.int = ...,
         slow_d_period: builtins.int = ...,
         slow_kma_type: builtins.str = ...,
         slow_dma_type: builtins.str = ...,
         time_series: global___GetTimeSeriesRequest | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["time_series", b"time_series"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["fast_k_period", b"fast_k_period", "slow_d_period", b"slow_d_period", "slow_dma_type", b"slow_dma_type", "slow_k_period", b"slow_k_period", "slow_kma_type", b"slow_kma_type", "time_series", b"time_series"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["time_series", b"time_series"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["fast_k_period", b"fast_k_period", "slow_d_period", b"slow_d_period", "slow_dma_type", b"slow_dma_type", "slow_k_period", b"slow_k_period", "slow_kma_type", b"slow_kma_type", "time_series", b"time_series"]) -> None: ...
 
 global___GetTimeSeriesStochRequest = GetTimeSeriesStochRequest
 
-@typing_extensions.final
+@typing.final
 class GetTimeSeriesStochResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Stoch(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         TIMESTAMP_FIELD_NUMBER: builtins.int
         SLOW_K_FIELD_NUMBER: builtins.int
         SLOW_D_FIELD_NUMBER: builtins.int
         timestamp: builtins.int
@@ -677,20 +670,20 @@
         def __init__(
             self,
             *,
             timestamp: builtins.int = ...,
             slow_k: builtins.str = ...,
             slow_d: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["slow_d", b"slow_d", "slow_k", b"slow_k", "timestamp", b"timestamp"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["slow_d", b"slow_d", "slow_k", b"slow_k", "timestamp", b"timestamp"]) -> None: ...
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GetTimeSeriesStochResponse.Stoch]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___GetTimeSeriesStochResponse.Stoch] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetTimeSeriesStochResponse = GetTimeSeriesStochResponse
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_pb2_grpc.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_service.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/trade_pb2.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/trade_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: finazon_grpc_python/trade.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,15 +16,14 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66inazon_grpc_python/trade.proto\x12\x07\x66inazon\"A\n\nTradesItem\x12\x12\n\ntrade_date\x18\x01 \x01(\x03\x12\r\n\x05price\x18\x02 \x01(\x01\x12\x10\n\x08quantity\x18\x03 \x01(\x03\"\xc4\x02\n\x10GetTradesRequest\x12\x11\n\tpublisher\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x0b\n\x03mic\x18\x03 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\t\x12\x0e\n\x06market\x18\x05 \x01(\t\x12\x10\n\x08start_at\x18\x06 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x07 \x01(\x03\x12\x0c\n\x04tape\x18\x08 \x01(\t\x12\x0c\n\x04page\x18\t \x01(\x05\x12\x11\n\tpage_size\x18\n \x01(\x05\x12\r\n\x05order\x18\x0b \x01(\t\x12\x0b\n\x03\x63qs\x18\x0c \x01(\t\x12\x0b\n\x03\x63ik\x18\r \x01(\t\x12\r\n\x05\x63usip\x18\x0e \x01(\t\x12\x0c\n\x04isin\x18\x0f \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\x10 \x01(\t\x12\x12\n\nshare_figi\x18\x11 \x01(\t\x12\x0b\n\x03lei\x18\x12 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x13 \x01(\t\"8\n\x11GetTradesResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.finazon.TradesItem2T\n\x0cTradeService\x12\x44\n\tGetTrades\x12\x19.finazon.GetTradesRequest\x1a\x1a.finazon.GetTradesResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.trade_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
   _globals['_TRADESITEM']._serialized_start=44
   _globals['_TRADESITEM']._serialized_end=109
   _globals['_GETTRADESREQUEST']._serialized_start=112
   _globals['_GETTRADESREQUEST']._serialized_end=436
   _globals['_GETTRADESRESPONSE']._serialized_start=438
   _globals['_GETTRADESRESPONSE']._serialized_end=494
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/trade_pb2.pyi` & `finazon_grpc_python-1.0.146/finazon_grpc_python/trade_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class TradesItem(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TRADE_DATE_FIELD_NUMBER: builtins.int
     PRICE_FIELD_NUMBER: builtins.int
     QUANTITY_FIELD_NUMBER: builtins.int
     trade_date: builtins.int
@@ -29,19 +25,19 @@
     def __init__(
         self,
         *,
         trade_date: builtins.int = ...,
         price: builtins.float = ...,
         quantity: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["price", b"price", "quantity", b"quantity", "trade_date", b"trade_date"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["price", b"price", "quantity", b"quantity", "trade_date", b"trade_date"]) -> None: ...
 
 global___TradesItem = TradesItem
 
-@typing_extensions.final
+@typing.final
 class GetTradesRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PUBLISHER_FIELD_NUMBER: builtins.int
     TICKER_FIELD_NUMBER: builtins.int
     MIC_FIELD_NUMBER: builtins.int
     COUNTRY_FIELD_NUMBER: builtins.int
@@ -98,26 +94,26 @@
         cusip: builtins.str = ...,
         isin: builtins.str = ...,
         composite_figi: builtins.str = ...,
         share_figi: builtins.str = ...,
         lei: builtins.str = ...,
         dataset: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "dataset", b"dataset", "end_at", b"end_at", "isin", b"isin", "lei", b"lei", "market", b"market", "mic", b"mic", "order", b"order", "page", b"page", "page_size", b"page_size", "publisher", b"publisher", "share_figi", b"share_figi", "start_at", b"start_at", "tape", b"tape", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "dataset", b"dataset", "end_at", b"end_at", "isin", b"isin", "lei", b"lei", "market", b"market", "mic", b"mic", "order", b"order", "page", b"page", "page_size", b"page_size", "publisher", b"publisher", "share_figi", b"share_figi", "start_at", b"start_at", "tape", b"tape", "ticker", b"ticker"]) -> None: ...
 
 global___GetTradesRequest = GetTradesRequest
 
-@typing_extensions.final
+@typing.final
 class GetTradesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TradesItem]: ...
     def __init__(
         self,
         *,
         result: collections.abc.Iterable[global___TradesItem] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["result", b"result"]) -> None: ...
 
 global___GetTradesResponse = GetTradesResponse
```

### Comparing `finazon_grpc_python-1.0.141/finazon_grpc_python/trade_pb2_grpc.py` & `finazon_grpc_python-1.0.146/finazon_grpc_python/trade_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.141/pyproject.toml` & `finazon_grpc_python-1.0.146/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "finazon-grpc-python"
 packages = [{include = "finazon_grpc_python"}]
 include = ["requirements.txt", "finazon_grpc_python/*.p*"]
-version = "1.0.141"
+version = "1.0.146"
 description = "Finazon gRPC client library for Python"
 authors = ["Finazon <team@finazon.io>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/finazon-io/finazon-grpc-python"
 repository = "https://github.com/finazon-io/finazon-grpc-python"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-grpcio-tools = "1.58.0"
-grpcio = "1.58.0"
+grpcio-tools = "^1.62.1"
+grpcio = "^1.62.1"
 mypy-protobuf = "^3.5.0"
 pandas = {version = "^2.2.1", optional = true}
 
 
 [tool.poetry.group.dev.dependencies]
 jinja2 = "^3.1.3"
 inflection = "^0.5.1"
```

### Comparing `finazon_grpc_python-1.0.141/PKG-INFO` & `finazon_grpc_python-1.0.146/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: finazon-grpc-python
-Version: 1.0.141
+Version: 1.0.146
 Summary: Finazon gRPC client library for Python
 Home-page: https://github.com/finazon-io/finazon-grpc-python
 License: MIT
 Author: Finazon
 Author-email: team@finazon.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: pandas
-Requires-Dist: grpcio (==1.58.0)
-Requires-Dist: grpcio-tools (==1.58.0)
+Requires-Dist: grpcio (>=1.62.1,<2.0.0)
+Requires-Dist: grpcio-tools (>=1.62.1,<2.0.0)
 Requires-Dist: mypy-protobuf (>=3.5.0,<4.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0) ; extra == "pandas"
 Project-URL: Repository, https://github.com/finazon-io/finazon-grpc-python
 Description-Content-Type: text/markdown
 
 # Finazon Python gRPC Client
 
@@ -27,15 +27,15 @@
 - Lists of datasets, publishers, markets, and tickers.
 - Market data: ticker snapshots, time series, trades, and technical indicators.
 - Data from specific datasets such as Benzinga, Binance, Crypto, Forex, SEC, and SIP.
 
 🔑 **API key** is essential. If you haven't got one yet, [sign up here](https://finazon.io/).
 
 ## Requirements
-Ensure you have Python 3.9 or later. 
+Ensure you have Python 3.9 or later.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Finazon Python gRPC Client library:
 ```shell
 pip install finazon-grpc-python
 ```
@@ -169,53 +169,51 @@
     print(response.result)
 except FinazonGrpcRequestError as e:
     print(f'Received error, code: {e.code}, message: {e.message}')
 ```
 
 👀 Check the full example and other examples [here](https://github.com/finazon-io/finazon-grpc-python/tree/main/finazon_grpc_python/examples)
 
-
 ## RPC support
 
 The following table outlines the supported rpc calls:
-<!--rpc_table_boundary-->
-| Service              | rpc                       | Description                                        |
-|----------------------|---------------------------|----------------------------------------------------|
-| ApiUsageService      | get_api_usage             | Get a list of products with quota limit/usage      |
-| BenzingaService      | get_dividents_calendar    | Returns the dividends calendar from Benzinga       |
-| BenzingaService      | get_earnings_calendar     | Returns the earnings calendar from Benzinga        |
-| BenzingaService      | get_news                  | Returns the news articles from Benzinga            |
-| BenzingaService      | get_ipo                   | Returns IPO data from Benzinga                     |
-| BinanceService       | get_time_series           | Get time series data without technical indicators  |
-| CryptoService        | get_time_series           | Get time series data for any given ticker          |
-| DatasetsService      | get_datasets              | Get a list of all datasets available at Finazon    |
-| ExchangeService      | get_markets_crypto        | Returns a list of supported crypto markets         |
-| ExchangeService      | get_markets_stocks        | Returns a list of supported stock markets          |
-| ForexService         | get_time_series           | Get time series data for any given ticker          |
-| PublisherService     | get_publishers            | Get a list of all publishers available at Finazon  |
-| SecService           | get_filings               | Real-time and historical access to all forms, filings, and exhibits directly from the SEC's EDGAR system |
-| SipService           | get_trades                | Returns detailed information on trades executed through the Securities Information Processor (SIP) |
-| SipService           | get_market_center         | Returns a list of market centers                   |
-| SnapshotService      | get_snapshot              | This endpoint returns a combination of different data points, such as daily performance, last quote, last trade, minute data, and previous day performance |
-| TickersService       | find_tickers_stocks       | This API call returns an array of stocks tickers available at Finazon Data API. This list is updated daily |
-| TickersService       | find_tickers_crypto       | This API call returns an array of crypto tickers available at Finazon Data API. This list is updated daily |
-| TickersService       | find_tickers_forex        | This API call returns an array of forex tickers available at Finazon Data API. This list is updated daily |
-| TickersService       | find_ticker_us            | This API call returns an array of US tickers available at Finazon Data API. This list is updated daily |
-| TimeSeriesService    | get_time_series           | Get time series data without technical indicators  |
-| TimeSeriesService    | get_time_series_atr       | Get time series data for ATR technical indicator   |
-| TimeSeriesService    | get_time_series_b_bands   | Get time series data for BBands technical indicator |
-| TimeSeriesService    | get_time_series_ichimoku  | Get time series data for Ichimoku technical indicator |
-| TimeSeriesService    | get_time_series_ma        | Get time series data for Ma technical indicator    |
-| TimeSeriesService    | get_time_series_macd      | Get time series data for Macd technical indicator  |
-| TimeSeriesService    | get_time_series_obv       | Get time series data for Obv technical indicator   |
-| TimeSeriesService    | get_time_series_rsi       | Get time series data for Rsi technical indicator   |
-| TimeSeriesService    | get_time_series_sar       | Get time series data for Sar technical indicator   |
-| TimeSeriesService    | get_time_series_stoch     | Get time series data for Stoch technical indicator |
-| TradeService         | get_trades                | Returns general information on executed trades     |
-<!--rpc_table_boundary-->
+|Service                |rpc                        |Description                                                                                                                                                      |
+|-----------------------|---------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| ApiUsageService       | getApiUsage               | Get a list of products with quota limit/usage                                                                                                                   |
+| BenzingaService       | getDividentsCalendar      | Returns the dividends calendar from Benzinga                                                                                                                    |
+| BenzingaService       | getEarningsCalendar       | Returns the earnings calendar from Benzinga                                                                                                                     |
+| BenzingaService       | getNews                   | Returns the news articles from Benzinga                                                                                                                         |
+| BenzingaService       | getIPO                    | Returns IPO data from Benzinga                                                                                                                                  |
+| BinanceService        | getTimeSeries             | Get time series data without technical indicators                                                                                                               |
+| CryptoService         | getTimeSeries             | Get time series data for any given ticker                                                                                                                       |
+| DatasetsService       | getDatasets               | Get a list of all datasets available at Finazon.                                                                                                                |
+| ExchangeService       | getMarketsCrypto          | Returns a list of supported crypto markets                                                                                                                      |
+| ExchangeService       | getMarketsStocks          | Returns a list of supported stock markets                                                                                                                       |
+| ForexService          | getTimeSeries             | Get time series data for any given ticker                                                                                                                       |
+| PublisherService      | getPublishers             | Get a list of all publishers available at Finazon.                                                                                                              |
+| SecService            | getFilings                | Real-time and historical access to all forms, filings, and exhibits directly from the SEC's EDGAR system.                                                       |
+| SipService            | getTrades                 | Returns detailed information on trades executed through the Securities Information Processor (SIP)                                                              |
+| SipService            | getMarketCenter           | Returns a list of market centers                                                                                                                                |
+| SnapshotService       | getSnapshot               | This endpoint returns a combination of different data points, such as daily performance, last quote, last trade, minute data, and previous day performance.     |
+| TickersService        | findTickersStocks         | This API call returns an array of stocks tickers available at Finazon Data API. This list is updated daily.                                                     |
+| TickersService        | findTickersCrypto         | This API call returns an array of crypto tickers available at Finazon Data API. This list is updated daily.                                                     |
+| TickersService        | findTickersForex          | This API call returns an array of forex tickers available at Finazon Data API. This list is updated daily.                                                      |
+| TickersService        | findTickerUS              | This API call returns an array of US tickers available at Finazon Data API. This list is updated daily.                                                         |
+| TimeSeriesService     | getTimeSeries             | Get time series data without technical indicators                                                                                                               |
+| TimeSeriesService     | getTimeSeriesAtr          | Get time series data for ATR technical indicator.                                                                                                               |
+| TimeSeriesService     | getTimeSeriesBBands       | Get time series data for BBands technical indicator.                                                                                                            |
+| TimeSeriesService     | getTimeSeriesIchimoku     | Get time series data for Ichimoku technical indicator.                                                                                                          |
+| TimeSeriesService     | getTimeSeriesMa           | Get time series data for Ma technical indicator.                                                                                                                |
+| TimeSeriesService     | getTimeSeriesMacd         | Get time series data for Macd technical indicator.                                                                                                              |
+| TimeSeriesService     | getTimeSeriesObv          | Get time series data for Obv technical indicator.                                                                                                               |
+| TimeSeriesService     | getTimeSeriesRsi          | Get time series data for Rsi technical indicator.                                                                                                               |
+| TimeSeriesService     | getTimeSeriesSar          | Get time series data for Sar technical indicator.                                                                                                               |
+| TimeSeriesService     | getTimeSeriesStoch        | Get time series data for Stoch technical indicator.                                                                                                             |
+| TradeService          | getTrades                 | Returns general information on executed trades                                                                                                                  |
+
 Here's how you can import `service` and `request` objects:
 
 ```python
 from finazon_grpc_python.service_name_service import ServiceNameService, RpcNameRequest
 
 # ...
 
@@ -245,8 +243,7 @@
 4. Push your branch and open a pull request with a comprehensive description.
 
 For more guidance on contributing, see the [GitHub Docs](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) on GitHub.
 
 ## License
 
 This project is licensed under the MIT License. See the `LICENSE.txt` file in this repository for more details.
-
```

