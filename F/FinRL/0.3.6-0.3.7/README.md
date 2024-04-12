# Comparing `tmp/finrl-0.3.6.tar.gz` & `tmp/FinRL-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finrl-0.3.6.tar", last modified: Tue Feb  7 13:56:24 2023, max compression
+gzip compressed data, was "FinRL-0.3.7.tar", last modified: Fri Apr 12 02:42:04 2024, max compression
```

## Comparing `finrl-0.3.6.tar` & `FinRL-0.3.7.tar`

### file list

```diff
@@ -1,80 +1,93 @@
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.643613 finrl-0.3.6/
--rwxr-xr-x   0 mingzhu    (501) staff       (20)     1088 2023-02-07 13:53:30.000000 finrl-0.3.6/LICENSE
--rw-r--r--   0 mingzhu    (501) staff       (20)      882 2023-02-07 13:56:24.643734 finrl-0.3.6/PKG-INFO
--rwxr-xr-x   0 mingzhu    (501) staff       (20)    17987 2023-02-07 13:53:30.000000 finrl-0.3.6/README.md
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.631847 finrl-0.3.6/finrl/
--rw-rw-r--   0 mingzhu    (501) staff       (20)      124 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/__init__.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)      121 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/__main__.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.633150 finrl-0.3.6/finrl/agents/
--rw-rw-r--   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/agents/__init__.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.633580 finrl-0.3.6/finrl/agents/elegantrl/
--rw-rw-r--   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/agents/elegantrl/__init__.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     4850 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/agents/elegantrl/models.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.634304 finrl-0.3.6/finrl/agents/rllib/
--rw-rw-r--   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/agents/rllib/__init__.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     9598 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/agents/rllib/drllibv2.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     6406 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/agents/rllib/models.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.635377 finrl-0.3.6/finrl/agents/stablebaselines3/
--rw-rw-r--   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/agents/stablebaselines3/__init__.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)    21639 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/agents/stablebaselines3/hyperparams_opt.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)    27434 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/agents/stablebaselines3/models.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     7178 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/agents/stablebaselines3/tune_sb3.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.635641 finrl-0.3.6/finrl/applications/
--rw-rw-r--   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/applications/__init__.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.635839 finrl-0.3.6/finrl/applications/cryptocurrency_trading/
--rw-rw-r--   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/applications/cryptocurrency_trading/__init__.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.636097 finrl-0.3.6/finrl/applications/high_frequency_trading/
--rw-rw-r--   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/applications/high_frequency_trading/__init__.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.636305 finrl-0.3.6/finrl/applications/portfolio_allocation/
--rw-rw-r--   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/applications/portfolio_allocation/__init__.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.636503 finrl-0.3.6/finrl/applications/stock_trading/
--rw-rw-r--   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/applications/stock_trading/__init__.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     2529 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/config.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)       85 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/config_private.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)    20559 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/config_tickers.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     4731 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/main.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.637225 finrl-0.3.6/finrl/meta/
--rw-rw-r--   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/__init__.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     2509 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/data_processor.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.639299 finrl-0.3.6/finrl/meta/data_processors/
--rw-rw-r--   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/data_processors/__init__.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     1754 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/data_processors/func.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)    15263 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/data_processors/processor_alpaca.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     5198 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/data_processors/processor_ccxt.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     4242 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/data_processors/processor_joinquant.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)      848 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/data_processors/processor_quantconnect.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)    12444 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/data_processors/processor_wrds.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)    19671 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/data_processors/processor_yahoofinance.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.640055 finrl-0.3.6/finrl/meta/env_cryptocurrency_trading/
--rw-rw-r--   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/env_cryptocurrency_trading/__init__.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     7644 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/env_cryptocurrency_trading/env_btc_ccxt.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     4367 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/env_cryptocurrency_trading/env_multiple_crypto.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.640513 finrl-0.3.6/finrl/meta/env_portfolio_allocation/
--rw-rw-r--   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/env_portfolio_allocation/__init__.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     9080 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/env_portfolio_allocation/env_portfolio.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.642362 finrl-0.3.6/finrl/meta/env_stock_trading/
--rw-rw-r--   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/env_stock_trading/__init__.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     8626 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/env_stock_trading/env_nas100_wrds.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)    14073 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/env_stock_trading/env_stock_papertrading.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)    21466 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/env_stock_trading/env_stocktrading.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)    16247 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/env_stock_trading/env_stocktrading_cashpenalty.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     6251 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/env_stock_trading/env_stocktrading_np.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)    20238 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/env_stock_trading/env_stocktrading_stoploss.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     7706 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/meta_config.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.643386 finrl-0.3.6/finrl/meta/preprocessor/
--rw-rw-r--   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/preprocessor/__init__.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     9675 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/preprocessor/preprocessors.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     3880 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/preprocessor/tusharedownloader.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     3279 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/meta/preprocessor/yahoodownloader.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     3941 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/plot.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     4247 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/test.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     2126 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/trade.py
--rw-rw-r--   0 mingzhu    (501) staff       (20)     5216 2023-02-07 13:53:30.000000 finrl-0.3.6/finrl/train.py
-drwxr-xr-x   0 mingzhu    (501) staff       (20)        0 2023-02-07 13:56:24.632890 finrl-0.3.6/finrl.egg-info/
--rw-r--r--   0 mingzhu    (501) staff       (20)      882 2023-02-07 13:56:24.000000 finrl-0.3.6/finrl.egg-info/PKG-INFO
--rw-r--r--   0 mingzhu    (501) staff       (20)     2172 2023-02-07 13:56:24.000000 finrl-0.3.6/finrl.egg-info/SOURCES.txt
--rw-r--r--   0 mingzhu    (501) staff       (20)        1 2023-02-07 13:56:24.000000 finrl-0.3.6/finrl.egg-info/dependency_links.txt
--rw-r--r--   0 mingzhu    (501) staff       (20)        6 2023-02-07 13:56:24.000000 finrl-0.3.6/finrl.egg-info/top_level.txt
--rw-rw-r--   0 mingzhu    (501) staff       (20)     1698 2023-02-07 13:53:30.000000 finrl-0.3.6/pyproject.toml
--rw-rw-r--   0 mingzhu    (501) staff       (20)      608 2023-02-07 13:56:24.644221 finrl-0.3.6/setup.cfg
--rw-rw-r--   0 mingzhu    (501) staff       (20)     1722 2023-02-07 13:53:30.000000 finrl-0.3.6/setup.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.725038 FinRL-0.3.7/
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.714837 FinRL-0.3.7/FinRL.egg-info/
+-rw-r--r--   0 bruce      (501) staff       (20)      909 2024-04-12 02:42:04.000000 FinRL-0.3.7/FinRL.egg-info/PKG-INFO
+-rw-r--r--   0 bruce      (501) staff       (20)     2768 2024-04-12 02:42:04.000000 FinRL-0.3.7/FinRL.egg-info/SOURCES.txt
+-rw-r--r--   0 bruce      (501) staff       (20)        1 2024-04-12 02:42:04.000000 FinRL-0.3.7/FinRL.egg-info/dependency_links.txt
+-rw-r--r--   0 bruce      (501) staff       (20)        6 2024-04-12 02:42:04.000000 FinRL-0.3.7/FinRL.egg-info/top_level.txt
+-rwxr-xr-x   0 bruce      (501) staff       (20)     1093 2024-04-12 02:40:20.000000 FinRL-0.3.7/LICENSE
+-rw-r--r--   0 bruce      (501) staff       (20)      909 2024-04-12 02:42:04.725102 FinRL-0.3.7/PKG-INFO
+-rwxr-xr-x   0 bruce      (501) staff       (20)    19047 2024-04-12 02:40:20.000000 FinRL-0.3.7/README.md
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.716932 FinRL-0.3.7/finrl/
+-rw-r--r--   0 bruce      (501) staff       (20)      124 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/__init__.py
+-rw-r--r--   0 bruce      (501) staff       (20)      121 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/__main__.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.717076 FinRL-0.3.7/finrl/agents/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/agents/__init__.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.717294 FinRL-0.3.7/finrl/agents/elegantrl/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/agents/elegantrl/__init__.py
+-rw-r--r--   0 bruce      (501) staff       (20)     6083 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/agents/elegantrl/models.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.718203 FinRL-0.3.7/finrl/agents/portfolio_optimization/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/agents/portfolio_optimization/__init__.py
+-rw-r--r--   0 bruce      (501) staff       (20)     9298 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/agents/portfolio_optimization/algorithms.py
+-rw-r--r--   0 bruce      (501) staff       (20)    18114 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/agents/portfolio_optimization/architectures.py
+-rw-r--r--   0 bruce      (501) staff       (20)     3492 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/agents/portfolio_optimization/models.py
+-rw-r--r--   0 bruce      (501) staff       (20)     3317 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/agents/portfolio_optimization/utils.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.718638 FinRL-0.3.7/finrl/agents/rllib/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/agents/rllib/__init__.py
+-rw-r--r--   0 bruce      (501) staff       (20)     9597 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/agents/rllib/drllibv2.py
+-rw-r--r--   0 bruce      (501) staff       (20)     6406 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/agents/rllib/models.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.719303 FinRL-0.3.7/finrl/agents/stablebaselines3/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/agents/stablebaselines3/__init__.py
+-rw-r--r--   0 bruce      (501) staff       (20)    21639 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/agents/stablebaselines3/hyperparams_opt.py
+-rw-r--r--   0 bruce      (501) staff       (20)    24966 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/agents/stablebaselines3/models.py
+-rw-r--r--   0 bruce      (501) staff       (20)     7013 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/agents/stablebaselines3/tune_sb3.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.719470 FinRL-0.3.7/finrl/applications/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/applications/__init__.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.719572 FinRL-0.3.7/finrl/applications/cryptocurrency_trading/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/applications/cryptocurrency_trading/__init__.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.719672 FinRL-0.3.7/finrl/applications/high_frequency_trading/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/applications/high_frequency_trading/__init__.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.719772 FinRL-0.3.7/finrl/applications/portfolio_allocation/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/applications/portfolio_allocation/__init__.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.720565 FinRL-0.3.7/finrl/applications/stock_trading/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/applications/stock_trading/__init__.py
+-rw-r--r--   0 bruce      (501) staff       (20)     5598 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/applications/stock_trading/ensemble_stock_trading.py
+-rw-r--r--   0 bruce      (501) staff       (20)    40037 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/applications/stock_trading/fundamental_stock_trading.py
+-rw-r--r--   0 bruce      (501) staff       (20)    11433 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/applications/stock_trading/stock_trading.py
+-rw-r--r--   0 bruce      (501) staff       (20)    17584 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/applications/stock_trading/stock_trading_rolling_window.py
+-rw-r--r--   0 bruce      (501) staff       (20)     2529 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/config.py
+-rw-r--r--   0 bruce      (501) staff       (20)       85 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/config_private.py
+-rw-r--r--   0 bruce      (501) staff       (20)    20559 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/config_tickers.py
+-rw-r--r--   0 bruce      (501) staff       (20)     4731 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/main.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.721006 FinRL-0.3.7/finrl/meta/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/__init__.py
+-rw-r--r--   0 bruce      (501) staff       (20)     3036 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/data_processor.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.722235 FinRL-0.3.7/finrl/meta/data_processors/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/data_processors/__init__.py
+-rw-r--r--   0 bruce      (501) staff       (20)     5033 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/data_processors/func.py
+-rw-r--r--   0 bruce      (501) staff       (20)    16755 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/data_processors/processor_alpaca.py
+-rw-r--r--   0 bruce      (501) staff       (20)     5198 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/data_processors/processor_ccxt.py
+-rw-r--r--   0 bruce      (501) staff       (20)     4242 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/data_processors/processor_joinquant.py
+-rw-r--r--   0 bruce      (501) staff       (20)      848 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/data_processors/processor_quantconnect.py
+-rw-r--r--   0 bruce      (501) staff       (20)    12686 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/data_processors/processor_wrds.py
+-rw-r--r--   0 bruce      (501) staff       (20)    18435 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/data_processors/processor_yahoofinance.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.722705 FinRL-0.3.7/finrl/meta/env_cryptocurrency_trading/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/env_cryptocurrency_trading/__init__.py
+-rw-r--r--   0 bruce      (501) staff       (20)     7711 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/env_cryptocurrency_trading/env_btc_ccxt.py
+-rw-r--r--   0 bruce      (501) staff       (20)     4434 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/env_cryptocurrency_trading/env_multiple_crypto.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.723002 FinRL-0.3.7/finrl/meta/env_portfolio_allocation/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/env_portfolio_allocation/__init__.py
+-rw-r--r--   0 bruce      (501) staff       (20)     9222 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/env_portfolio_allocation/env_portfolio.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.723269 FinRL-0.3.7/finrl/meta/env_portfolio_optimization/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/env_portfolio_optimization/__init__.py
+-rw-r--r--   0 bruce      (501) staff       (20)    27935 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/env_portfolio_optimization/env_portfolio_optimization.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.724323 FinRL-0.3.7/finrl/meta/env_stock_trading/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/env_stock_trading/__init__.py
+-rw-r--r--   0 bruce      (501) staff       (20)     8693 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/env_stock_trading/env_nas100_wrds.py
+-rw-r--r--   0 bruce      (501) staff       (20)    14152 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/env_stock_trading/env_stock_papertrading.py
+-rw-r--r--   0 bruce      (501) staff       (20)    21576 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/env_stock_trading/env_stocktrading.py
+-rw-r--r--   0 bruce      (501) staff       (20)    16313 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/env_stock_trading/env_stocktrading_cashpenalty.py
+-rw-r--r--   0 bruce      (501) staff       (20)     6342 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/env_stock_trading/env_stocktrading_np.py
+-rw-r--r--   0 bruce      (501) staff       (20)    20305 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/env_stock_trading/env_stocktrading_stoploss.py
+-rw-r--r--   0 bruce      (501) staff       (20)     7706 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/meta_config.py
+drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-04-12 02:42:04.724908 FinRL-0.3.7/finrl/meta/preprocessor/
+-rw-r--r--   0 bruce      (501) staff       (20)        0 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/preprocessor/__init__.py
+-rw-r--r--   0 bruce      (501) staff       (20)     9801 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/preprocessor/preprocessors.py
+-rw-r--r--   0 bruce      (501) staff       (20)     3507 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/preprocessor/tusharedownloader.py
+-rw-r--r--   0 bruce      (501) staff       (20)     3561 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/meta/preprocessor/yahoodownloader.py
+-rw-r--r--   0 bruce      (501) staff       (20)    11103 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/plot.py
+-rw-r--r--   0 bruce      (501) staff       (20)     4246 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/test.py
+-rw-r--r--   0 bruce      (501) staff       (20)     2126 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/trade.py
+-rw-r--r--   0 bruce      (501) staff       (20)     5215 2024-04-12 02:40:20.000000 FinRL-0.3.7/finrl/train.py
+-rw-r--r--   0 bruce      (501) staff       (20)     1636 2024-04-12 02:40:20.000000 FinRL-0.3.7/pyproject.toml
+-rw-r--r--   0 bruce      (501) staff       (20)      608 2024-04-12 02:42:04.725313 FinRL-0.3.7/setup.cfg
+-rw-r--r--   0 bruce      (501) staff       (20)     1750 2024-04-12 02:40:20.000000 FinRL-0.3.7/setup.py
```

### Comparing `finrl-0.3.6/LICENSE` & `FinRL-0.3.7/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2020 AI4Finance Foundation
+Copyright (c) 2024 AI4Finance Foundation Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `finrl-0.3.6/PKG-INFO` & `FinRL-0.3.7/FinRL.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
-Name: finrl
-Version: 0.3.6
+Name: FinRL
+Version: 0.3.7
 Summary: FinRL: Financial Reinforcement Learning Framework.
-Home-page: https://github.com/finrl/finrl-library
-Author: Hongyang Yang, Xiaoyang Liu, Ming Zhu
-Author-email: hy2500@columbia.edu
+Home-page: https://github.com/AI4Finance-Foundation/FinRL
+Author: AI4Finance Foundation
+Author-email: contact@ai4finance.org
 License: MIT
 Keywords: Reinforcement Learning,Finance
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 License-File: LICENSE
 
 Version 0.3.5 notes: stable version, code refactoring, more tutorials, clear documentation
-
```

