# Comparing `tmp/goto_conversion-0.1.1.tar.gz` & `tmp/goto_conversion-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/gotoukaijin/Desktop/goto_conversion-main/dist/.tmp-uyvq93uu/goto_conversion-0.1.1.tar", last modified: Sat Sep 30 01:15:42 2023, max compression
+gzip compressed data, was "goto_conversion-0.2.0.tar", last modified: Fri Apr 12 05:59:49 2024, max compression
```

## Comparing `goto_conversion-0.1.1.tar` & `goto_conversion-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2023-09-30 01:15:42.336956 goto_conversion-0.1.1/
--rw-rw-r--   0 gotoukaijin   (501) staff       (20)     1073 2023-09-30 01:13:28.000000 goto_conversion-0.1.1/LICENSE.txt
--rw-r--r--   0 gotoukaijin   (501) staff       (20)     4236 2023-09-30 01:15:42.336531 goto_conversion-0.1.1/PKG-INFO
--rw-rw-r--   0 gotoukaijin   (501) staff       (20)     3707 2023-09-30 01:13:28.000000 goto_conversion-0.1.1/README.md
--rw-rw-r--   0 gotoukaijin   (501) staff       (20)      596 2023-09-30 01:13:28.000000 goto_conversion-0.1.1/pyproject.toml
--rw-r--r--   0 gotoukaijin   (501) staff       (20)       38 2023-09-30 01:15:42.337065 goto_conversion-0.1.1/setup.cfg
-drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2023-09-30 01:15:42.332612 goto_conversion-0.1.1/src/
-drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2023-09-30 01:15:42.334408 goto_conversion-0.1.1/src/goto_conversion/
--rw-rw-r--   0 gotoukaijin   (501) staff       (20)     1602 2023-09-30 01:13:28.000000 goto_conversion-0.1.1/src/goto_conversion/__init__.py
-drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2023-09-30 01:15:42.335985 goto_conversion-0.1.1/src/goto_conversion.egg-info/
--rw-r--r--   0 gotoukaijin   (501) staff       (20)     4236 2023-09-30 01:15:42.000000 goto_conversion-0.1.1/src/goto_conversion.egg-info/PKG-INFO
--rw-r--r--   0 gotoukaijin   (501) staff       (20)      240 2023-09-30 01:15:42.000000 goto_conversion-0.1.1/src/goto_conversion.egg-info/SOURCES.txt
--rw-r--r--   0 gotoukaijin   (501) staff       (20)        1 2023-09-30 01:15:42.000000 goto_conversion-0.1.1/src/goto_conversion.egg-info/dependency_links.txt
--rw-r--r--   0 gotoukaijin   (501) staff       (20)       16 2023-09-30 01:15:42.000000 goto_conversion-0.1.1/src/goto_conversion.egg-info/top_level.txt
+drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-04-12 05:59:49.729019 goto_conversion-0.2.0/
+-rw-rw-r--   0 gotoukaijin   (501) staff       (20)     1073 2024-04-12 05:54:23.000000 goto_conversion-0.2.0/LICENSE.txt
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)     5561 2024-04-12 05:59:49.728235 goto_conversion-0.2.0/PKG-INFO
+-rw-rw-r--   0 gotoukaijin   (501) staff       (20)     5032 2024-04-12 05:54:23.000000 goto_conversion-0.2.0/README.md
+-rw-rw-r--   0 gotoukaijin   (501) staff       (20)      596 2024-04-12 05:54:23.000000 goto_conversion-0.2.0/pyproject.toml
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)       38 2024-04-12 05:59:49.729164 goto_conversion-0.2.0/setup.cfg
+drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-04-12 05:59:49.722608 goto_conversion-0.2.0/src/
+drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-04-12 05:59:49.727434 goto_conversion-0.2.0/src/goto_conversion.egg-info/
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)     5561 2024-04-12 05:59:49.000000 goto_conversion-0.2.0/src/goto_conversion.egg-info/PKG-INFO
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)      208 2024-04-12 05:59:49.000000 goto_conversion-0.2.0/src/goto_conversion.egg-info/SOURCES.txt
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)        1 2024-04-12 05:59:49.000000 goto_conversion-0.2.0/src/goto_conversion.egg-info/dependency_links.txt
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)        1 2024-04-12 05:59:49.000000 goto_conversion-0.2.0/src/goto_conversion.egg-info/top_level.txt
```

### Comparing `goto_conversion-0.1.1/LICENSE.txt` & `goto_conversion-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goto_conversion-0.1.1/PKG-INFO` & `goto_conversion-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-Metadata-Version: 2.1
-Name: goto_conversion
-Version: 0.1.1
-Summary: Novel Conversion of Betting Odds to Probabilities
-Author: Kaito Goto
-Project-URL: Homepage, https://github.com/gotoConversion/goto_conversion
-Project-URL: Bug Tracker, https://github.com/gotoConversion/goto_conversion/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# goto_conversion (Novel Conversion of Betting Odds to Probabilities)
+# goto_conversion: Novel Conversion of Betting Odds to Probabilities
 
 The most common method used to convert betting odds to probabilities is to normalise the inverse odds (Multiplicative conversion). However, this method does not consider the favourite-longshot bias. 
 
 To the best of our knowledge, there are two existing methods that attempt to consider the favourite-longshot bias. (i) Shin conversion [[1](#1),[2](#2),[3](#3)] maximises the expected profit for the bookmakers assuming a small proportion of bettors have inside information. (ii) Power conversion [[4](#4)] raises all inverse odds to the same constant power. However, both of these methods require iterative computation to convert betting odds to probabilities.
 
-Our proposed method (goto_conversion) is significantly more efficient than Shin and Power conversion because it converts betting odds to probabilities directly without iterative computation.
+Our proposed method (`goto_conversion`) is significantly more efficient than Shin and Power conversion because it converts betting odds to probabilities directly without iterative computation.
+
+The `goto_conversion` reduces all inverse odds by the same units of standard error. This attempts to consider the favourite-longshot bias by utilising the proportionately wider standard errors implied for inverses of longshot odds and vice-versa.
+
+Furthermore, our tables of experiment results show that the `goto_conversion` converts betting odds to probabilities more accurately than all three of these existing methods.
+
+The favourite-longshot bias is not limited to gambling markets, it exists in stock markets too. Thus, we applied the original `goto_conversion` to stock markets by defining the `zero_sum` variant. Under the same philosophy as the original `goto_conversion`, `zero_sum` adjusts all predicted stock prices (e.g. weighted average price) by the same units of standard error to ensure all predicted stock prices relative to the index price (e.g. weighted average nasdaq price) sum to zero. This attempts to consider the favourite-longshot bias by utilising the wider standard errors implied for predicted stock prices with low trade volume and vice-versa.
 
-The goto_conversion reduces all inverse odds by the same units of standard error. This attempts to consider the favourite-longshot bias by utilising the proportionately wider standard errors implied for inverses of longshot odds and vice-versa.
+# Citations (not limited to, unofficial)
 
-Furthermore, our tables of experiment results below show that the goto_conversion converts betting odds to probabilities more accurately than all three of these existing methods.
+[Most Voted Public Solution from 2024 Optiver Kaggle Competition](https://www.kaggle.com/code/ravi20076/optiver-baseline-models?scriptVersionId=152991375)
+
+[1xGold and 2xSilver Medal Winning Public Solution from 2019 to 2022 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/1xgold-2xsilvers-key-ingredient)
+
+[Bronze Medal Winning Public Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/updated-1xgold-2xsilvers-key-ingredient)
 
 # Installation
 
 Requires Python 3.7 or above.
 
 ```
 pip install goto-conversion
@@ -92,12 +88,14 @@
 <a id="4">[4]</a>
 [S. Clarke, S. Kovalchik, M. Ingram, "Adjusting bookmaker’s odds to allow for
 overround". American Journal of Sports Science, 2017, Volume 5, Issue 6,
 pp. 45-49.](https://doi.org/10.11648/j.ajss.20170506.12)
 
 # Contact Me
 
-LinkedIn Message: https://www.linkedin.com/in/goto/
+via kaggle message: https://www.kaggle.com/kaito510/competitions
+
+# Q&A
 
-Kaggle Message: https://www.kaggle.com/kaito510/competitions
+Q1. I want to know whether the teams in the csv file named mensProbabilitiesTable in the 538 data you created are in 2024 or 2023?
 
-Or fire an issue on this repo.
+A1. 2024 but it is NOT 538 data, it is my data displayed in a format inspired by 538.
```

### Comparing `goto_conversion-0.1.1/pyproject.toml` & `goto_conversion-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "goto_conversion"
-version = "0.1.1"
+version = "0.2.0"
 authors = [{ name = 'Kaito Goto' },]
 description = "Novel Conversion of Betting Odds to Probabilities"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `goto_conversion-0.1.1/src/goto_conversion.egg-info/PKG-INFO` & `goto_conversion-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 Metadata-Version: 2.1
-Name: goto-conversion
-Version: 0.1.1
+Name: goto_conversion
+Version: 0.2.0
 Summary: Novel Conversion of Betting Odds to Probabilities
 Author: Kaito Goto
 Project-URL: Homepage, https://github.com/gotoConversion/goto_conversion
 Project-URL: Bug Tracker, https://github.com/gotoConversion/goto_conversion/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# goto_conversion (Novel Conversion of Betting Odds to Probabilities)
+# goto_conversion: Novel Conversion of Betting Odds to Probabilities
 
 The most common method used to convert betting odds to probabilities is to normalise the inverse odds (Multiplicative conversion). However, this method does not consider the favourite-longshot bias. 
 
 To the best of our knowledge, there are two existing methods that attempt to consider the favourite-longshot bias. (i) Shin conversion [[1](#1),[2](#2),[3](#3)] maximises the expected profit for the bookmakers assuming a small proportion of bettors have inside information. (ii) Power conversion [[4](#4)] raises all inverse odds to the same constant power. However, both of these methods require iterative computation to convert betting odds to probabilities.
 
-Our proposed method (goto_conversion) is significantly more efficient than Shin and Power conversion because it converts betting odds to probabilities directly without iterative computation.
+Our proposed method (`goto_conversion`) is significantly more efficient than Shin and Power conversion because it converts betting odds to probabilities directly without iterative computation.
 
-The goto_conversion reduces all inverse odds by the same units of standard error. This attempts to consider the favourite-longshot bias by utilising the proportionately wider standard errors implied for inverses of longshot odds and vice-versa.
+The `goto_conversion` reduces all inverse odds by the same units of standard error. This attempts to consider the favourite-longshot bias by utilising the proportionately wider standard errors implied for inverses of longshot odds and vice-versa.
 
-Furthermore, our tables of experiment results below show that the goto_conversion converts betting odds to probabilities more accurately than all three of these existing methods.
+Furthermore, our tables of experiment results show that the `goto_conversion` converts betting odds to probabilities more accurately than all three of these existing methods.
+
+The favourite-longshot bias is not limited to gambling markets, it exists in stock markets too. Thus, we applied the original `goto_conversion` to stock markets by defining the `zero_sum` variant. Under the same philosophy as the original `goto_conversion`, `zero_sum` adjusts all predicted stock prices (e.g. weighted average price) by the same units of standard error to ensure all predicted stock prices relative to the index price (e.g. weighted average nasdaq price) sum to zero. This attempts to consider the favourite-longshot bias by utilising the wider standard errors implied for predicted stock prices with low trade volume and vice-versa.
+
+# Citations (not limited to, unofficial)
+
+[Most Voted Public Solution from 2024 Optiver Kaggle Competition](https://www.kaggle.com/code/ravi20076/optiver-baseline-models?scriptVersionId=152991375)
+
+[1xGold and 2xSilver Medal Winning Public Solution from 2019 to 2022 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/1xgold-2xsilvers-key-ingredient)
+
+[Bronze Medal Winning Public Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/updated-1xgold-2xsilvers-key-ingredient)
 
 # Installation
 
 Requires Python 3.7 or above.
 
 ```
 pip install goto-conversion
@@ -92,12 +102,14 @@
 <a id="4">[4]</a>
 [S. Clarke, S. Kovalchik, M. Ingram, "Adjusting bookmaker’s odds to allow for
 overround". American Journal of Sports Science, 2017, Volume 5, Issue 6,
 pp. 45-49.](https://doi.org/10.11648/j.ajss.20170506.12)
 
 # Contact Me
 
-LinkedIn Message: https://www.linkedin.com/in/goto/
+via kaggle message: https://www.kaggle.com/kaito510/competitions
+
+# Q&A
 
-Kaggle Message: https://www.kaggle.com/kaito510/competitions
+Q1. I want to know whether the teams in the csv file named mensProbabilitiesTable in the 538 data you created are in 2024 or 2023?
 
-Or fire an issue on this repo.
+A1. 2024 but it is NOT 538 data, it is my data displayed in a format inspired by 538.
```

