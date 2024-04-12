# Comparing `tmp/py_predpurchase-0.1.2.tar.gz` & `tmp/py_predpurchase-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_predpurchase-0.1.2.tar", max compression
+gzip compressed data, was "py_predpurchase-0.1.3.tar", max compression
```

## Comparing `py_predpurchase-0.1.2.tar` & `py_predpurchase-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1114 2024-04-12 00:28:02.206022 py_predpurchase-0.1.2/LICENSE
--rw-r--r--   0        0        0     3403 2024-04-12 00:28:02.206022 py_predpurchase-0.1.2/README.md
--rw-r--r--   0        0        0     1404 2024-04-12 00:28:16.226134 py_predpurchase-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      117 2024-04-12 00:28:02.206022 py_predpurchase-0.1.2/src/py_predpurchase/__init__.py
--rw-r--r--   0        0        0     1495 2024-04-12 00:28:02.206022 py_predpurchase-0.1.2/src/py_predpurchase/function_classification_metrics.py
--rw-r--r--   0        0        0     1716 2024-04-12 00:28:02.206022 py_predpurchase-0.1.2/src/py_predpurchase/function_feature_importance.py
--rw-r--r--   0        0        0     3135 2024-04-12 00:28:02.206022 py_predpurchase-0.1.2/src/py_predpurchase/function_model_cross_val.py
--rw-r--r--   0        0        0     3203 2024-04-12 00:28:02.206022 py_predpurchase-0.1.2/src/py_predpurchase/function_preprocessing.py
--rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 py_predpurchase-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1114 2024-04-12 01:47:33.424714 py_predpurchase-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3403 2024-04-12 01:47:33.424714 py_predpurchase-0.1.3/README.md
+-rw-r--r--   0        0        0     1404 2024-04-12 01:47:44.812763 py_predpurchase-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-04-12 01:47:33.424714 py_predpurchase-0.1.3/src/py_predpurchase/__init__.py
+-rw-r--r--   0        0        0     1495 2024-04-12 01:47:33.424714 py_predpurchase-0.1.3/src/py_predpurchase/function_classification_metrics.py
+-rw-r--r--   0        0        0     1716 2024-04-12 01:47:33.424714 py_predpurchase-0.1.3/src/py_predpurchase/function_feature_importance.py
+-rw-r--r--   0        0        0     3135 2024-04-12 01:47:33.424714 py_predpurchase-0.1.3/src/py_predpurchase/function_model_cross_val.py
+-rw-r--r--   0        0        0     3203 2024-04-12 01:47:33.424714 py_predpurchase-0.1.3/src/py_predpurchase/function_preprocessing.py
+-rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 py_predpurchase-0.1.3/PKG-INFO
```

### Comparing `py_predpurchase-0.1.2/LICENSE` & `py_predpurchase-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_predpurchase-0.1.2/README.md` & `py_predpurchase-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `py_predpurchase-0.1.2/pyproject.toml` & `py_predpurchase-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py_predpurchase"
-version = "0.1.2"
+version = "0.1.3"
 description = "```py_predpurchase```is a package for predicting online shopper purchasing intentions, containing functions to aid with data analysis processes including conducting data preprocessing as well as calculating classification metrics, cross validation scores and feature importances.The package features functions that focus mainly on analyzing the data and evaluating model performance."
 authors = ["Nour Abdelfattah, Sana Shams, Calvin Choi, Sai Pusuluri"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `py_predpurchase-0.1.2/src/py_predpurchase/function_classification_metrics.py` & `py_predpurchase-0.1.3/src/py_predpurchase/function_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `py_predpurchase-0.1.2/src/py_predpurchase/function_feature_importance.py` & `py_predpurchase-0.1.3/src/py_predpurchase/function_feature_importance.py`

 * *Files identical despite different names*

### Comparing `py_predpurchase-0.1.2/src/py_predpurchase/function_model_cross_val.py` & `py_predpurchase-0.1.3/src/py_predpurchase/function_model_cross_val.py`

 * *Files identical despite different names*

### Comparing `py_predpurchase-0.1.2/src/py_predpurchase/function_preprocessing.py` & `py_predpurchase-0.1.3/src/py_predpurchase/function_preprocessing.py`

 * *Files identical despite different names*

### Comparing `py_predpurchase-0.1.2/PKG-INFO` & `py_predpurchase-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_predpurchase
-Version: 0.1.2
+Version: 0.1.3
 Summary: ```py_predpurchase```is a package for predicting online shopper purchasing intentions, containing functions to aid with data analysis processes including conducting data preprocessing as well as calculating classification metrics, cross validation scores and feature importances.The package features functions that focus mainly on analyzing the data and evaluating model performance.
 License: MIT
 Author: Nour Abdelfattah, Sana Shams, Calvin Choi, Sai Pusuluri
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