### Comparing `finrl-0.3.6/README.md` & `FinRL-0.3.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,47 +11,54 @@
 [4]: https://www.linkedin.com/sharing/share-offsite/?url=http%3A%2F%2Fgithub.com%2FAI4Finance-Foundation%2FFinRL
 
 <div align="center">
 <img align="center" src=figs/logo_transparent_background.png width="55%"/>
 </div>
 
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
-[![Downloads](https://pepy.tech/badge/finrl)](https://pepy.tech/project/finrl)
-[![Downloads](https://pepy.tech/badge/finrl/week)](https://pepy.tech/project/finrl)
+[![Downloads](https://static.pepy.tech/badge/finrl)](https://pepy.tech/project/finrl)
+[![Downloads](https://static.pepy.tech/badge/finrl/week)](https://pepy.tech/project/finrl)
 [![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![PyPI](https://img.shields.io/pypi/v/finrl.svg)](https://pypi.org/project/finrl/)
 [![Documentation Status](https://readthedocs.org/projects/finrl/badge/?version=latest)](https://finrl.readthedocs.io/en/latest/?badge=latest)
 ![License](https://img.shields.io/github/license/AI4Finance-Foundation/finrl.svg?color=brightgreen)
 
+[FinGPT](https://github.com/AI4Finance-Foundation/ChatGPT-for-FinTech): Open-source for open-finance! Revolutionize FinTech.
+
+Check out our latest competition: [ACM ICAIF 2023 FinRL Contest](https://finrl-contest.github.io/)
+
+
+[![](https://dcbadge.vercel.app/api/server/trsr8SXpW5)](https://discord.gg/trsr8SXpW5)
 
 
 **Financial reinforcement learning (FinRL)** ([Document website](https://finrl.readthedocs.io/en/latest/index.html)) is **the first open-source framework** for financial reinforcement learning. FinRL has evolved into an **ecosystem**
 
 | Dev Roadmap  | Stage | Users | Project | Desription |
 |----|----|----|----|----|
 | 0.0 (Preparation) | entrance | practitioners | [FinRL-Meta](https://github.com/AI4Finance-Foundation/FinRL-Meta)| gym-style market environments |
 | 1.0 (Proof-of-Concept)| full-stack | developers | [this repo](https://github.com/AI4Finance-Foundation/FinRL) | automatic pipeline |
 | 2.0 (Professional) | profession | experts | [ElegantRL](https://github.com/AI4Finance-Foundation/ElegantRL) | algorithms |
 | 3.0 (Production) | service | hedge funds | [Podracer](https://github.com/AI4Finance-Foundation/FinRL_Podracer) | cloud-native deployment |
 
 
 ## Outline
 
-- [Overview](#Overview)
-- [File Structure](#File-Structure)
-- [Supported Data Sources](#Supported-Data-Sources)
-- [Installation](#Installation)
-- [Status Update](#Status-Update)
-- [Tutorials](#Tutorials)
-- [Publications](#Publications)
-- [News](#News)
-- [Citing FinRL](#Citing-FinRL)
-- [Welcome Contributions](#To-Contribute)
-- [Sponsorship](#Sponsorship)
-- [LICENSE](#LICENSE)
+  - [Overview](#overview)
+  - [File Structure](#file-structure)
+  - [Supported Data Sources](#supported-data-sources)
+  - [Installation](#installation)
+  - [Status Update](#status-update)
+  - [Tutorials](#tutorials)
+  - [Publications](#publications)
+  - [News](#news)
+  - [Citing FinRL](#citing-finrl)
+  - [Join and Contribute](#join-and-contribute)
+    - [Contributors](#contributors)
+    - [Sponsorship](#sponsorship)
+  - [LICENSE](#license)
 
 ## Overview
 
 FinRL has three layers: market environments, agents, and applications.  For a trading task (on the top), an agent (in the middle) interacts with a market environment (at the bottom), making sequential decisions.
 
 <div align="center">
 <img align="center" src=figs/finrl_framework.png>
@@ -64,14 +71,16 @@
 
 The main folder **finrl** has three subfolders **applications, agents, meta**. We employ a **train-test-trade** pipeline with three files: train.py, test.py, and trade.py.
 
 ```
 FinRL
 ├── finrl (main folder)
 │   ├── applications
+│   	├── Stock_NeurIPS2018
+│   	├── imitation_learning
 │   	├── cryptocurrency_trading
 │   	├── high_frequency_trading
 │   	├── portfolio_allocation
 │   	└── stock_trading
 │   ├── agents
 │   	├── elegantrl
 │   	├── rllib
@@ -105,18 +114,20 @@
 └── README.md
 ```
 
 ## Supported Data Sources
 
 |Data Source |Type |Range and Frequency |Request Limits|Raw Data|Preprocessed Data|
 |  ----  |  ----  |  ----  |  ----  |  ----  |  ----  |
+|[Akshare](https://alpaca.markets/docs/introduction/)| CN Securities| 2015-now, 1day| Account-specific| OHLCV| Prices&Indicators|
 |[Alpaca](https://alpaca.markets/docs/introduction/)| US Stocks, ETFs| 2015-now, 1min| Account-specific| OHLCV| Prices&Indicators|
 |[Baostock](http://baostock.com/baostock/index.php/Python_API%E6%96%87%E6%A1%A3)| CN Securities| 1990-12-19-now, 5min| Account-specific| OHLCV| Prices&Indicators|
 |[Binance](https://binance-docs.github.io/apidocs/spot/en/#public-api-definitions)| Cryptocurrency| API-specific, 1s, 1min| API-specific| Tick-level daily aggegrated trades, OHLCV| Prices&Indicators|
 |[CCXT](https://docs.ccxt.com/en/latest/manual.html)| Cryptocurrency| API-specific, 1min| API-specific| OHLCV| Prices&Indicators|
+|[EODhistoricaldata](https://eodhistoricaldata.com/financial-apis/)| US Securities| Frequency-specific, 1min| API-specific | OHLCV | Prices&Indicators|
 |[IEXCloud](https://iexcloud.io/docs/api/)| NMS US securities|1970-now, 1 day|100 per second per IP|OHLCV| Prices&Indicators|
 |[JoinQuant](https://www.joinquant.com/)| CN Securities| 2005-now, 1min| 3 requests each time| OHLCV| Prices&Indicators|
 |[QuantConnect](https://www.quantconnect.com/docs/home/home)| US Securities| 1998-now, 1s| NA| OHLCV| Prices&Indicators|
 |[RiceQuant](https://www.ricequant.com/doc/rqdata/python/)| CN Securities| 2005-now, 1ms| Account-specific| OHLCV| Prices&Indicators|
 |[Tushare](https://tushare.pro/document/1?doc_id=131)| CN Securities, A share| -now, 1 min| Account-specific| OHLCV| Prices&Indicators|
 |[WRDS](https://wrds-www.wharton.upenn.edu/pages/about/data-vendors/nyse-trade-and-quote-taq/)| US Securities| 2003-now, 1ms| 5 requests each time| Intraday Trades|Prices&Indicators|
 |[YahooFinance](https://pypi.org/project/yfinance/)| US Securities| Frequency-specific, 1min| 2,000/hour| OHLCV | Prices&Indicators|
@@ -188,23 +199,22 @@
 + [Towardsdatascience] [Deep Reinforcement Learning for Automated Stock Trading](https://towardsdatascience.com/deep-reinforcement-learning-for-automated-stock-trading-f1dad0126a02)
 
 A complete list at [blogs](https://github.com/AI4Finance-Foundation/Blogs)
 
 
 ## Publications
 
-|Title |Conference |Link|Citations|Year|
+|Title |Conference/Journal |Link|Citations|Year|
 |  ----  |  ----  |  ----  |  ----  |  ----  |
-|**FinRL-Meta**: FinRL-Meta: Market Environments and Benchmarks for Data-Driven Financial Reinforcement Learning| NeurIPS 2022| [paper](https://arxiv.org/abs/2211.03107) [code](https://github.com/AI4Finance-Foundation/FinRL-Meta) | 1 | 2022 |
-|**FinRL**: Deep reinforcement learning framework to automate trading in quantitative finance| ACM International Conference on AI in Finance (ICAIF) | [paper](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3955949) | 19 | 2021 |
-|**FinRL-Podracer**: High performance and scalable deep reinforcement learning for quantitative finance | ACM International Conference on AI in Finance (ICAIF) | [paper](https://arxiv.org/abs/2111.05188) [code](https://github.com/AI4Finance-Foundation/FinRL_Podracer) | 8 | 2021 |
-|Explainable deep reinforcement learning for portfolio management: An empirical approach| ACM International Conference on AI in Finance (ICAIF) | [paper](https://arxiv.org/abs/2111.03995) [code](https://github.com/AI4Finance-Foundation/FinRL-Meta/blob/master/tutorials/2-Advance/FinRL_PortfolioAllocation_Explainable_DRL/FinRL_PortfolioAllocation_Explainable_DRL.py](https://github.com/AI4Finance-Foundation/FinRL-Tutorials/tree/master/2-Advance))| 3 | 2021 |
-|**FinRL**: A deep reinforcement learning library for automated stock trading in quantitative finance| NeurIPS 2020 Deep RL Workshop  | [paper](https://arxiv.org/abs/2011.09607) | 46 | 2020 |
-|Deep reinforcement learning for automated stock trading: An ensemble strategy| ACM International Conference on AI in Finance (ICAIF) | [paper](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3690996) [code](https://github.com/AI4Finance-Foundation/FinRL-Meta/blob/master/tutorials/2-Advance/FinRL_Ensemble_StockTrading_ICAIF_2020/FinRL_Ensemble_StockTrading_ICAIF_2020.ipynb) | 94 | 2020 |
-|Practical deep reinforcement learning approach for stock trading | NeurIPS 2018 Workshop on Challenges and Opportunities for AI in Financial Services| [paper](https://arxiv.org/abs/1811.07522) [code](https://github.com/AI4Finance-Foundation/DQN-DDPG_Stock_Trading](https://github.com/AI4Finance-Foundation/FinRL/tree/master/examples))| 127 | 2018 |
+|Dynamic Datasets and Market Environments for Financial Reinforcement Learning| Machine Learning - Nature| [paper](https://arxiv.org/abs/2304.13174) [code](https://github.com/AI4Finance-Foundation/FinRL-Meta) | 1 | 2024 |
+|**FinRL-Meta**: FinRL-Meta: Market Environments and Benchmarks for Data-Driven Financial Reinforcement Learning| NeurIPS 2022| [paper](https://arxiv.org/abs/2211.03107) [code](https://github.com/AI4Finance-Foundation/FinRL-Meta) | 12 | 2022 |
+|**FinRL**: Deep reinforcement learning framework to automate trading in quantitative finance| ACM International Conference on AI in Finance (ICAIF) | [paper](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3955949) | 49 | 2021 |
+|**FinRL**: A deep reinforcement learning library for automated stock trading in quantitative finance| NeurIPS 2020 Deep RL Workshop  | [paper](https://arxiv.org/abs/2011.09607) | 87 | 2020 |
+|Deep reinforcement learning for automated stock trading: An ensemble strategy| ACM International Conference on AI in Finance (ICAIF) | [paper](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3690996) [code](https://github.com/AI4Finance-Foundation/FinRL-Meta/blob/master/tutorials/2-Advance/FinRL_Ensemble_StockTrading_ICAIF_2020/FinRL_Ensemble_StockTrading_ICAIF_2020.ipynb) | 154 | 2020 |
+|Practical deep reinforcement learning approach for stock trading | NeurIPS 2018 Workshop on Challenges and Opportunities for AI in Financial Services| [paper](https://arxiv.org/abs/1811.07522) [code](https://github.com/AI4Finance-Foundation/DQN-DDPG_Stock_Trading](https://github.com/AI4Finance-Foundation/FinRL/tree/master/examples))| 164 | 2018 |
 
 
 ## News
 + [央广网] [2021 IDEA大会于福田圆满落幕：群英荟萃论道AI 多项目发布亮点纷呈](http://tech.cnr.cn/techph/20211123/t20211123_525669092.shtml)
 + [央广网] [2021 IDEA大会开启AI思想盛宴 沈向洋理事长发布六大前沿产品](https://baijiahao.baidu.com/s?id=1717101783873523790&wfr=spider&for=pc)
 + [IDEA新闻] [2021 IDEA大会发布产品FinRL-Meta——基于数据驱动的强化学习金融风险模拟系统](https://idea.edu.cn/news/20211213143128.html)
 + [知乎] [FinRL-Meta基于数据驱动的强化学习金融元宇宙](https://zhuanlan.zhihu.com/p/437804814)
@@ -213,17 +223,29 @@
 + [深度强化实验室] [【重磅推荐】哥大开源“FinRL”: 一个用于量化金融自动交易的深度强化学习库](https://blog.csdn.net/deeprl/article/details/114828024)
 + [商业新知] [金融科技讲座回顾|AI4Finance: 从AlphaGo到FinRL](https://www.shangyexinzhi.com/article/4170766.html)
 + [Kaggle] [Jane Street Market Prediction](https://www.kaggle.com/c/jane-street-market-prediction/discussion/199313)
 + [矩池云Matpool] [在矩池云上如何运行FinRL股票交易策略框架](http://www.python88.com/topic/111918)
 + [财智无界] [金融学会常务理事陈学彬: 深度强化学习在金融资产管理中的应用](https://www.sohu.com/a/486837028_120929319)
 + [Neurohive] [FinRL: глубокое обучение с подкреплением для трейдинга](https://neurohive.io/ru/gotovye-prilozhenija/finrl-glubokoe-obuchenie-s-podkrepleniem-dlya-trejdinga/)
 + [ICHI.PRO] [양적 금융을위한 FinRL: 단일 주식 거래를위한 튜토리얼](https://ichi.pro/ko/yangjeog-geum-yung-eul-wihan-finrl-dan-il-jusig-geolaeleul-wihan-tyutolieol-61395882412716)
++ [知乎] [基于深度强化学习的金融交易策略（FinRL+Stable baselines3，以道琼斯30股票为例）](https://zhuanlan.zhihu.com/p/563238735)
++ [知乎] [动态数据驱动的金融强化学习](https://zhuanlan.zhihu.com/p/616799055)
++ [知乎] [FinRL的W&B化+超参数搜索和模型优化(基于Stable Baselines 3）](https://zhuanlan.zhihu.com/p/498115373)
++
+## Citing FinRL
 
+```
+@article{dynamic_datasets,
+    author = {Liu, Xiao-Yang and Xia, Ziyi and Yang, Hongyang and Gao, Jiechao and Zha, Daochen and Zhu, Ming and Wang, Christina Dan and Wang, Zhaoran and Guo, Jian},
+    title = {Dynamic Datasets and Market Environments for Financial Reinforcement Learning},
+    journal = {Machine Learning - Springer Nature},
+    year = {2024}
+}
+```
 
-## Citing FinRL
 
 ```
 @article{liu2022finrl_meta,
   title={FinRL-Meta: Market Environments and Benchmarks for Data-Driven Financial Reinforcement Learning},
   author={Liu, Xiao-Yang and Xia, Ziyi and Rui, Jingyang and Gao, Jiechao and Yang, Hongyang and Zhu, Ming and Wang, Christina Dan and Wang, Zhaoran and Guo, Jian},
   journal={NeurIPS},
   year={2022}
@@ -275,15 +297,15 @@
 </a>
 <b>Follow us on WeChat:</b>
 	<div align="center">
 		<img src=http://www.tensorlet.org/wp-content/uploads/2021/01/qrcode_for_gh_feece88824ab_258.jpg width="25%" />
 	</div>
 </b>
 
-Please check [Contributing Guidances](https://github.com/AI4Finance-Foundation/FinRL/blob/master/tutorials/Contributing.md).
+Please check [Contributing Guidances](https://github.com/AI4Finance-Foundation/FinRL-Tutorials/blob/master/Contributing.md).
 
 ### Contributors
 
 Thank you!
 
 <a href="https://github.com/AI4Finance-LLC/FinRL-Library/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=AI4Finance-LLC/FinRL-Library" />
@@ -303,8 +325,8 @@
 
 
 
 ## LICENSE
 
 MIT License
 
-**Disclaimer: Nothing herein is financial advice, and NOT a recommendation to trade real money. Please use common sense and always first consult a professional before trading or investing.**
+**Disclaimer: We are sharing codes for academic purpose under the MIT education license. Nothing herein is financial advice, and NOT a recommendation to trade real money. Please use common sense and always first consult a professional before trading or investing.**
```

### Comparing `finrl-0.3.6/finrl/agents/elegantrl/models.py` & `FinRL-0.3.7/finrl/test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,131 +1,137 @@
-"""
-DRL models from ElegantRL: https://github.com/AI4Finance-Foundation/ElegantRL
-"""
 from __future__ import annotations
 
-import torch
-from elegantrl.agents import AgentDDPG
-from elegantrl.agents import AgentPPO
-from elegantrl.agents import AgentSAC
-from elegantrl.agents import AgentTD3
-from elegantrl.train.config import Arguments
-from elegantrl.train.run import init_agent
-from elegantrl.train.run import train_and_evaluate
-
-# from elegantrl.agents import AgentA2C
-
-MODELS = {"ddpg": AgentDDPG, "td3": AgentTD3, "sac": AgentSAC, "ppo": AgentPPO}
-OFF_POLICY_MODELS = ["ddpg", "td3", "sac"]
-ON_POLICY_MODELS = ["ppo"]
-# MODEL_KWARGS = {x: config.__dict__[f"{x.upper()}_PARAMS"] for x in MODELS.keys()}
-#
-# NOISE = {
-#     "normal": NormalActionNoise,
-#     "ornstein_uhlenbeck": OrnsteinUhlenbeckActionNoise,
-# }
-
-
-class DRLAgent:
-    """Implementations of DRL algorithms
-    Attributes
-    ----------
-        env: gym environment class
-            user-defined class
-    Methods
-    -------
-        get_model()
-            setup DRL algorithms
-        train_model()
-            train DRL algorithms in a train dataset
-            and output the trained model
-        DRL_prediction()
-            make a prediction in a test dataset and get results
-    """
-
-    def __init__(self, env, price_array, tech_array, turbulence_array):
-        self.env = env
-        self.price_array = price_array
-        self.tech_array = tech_array
-        self.turbulence_array = turbulence_array
-
-    def get_model(self, model_name, model_kwargs):
-        env_config = {
-            "price_array": self.price_array,
-            "tech_array": self.tech_array,
-            "turbulence_array": self.turbulence_array,
-            "if_train": True,
-        }
-        env = self.env(config=env_config)
-        env.env_num = 1
-        agent = MODELS[model_name]
-        if model_name not in MODELS:
-            raise NotImplementedError("NotImplementedError")
-        model = Arguments(agent_class=agent, env=env)
-        model.if_off_policy = model_name in OFF_POLICY_MODELS
-        if model_kwargs is not None:
-            try:
-                model.learning_rate = model_kwargs["learning_rate"]
-                model.batch_size = model_kwargs["batch_size"]
-                model.gamma = model_kwargs["gamma"]
-                model.seed = model_kwargs["seed"]
-                model.net_dim = model_kwargs["net_dimension"]
-                model.target_step = model_kwargs["target_step"]
-                model.eval_gap = model_kwargs["eval_gap"]
-                model.eval_times = model_kwargs["eval_times"]
-            except BaseException:
-                raise ValueError(
-                    "Fail to read arguments, please check 'model_kwargs' input."
-                )
-        return model
-
-    def train_model(self, model, cwd, total_timesteps=5000):
-        model.cwd = cwd
-        model.break_step = total_timesteps
-        train_and_evaluate(model)
-
-    @staticmethod
-    def DRL_prediction(model_name, cwd, net_dimension, environment):
-        if model_name not in MODELS:
-            raise NotImplementedError("NotImplementedError")
-        agent = MODELS[model_name]
-        environment.env_num = 1
-        args = Arguments(agent_class=agent, env=environment)
-        args.cwd = cwd
-        args.net_dim = net_dimension
-        # load agent
-        try:
-            agent = init_agent(args, gpu_id=0)
-            act = agent.act
-            device = agent.device
-        except BaseException:
-            raise ValueError("Fail to load agent!")
-
-        # test on the testing env
-        _torch = torch
-        state = environment.reset()
-        episode_returns = []  # the cumulative_return / initial_account
-        episode_total_assets = [environment.initial_total_asset]
-        with _torch.no_grad():
-            for i in range(environment.max_step):
-                s_tensor = _torch.as_tensor((state,), device=device)
-                a_tensor = act(s_tensor)  # action_tanh = act.forward()
-                action = (
-                    a_tensor.detach().cpu().numpy()[0]
-                )  # not need detach(), because with torch.no_grad() outside
-                state, reward, done, _ = environment.step(action)
-
-                total_asset = (
-                    environment.amount
-                    + (
-                        environment.price_ary[environment.day] * environment.stocks
-                    ).sum()
-                )
-                episode_total_assets.append(total_asset)
-                episode_return = total_asset / environment.initial_total_asset
-                episode_returns.append(episode_return)
-                if done:
-                    break
-        print("Test Finished!")
-        # return episode total_assets on testing data
-        print("episode_return", episode_return)
+from finrl.config import INDICATORS
+from finrl.config import RLlib_PARAMS
+from finrl.config import TEST_END_DATE
+from finrl.config import TEST_START_DATE
+from finrl.config_tickers import DOW_30_TICKER
+from finrl.meta.env_stock_trading.env_stocktrading import StockTradingEnv
+
+
+def test(
+    start_date,
+    end_date,
+    ticker_list,
+    data_source,
+    time_interval,
+    technical_indicator_list,
+    drl_lib,
+    env,
+    model_name,
+    if_vix=True,
+    **kwargs,
+):
+    # import data processor
+    from finrl.meta.data_processor import DataProcessor
+
+    # fetch data
+    dp = DataProcessor(data_source, **kwargs)
+    data = dp.download_data(ticker_list, start_date, end_date, time_interval)
+    data = dp.clean_data(data)
+    data = dp.add_technical_indicator(data, technical_indicator_list)
+
+    if if_vix:
+        data = dp.add_vix(data)
+    price_array, tech_array, turbulence_array = dp.df_to_array(data, if_vix)
+
+    env_config = {
+        "price_array": price_array,
+        "tech_array": tech_array,
+        "turbulence_array": turbulence_array,
+        "if_train": False,
+    }
+    env_instance = env(config=env_config)
+
+    # load elegantrl needs state dim, action dim and net dim
+    net_dimension = kwargs.get("net_dimension", 2**7)
+    cwd = kwargs.get("cwd", "./" + str(model_name))
+    print("price_array: ", len(price_array))
+
+    if drl_lib == "elegantrl":
+        from finrl.agents.elegantrl.models import DRLAgent as DRLAgent_erl
+
+        episode_total_assets = DRLAgent_erl.DRL_prediction(
+            model_name=model_name,
+            cwd=cwd,
+            net_dimension=net_dimension,
+            environment=env_instance,
+        )
         return episode_total_assets
+    elif drl_lib == "rllib":
+        from finrl.agents.rllib.models import DRLAgent as DRLAgent_rllib
+
+        episode_total_assets = DRLAgent_rllib.DRL_prediction(
+            model_name=model_name,
+            env=env,
+            price_array=price_array,
+            tech_array=tech_array,
+            turbulence_array=turbulence_array,
+            agent_path=cwd,
+        )
+        return episode_total_assets
+    elif drl_lib == "stable_baselines3":
+        from finrl.agents.stablebaselines3.models import DRLAgent as DRLAgent_sb3
+
+        episode_total_assets = DRLAgent_sb3.DRL_prediction_load_from_file(
+            model_name=model_name, environment=env_instance, cwd=cwd
+        )
+        return episode_total_assets
+    else:
+        raise ValueError("DRL library input is NOT supported. Please check.")
+
+
+if __name__ == "__main__":
+    env = StockTradingEnv
+
+    # demo for elegantrl
+    kwargs = (
+        {}
+    )  # in current meta, with respect yahoofinance, kwargs is {}. For other data sources, such as joinquant, kwargs is not empty
+
+    account_value_erl = test(
+        start_date=TEST_START_DATE,
+        end_date=TEST_END_DATE,
+        ticker_list=DOW_30_TICKER,
+        data_source="yahoofinance",
+        time_interval="1D",
+        technical_indicator_list=INDICATORS,
+        drl_lib="elegantrl",
+        env=env,
+        model_name="ppo",
+        cwd="./test_ppo",
+        net_dimension=512,
+        kwargs=kwargs,
+    )
+
+    ## if users want to use rllib, or stable-baselines3, users can remove the following comments
+
+    # # demo for rllib
+    # import ray
+    # ray.shutdown()  # always shutdown previous session if any
+    # account_value_rllib = test(
+    #     start_date=TEST_START_DATE,
+    #     end_date=TEST_END_DATE,
+    #     ticker_list=DOW_30_TICKER,
+    #     data_source="yahoofinance",
+    #     time_interval="1D",
+    #     technical_indicator_list=INDICATORS,
+    #     drl_lib="rllib",
+    #     env=env,
+    #     model_name="ppo",
+    #     cwd="./test_ppo/checkpoint_000030/checkpoint-30",
+    #     rllib_params=RLlib_PARAMS,
+    # )
+    #
+    # # demo for stable baselines3
+    # account_value_sb3 = test(
+    #     start_date=TEST_START_DATE,
+    #     end_date=TEST_END_DATE,
+    #     ticker_list=DOW_30_TICKER,
+    #     data_source="yahoofinance",
+    #     time_interval="1D",
+    #     technical_indicator_list=INDICATORS,
+    #     drl_lib="stable_baselines3",
+    #     env=env,
+    #     model_name="sac",
+    #     cwd="./test_sac.zip",
+    # )
```

### Comparing `finrl-0.3.6/finrl/agents/rllib/drllibv2.py` & `FinRL-0.3.7/finrl/agents/rllib/drllibv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,14 @@
         mode: str | list[str] = "max",
         max_failures: int = 0,
         training_iterations: int = 100,
         checkpoint_num_to_keep: None | int = None,
         checkpoint_freq: int = 0,
         reuse_actors: bool = False,
     ):
-
         if train_env is not None:
             register_env(train_env_name, lambda config: train_env)
 
         self.params = params
         self.params["framework"] = framework
         self.params["log_level"] = log_level
         self.params["num_gpus"] = num_gpus
```

### Comparing `finrl-0.3.6/finrl/agents/rllib/models.py` & `FinRL-0.3.7/finrl/agents/rllib/models.py`

 * *Files identical despite different names*

### Comparing `finrl-0.3.6/finrl/agents/stablebaselines3/hyperparams_opt.py` & `FinRL-0.3.7/finrl/agents/stablebaselines3/hyperparams_opt.py`

 * *Files identical despite different names*

### Comparing `finrl-0.3.6/finrl/agents/stablebaselines3/models.py` & `FinRL-0.3.7/finrl/agents/stablebaselines3/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,16 +36,25 @@
 
     def __init__(self, verbose=0):
         super().__init__(verbose)
 
     def _on_step(self) -> bool:
         try:
             self.logger.record(key="train/reward", value=self.locals["rewards"][0])
-        except BaseException:
-            self.logger.record(key="train/reward", value=self.locals["reward"][0])
+
+        except BaseException as error:
+            try:
+                self.logger.record(key="train/reward", value=self.locals["reward"][0])
+
+            except BaseException as inner_error:
+                # Handle the case where neither "rewards" nor "reward" is found
+                self.logger.record(key="train/reward", value=None)
+                # Print the original error and the inner error for debugging
+                print("Original Error:", error)
+                print("Inner Error:", inner_error)
         return True
 
 
 class DRLAgent:
     """Provides implementations for DRL algorithms
 
     Attributes
@@ -74,15 +83,17 @@
         policy_kwargs=None,
         model_kwargs=None,
         verbose=1,
         seed=None,
         tensorboard_log=None,
     ):
         if model_name not in MODELS:
-            raise NotImplementedError("NotImplementedError")
+            raise ValueError(
+                f"Model '{model_name}' not found in MODELS."
+            )  # this is more informative than NotImplementedError("NotImplementedError")
 
         if model_kwargs is None:
             model_kwargs = MODEL_KWARGS[model_name]
 
         if "action_noise" in model_kwargs:
             n_actions = self.env.action_space.shape[-1]
             model_kwargs["action_noise"] = NOISE[model_kwargs["action_noise"]](
@@ -95,54 +106,67 @@
             tensorboard_log=tensorboard_log,
             verbose=verbose,
             policy_kwargs=policy_kwargs,
             seed=seed,
             **model_kwargs,
         )
 
-    def train_model(self, model, tb_log_name, total_timesteps=5000):
+    @staticmethod
+    def train_model(
+        model, tb_log_name, total_timesteps=5000
+    ):  # this function is static method, so it can be called without creating an instance of the class
         model = model.learn(
             total_timesteps=total_timesteps,
             tb_log_name=tb_log_name,
             callback=TensorboardCallback(),
         )
         return model
 
     @staticmethod
     def DRL_prediction(model, environment, deterministic=True):
+        """make a prediction and get results"""
         test_env, test_obs = environment.get_sb_env()
-        """make a prediction"""
-        account_memory = []
-        actions_memory = []
-        #         state_memory=[] #add memory pool to store states
+        account_memory = None  # This help avoid unnecessary list creation
+        actions_memory = None  # optimize memory consumption
+        # state_memory=[] #add memory pool to store states
+
         test_env.reset()
+        max_steps = len(environment.df.index.unique()) - 1
+
         for i in range(len(environment.df.index.unique())):
             action, _states = model.predict(test_obs, deterministic=deterministic)
             # account_memory = test_env.env_method(method_name="save_asset_memory")
             # actions_memory = test_env.env_method(method_name="save_action_memory")
             test_obs, rewards, dones, info = test_env.step(action)
-            if i == (len(environment.df.index.unique()) - 2):
+
+            if (
+                i == max_steps - 1
+            ):  # more descriptive condition for early termination to clarify the logic
                 account_memory = test_env.env_method(method_name="save_asset_memory")
                 actions_memory = test_env.env_method(method_name="save_action_memory")
-            #                 state_memory=test_env.env_method(method_name="save_state_memory") # add current state to state memory
+            # add current state to state memory
+            # state_memory=test_env.env_method(method_name="save_state_memory")
+
             if dones[0]:
                 print("hit end!")
                 break
         return account_memory[0], actions_memory[0]
 
     @staticmethod
     def DRL_prediction_load_from_file(model_name, environment, cwd, deterministic=True):
         if model_name not in MODELS:
-            raise NotImplementedError("NotImplementedError")
+            raise ValueError(
+                f"Model '{model_name}' not found in MODELS."
+            )  # this is more informative than NotImplementedError("NotImplementedError")
         try:
             # load agent
             model = MODELS[model_name].load(cwd)
             print("Successfully load model", cwd)
-        except BaseException:
-            raise ValueError("Fail to load agent!")
+        except BaseException as error:
+            raise ValueError(f"Failed to load agent. Error: {str(error)}") from error
 
         # test on the testing env
         state = environment.reset()
         episode_returns = []  # the cumulative_return / initial_account
         episode_total_assets = [environment.initial_total_asset]
         done = False
         while not done:
@@ -169,17 +193,18 @@
         env,
         policy="MlpPolicy",
         policy_kwargs=None,
         model_kwargs=None,
         seed=None,
         verbose=1,
     ):
-
         if model_name not in MODELS:
-            raise NotImplementedError("NotImplementedError")
+            raise ValueError(
+                f"Model '{model_name}' not found in MODELS."
+            )  # this is more informative than NotImplementedError("NotImplementedError")
 
         if model_kwargs is None:
             temp_model_kwargs = MODEL_KWARGS[model_name]
         else:
             temp_model_kwargs = model_kwargs.copy()
 
         if "action_noise" in temp_model_kwargs:
@@ -243,15 +268,14 @@
         sell_cost_pct,
         reward_scaling,
         state_space,
         action_space,
         tech_indicator_list,
         print_verbosity,
     ):
-
         self.df = df
         self.train_period = train_period
         self.val_test_period = val_test_period
 
         self.unique_trade_date = df[
             (df.date > val_test_period[0]) & (df.date <= val_test_period[1])
         ].date.unique()
@@ -264,27 +288,28 @@
         self.buy_cost_pct = buy_cost_pct
         self.sell_cost_pct = sell_cost_pct
         self.reward_scaling = reward_scaling
         self.state_space = state_space
         self.action_space = action_space
         self.tech_indicator_list = tech_indicator_list
         self.print_verbosity = print_verbosity
+        self.train_env = None  # defined in train_validation() function
 
     def DRL_validation(self, model, test_data, test_env, test_obs):
         """validation process"""
         for _ in range(len(test_data.index.unique())):
             action, _states = model.predict(test_obs)
             test_obs, rewards, dones, info = test_env.step(action)
 
     def DRL_prediction(
         self, model, name, last_state, iter_num, turbulence_threshold, initial
     ):
         """make a prediction based on trained model"""
 
-        ## trading env
+        # trading env
         trade_data = data_split(
             self.df,
             start=self.unique_trade_date[iter_num - self.rebalance_window],
             end=self.unique_trade_date[iter_num],
         )
         trade_env = DummyVecEnv(
             [
@@ -314,33 +339,115 @@
         trade_obs = trade_env.reset()
 
         for i in range(len(trade_data.index.unique())):
             action, _states = model.predict(trade_obs)
             trade_obs, rewards, dones, info = trade_env.step(action)
             if i == (len(trade_data.index.unique()) - 2):
                 # print(env_test.render())
-                last_state = trade_env.render()
+                last_state = trade_env.envs[0].render()
 
         df_last_state = pd.DataFrame({"last_state": last_state})
         df_last_state.to_csv(f"results/last_state_{name}_{i}.csv", index=False)
         return last_state
 
+    def _train_window(
+        self,
+        model_name,
+        model_kwargs,
+        sharpe_list,
+        validation_start_date,
+        validation_end_date,
+        timesteps_dict,
+        i,
+        validation,
+        turbulence_threshold,
+    ):
+        """
+        Train the model for a single window.
+        """
+        if model_kwargs is None:
+            return None, sharpe_list, -1
+
+        print(f"======{model_name} Training========")
+        model = self.get_model(
+            model_name, self.train_env, policy="MlpPolicy", model_kwargs=model_kwargs
+        )
+        model = self.train_model(
+            model,
+            model_name,
+            tb_log_name=f"{model_name}_{i}",
+            iter_num=i,
+            total_timesteps=timesteps_dict[model_name],
+        )  # 100_000
+        print(
+            f"======{model_name} Validation from: ",
+            validation_start_date,
+            "to ",
+            validation_end_date,
+        )
+        val_env = DummyVecEnv(
+            [
+                lambda: StockTradingEnv(
+                    df=validation,
+                    stock_dim=self.stock_dim,
+                    hmax=self.hmax,
+                    initial_amount=self.initial_amount,
+                    num_stock_shares=[0] * self.stock_dim,
+                    buy_cost_pct=[self.buy_cost_pct] * self.stock_dim,
+                    sell_cost_pct=[self.sell_cost_pct] * self.stock_dim,
+                    reward_scaling=self.reward_scaling,
+                    state_space=self.state_space,
+                    action_space=self.action_space,
+                    tech_indicator_list=self.tech_indicator_list,
+                    turbulence_threshold=turbulence_threshold,
+                    iteration=i,
+                    model_name=model_name,
+                    mode="validation",
+                    print_verbosity=self.print_verbosity,
+                )
+            ]
+        )
+        val_obs = val_env.reset()
+        self.DRL_validation(
+            model=model,
+            test_data=validation,
+            test_env=val_env,
+            test_obs=val_obs,
+        )
+        sharpe = self.get_validation_sharpe(i, model_name=model_name)
+        print(f"{model_name} Sharpe Ratio: ", sharpe)
+        sharpe_list.append(sharpe)
+        return model, sharpe_list, sharpe
+
     def run_ensemble_strategy(
-        self, A2C_model_kwargs, PPO_model_kwargs, DDPG_model_kwargs, timesteps_dict
+        self,
+        A2C_model_kwargs,
+        PPO_model_kwargs,
+        DDPG_model_kwargs,
+        SAC_model_kwargs,
+        TD3_model_kwargs,
+        timesteps_dict,
     ):
-        """Ensemble Strategy that combines PPO, A2C and DDPG"""
+        # Model Parameters
+        kwargs = {
+            "a2c": A2C_model_kwargs,
+            "ppo": PPO_model_kwargs,
+            "ddpg": DDPG_model_kwargs,
+            "sac": SAC_model_kwargs,
+            "td3": TD3_model_kwargs,
+        }
+        # Model Sharpe Ratios
+        model_dct = {k: {"sharpe_list": [], "sharpe": -1} for k in MODELS.keys()}
+
+        """Ensemble Strategy that combines A2C, PPO, DDPG, SAC, and TD3"""
         print("============Start Ensemble Strategy============")
         # for ensemble model, it's necessary to feed the last state
         # of the previous model to the current model as the initial state
         last_state_ensemble = []
 
-        ppo_sharpe_list = []
-        ddpg_sharpe_list = []
-        a2c_sharpe_list = []
-
         model_use = []
         validation_start_date_list = []
         validation_end_date_list = []
         iteration_list = []
 
         insample_turbulence = self.df[
             (self.df.date < self.train_period[1])
@@ -362,15 +469,15 @@
             validation_end_date = self.unique_trade_date[i - self.rebalance_window]
 
             validation_start_date_list.append(validation_start_date)
             validation_end_date_list.append(validation_end_date)
             iteration_list.append(i)
 
             print("============================================")
-            ## initial state is empty
+            # initial state is empty
             if i - self.rebalance_window - self.validation_window == 0:
                 # inital state
                 initial = True
             else:
                 # previous state
                 initial = False
 
@@ -412,16 +519,16 @@
                 )
 
             turbulence_threshold = np.quantile(
                 insample_turbulence.turbulence.values, 0.99
             )
             print("turbulence_threshold: ", turbulence_threshold)
 
-            ############## Environment Setup starts ##############
-            ## training env
+            # Environment Setup starts
+            # training env
             train = data_split(
                 self.df,
                 start=self.train_period[0],
                 end=self.unique_trade_date[
                     i - self.rebalance_window - self.validation_window
                 ],
             )
@@ -447,223 +554,77 @@
             validation = data_split(
                 self.df,
                 start=self.unique_trade_date[
                     i - self.rebalance_window - self.validation_window
                 ],
                 end=self.unique_trade_date[i - self.rebalance_window],
             )
-            ############## Environment Setup ends ##############
+            # Environment Setup ends
 
-            ############## Training and Validation starts ##############
+            # Training and Validation starts
             print(
                 "======Model training from: ",
                 self.train_period[0],
                 "to ",
                 self.unique_trade_date[
                     i - self.rebalance_window - self.validation_window
                 ],
             )
             # print("training: ",len(data_split(df, start=20090000, end=test.datadate.unique()[i-rebalance_window]) ))
             # print("==============Model Training===========")
-            print("======A2C Training========")
-            model_a2c = self.get_model(
-                "a2c", self.train_env, policy="MlpPolicy", model_kwargs=A2C_model_kwargs
-            )
-            model_a2c = self.train_model(
-                model_a2c,
-                "a2c",
-                tb_log_name=f"a2c_{i}",
-                iter_num=i,
-                total_timesteps=timesteps_dict["a2c"],
-            )  # 100_000
-
-            print(
-                "======A2C Validation from: ",
-                validation_start_date,
-                "to ",
-                validation_end_date,
-            )
-            val_env_a2c = DummyVecEnv(
-                [
-                    lambda: StockTradingEnv(
-                        df=validation,
-                        stock_dim=self.stock_dim,
-                        hmax=self.hmax,
-                        initial_amount=self.initial_amount,
-                        num_stock_shares=[0] * self.stock_dim,
-                        buy_cost_pct=[self.buy_cost_pct] * self.stock_dim,
-                        sell_cost_pct=[self.sell_cost_pct] * self.stock_dim,
-                        reward_scaling=self.reward_scaling,
-                        state_space=self.state_space,
-                        action_space=self.action_space,
-                        tech_indicator_list=self.tech_indicator_list,
-                        turbulence_threshold=turbulence_threshold,
-                        iteration=i,
-                        model_name="A2C",
-                        mode="validation",
-                        print_verbosity=self.print_verbosity,
-                    )
-                ]
-            )
-            val_obs_a2c = val_env_a2c.reset()
-            self.DRL_validation(
-                model=model_a2c,
-                test_data=validation,
-                test_env=val_env_a2c,
-                test_obs=val_obs_a2c,
-            )
-            sharpe_a2c = self.get_validation_sharpe(i, model_name="A2C")
-            print("A2C Sharpe Ratio: ", sharpe_a2c)
-
-            print("======PPO Training========")
-            model_ppo = self.get_model(
-                "ppo", self.train_env, policy="MlpPolicy", model_kwargs=PPO_model_kwargs
-            )
-            model_ppo = self.train_model(
-                model_ppo,
-                "ppo",
-                tb_log_name=f"ppo_{i}",
-                iter_num=i,
-                total_timesteps=timesteps_dict["ppo"],
-            )  # 100_000
-            print(
-                "======PPO Validation from: ",
-                validation_start_date,
-                "to ",
-                validation_end_date,
-            )
-            val_env_ppo = DummyVecEnv(
-                [
-                    lambda: StockTradingEnv(
-                        df=validation,
-                        stock_dim=self.stock_dim,
-                        hmax=self.hmax,
-                        initial_amount=self.initial_amount,
-                        num_stock_shares=[0] * self.stock_dim,
-                        buy_cost_pct=[self.buy_cost_pct] * self.stock_dim,
-                        sell_cost_pct=[self.sell_cost_pct] * self.stock_dim,
-                        reward_scaling=self.reward_scaling,
-                        state_space=self.state_space,
-                        action_space=self.action_space,
-                        tech_indicator_list=self.tech_indicator_list,
-                        turbulence_threshold=turbulence_threshold,
-                        iteration=i,
-                        model_name="PPO",
-                        mode="validation",
-                        print_verbosity=self.print_verbosity,
-                    )
-                ]
-            )
-            val_obs_ppo = val_env_ppo.reset()
-            self.DRL_validation(
-                model=model_ppo,
-                test_data=validation,
-                test_env=val_env_ppo,
-                test_obs=val_obs_ppo,
-            )
-            sharpe_ppo = self.get_validation_sharpe(i, model_name="PPO")
-            print("PPO Sharpe Ratio: ", sharpe_ppo)
-
-            print("======DDPG Training========")
-            model_ddpg = self.get_model(
-                "ddpg",
-                self.train_env,
-                policy="MlpPolicy",
-                model_kwargs=DDPG_model_kwargs,
-            )
-            model_ddpg = self.train_model(
-                model_ddpg,
-                "ddpg",
-                tb_log_name=f"ddpg_{i}",
-                iter_num=i,
-                total_timesteps=timesteps_dict["ddpg"],
-            )  # 50_000
-            print(
-                "======DDPG Validation from: ",
-                validation_start_date,
-                "to ",
-                validation_end_date,
-            )
-            val_env_ddpg = DummyVecEnv(
-                [
-                    lambda: StockTradingEnv(
-                        df=validation,
-                        stock_dim=self.stock_dim,
-                        hmax=self.hmax,
-                        initial_amount=self.initial_amount,
-                        num_stock_shares=[0] * self.stock_dim,
-                        buy_cost_pct=[self.buy_cost_pct] * self.stock_dim,
-                        sell_cost_pct=[self.sell_cost_pct] * self.stock_dim,
-                        reward_scaling=self.reward_scaling,
-                        state_space=self.state_space,
-                        action_space=self.action_space,
-                        tech_indicator_list=self.tech_indicator_list,
-                        turbulence_threshold=turbulence_threshold,
-                        iteration=i,
-                        model_name="DDPG",
-                        mode="validation",
-                        print_verbosity=self.print_verbosity,
-                    )
-                ]
-            )
-            val_obs_ddpg = val_env_ddpg.reset()
-            self.DRL_validation(
-                model=model_ddpg,
-                test_data=validation,
-                test_env=val_env_ddpg,
-                test_obs=val_obs_ddpg,
-            )
-            sharpe_ddpg = self.get_validation_sharpe(i, model_name="DDPG")
-
-            ppo_sharpe_list.append(sharpe_ppo)
-            a2c_sharpe_list.append(sharpe_a2c)
-            ddpg_sharpe_list.append(sharpe_ddpg)
+            # Train Each Model
+            for model_name in MODELS.keys():
+                # Train The Model
+                model, sharpe_list, sharpe = self._train_window(
+                    model_name,
+                    kwargs[model_name],
+                    model_dct[model_name]["sharpe_list"],
+                    validation_start_date,
+                    validation_end_date,
+                    timesteps_dict,
+                    i,
+                    validation,
+                    turbulence_threshold,
+                )
+                # Save the model's sharpe ratios, and the model itself
+                model_dct[model_name]["sharpe_list"] = sharpe_list
+                model_dct[model_name]["model"] = model
+                model_dct[model_name]["sharpe"] = sharpe
 
             print(
                 "======Best Model Retraining from: ",
                 self.train_period[0],
                 "to ",
                 self.unique_trade_date[i - self.rebalance_window],
             )
             # Environment setup for model retraining up to first trade date
-            # train_full = data_split(self.df, start=self.train_period[0], end=self.unique_trade_date[i - self.rebalance_window])
+            # train_full = data_split(self.df, start=self.train_period[0],
+            # end=self.unique_trade_date[i - self.rebalance_window])
             # self.train_full_env = DummyVecEnv([lambda: StockTradingEnv(train_full,
-            #                                                    self.stock_dim,
-            #                                                    self.hmax,
-            #                                                    self.initial_amount,
-            #                                                    self.buy_cost_pct,
-            #                                                    self.sell_cost_pct,
-            #                                                    self.reward_scaling,
-            #                                                    self.state_space,
-            #                                                    self.action_space,
-            #                                                    self.tech_indicator_list,
-            #                                                    print_verbosity=self.print_verbosity)])
+            #                                               self.stock_dim,
+            #                                               self.hmax,
+            #                                               self.initial_amount,
+            #                                               self.buy_cost_pct,
+            #                                               self.sell_cost_pct,
+            #                                               self.reward_scaling,
+            #                                               self.state_space,
+            #                                               self.action_space,
+            #                                               self.tech_indicator_list,
+            #                                              print_verbosity=self.print_verbosity
+            # )])
             # Model Selection based on sharpe ratio
-            if (sharpe_ppo >= sharpe_a2c) & (sharpe_ppo >= sharpe_ddpg):
-                model_use.append("PPO")
-                model_ensemble = model_ppo
-
-                # model_ensemble = self.get_model("ppo",self.train_full_env,policy="MlpPolicy",model_kwargs=PPO_model_kwargs)
-                # model_ensemble = self.train_model(model_ensemble, "ensemble", tb_log_name="ensemble_{}".format(i), iter_num = i, total_timesteps=timesteps_dict['ppo']) #100_000
-            elif (sharpe_a2c > sharpe_ppo) & (sharpe_a2c > sharpe_ddpg):
-                model_use.append("A2C")
-                model_ensemble = model_a2c
-
-                # model_ensemble = self.get_model("a2c",self.train_full_env,policy="MlpPolicy",model_kwargs=A2C_model_kwargs)
-                # model_ensemble = self.train_model(model_ensemble, "ensemble", tb_log_name="ensemble_{}".format(i), iter_num = i, total_timesteps=timesteps_dict['a2c']) #100_000
-            else:
-                model_use.append("DDPG")
-                model_ensemble = model_ddpg
-
-                # model_ensemble = self.get_model("ddpg",self.train_full_env,policy="MlpPolicy",model_kwargs=DDPG_model_kwargs)
-                # model_ensemble = self.train_model(model_ensemble, "ensemble", tb_log_name="ensemble_{}".format(i), iter_num = i, total_timesteps=timesteps_dict['ddpg']) #50_000
-
-            ############## Training and Validation ends ##############
+            # Same order as MODELS: {"a2c": A2C, "ddpg": DDPG, "td3": TD3, "sac": SAC, "ppo": PPO}
+            sharpes = [model_dct[k]["sharpe"] for k in MODELS.keys()]
+            # Find the model with the highest sharpe ratio
+            max_mod = list(MODELS.keys())[np.argmax(sharpes)]
+            model_use.append(max_mod.upper())
+            model_ensemble = model_dct[max_mod]["model"]
+            # Training and Validation ends
 
-            ############## Trading starts ##############
+            # Trading starts
             print(
                 "======Trading from: ",
                 self.unique_trade_date[i - self.rebalance_window],
                 "to ",
                 self.unique_trade_date[i],
             )
             # print("Used Model: ", model_ensemble)
@@ -671,34 +632,38 @@
                 model=model_ensemble,
                 name="ensemble",
                 last_state=last_state_ensemble,
                 iter_num=i,
                 turbulence_threshold=turbulence_threshold,
                 initial=initial,
             )
-            ############## Trading ends ##############
+            # Trading ends
 
         end = time.time()
         print("Ensemble Strategy took: ", (end - start) / 60, " minutes")
 
         df_summary = pd.DataFrame(
             [
                 iteration_list,
                 validation_start_date_list,
                 validation_end_date_list,
                 model_use,
-                a2c_sharpe_list,
-                ppo_sharpe_list,
-                ddpg_sharpe_list,
+                model_dct["a2c"]["sharpe_list"],
+                model_dct["ppo"]["sharpe_list"],
+                model_dct["ddpg"]["sharpe_list"],
+                model_dct["sac"]["sharpe_list"],
+                model_dct["td3"]["sharpe_list"],
             ]
         ).T
         df_summary.columns = [
             "Iter",
             "Val Start",
             "Val End",
             "Model Used",
             "A2C Sharpe",
             "PPO Sharpe",
             "DDPG Sharpe",
+            "SAC Sharpe",
+            "TD3 Sharpe",
         ]
 
         return df_summary
```

### Comparing `finrl-0.3.6/finrl/agents/stablebaselines3/tune_sb3.py` & `FinRL-0.3.7/finrl/agents/stablebaselines3/tune_sb3.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 from __future__ import annotations
 
 import datetime
-import sys
-from pprint import pprint
-from typing import Tuple
-from typing import Union
 
-import hyperparams_opt as hpt
 import joblib
 import optuna
 import pandas as pd
-from main import check_and_make_directories
 from stable_baselines3 import A2C
 from stable_baselines3 import DDPG
 from stable_baselines3 import PPO
 from stable_baselines3 import SAC
 from stable_baselines3 import TD3
 
+import finrl.agents.stablebaselines3.hyperparams_opt as hpt
 from finrl import config
 from finrl.agents.stablebaselines3.models import DRLAgent
-from finrl.plot import backtest_plot
+from finrl.main import check_and_make_directories
 from finrl.plot import backtest_stats
-from finrl.plot import get_baseline
-from finrl.plot import get_daily_return
 
 
 class LoggingCallback:
     def __init__(self, threshold: int, trial_number: int, patience: int):
         """
         threshold:int tolerance for increase in sharpe ratio
         trial_number: int Prune after minimum number of trials
@@ -90,15 +83,14 @@
         env_train,
         model_name: str,
         env_trade,
         logging_callback,
         total_timesteps: int = 50000,
         n_trials: int = 30,
     ):
-
         self.env_train = env_train
         self.agent = DRLAgent(env=env_train)
         self.model_name = model_name
         self.env_trade = env_trade
         self.total_timesteps = total_timesteps
         self.n_trials = n_trials
         self.logging_callback = logging_callback
```

### Comparing `finrl-0.3.6/finrl/config.py` & `FinRL-0.3.7/finrl/config.py`

 * *Files identical despite different names*

### Comparing `finrl-0.3.6/finrl/config_tickers.py` & `FinRL-0.3.7/finrl/config_tickers.py`

 * *Files identical despite different names*

### Comparing `finrl-0.3.6/finrl/main.py` & `FinRL-0.3.7/finrl/main.py`

 * *Files identical despite different names*

### Comparing `finrl-0.3.6/finrl/meta/data_processor.py` & `FinRL-0.3.7/finrl/meta/data_processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 from finrl.meta.data_processors.processor_wrds import WrdsProcessor as Wrds
 from finrl.meta.data_processors.processor_yahoofinance import (
     YahooFinanceProcessor as YahooFinance,
 )
 
 
 class DataProcessor:
-    def __init__(self, data_source, **kwargs):
+    def __init__(self, data_source, tech_indicator=None, vix=None, **kwargs):
         if data_source == "alpaca":
-
             try:
                 API_KEY = kwargs.get("API_KEY")
                 API_SECRET = kwargs.get("API_SECRET")
                 API_BASE_URL = kwargs.get("API_BASE_URL")
                 self.processor = Alpaca(API_KEY, API_SECRET, API_BASE_URL)
                 print("Alpaca successfully connected")
             except BaseException:
@@ -28,14 +27,18 @@
 
         elif data_source == "yahoofinance":
             self.processor = YahooFinance()
 
         else:
             raise ValueError("Data source input is NOT supported yet.")
 
+        # Initialize variable in case it is using cache and does not use download_data() method
+        self.tech_indicator_list = tech_indicator
+        self.vix = vix
+
     def download_data(
         self, ticker_list, start_date, end_date, time_interval
     ) -> pd.DataFrame:
         df = self.processor.download_data(
             ticker_list=ticker_list,
             start_date=start_date,
             end_date=end_date,
@@ -60,14 +63,29 @@
         return df
 
     def add_vix(self, df) -> pd.DataFrame:
         df = self.processor.add_vix(df)
 
         return df
 
+    def add_turbulence(self, df) -> pd.DataFrame:
+        df = self.processor.add_turbulence(df)
+
+        return df
+
+    def add_vix(self, df) -> pd.DataFrame:
+        df = self.processor.add_vix(df)
+
+        return df
+
+    def add_vixor(self, df) -> pd.DataFrame:
+        df = self.processor.add_vixor(df)
+
+        return df
+
     def df_to_array(self, df, if_vix) -> np.array:
         price_array, tech_array, turbulence_array = self.processor.df_to_array(
             df, self.tech_indicator_list, if_vix
         )
         # fill nan and inf values with 0 for technical indicators
         tech_nan_positions = np.isnan(tech_array)
         tech_array[tech_nan_positions] = 0
```

### Comparing `finrl-0.3.6/finrl/meta/data_processors/processor_alpaca.py` & `FinRL-0.3.7/finrl/meta/data_processors/processor_alpaca.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from __future__ import annotations
 
+from concurrent.futures import ProcessPoolExecutor
+from concurrent.futures import ThreadPoolExecutor
+
 import alpaca_trade_api as tradeapi
 import exchange_calendars as tc
 import numpy as np
 import pandas as pd
 import pytz
 from stockstats import StockDataFrame as Sdf
 
@@ -14,147 +17,167 @@
             try:
                 self.api = tradeapi.REST(API_KEY, API_SECRET, API_BASE_URL, "v2")
             except BaseException:
                 raise ValueError("Wrong Account Info!")
         else:
             self.api = api
 
+    def _fetch_data_for_ticker(self, ticker, start_date, end_date, time_interval):
+        bars = self.api.get_bars(
+            ticker,
+            time_interval,
+            start=start_date.isoformat(),
+            end=end_date.isoformat(),
+        ).df
+        bars["symbol"] = ticker
+        return bars
+
     def download_data(
         self, ticker_list, start_date, end_date, time_interval
     ) -> pd.DataFrame:
         """
-        ticker_list : list string of ticket
-        time_interval: time interval
-        start_date : start date of America/New_York time
-        end_date : end date of America/New_York time
-
-        The function tries to retrieve the data, between the start date and the end date, from the Alpaca server.
-        if time_interval < 1D: period of data retrieved is the opening time of the New York Stock Exchange (NYSE) (from 9:30 am to 4:00 pm), in UTC offset zone.
-        if time_interval >= 1D: each bar is the midnight of the day in America/New_York time, in UTC offset zone.
+        Downloads data using Alpaca's tradeapi.REST method.
+
+        Parameters:
+        - ticker_list : list of strings, each string is a ticker
+        - start_date : string in the format 'YYYY-MM-DD'
+        - end_date : string in the format 'YYYY-MM-DD'
+        - time_interval: string representing the interval ('1D', '1Min', etc.)
+
+        Returns:
+        - pd.DataFrame with the requested data
         """
         self.start = start_date
         self.end = end_date
         self.time_interval = time_interval
 
-        # download
         NY = "America/New_York"
         start_date = pd.Timestamp(start_date + " 09:30:00", tz=NY)
         end_date = pd.Timestamp(end_date + " 15:59:00", tz=NY)
-        barset = self.api.get_bars(
-            ticker_list,
-            time_interval,
-            start=start_date.isoformat(),
-            end=end_date.isoformat(),
-        ).df
 
-        # from trepan.api import debug;debug()
-        # filter opening time of the New York Stock Exchange (NYSE) (from 9:30 am to 4:00 pm) if time_interval < 1D
-        day_delta = 86400000000000  # pd.Timedelta('1D').delta == 86400000000000
-        if pd.Timedelta(time_interval).delta < day_delta:
-            NYSE_open_hour = "14:30"  # in UTC
-            NYSE_close_hour = "20:59"  # in UTC
-            data_df = barset.between_time(NYSE_open_hour, NYSE_close_hour)
-        else:
-            data_df = barset
+        # Use ThreadPoolExecutor to fetch data for multiple tickers concurrently
+        with ThreadPoolExecutor(max_workers=10) as executor:
+            futures = [
+                executor.submit(
+                    self._fetch_data_for_ticker,
+                    ticker,
+                    start_date,
+                    end_date,
+                    time_interval,
+                )
+                for ticker in ticker_list
+            ]
+            data_list = [future.result() for future in futures]
+
+        # Combine the data
+        data_df = pd.concat(data_list, axis=0)
 
-        # reformat to finrl expected schema
-        data_df = data_df.reset_index().rename(columns={"symbol": "tic"})
-        data_df["timestamp"] = data_df["timestamp"].apply(lambda x: x.tz_convert(NY))
+        # Convert the timezone
+        data_df = data_df.tz_convert(NY)
+
+        # If time_interval is less than a day, filter out the times outside of NYSE trading hours
+        if pd.Timedelta(time_interval) < pd.Timedelta(days=1):
+            data_df = data_df.between_time("09:30", "15:59")
+
+        # Reset the index and rename the columns for consistency
+        data_df = data_df.reset_index().rename(
+            columns={"index": "timestamp", "symbol": "tic"}
+        )
+
+        # Sort the data by both timestamp and tic for consistent ordering
+        data_df = data_df.sort_values(by=["tic", "timestamp"])
+
+        # Reset the index and drop the old index column
+        data_df = data_df.reset_index(drop=True)
 
         return data_df
 
+    @staticmethod
+    def clean_individual_ticker(args):
+        tic, df, times = args
+        tmp_df = pd.DataFrame(index=times)
+        tic_df = df[df.tic == tic].set_index("timestamp")
+
+        # Step 1: Merging dataframes to avoid loop
+        tmp_df = tmp_df.merge(
+            tic_df[["open", "high", "low", "close", "volume"]],
+            left_index=True,
+            right_index=True,
+            how="left",
+        )
+
+        # Step 2: Handling NaN values efficiently
+        if pd.isna(tmp_df.iloc[0]["close"]):
+            first_valid_index = tmp_df["close"].first_valid_index()
+            if first_valid_index is not None:
+                first_valid_price = tmp_df.loc[first_valid_index, "close"]
+                print(
+                    f"The price of the first row for ticker {tic} is NaN. It will be filled with the first valid price."
+                )
+                tmp_df.iloc[0] = [first_valid_price] * 4 + [0.0]  # Set volume to zero
+            else:
+                print(
+                    f"Missing data for ticker: {tic}. The prices are all NaN. Fill with 0."
+                )
+                tmp_df.iloc[0] = [0.0] * 5
+
+        for i in range(1, tmp_df.shape[0]):
+            if pd.isna(tmp_df.iloc[i]["close"]):
+                previous_close = tmp_df.iloc[i - 1]["close"]
+                tmp_df.iloc[i] = [previous_close] * 4 + [0.0]
+
+        # Setting the volume for the market opening timestamp to zero - Not needed
+        # tmp_df.loc[tmp_df.index.time == pd.Timestamp("09:30:00").time(), 'volume'] = 0.0
+
+        # Step 3: Data type conversion
+        tmp_df = tmp_df.astype(float)
+
+        tmp_df["tic"] = tic
+
+        return tmp_df
+
     def clean_data(self, df):
+        print("Data cleaning started")
         tic_list = np.unique(df.tic.values)
         n_tickers = len(tic_list)
 
-        # align start and end dates
-        unique_times = df["timestamp"].unique()
-        for time in unique_times:
-            if len(df[df.timestamp == time].index) < n_tickers:
-                df = df[df.timestamp != time]
+        print("align start and end dates")
+        grouped = df.groupby("timestamp")
+        filter_mask = grouped.transform("count")["tic"] >= n_tickers
+        df = df[filter_mask]
+
+        # ... (generating 'times' series, same as in your existing code)
 
         trading_days = self.get_trading_days(start=self.start, end=self.end)
+
         # produce full timestamp index
+        print("produce full timestamp index")
         times = []
         for day in trading_days:
             NY = "America/New_York"
             current_time = pd.Timestamp(day + " 09:30:00").tz_localize(NY)
             for i in range(390):
                 times.append(current_time)
                 current_time += pd.Timedelta(minutes=1)
 
-        # create a new dataframe with full timestamp series
-        new_df = pd.DataFrame()
-        for tic in tic_list:
-            tmp_df = pd.DataFrame(
-                columns=["open", "high", "low", "close", "volume"], index=times
-            )
-            tic_df = df[df.tic == tic]
-            for i in range(tic_df.shape[0]):
-                tmp_df.loc[tic_df.iloc[i]["timestamp"]] = tic_df.iloc[i][
-                    ["open", "high", "low", "close", "volume"]
-                ]
+        print("Start processing tickers")
 
-            # if the close price of the first row is NaN
-            if str(tmp_df.iloc[0]["close"]) == "nan":
-                print(
-                    "The price of the first row for ticker ",
-                    tic,
-                    " is NaN. ",
-                    "It will filled with the first valid price.",
-                )
-                for i in range(tmp_df.shape[0]):
-                    if str(tmp_df.iloc[i]["close"]) != "nan":
-                        first_valid_price = tmp_df.iloc[i]["close"]
-                        tmp_df.iloc[0] = [
-                            first_valid_price,
-                            first_valid_price,
-                            first_valid_price,
-                            first_valid_price,
-                            0.0,
-                        ]
-                        break
+        future_results = []
+        for tic in tic_list:
+            result = self.clean_individual_ticker((tic, df.copy(), times))
+            future_results.append(result)
 
-            # if the close price of the first row is still NaN (All the prices are NaN in this case)
-            if str(tmp_df.iloc[0]["close"]) == "nan":
-                print(
-                    "Missing data for ticker: ",
-                    tic,
-                    " . The prices are all NaN. Fill with 0.",
-                )
-                tmp_df.iloc[0] = [
-                    0.0,
-                    0.0,
-                    0.0,
-                    0.0,
-                    0.0,
-                ]
-
-            # forward filling row by row
-            for i in range(tmp_df.shape[0]):
-                if str(tmp_df.iloc[i]["close"]) == "nan":
-                    previous_close = tmp_df.iloc[i - 1]["close"]
-                    if str(previous_close) == "nan":
-                        raise ValueError
-                    tmp_df.iloc[i] = [
-                        previous_close,
-                        previous_close,
-                        previous_close,
-                        previous_close,
-                        0.0,
-                    ]
-
-            tmp_df = tmp_df.astype(float)
-            tmp_df["tic"] = tic
-            new_df = pd.concat([new_df, tmp_df])
+        print("ticker list complete")
 
+        print("Start concat and rename")
+        new_df = pd.concat(future_results)
         new_df = new_df.reset_index()
         new_df = new_df.rename(columns={"index": "timestamp"})
 
-        # print("Data clean finished!")
+        print("Data clean finished!")
 
         return new_df
 
     def add_technical_indicator(
         self,
         df,
         tech_indicator_list=[
@@ -163,53 +186,92 @@
             "boll_lb",
             "rsi_30",
             "dx_30",
             "close_30_sma",
             "close_60_sma",
         ],
     ):
-        df = df.rename(columns={"timestamp": "date"})
-        df = df.copy()
-        df = df.sort_values(by=["tic", "date"])
-        stock = Sdf.retype(df.copy())
+        print("Started adding Indicators")
+
+        # Store the original data type of the 'timestamp' column
+        original_timestamp_dtype = df["timestamp"].dtype
+
+        # Convert df to stock data format just once
+        stock = Sdf.retype(df)
         unique_ticker = stock.tic.unique()
-        tech_indicator_list = tech_indicator_list
 
+        # Convert timestamp to a consistent datatype (timezone-naive) before entering the loop
+        df["timestamp"] = df["timestamp"].dt.tz_convert(None)
+
+        print("Running Loop")
         for indicator in tech_indicator_list:
-            indicator_df = pd.DataFrame()
-            for i in range(len(unique_ticker)):
-                # print(unique_ticker[i], i)
-                temp_indicator = stock[stock.tic == unique_ticker[i]][indicator]
-                temp_indicator = pd.DataFrame(temp_indicator)
-                temp_indicator["tic"] = unique_ticker[i]
-                # print(len(df[df.tic == unique_ticker[i]]['date'].to_list()))
-                temp_indicator["date"] = df[df.tic == unique_ticker[i]][
-                    "date"
-                ].to_list()
-                indicator_df = pd.concat(
-                    [indicator_df, temp_indicator], ignore_index=True
+            indicator_dfs = []
+            for tic in unique_ticker:
+                tic_data = stock[stock.tic == tic]
+                indicator_series = tic_data[indicator]
+
+                tic_timestamps = df.loc[df.tic == tic, "timestamp"]
+
+                indicator_df = pd.DataFrame(
+                    {
+                        "tic": tic,
+                        "date": tic_timestamps.values,
+                        indicator: indicator_series.values,
+                    }
                 )
+                indicator_dfs.append(indicator_df)
+
+            # Concatenate all intermediate dataframes at once
+            indicator_df = pd.concat(indicator_dfs, ignore_index=True)
+
+            # Merge the indicator data frame
             df = df.merge(
-                indicator_df[["tic", "date", indicator]], on=["tic", "date"], how="left"
-            )
-        df = df.sort_values(by=["date", "tic"])
-        df = df.rename(columns={"date": "timestamp"})
-        #        print("Succesfully add technical indicators")
+                indicator_df[["tic", "date", indicator]],
+                left_on=["tic", "timestamp"],
+                right_on=["tic", "date"],
+                how="left",
+            ).drop(columns="date")
+
+        print("Restore Timestamps")
+        # Restore the original data type of the 'timestamp' column
+        if isinstance(original_timestamp_dtype, pd.DatetimeTZDtype):
+            if df["timestamp"].dt.tz is None:
+                df["timestamp"] = df["timestamp"].dt.tz_localize("UTC")
+            df["timestamp"] = df["timestamp"].dt.tz_convert(original_timestamp_dtype.tz)
+        else:
+            df["timestamp"] = df["timestamp"].astype(original_timestamp_dtype)
+
+        print("Finished adding Indicators")
         return df
 
-    def add_vix(self, data):
+    # Allows to multithread the add_vix function for quicker execution
+    def download_and_clean_data(self):
         vix_df = self.download_data(["VIXY"], self.start, self.end, self.time_interval)
-        cleaned_vix = self.clean_data(vix_df)
+        return self.clean_data(vix_df)
+
+    def add_vix(self, data):
+        with ThreadPoolExecutor() as executor:
+            future = executor.submit(self.download_and_clean_data)
+            cleaned_vix = future.result()
+
         vix = cleaned_vix[["timestamp", "close"]]
-        vix = vix.rename(columns={"close": "VIXY"})
 
-        df = data.copy()
-        df = df.merge(vix, on="timestamp")
-        df = df.sort_values(["timestamp", "tic"]).reset_index(drop=True)
-        return df
+        merge_column = "date" if "date" in data.columns else "timestamp"
+
+        vix = vix.rename(
+            columns={"timestamp": merge_column, "close": "VIXY"}
+        )  # Change column name dynamically
+
+        data = data.copy()
+        data = data.merge(
+            vix, on=merge_column
+        )  # Use the dynamic column name for merging
+        data = data.sort_values([merge_column, "tic"]).reset_index(drop=True)
+
+        return data
 
     def calculate_turbulence(self, data, time_period=252):
         # can add other market assets
         df = data.copy()
         df_price_pivot = df.pivot(index="timestamp", columns="tic", values="close")
         # use returns to calculate turbulence
         df_price_pivot = df_price_pivot.pct_change()
@@ -292,26 +354,25 @@
                 )
         #        print("Successfully transformed into array")
         return price_array, tech_array, turbulence_array
 
     def get_trading_days(self, start, end):
         nyse = tc.get_calendar("NYSE")
         df = nyse.sessions_in_range(
-            pd.Timestamp(start, tz=pytz.UTC), pd.Timestamp(end, tz=pytz.UTC)
+            pd.Timestamp(start).tz_localize(None), pd.Timestamp(end).tz_localize(None)
         )
         trading_days = []
         for day in df:
             trading_days.append(str(day)[:10])
 
         return trading_days
 
     def fetch_latest_data(
         self, ticker_list, time_interval, tech_indicator_list, limit=100
     ) -> pd.DataFrame:
-
         data_df = pd.DataFrame()
         for tic in ticker_list:
             barset = self.api.get_bars([tic], time_interval, limit=limit).df  # [tic]
             barset["tic"] = tic
             barset = barset.reset_index()
             data_df = pd.concat([data_df, barset])
```

### Comparing `finrl-0.3.6/finrl/meta/data_processors/processor_ccxt.py` & `FinRL-0.3.7/finrl/meta/data_processors/processor_ccxt.py`

 * *Files identical despite different names*

### Comparing `finrl-0.3.6/finrl/meta/data_processors/processor_joinquant.py` & `FinRL-0.3.7/finrl/meta/data_processors/processor_joinquant.py`

 * *Files identical despite different names*

### Comparing `finrl-0.3.6/finrl/meta/data_processors/processor_quantconnect.py` & `FinRL-0.3.7/finrl/meta/data_processors/processor_quantconnect.py`

 * *Files identical despite different names*

### Comparing `finrl-0.3.6/finrl/meta/data_processors/processor_wrds.py` & `FinRL-0.3.7/finrl/meta/data_processors/processor_wrds.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         start_date,
         end_date,
         ticker_list,
         time_interval,
         if_save_tempfile=False,
         filter_shares=0,
     ):
-
         self.start = start_date
         self.end = end_date
         self.time_interval = time_interval
 
         def get_trading_days(start, end):
             nyse = tc.get_calendar("NYSE")
             df = nyse.sessions_in_range(
@@ -51,15 +50,16 @@
             parm = {"syms": stock_set, "num_shares": filter_shares}
             try:
                 data = self.db.raw_sql(
                     "select * from "
                     + lib
                     + "."
                     + table
-                    + " where sym_root in %(syms)s and time_m between '9:30:00' and '16:00:00' and size > %(num_shares)s and sym_suffix is null",
+                    + " where sym_root in %(syms)s "
+                    + "and time_m between '9:30:00' and '16:00:00' and size > %(num_shares)s and sym_suffix is null",
                     params=parm,
                 )
                 if_empty = False
                 return data, if_empty
             except BaseException:
                 print("Data for date: " + date + " error")
                 if_empty = True
@@ -174,15 +174,16 @@
                 if i not in tic_time:
                     missing_time.append(i)
             for time in missing_time:
                 temp_df = pd.DataFrame(
                     [[time, np.nan, np.nan, np.nan, np.nan, 0, tic]],
                     columns=["time", "open", "high", "low", "close", "volume", "tic"],
                 )
-                df2 = df2.append(temp_df, ignore_index=True)
+                # df2 = df2.append(temp_df, ignore_index=True)
+                df2 = pd.concat([df2, temp_df], axis=0, ignore_index=True)
 
         # fill nan data
         df = df2.sort_values(by=["tic", "time"])
         for i in range(df.shape[0]):
             if float(df.iloc[i]["volume"]) == 0:
                 previous_close = df.iloc[i - 1]["close"]
                 if str(previous_close) == "nan":
@@ -227,15 +228,19 @@
                 temp_indicator = stock[stock.tic == unique_ticker[i]][indicator]
                 temp_indicator = pd.DataFrame(temp_indicator)
                 temp_indicator["tic"] = unique_ticker[i]
                 # print(len(df[df.tic == unique_ticker[i]]['date'].to_list()))
                 temp_indicator["date"] = df[df.tic == unique_ticker[i]][
                     "date"
                 ].to_list()
-                indicator_df = indicator_df.append(temp_indicator, ignore_index=True)
+                # indicator_df = indicator_df.append(temp_indicator, ignore_index=True)
+                indicator_df = pd.concat(
+                    [indicator_df, temp_indicator], axis=0, ignore_index=True
+                )
+
             df = df.merge(
                 indicator_df[["tic", "date", indicator]], on=["tic", "date"], how="left"
             )
         df = df.sort_values(by=["date", "tic"])
         print("Succesfully add technical indicators")
         return df
```

### Comparing `finrl-0.3.6/finrl/meta/data_processors/processor_yahoofinance.py` & `FinRL-0.3.7/finrl/meta/data_processors/processor_yahoofinance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Reference: https://github.com/AI4Finance-LLC/FinRL"""
+
 from __future__ import annotations
 
 import datetime
 from datetime import date
 from datetime import timedelta
 from sqlite3 import Timestamp
 from typing import Any
@@ -51,47 +52,47 @@
     0	2009-01-02	AAPL	3.067143	3.251429	3.041429	2.767330	746015200.0
     1	2009-01-02	AMGN	58.590000	59.080002	57.750000	44.523766	6547900.0
     2	2009-01-02	AXP	    18.570000	19.520000	18.400000	15.477426	10955700.0
     3	2009-01-02	BA	    42.799999	45.560001	42.779999	33.941093	7010200.0
     ...
     """
 
-    def download_data(
-        self, ticker_list: list[str], start_date: str, end_date: str, time_interval: str
-    ) -> pd.DataFrame:
+    def convert_interval(self, time_interval: str) -> str:
         # Convert FinRL 'standardised' time periods to Yahoo format: 1m, 2m, 5m, 15m, 30m, 60m, 90m, 1h, 1d, 5d, 1wk, 1mo, 3mo
-        if time_interval == "1Min":
-            time_interval = "1m"
-        elif time_interval == "2Min":
-            time_interval = "2m"
-        elif time_interval == "5Min":
-            time_interval = "5m"
-        elif time_interval == "15Min":
-            time_interval = "15m"
-        elif time_interval == "30Min":
-            time_interval = "30m"
-        elif time_interval == "60Min":
-            time_interval = "60m"
-        elif time_interval == "90Min":
-            time_interval = "90m"
-        elif time_interval == "1H":
-            time_interval = "1h"
-        elif time_interval == "1D":
-            time_interval = "1d"
-        elif time_interval == "5D":
-            time_interval = "5d"
+        if time_interval in [
+            "1Min",
+            "2Min",
+            "5Min",
+            "15Min",
+            "30Min",
+            "60Min",
+            "90Min",
+        ]:
+            time_interval = time_interval.replace("Min", "m")
+        elif time_interval in ["1H", "1D", "5D", "1h", "1d", "5d"]:
+            time_interval = time_interval.lower()
         elif time_interval == "1W":
             time_interval = "1wk"
-        elif time_interval == "1M":
-            time_interval = "1mo"
-        elif time_interval == "3M":
-            time_interval = "3mo"
+        elif time_interval in ["1M", "3M"]:
+            time_interval = time_interval.replace("M", "mo")
         else:
             raise ValueError("wrong time_interval")
 
+        return time_interval
+
+    def download_data(
+        self,
+        ticker_list: list[str],
+        start_date: str,
+        end_date: str,
+        time_interval: str,
+        proxy: str | dict = None,
+    ) -> pd.DataFrame:
+        time_interval = self.convert_interval(time_interval)
+
         self.start = start_date
         self.end = end_date
         self.time_interval = time_interval
 
         # Download and save the data in a pandas DataFrame
         start_date = pd.Timestamp(start_date)
         end_date = pd.Timestamp(end_date)
@@ -102,14 +103,15 @@
                 start_date <= end_date
             ):  # downloading daily to workaround yfinance only allowing  max 7 calendar (not trading) days of 1 min data per single download
                 temp_df = yf.download(
                     tic,
                     start=start_date,
                     end=start_date + delta,
                     interval=self.time_interval,
+                    proxy=proxy,
                 )
                 temp_df["tic"] = tic
                 data_df = pd.concat([data_df, temp_df])
                 start_date += delta
 
         data_df = data_df.reset_index().drop(columns=["Adj Close"])
         # convert the column names to match processor_alpaca.py as far as poss
@@ -366,61 +368,30 @@
                     [tech_array, df[df.tic == tic][tech_indicator_list].values]
                 )
         #        print("Successfully transformed into array")
         return price_array, tech_array, turbulence_array
 
     def get_trading_days(self, start: str, end: str) -> list[str]:
         nyse = tc.get_calendar("NYSE")
-        df = nyse.sessions_in_range(
-            pd.Timestamp(start, tz=pytz.UTC), pd.Timestamp(end, tz=pytz.UTC)
-        )
+        df = nyse.sessions_in_range(pd.Timestamp(start), pd.Timestamp(end))
         trading_days = []
         for day in df:
             trading_days.append(str(day)[:10])
 
         return trading_days
 
     # ****** NB: YAHOO FINANCE DATA MAY BE IN REAL-TIME OR DELAYED BY 15 MINUTES OR MORE, DEPENDING ON THE EXCHANGE ******
     def fetch_latest_data(
         self,
         ticker_list: list[str],
         time_interval: str,
         tech_indicator_list: list[str],
         limit: int = 100,
     ) -> pd.DataFrame:
-
-        # Convert FinRL 'standardised' Alpaca time periods to Yahoo format: 1m, 2m, 5m, 15m, 30m, 60m, 90m, 1h, 1d, 5d, 1wk, 1mo, 3mo
-        if time_interval == "1Min":
-            time_interval = "1m"
-        elif time_interval == "2Min":
-            time_interval = "2m"
-        elif time_interval == "5Min":
-            time_interval = "5m"
-        elif time_interval == "15Min":
-            time_interval = "15m"
-        elif time_interval == "30Min":
-            time_interval = "30m"
-        elif time_interval == "60Min":
-            time_interval = "60m"
-        elif time_interval == "90Min":
-            time_interval = "90m"
-        elif time_interval == "1H":
-            time_interval = "1h"
-        elif time_interval == "1D":
-            time_interval = "1d"
-        elif time_interval == "5D":
-            time_interval = "5d"
-        elif time_interval == "1W":
-            time_interval = "1wk"
-        elif time_interval == "1M":
-            time_interval = "1mo"
-        elif time_interval == "3M":
-            time_interval = "3mo"
-        else:
-            raise ValueError("wrong time_interval")
+        time_interval = self.convert_interval(time_interval)
 
         end_datetime = datetime.datetime.now()
         start_datetime = end_datetime - datetime.timedelta(
             minutes=limit + 1
         )  # get the last rows up to limit
 
         data_df = pd.DataFrame()
```

### Comparing `finrl-0.3.6/finrl/meta/env_cryptocurrency_trading/env_btc_ccxt.py` & `FinRL-0.3.7/finrl/meta/env_cryptocurrency_trading/env_btc_ccxt.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,20 @@
         self.env_name = "BitcoinEnv4"
         self.state_dim = 1 + 1 + self.price_ary.shape[1] + self.tech_ary.shape[1]
         self.action_dim = 1
         self.if_discrete = False
         self.target_return = 10
         self.max_step = self.price_ary.shape[0]
 
-    def reset(self) -> np.ndarray:
+    def reset(
+        self,
+        *,
+        seed=None,
+        options=None,
+    ) -> np.ndarray:
         self.day = 0
         self.day_price = self.price_ary[self.day]
         self.day_tech = self.tech_ary[self.day]
         self.initial_account__reset = self.initial_account  # reset()
         self.account = self.initial_account__reset
         self.stocks = 0.0
         self.total_asset = self.account + self.day_price[0] * self.stocks
@@ -145,15 +150,15 @@
         episode_returns = list()
         episode_returns.append(1)
         btc_returns = list()  # the cumulative_return / initial_account
         with _torch.no_grad():
             for i in range(self.max_step):
                 if i == 0:
                     init_price = self.day_price[0]
-                btc_returns.append(self.day_price[0] / init_price)
+                btc_returns.append(self.day_price[i] / init_price)
                 s_tensor = _torch.as_tensor((state,), device=device)
                 a_tensor = act(s_tensor)  # action_tanh = act.forward()
                 action = (
                     a_tensor.detach().cpu().numpy()[0]
                 )  # not need detach(), because with torch.no_grad() outside
                 state, reward, done, _ = self.step(action)
```

### Comparing `finrl-0.3.6/finrl/meta/env_cryptocurrency_trading/env_multiple_crypto.py` & `FinRL-0.3.7/finrl/meta/env_cryptocurrency_trading/env_multiple_crypto.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,20 @@
         self.state_dim = (
             1 + (self.price_array.shape[1] + self.tech_array.shape[1]) * lookback
         )
         self.action_dim = self.price_array.shape[1]
         self.if_discrete = False
         self.target_return = 10
 
-    def reset(self) -> np.ndarray:
+    def reset(
+        self,
+        *,
+        seed=None,
+        options=None,
+    ) -> np.ndarray:
         self.time = self.lookback - 1
         self.current_price = self.price_array[self.time]
         self.current_tech = self.tech_array[self.time]
         self.cash = self.initial_cash  # reset()
         self.stocks = np.zeros(self.crypto_num, dtype=np.float32)
         self.total_asset = self.cash + (self.stocks * self.price_array[self.time]).sum()
```

### Comparing `finrl-0.3.6/finrl/meta/env_portfolio_allocation/env_portfolio.py` & `FinRL-0.3.7/finrl/meta/env_portfolio_allocation/env_portfolio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
-import gym
+import gymnasium as gym
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-from gym import spaces
-from gym.utils import seeding
+from gymnasium import spaces
+from gymnasium.utils import seeding
 from stable_baselines3.common.vec_env import DummyVecEnv
 
 matplotlib.use("Agg")
 
 
 class StockPortfolioEnv(gym.Env):
     """A single stock trading environment for OpenAI gym
@@ -149,22 +149,23 @@
                     (252**0.5)
                     * df_daily_return["daily_return"].mean()
                     / df_daily_return["daily_return"].std()
                 )
                 print("Sharpe: ", sharpe)
             print("=================================")
 
-            return self.state, self.reward, self.terminal, {}
+            return self.state, self.reward, self.terminal, False, {}
 
         else:
             # print("Model actions: ",actions)
             # actions are the portfolio weight
             # normalize to sum of 1
             # if (np.array(actions) - np.array(actions).min()).sum() != 0:
-            #  norm_actions = (np.array(actions) - np.array(actions).min()) / (np.array(actions) - np.array(actions).min()).sum()
+            #  norm_actions = (np.array(actions) - np.array(actions).min()) /
+            #                   (np.array(actions) - np.array(actions).min()).sum()
             # else:
             #  norm_actions = actions
             weights = self.softmax_normalization(actions)
             # print("Normalized actions: ", weights)
             self.actions_memory.append(weights)
             last_day_memory = self.data
 
@@ -193,17 +194,22 @@
             self.asset_memory.append(new_portfolio_value)
 
             # the reward is the new portfolio value or end portfolo value
             self.reward = new_portfolio_value
             # print("Step reward: ", self.reward)
             # self.reward = self.reward*self.reward_scaling
 
-        return self.state, self.reward, self.terminal, {}
+        return self.state, self.reward, self.terminal, False, {}
 
-    def reset(self):
+    def reset(
+        self,
+        *,
+        seed=None,
+        options=None,
+    ):
         self.asset_memory = [self.initial_amount]
         self.day = 0
         self.data = self.df.loc[self.day, :]
         # load states
         self.covs = self.data["cov_list"].values[0]
         self.state = np.append(
             np.array(self.covs),
@@ -213,15 +219,15 @@
         self.portfolio_value = self.initial_amount
         # self.cost = 0
         # self.trades = 0
         self.terminal = False
         self.portfolio_return_memory = [0]
         self.actions_memory = [[1 / self.stock_dim] * self.stock_dim]
         self.date_memory = [self.data.date.unique()[0]]
-        return self.state
+        return self.state, {}
 
     def render(self, mode="human"):
         return self.state
 
     def softmax_normalization(self, actions):
         numerator = np.exp(actions)
         denominator = np.sum(np.exp(actions))
```

### Comparing `finrl-0.3.6/finrl/meta/env_stock_trading/env_nas100_wrds.py` & `FinRL-0.3.7/finrl/meta/env_stock_trading/env_nas100_wrds.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,20 @@
         self.stocks_cd = None
         self.action_dim = stock_dim
         self.max_step = self.price_ary.shape[0] - 1
         self.if_discrete = False
         self.target_return = 2.2
         self.episode_return = 0.0
 
-    def reset(self):
+    def reset(
+        self,
+        *,
+        seed=None,
+        options=None,
+    ):
         self.day = 0
         price = self.price_ary[self.day]
 
         self.stocks = (
             self.initial_stocks + rd.randint(0, 64, size=self.initial_stocks.shape)
         ).astype(np.float32)
         self.stocks_cd = np.zeros_like(self.stocks)
```

### Comparing `finrl-0.3.6/finrl/meta/env_stock_trading/env_stock_papertrading.py` & `FinRL-0.3.7/finrl/meta/env_stock_trading/env_stock_papertrading.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import datetime
 import threading
 import time
 
 import alpaca_trade_api as tradeapi
-import gym
+import gymnasium as gym
 import numpy as np
 import pandas as pd
 import torch
 
 from finrl.meta.data_processors.processor_alpaca import AlpacaProcessor
 
 
@@ -160,15 +160,14 @@
         # Wait for market to open.
         print("Waiting for market to open...")
         tAMO = threading.Thread(target=self.awaitMarketOpen)
         tAMO.start()
         tAMO.join()
         print("Market opened.")
         while True:
-
             # Figure out when the market will close so we can prepare to sell beforehand.
             clock = self.alpaca.get_clock()
             closingTime = clock.next_close.replace(
                 tzinfo=datetime.timezone.utc
             ).timestamp()
             currTime = clock.timestamp.replace(tzinfo=datetime.timezone.utc).timestamp()
             self.timeToClose = closingTime - currTime
@@ -398,12 +397,17 @@
         self.observation_space = gym.spaces.Box(
             low=-3000, high=3000, shape=(state_dim,), dtype=np.float32
         )
         self.action_space = gym.spaces.Box(
             low=-1, high=1, shape=(action_dim,), dtype=np.float32
         )
 
-    def reset(self):
+    def reset(
+        self,
+        *,
+        seed=None,
+        options=None,
+    ):
         return
 
     def step(self, actions):
         return
```

### Comparing `finrl-0.3.6/finrl/meta/env_stock_trading/env_stocktrading.py` & `FinRL-0.3.7/finrl/meta/env_stock_trading/env_stocktrading.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from typing import List
 
-import gym
+import gymnasium as gym
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-from gym import spaces
-from gym.utils import seeding
+from gymnasium import spaces
+from gymnasium.utils import seeding
 from stable_baselines3.common.vec_env import DummyVecEnv
 
 matplotlib.use("Agg")
 
 # from stable_baselines3.common.logger import Logger, KVWriter, CSVOutputFormat
 
 
@@ -293,15 +293,15 @@
             # Add outputs to logger interface
             # logger.record("environment/portfolio_value", end_total_asset)
             # logger.record("environment/total_reward", tot_reward)
             # logger.record("environment/total_reward_pct", (tot_reward / (end_total_asset - tot_reward)) * 100)
             # logger.record("environment/total_cost", self.cost)
             # logger.record("environment/total_trades", self.trades)
 
-            return self.state, self.reward, self.terminal, {}
+            return self.state, self.reward, self.terminal, False, {}
 
         else:
             actions = actions * self.hmax  # actions initially is scaled between 0 to 1
             actions = actions.astype(
                 int
             )  # convert into integer because we can't by fraction of shares
             if self.turbulence_threshold is not None:
@@ -349,18 +349,25 @@
             self.reward = end_total_asset - begin_total_asset
             self.rewards_memory.append(self.reward)
             self.reward = self.reward * self.reward_scaling
             self.state_memory.append(
                 self.state
             )  # add current state in state_recorder for each step
 
-        return self.state, self.reward, self.terminal, {}
+        return self.state, self.reward, self.terminal, False, {}
 
-    def reset(self):
+    def reset(
+        self,
+        *,
+        seed=None,
+        options=None,
+    ):
         # initiate state
+        self.day = 0
+        self.data = self.df.loc[self.day, :]
         self.state = self._initiate_state()
 
         if self.initial:
             self.asset_memory = [
                 self.initial_amount
                 + np.sum(
                     np.array(self.num_stock_shares)
@@ -372,28 +379,26 @@
                 np.array(self.state[1 : (self.stock_dim + 1)])
                 * np.array(
                     self.previous_state[(self.stock_dim + 1) : (self.stock_dim * 2 + 1)]
                 )
             )
             self.asset_memory = [previous_total_asset]
 
-        self.day = 0
-        self.data = self.df.loc[self.day, :]
         self.turbulence = 0
         self.cost = 0
         self.trades = 0
         self.terminal = False
         # self.iteration=self.iteration
         self.rewards_memory = []
         self.actions_memory = []
         self.date_memory = [self._get_date()]
 
         self.episode += 1
 
-        return self.state
+        return self.state, {}
 
     def render(self, mode="human", close=False):
         return self.state
 
     def _initiate_state(self):
         if self.initial:
             # For Initial State
```

### Comparing `finrl-0.3.6/finrl/meta/env_stock_trading/env_stocktrading_cashpenalty.py` & `FinRL-0.3.7/finrl/meta/env_stock_trading/env_stocktrading_cashpenalty.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,20 @@
         # Quantity of shares held at current timestep
         return self.state_memory[-1][1 : len(self.assets) + 1]
 
     @property
     def closings(self):
         return np.array(self.get_date_vector(self.date_index, cols=["close"]))
 
-    def reset(self):
+    def reset(
+        self,
+        *,
+        seed=None,
+        options=None,
+    ):
         self.seed()
         self.sum_trades = 0
         if self.random_start:
             starting_point = random.choice(range(int(len(self.dates) * 0.5)))
             self.starting_point = starting_point
         else:
             self.starting_point = 0
@@ -201,15 +206,14 @@
             "environment/cash_proportion",
             self.account_information["cash"][-1]
             / self.account_information["total_assets"][-1],
         )
         return state, reward, True, {}
 
     def log_step(self, reason, terminal_reward=None):
-
         if terminal_reward is None:
             terminal_reward = self.account_information["reward"][-1]
         cash_pct = (
             self.account_information["cash"][-1]
             / self.account_information["total_assets"][-1]
         )
         gl_pct = self.account_information["total_assets"][-1] / self.initial_amount
```

### Comparing `finrl-0.3.6/finrl/meta/env_stock_trading/env_stocktrading_np.py` & `FinRL-0.3.7/finrl/meta/env_stock_trading/env_stocktrading_np.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-import gym
+import gymnasium as gym
 import numpy as np
 from numpy import random as rd
 
 
 class StockTradingEnv(gym.Env):
     def __init__(
         self,
@@ -73,15 +73,20 @@
         self.observation_space = gym.spaces.Box(
             low=-3000, high=3000, shape=(self.state_dim,), dtype=np.float32
         )
         self.action_space = gym.spaces.Box(
             low=-1, high=1, shape=(self.action_dim,), dtype=np.float32
         )
 
-    def reset(self):
+    def reset(
+        self,
+        *,
+        seed=None,
+        options=None,
+    ):
         self.day = 0
         price = self.price_ary[self.day]
 
         if self.if_train:
             self.stocks = (
                 self.initial_stocks + rd.randint(0, 64, size=self.initial_stocks.shape)
             ).astype(np.float32)
@@ -94,15 +99,15 @@
             self.stocks = self.initial_stocks.astype(np.float32)
             self.stocks_cool_down = np.zeros_like(self.stocks)
             self.amount = self.initial_capital
 
         self.total_asset = self.amount + (self.stocks * price).sum()
         self.initial_total_asset = self.total_asset
         self.gamma_reward = 0.0
-        return self.get_state(price)  # state
+        return self.get_state(price), {}  # state
 
     def step(self, actions):
         actions = (actions * self.max_stock).astype(int)
 
         self.day += 1
         price = self.price_ary[self.day]
         self.stocks_cool_down += 1
@@ -140,15 +145,15 @@
 
         self.gamma_reward = self.gamma_reward * self.gamma + reward
         done = self.day == self.max_step
         if done:
             reward = self.gamma_reward
             self.episode_return = total_asset / self.initial_total_asset
 
-        return state, reward, done, dict()
+        return state, reward, done, False, dict()
 
     def get_state(self, price):
         amount = np.array(self.amount * (2**-12), dtype=np.float32)
         scale = np.array(2**-6, dtype=np.float32)
         return np.hstack(
             (
                 amount,
```

### Comparing `finrl-0.3.6/finrl/meta/env_stock_trading/env_stocktrading_stoploss.py` & `FinRL-0.3.7/finrl/meta/env_stock_trading/env_stocktrading_stoploss.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,20 @@
             seed = int(round(time.time() * 1000))
         random.seed(seed)
 
     @property
     def current_step(self):
         return self.date_index - self.starting_point
 
-    def reset(self):
+    def reset(
+        self,
+        *,
+        seed=None,
+        options=None,
+    ):
         self.seed()
         self.sum_trades = 0
         self.actual_num_trades = 0
         self.closing_diff_avg_buy = np.zeros(len(self.assets))
         self.profit_sell_diff_avg_buy = np.zeros(len(self.assets))
         self.n_buys = np.zeros(len(self.assets))
         self.avg_buy_price = np.zeros(len(self.assets))
```

### Comparing `finrl-0.3.6/finrl/meta/meta_config.py` & `FinRL-0.3.7/finrl/meta/meta_config.py`

 * *Files identical despite different names*

### Comparing `finrl-0.3.6/finrl/meta/preprocessor/preprocessors.py` & `FinRL-0.3.7/finrl/meta/preprocessor/preprocessors.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
         # add user defined feature
         if self.user_defined_feature:
             df = self.add_user_defined_feature(df)
             print("Successfully added user defined features")
 
         # fill the missing values at the beginning and the end
-        df = df.fillna(method="ffill").fillna(method="bfill")
+        df = df.ffill().bfill()
         return df
 
     def clean_data(self, data):
         """
         clean the raw data
         deal with missing values
         reasons: stocks could be delisted, not incorporated at the time step
@@ -151,16 +151,19 @@
                 try:
                     temp_indicator = stock[stock.tic == unique_ticker[i]][indicator]
                     temp_indicator = pd.DataFrame(temp_indicator)
                     temp_indicator["tic"] = unique_ticker[i]
                     temp_indicator["date"] = df[df.tic == unique_ticker[i]][
                         "date"
                     ].to_list()
-                    indicator_df = indicator_df.append(
-                        temp_indicator, ignore_index=True
+                    # indicator_df = indicator_df.append(
+                    #     temp_indicator, ignore_index=True
+                    # )
+                    indicator_df = pd.concat(
+                        [indicator_df, temp_indicator], axis=0, ignore_index=True
                     )
                 except Exception as e:
                     print(e)
             df = df.merge(
                 indicator_df[["tic", "date", indicator]], on=["tic", "date"], how="left"
             )
         df = df.sort_values(by=["date", "tic"])
```

### Comparing `finrl-0.3.6/finrl/meta/preprocessor/tusharedownloader.py` & `FinRL-0.3.7/finrl/meta/preprocessor/tusharedownloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Contains methods and classes to collect data from
 tushare API
 """
+
 from __future__ import annotations
 
 import pandas as pd
 import tushare as ts
 from tqdm import tqdm
 
 
@@ -19,15 +20,15 @@
             end date of the data (modified from config.py)
         ticker_list : list
             a list of stock tickers (modified from config.py)
     Methods
     -------
     fetch_data()
         Fetches data from tushare API
-    date：date
+    date: date
     Open: opening price
     High: the highest price
     Close: closing price
     Low: lowest price
     Volume: volume
     Price_change: price change
     P_change: fluctuation
@@ -36,21 +37,20 @@
     Ma20:20 average daily price
     V_ma5:5 daily average
     V_ma10:10 daily average
     V_ma20:20 daily average
     """
 
     def __init__(self, start_date: str, end_date: str, ticker_list: list):
-
         self.start_date = start_date
         self.end_date = end_date
         self.ticker_list = ticker_list
 
     def fetch_data(self) -> pd.DataFrame:
-        """Fetches data from Yahoo API
+        """Fetches data from Alpaca
         Parameters
         ----------
         Returns
         -------
         `pd.DataFrame`
             7 columns: A date, open, high, low, close, volume and tick symbol
             for the specified stock ticker
@@ -58,15 +58,17 @@
         # Download and save the data in a pandas DataFrame:
         data_df = pd.DataFrame()
         for tic in tqdm(self.ticker_list, total=len(self.ticker_list)):
             temp_df = ts.get_hist_data(
                 tic[0:6], start=self.start_date, end=self.end_date
             )
             temp_df["tic"] = tic[0:6]
-            data_df = data_df.append(temp_df)
+            # data_df = data_df.append(temp_df)
+            data_df = pd.concat([data_df, temp_df], axis=0, ignore_index=True)
+
         data_df = data_df.reset_index(level="date")
 
         # create day of the week column (monday = 0)
         data_df = data_df.drop(
             [
                 "price_change",
                 "p_change",
@@ -78,40 +80,29 @@
                 "v_ma20",
             ],
             1,
         )
         data_df["day"] = pd.to_datetime(data_df["date"]).dt.dayofweek
         # rank desc
         data_df = data_df.sort_index(axis=0, ascending=False)
-        data_df = data_df.reset_index(drop=True)
         # convert date to standard string format, easy to filter
         data_df["date"] = pd.to_datetime(data_df["date"])
         data_df["date"] = data_df.date.apply(lambda x: x.strftime("%Y-%m-%d"))
         # drop missing data
         data_df = data_df.dropna()
+        data_df = data_df.reset_index(drop=True)
         print("Shape of DataFrame: ", data_df.shape)
         # print("Display DataFrame: ", data_df.head())
         print(data_df)
         data_df = data_df.sort_values(by=["date", "tic"]).reset_index(drop=True)
         return data_df
 
     def select_equal_rows_stock(self, df):
         df_check = df.tic.value_counts()
         df_check = pd.DataFrame(df_check).reset_index()
         df_check.columns = ["tic", "counts"]
         mean_df = df_check.counts.mean()
         equal_list = list(df.tic.value_counts() >= mean_df)
-        names = df.tic.value_counts().index
-        select_stocks_list = list(names[equal_list])
-        df = df[df.tic.isin(select_stocks_list)]
-        return df
-
-    def select_equal_rows_stock(self, df):
-        df_check = df.tic.value_counts()
-        df_check = pd.DataFrame(df_check).reset_index()
-        df_check.columns = ["tic", "counts"]
-        mean_df = df_check.counts.mean()
-        equal_list = list(df.tic.value_counts() >= mean_df)
         names = df.tic.value_counts().index
         select_stocks_list = list(names[equal_list])
         df = df[df.tic.isin(select_stocks_list)]
         return df
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `finrl-0.3.6/finrl/meta/preprocessor/yahoodownloader.py` & `FinRL-0.3.7/finrl/meta/preprocessor/yahoodownloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Contains methods and classes to collect data from
 Yahoo Finance API
 """
+
 from __future__ import annotations
 
 import pandas as pd
 import yfinance as yf
 
 
 class YahooDownloader:
@@ -24,15 +25,14 @@
     -------
     fetch_data()
         Fetches data from yahoo API
 
     """
 
     def __init__(self, start_date: str, end_date: str, ticker_list: list):
-
         self.start_date = start_date
         self.end_date = end_date
         self.ticker_list = ticker_list
 
     def fetch_data(self, proxy=None) -> pd.DataFrame:
         """Fetches data from Yahoo API
         Parameters
@@ -42,20 +42,27 @@
         -------
         `pd.DataFrame`
             7 columns: A date, open, high, low, close, volume and tick symbol
             for the specified stock ticker
         """
         # Download and save the data in a pandas DataFrame:
         data_df = pd.DataFrame()
+        num_failures = 0
         for tic in self.ticker_list:
             temp_df = yf.download(
                 tic, start=self.start_date, end=self.end_date, proxy=proxy
             )
             temp_df["tic"] = tic
-            data_df = data_df.append(temp_df)
+            if len(temp_df) > 0:
+                # data_df = data_df.append(temp_df)
+                data_df = pd.concat([data_df, temp_df], axis=0)
+            else:
+                num_failures += 1
+        if num_failures == len(self.ticker_list):
+            raise ValueError("no data is fetched.")
         # reset the index, we want to use numbers as index instead of dates
         data_df = data_df.reset_index()
         try:
             # convert the column names to standardized names
             data_df.columns = [
                 "date",
                 "open",
```

### Comparing `finrl-0.3.6/finrl/test.py` & `FinRL-0.3.7/finrl/train.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,138 +1,160 @@
 from __future__ import annotations
 
+from finrl.config import ERL_PARAMS
 from finrl.config import INDICATORS
 from finrl.config import RLlib_PARAMS
-from finrl.config import TEST_END_DATE
-from finrl.config import TEST_START_DATE
+from finrl.config import SAC_PARAMS
+from finrl.config import TRAIN_END_DATE
+from finrl.config import TRAIN_START_DATE
 from finrl.config_tickers import DOW_30_TICKER
-from finrl.meta.env_stock_trading.env_stocktrading import StockTradingEnv
+from finrl.meta.data_processor import DataProcessor
+from finrl.meta.env_stock_trading.env_stocktrading_np import StockTradingEnv
 
+# construct environment
 
-def test(
+
+def train(
     start_date,
     end_date,
     ticker_list,
     data_source,
     time_interval,
     technical_indicator_list,
     drl_lib,
     env,
     model_name,
     if_vix=True,
     **kwargs,
 ):
-
-    # import data processor
-    from finrl.meta.data_processor import DataProcessor
-
-    # fetch data
+    # download data
     dp = DataProcessor(data_source, **kwargs)
     data = dp.download_data(ticker_list, start_date, end_date, time_interval)
     data = dp.clean_data(data)
     data = dp.add_technical_indicator(data, technical_indicator_list)
-
     if if_vix:
         data = dp.add_vix(data)
     price_array, tech_array, turbulence_array = dp.df_to_array(data, if_vix)
-
     env_config = {
         "price_array": price_array,
         "tech_array": tech_array,
         "turbulence_array": turbulence_array,
-        "if_train": False,
+        "if_train": True,
     }
     env_instance = env(config=env_config)
 
-    # load elegantrl needs state dim, action dim and net dim
-    net_dimension = kwargs.get("net_dimension", 2**7)
+    # read parameters
     cwd = kwargs.get("cwd", "./" + str(model_name))
-    print("price_array: ", len(price_array))
 
     if drl_lib == "elegantrl":
         from finrl.agents.elegantrl.models import DRLAgent as DRLAgent_erl
 
-        episode_total_assets = DRLAgent_erl.DRL_prediction(
-            model_name=model_name,
-            cwd=cwd,
-            net_dimension=net_dimension,
-            environment=env_instance,
+        break_step = kwargs.get("break_step", 1e6)
+        erl_params = kwargs.get("erl_params")
+        agent = DRLAgent_erl(
+            env=env,
+            price_array=price_array,
+            tech_array=tech_array,
+            turbulence_array=turbulence_array,
+        )
+        model = agent.get_model(model_name, model_kwargs=erl_params)
+        trained_model = agent.train_model(
+            model=model, cwd=cwd, total_timesteps=break_step
         )
-        return episode_total_assets
     elif drl_lib == "rllib":
+        total_episodes = kwargs.get("total_episodes", 100)
+        rllib_params = kwargs.get("rllib_params")
         from finrl.agents.rllib.models import DRLAgent as DRLAgent_rllib
 
-        episode_total_assets = DRLAgent_rllib.DRL_prediction(
-            model_name=model_name,
+        agent_rllib = DRLAgent_rllib(
             env=env,
             price_array=price_array,
             tech_array=tech_array,
             turbulence_array=turbulence_array,
-            agent_path=cwd,
         )
-        return episode_total_assets
+        model, model_config = agent_rllib.get_model(model_name)
+        model_config["lr"] = rllib_params["lr"]
+        model_config["train_batch_size"] = rllib_params["train_batch_size"]
+        model_config["gamma"] = rllib_params["gamma"]
+        # ray.shutdown()
+        trained_model = agent_rllib.train_model(
+            model=model,
+            model_name=model_name,
+            model_config=model_config,
+            total_episodes=total_episodes,
+        )
+        trained_model.save(cwd)
     elif drl_lib == "stable_baselines3":
+        total_timesteps = kwargs.get("total_timesteps", 1e6)
+        agent_params = kwargs.get("agent_params")
         from finrl.agents.stablebaselines3.models import DRLAgent as DRLAgent_sb3
 
-        episode_total_assets = DRLAgent_sb3.DRL_prediction_load_from_file(
-            model_name=model_name, environment=env_instance, cwd=cwd
+        agent = DRLAgent_sb3(env=env_instance)
+        model = agent.get_model(model_name, model_kwargs=agent_params)
+        trained_model = agent.train_model(
+            model=model, tb_log_name=model_name, total_timesteps=total_timesteps
         )
-        return episode_total_assets
+        print("Training is finished!")
+        trained_model.save(cwd)
+        print("Trained model is saved in " + str(cwd))
     else:
         raise ValueError("DRL library input is NOT supported. Please check.")
 
 
 if __name__ == "__main__":
     env = StockTradingEnv
 
     # demo for elegantrl
     kwargs = (
         {}
     )  # in current meta, with respect yahoofinance, kwargs is {}. For other data sources, such as joinquant, kwargs is not empty
-
-    account_value_erl = test(
-        start_date=TEST_START_DATE,
-        end_date=TEST_END_DATE,
+    train(
+        start_date=TRAIN_START_DATE,
+        end_date=TRAIN_END_DATE,
         ticker_list=DOW_30_TICKER,
         data_source="yahoofinance",
         time_interval="1D",
         technical_indicator_list=INDICATORS,
         drl_lib="elegantrl",
         env=env,
         model_name="ppo",
         cwd="./test_ppo",
-        net_dimension=512,
+        erl_params=ERL_PARAMS,
+        break_step=1e5,
         kwargs=kwargs,
     )
 
     ## if users want to use rllib, or stable-baselines3, users can remove the following comments
 
     # # demo for rllib
     # import ray
     # ray.shutdown()  # always shutdown previous session if any
-    # account_value_rllib = test(
-    #     start_date=TEST_START_DATE,
-    #     end_date=TEST_END_DATE,
+    # train(
+    #     start_date=TRAIN_START_DATE,
+    #     end_date=TRAIN_END_DATE,
     #     ticker_list=DOW_30_TICKER,
     #     data_source="yahoofinance",
     #     time_interval="1D",
     #     technical_indicator_list=INDICATORS,
     #     drl_lib="rllib",
     #     env=env,
     #     model_name="ppo",
-    #     cwd="./test_ppo/checkpoint_000030/checkpoint-30",
+    #     cwd="./test_ppo",
     #     rllib_params=RLlib_PARAMS,
+    #     total_episodes=30,
     # )
     #
-    # # demo for stable baselines3
-    # account_value_sb3 = test(
-    #     start_date=TEST_START_DATE,
-    #     end_date=TEST_END_DATE,
+    # # demo for stable-baselines3
+    # train(
+    #     start_date=TRAIN_START_DATE,
+    #     end_date=TRAIN_END_DATE,
     #     ticker_list=DOW_30_TICKER,
     #     data_source="yahoofinance",
     #     time_interval="1D",
     #     technical_indicator_list=INDICATORS,
     #     drl_lib="stable_baselines3",
     #     env=env,
     #     model_name="sac",
-    #     cwd="./test_sac.zip",
+    #     cwd="./test_sac",
+    #     agent_params=SAC_PARAMS,
+    #     total_timesteps=1e4,
     # )
```

### Comparing `finrl-0.3.6/finrl/trade.py` & `FinRL-0.3.7/finrl/trade.py`

 * *Files identical despite different names*

### Comparing `finrl-0.3.6/finrl.egg-info/PKG-INFO` & `FinRL-0.3.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
-Name: finrl
-Version: 0.3.6
+Name: FinRL
+Version: 0.3.7
 Summary: FinRL: Financial Reinforcement Learning Framework.
-Home-page: https://github.com/finrl/finrl-library
-Author: Hongyang Yang, Xiaoyang Liu, Ming Zhu
-Author-email: hy2500@columbia.edu
+Home-page: https://github.com/AI4Finance-Foundation/FinRL
+Author: AI4Finance Foundation
+Author-email: contact@ai4finance.org
 License: MIT
 Keywords: Reinforcement Learning,Finance
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 License-File: LICENSE
 
 Version 0.3.5 notes: stable version, code refactoring, more tutorials, clear documentation
-
```

### Comparing `finrl-0.3.6/finrl.egg-info/SOURCES.txt` & `FinRL-0.3.7/FinRL.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+FinRL.egg-info/PKG-INFO
+FinRL.egg-info/SOURCES.txt
+FinRL.egg-info/dependency_links.txt
+FinRL.egg-info/top_level.txt
 finrl/__init__.py
 finrl/__main__.py
 finrl/config.py
 finrl/config_private.py
 finrl/config_tickers.py
 finrl/main.py
 finrl/plot.py
 finrl/test.py
 finrl/trade.py
 finrl/train.py
-finrl.egg-info/PKG-INFO
-finrl.egg-info/SOURCES.txt
-finrl.egg-info/dependency_links.txt
-finrl.egg-info/top_level.txt
 finrl/agents/__init__.py
 finrl/agents/elegantrl/__init__.py
 finrl/agents/elegantrl/models.py
+finrl/agents/portfolio_optimization/__init__.py
+finrl/agents/portfolio_optimization/algorithms.py
+finrl/agents/portfolio_optimization/architectures.py
+finrl/agents/portfolio_optimization/models.py
+finrl/agents/portfolio_optimization/utils.py
 finrl/agents/rllib/__init__.py
 finrl/agents/rllib/drllibv2.py
 finrl/agents/rllib/models.py
 finrl/agents/stablebaselines3/__init__.py
 finrl/agents/stablebaselines3/hyperparams_opt.py
 finrl/agents/stablebaselines3/models.py
 finrl/agents/stablebaselines3/tune_sb3.py
 finrl/applications/__init__.py
 finrl/applications/cryptocurrency_trading/__init__.py
 finrl/applications/high_frequency_trading/__init__.py
 finrl/applications/portfolio_allocation/__init__.py
 finrl/applications/stock_trading/__init__.py
+finrl/applications/stock_trading/ensemble_stock_trading.py
+finrl/applications/stock_trading/fundamental_stock_trading.py
+finrl/applications/stock_trading/stock_trading.py
+finrl/applications/stock_trading/stock_trading_rolling_window.py
 finrl/meta/__init__.py
 finrl/meta/data_processor.py
 finrl/meta/meta_config.py
 finrl/meta/data_processors/__init__.py
 finrl/meta/data_processors/func.py
 finrl/meta/data_processors/processor_alpaca.py
 finrl/meta/data_processors/processor_ccxt.py
@@ -44,14 +53,16 @@
 finrl/meta/data_processors/processor_wrds.py
 finrl/meta/data_processors/processor_yahoofinance.py
 finrl/meta/env_cryptocurrency_trading/__init__.py
 finrl/meta/env_cryptocurrency_trading/env_btc_ccxt.py
 finrl/meta/env_cryptocurrency_trading/env_multiple_crypto.py
 finrl/meta/env_portfolio_allocation/__init__.py
 finrl/meta/env_portfolio_allocation/env_portfolio.py
+finrl/meta/env_portfolio_optimization/__init__.py
+finrl/meta/env_portfolio_optimization/env_portfolio_optimization.py
 finrl/meta/env_stock_trading/__init__.py
 finrl/meta/env_stock_trading/env_nas100_wrds.py
 finrl/meta/env_stock_trading/env_stock_papertrading.py
 finrl/meta/env_stock_trading/env_stocktrading.py
 finrl/meta/env_stock_trading/env_stocktrading_cashpenalty.py
 finrl/meta/env_stock_trading/env_stocktrading_np.py
 finrl/meta/env_stock_trading/env_stocktrading_stoploss.py
```

### Comparing `finrl-0.3.6/pyproject.toml` & `FinRL-0.3.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finrl"
-version = "0.3.5"
+version = "0.3.6"
 
 description = "FinRL: Financial Reinforcement Learning Framework. Version 0.3.5 notes: stable version, code refactoring, more tutorials, clear documentation"
 authors = ["Hongyang Yang, Xiaoyang Liu"]
 license = "MIT"
 
 readme = "README.md"
 classifiers=[
@@ -12,43 +12,41 @@
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ]
 keywords=["Reinforcement Learning", "Finance"]
 [tool.poetry.urls]
 github = "https://github.com/finrl/finrl-library"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.9"
-pyfolio = {git="https://github.com/quantopian/pyfolio.git#egg=pyfolio-0.9.2"}
+python = "~3.10"
 elegantrl = {git="https://github.com/AI4Finance-Foundation/ElegantRL.git#egg=elegantrl"}
-alpaca_trade_api = ">=2.1.0"
-ccxt = ">=1.66.32"
-exchange_calendars = "3.6.3"
-gputil = "*"
-gym = ">=0.17"
-importlib-metadata = "4.13.0"
-jqdatasdk = "*"
-lz4 = "*"
-matplotlib = "*"
-pandas = ">=1.1.5"
-numpy = ">=1.17.3"
-tensorboardX = "*"
-yfinance = "*"
-stockstats = ">=0.4.0"
-scikit-learn = ">=0.21.0"
-ray = {extras=["default", "tune"], version=">=2.0.0"}
-stable-baselines3 = "^1.6.2"
+alpaca-trade-api = "^3"
+ccxt = "^3"
+exchange-calendars = "^4"
+jqdatasdk = "^1"
+pyfolio = "^0.9"
+pyportfolioopt = "^1"
+ray = {extras=["default", "tune"], version = "^2"}
+scikit-learn = "^1"
+stable-baselines3 = {version = ">=2.0.0a5", extras = ["extra"]}
+stockstats = "^0.5"
+wrds = "^3"
+yfinance = "^0.2"
 
-[tool.poetry.dev-dependencies]
-pytest = "*"
-pre-commit = "*"
+[tool.poetry.group.dev.dependencies]
+black = "^24"
+isort = "^5"
+jupyter = "^1"
+mypy = "^1"
+pandas-stubs = "^2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `finrl-0.3.6/setup.cfg` & `FinRL-0.3.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `finrl-0.3.6/setup.py` & `FinRL-0.3.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,35 +14,36 @@
         if line:
             REQUIRES.append(line)
 except FileNotFoundError:
     print("'requirements.txt' not found!")
     REQUIRES = list()
 
 setup(
-    name="finrl",
-    version="0.3.6",
+    name="FinRL",
+    version="0.3.7",
     include_package_data=True,
-    author="Hongyang Yang, Xiaoyang Liu, Ming Zhu",
-    author_email="hy2500@columbia.edu",
-    url="https://github.com/finrl/finrl-library",
+    author="AI4Finance Foundation",
+    author_email="contact@ai4finance.org",
+    url="https://github.com/AI4Finance-Foundation/FinRL",
     license="MIT",
     packages=find_packages(),
     description="FinRL: Financial Reinforcement Learning Framework.",
     long_description="Version 0.3.5 notes: stable version, code refactoring, more tutorials, clear documentation",
     # It is developed by `AI4Finance`_. \
-    # _AI4Finance: https://github.com/AI4Finance-Foundation",
+    # _AI4Finance: https://ai4finance.org/",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     keywords="Reinforcement Learning, Finance",
     platform=["any"],
     python_requires=">=3.7",
 )
```

