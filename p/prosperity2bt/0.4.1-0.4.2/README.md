# Comparing `tmp/prosperity2bt-0.4.1.tar.gz` & `tmp/prosperity2bt-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.4.1.tar", last modified: Wed Apr 10 23:12:02 2024, max compression
+gzip compressed data, was "prosperity2bt-0.4.2.tar", last modified: Thu Apr 11 00:38:16 2024, max compression
```

## Comparing `prosperity2bt-0.4.1.tar` & `prosperity2bt-0.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:12:02.305780 prosperity2bt-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-10 23:12:02.305780 prosperity2bt-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:12:02.297780 prosperity2bt-0.4.1/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/datamodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:12:02.297780 prosperity2bt-0.4.1/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:12:02.301780 prosperity2bt-0.4.1/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:12:02.305780 prosperity2bt-0.4.1/prosperity2bt/resources/round1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-10 23:11:58.000000 prosperity2bt-0.4.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:12:02.305780 prosperity2bt-0.4.1/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-10 23:12:02.000000 prosperity2bt-0.4.1/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-10 23:12:02.000000 prosperity2bt-0.4.1/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:12:02.000000 prosperity2bt-0.4.1/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 23:12:02.000000 prosperity2bt-0.4.1/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 23:12:02.000000 prosperity2bt-0.4.1/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 23:12:02.000000 prosperity2bt-0.4.1/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-10 23:12:00.000000 prosperity2bt-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:12:02.305780 prosperity2bt-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:16.857293 prosperity2bt-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-11 00:38:16.857293 prosperity2bt-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:16.845292 prosperity2bt-0.4.2/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/datamodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:16.849292 prosperity2bt-0.4.2/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:16.849292 prosperity2bt-0.4.2/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:16.853292 prosperity2bt-0.4.2/prosperity2bt/resources/round1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/resources/round1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/resources/round1/prices_round_1_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-11 00:38:08.000000 prosperity2bt-0.4.2/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:38:16.857293 prosperity2bt-0.4.2/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-11 00:38:16.000000 prosperity2bt-0.4.2/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-11 00:38:16.000000 prosperity2bt-0.4.2/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:38:16.000000 prosperity2bt-0.4.2/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 00:38:16.000000 prosperity2bt-0.4.2/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 00:38:16.000000 prosperity2bt-0.4.2/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 00:38:16.000000 prosperity2bt-0.4.2/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-11 00:38:13.000000 prosperity2bt-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:38:16.857293 prosperity2bt-0.4.2/setup.cfg
```

### Comparing `prosperity2bt-0.4.1/LICENSE` & `prosperity2bt-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.1/PKG-INFO` & `prosperity2bt-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.4.1
+Version: 0.4.2
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -89,14 +89,17 @@
 # Backtest on custom data
 # Requires the value passed to `--data` to be a path to a directory that is similar in structure to https://github.com/jmerle/imc-prosperity-2-backtester/tree/master/prosperity2bt/resources
 $ prosperity2bt example/starter.py 1 --data prosperity2bt/resources
 
 # Print trader's output to stdout while running
 # This may be helpful when debugging a broken trader
 $ prosperity2bt example/starter.py 1 --print
+
+# Only match orders against order depths, not against market trades
+$ prosperity2bt example/starter.py 1 --no-trades-matching
 ```
 
 ## Order Matching
 
 Orders placed by `Trader.run` at a given timestamp are matched against the order depths and market trades of that timestamp's state. Order depths take priority, if an order can be filled completely using volume in the relevant order depth, market trades are not considered. If not, the backtester matches your order against the timestamp's market trades. In this case the backtester assumes that for each trade, the buyer and the seller of the trade are willing to trade with you instead at the trade's price and volume. Market trades are matched at the price of your orders, e.g. if you place a sell order for €9 and there is a market trade for €10, the sell order is matched at €9 (even though there is a buyer willing to pay €10, this appears to be consistent with what the official Prosperity environment does).
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
```

### Comparing `prosperity2bt-0.4.1/README.md` & `prosperity2bt-0.4.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,17 @@
 # Backtest on custom data
 # Requires the value passed to `--data` to be a path to a directory that is similar in structure to https://github.com/jmerle/imc-prosperity-2-backtester/tree/master/prosperity2bt/resources
 $ prosperity2bt example/starter.py 1 --data prosperity2bt/resources
 
 # Print trader's output to stdout while running
 # This may be helpful when debugging a broken trader
 $ prosperity2bt example/starter.py 1 --print
+
+# Only match orders against order depths, not against market trades
+$ prosperity2bt example/starter.py 1 --no-trades-matching
 ```
 
 ## Order Matching
 
 Orders placed by `Trader.run` at a given timestamp are matched against the order depths and market trades of that timestamp's state. Order depths take priority, if an order can be filled completely using volume in the relevant order depth, market trades are not considered. If not, the backtester matches your order against the timestamp's market trades. In this case the backtester assumes that for each trade, the buyer and the seller of the trade are willing to trade with you instead at the trade's price and volume. Market trades are matched at the price of your orders, e.g. if you place a sell order for €9 and there is a market trade for €10, the sell order is matched at €9 (even though there is a buyer willing to pay €10, this appears to be consistent with what the official Prosperity environment does).
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
```

### Comparing `prosperity2bt-0.4.1/prosperity2bt/__main__.py` & `prosperity2bt-0.4.2/prosperity2bt/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,23 +144,24 @@
     parser.add_argument("algorithm", type=str, help="path to the Python file containing the algoritm to backtest")
     parser.add_argument("days", type=str, nargs="+", help="the days to backtest on (<round>-<day> for a single day, <round> for all days in a round)")
     parser.add_argument("--merge-pnl", action="store_true", help="merge profit and loss across days")
     parser.add_argument("--vis", action="store_true", help="open backtest result in visualizer when done")
     parser.add_argument("--out", type=str, help="path to save output log to (defaults to backtests/<timestamp>.log)")
     parser.add_argument("--data", type=str, help="path to data directory (must look similar in structure to https://github.com/jmerle/imc-prosperity-2-backtester/tree/master/prosperity2bt/resources)")
     parser.add_argument("--print", action="store_true", help="print the trader's output to stdout while it's running")
+    parser.add_argument("--no-trades-matching", action="store_true", help="disable matching orders against market trades")
     parser.add_argument("-v", "--version", action="version", version=f"%(prog)s {metadata.version(__package__)}")
 
     args = parser.parse_args()
 
     Trader = parse_algorithm(args.algorithm)
     days = parse_days(args.days, args.data)
     output_file = parse_out(args.out)
 
-    results = [run_backtest(Trader(), day, args.print) for day in days]
+    results = [run_backtest(Trader(), day, args.print, args.no_trades_matching) for day in days]
     merged_results = reduce(lambda a, b: merge_results(a, b, args.merge_pnl), results)
 
     write_output(output_file, merged_results)
 
     if len(days) > 1:
         print_overall_summary(results)
```

### Comparing `prosperity2bt-0.4.1/prosperity2bt/core.py` & `prosperity2bt-0.4.2/prosperity2bt/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
         if row.timestamp != last_timestamp:
             break
 
         total_profit += row.columns[-1]
 
     print(f"Total profit: {total_profit:,.0f}\n")
 
-def run_backtest(trader: Any, data: DayData, print_output: bool) -> DayResult:
+def run_backtest(trader: Any, data: DayData, print_output: bool, disable_trades_matching: bool) -> DayResult:
     print(f"Backtesting {trader.__module__} on round {data.round} day {data.day}")
 
     result = DayResult(data.round, data.day, [], [], [])
     trader_data = ""
 
     prices_by_timestamp = defaultdict(dict)
     for row in data.prices:
@@ -327,15 +327,15 @@
             for order in orders_by_symbol.get(product, []):
                 new_trades.extend(process_order(
                     timestamp,
                     order,
                     order_depths,
                     own_positions,
                     profit_loss_by_product,
-                    current_market_trades.get(product, []),
+                    [] if disable_trades_matching else current_market_trades.get(product, []),
                 ))
 
             if len(new_trades) > 0:
                 own_trades[product] = new_trades
 
         for product, trades in current_market_trades.items():
             for trade in trades:
```

### Comparing `prosperity2bt-0.4.1/prosperity2bt/data.py` & `prosperity2bt-0.4.2/prosperity2bt/data.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.1/prosperity2bt/datamodel.py` & `prosperity2bt-0.4.2/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.4.2/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.4.2/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv` & `prosperity2bt-0.4.2/prosperity2bt/resources/round1/prices_round_1_day_-1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv` & `prosperity2bt-0.4.2/prosperity2bt/resources/round1/prices_round_1_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv` & `prosperity2bt-0.4.2/prosperity2bt/resources/round1/prices_round_1_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv` & `prosperity2bt-0.4.2/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv` & `prosperity2bt-0.4.2/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv` & `prosperity2bt-0.4.2/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.1/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.4.2/prosperity2bt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.4.1
+Version: 0.4.2
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -89,14 +89,17 @@
 # Backtest on custom data
 # Requires the value passed to `--data` to be a path to a directory that is similar in structure to https://github.com/jmerle/imc-prosperity-2-backtester/tree/master/prosperity2bt/resources
 $ prosperity2bt example/starter.py 1 --data prosperity2bt/resources
 
 # Print trader's output to stdout while running
 # This may be helpful when debugging a broken trader
 $ prosperity2bt example/starter.py 1 --print
+
+# Only match orders against order depths, not against market trades
+$ prosperity2bt example/starter.py 1 --no-trades-matching
 ```
 
 ## Order Matching
 
 Orders placed by `Trader.run` at a given timestamp are matched against the order depths and market trades of that timestamp's state. Order depths take priority, if an order can be filled completely using volume in the relevant order depth, market trades are not considered. If not, the backtester matches your order against the timestamp's market trades. In this case the backtester assumes that for each trade, the buyer and the seller of the trade are willing to trade with you instead at the trade's price and volume. Market trades are matched at the price of your orders, e.g. if you place a sell order for €9 and there is a market trade for €10, the sell order is matched at €9 (even though there is a buyer willing to pay €10, this appears to be consistent with what the official Prosperity environment does).
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
```

### Comparing `prosperity2bt-0.4.1/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.4.2/prosperity2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.1/pyproject.toml` & `prosperity2bt-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.4.1"
+version = "0.4.2"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

