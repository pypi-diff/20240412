# Comparing `tmp/py_predpurchase-0.1.1.tar.gz` & `tmp/py_predpurchase-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_predpurchase-0.1.1.tar", max compression
+gzip compressed data, was "py_predpurchase-0.1.2.tar", max compression
```

## Comparing `py_predpurchase-0.1.1.tar` & `py_predpurchase-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1114 2024-04-11 23:33:17.384827 py_predpurchase-0.1.1/LICENSE
--rw-r--r--   0        0        0     3403 2024-04-11 23:33:17.384827 py_predpurchase-0.1.1/README.md
--rw-r--r--   0        0        0     1404 2024-04-11 23:33:27.580870 py_predpurchase-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      117 2024-04-11 23:33:17.384827 py_predpurchase-0.1.1/src/py_predpurchase/__init__.py
--rw-r--r--   0        0        0     1490 2024-04-11 23:33:17.384827 py_predpurchase-0.1.1/src/py_predpurchase/function_classification_metrics.py
--rw-r--r--   0        0        0     1716 2024-04-11 23:33:17.384827 py_predpurchase-0.1.1/src/py_predpurchase/function_feature_importance.py
--rw-r--r--   0        0        0     3139 2024-04-11 23:33:17.384827 py_predpurchase-0.1.1/src/py_predpurchase/function_model_cross_val.py
--rw-r--r--   0        0        0     3202 2024-04-11 23:33:17.384827 py_predpurchase-0.1.1/src/py_predpurchase/function_preprocessing.py
--rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 py_predpurchase-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1114 2024-04-12 00:28:02.206022 py_predpurchase-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3403 2024-04-12 00:28:02.206022 py_predpurchase-0.1.2/README.md
+-rw-r--r--   0        0        0     1404 2024-04-12 00:28:16.226134 py_predpurchase-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-04-12 00:28:02.206022 py_predpurchase-0.1.2/src/py_predpurchase/__init__.py
+-rw-r--r--   0        0        0     1495 2024-04-12 00:28:02.206022 py_predpurchase-0.1.2/src/py_predpurchase/function_classification_metrics.py
+-rw-r--r--   0        0        0     1716 2024-04-12 00:28:02.206022 py_predpurchase-0.1.2/src/py_predpurchase/function_feature_importance.py
+-rw-r--r--   0        0        0     3135 2024-04-12 00:28:02.206022 py_predpurchase-0.1.2/src/py_predpurchase/function_model_cross_val.py
+-rw-r--r--   0        0        0     3203 2024-04-12 00:28:02.206022 py_predpurchase-0.1.2/src/py_predpurchase/function_preprocessing.py
+-rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 py_predpurchase-0.1.2/PKG-INFO
```

### Comparing `py_predpurchase-0.1.1/LICENSE` & `py_predpurchase-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_predpurchase-0.1.1/README.md` & `py_predpurchase-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `py_predpurchase-0.1.1/pyproject.toml` & `py_predpurchase-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py_predpurchase"
-version = "0.1.1"
+version = "0.1.2"
 description = "```py_predpurchase```is a package for predicting online shopper purchasing intentions, containing functions to aid with data analysis processes including conducting data preprocessing as well as calculating classification metrics, cross validation scores and feature importances.The package features functions that focus mainly on analyzing the data and evaluating model performance."
 authors = ["Nour Abdelfattah, Sana Shams, Calvin Choi, Sai Pusuluri"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `py_predpurchase-0.1.1/src/py_predpurchase/function_classification_metrics.py` & `py_predpurchase-0.1.2/src/py_predpurchase/function_classification_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     dict
         Contains precision, recall, accuracy, and F1 score.
     
     Examples:
     --------
 
     Assume `y_true` and `y_pred` are as follows:
+    
     >>> y_true = [0, 1, 2, 0, 1]
     >>> y_pred = [0, 2, 1, 0, 0]
     >>> calculate_classification_metrics(y_true, y_pred)
 
     """
 
     if not all(isinstance(y, (int, float, np.number)) for y in np.concatenate([y_true, y_pred])):
```

### Comparing `py_predpurchase-0.1.1/src/py_predpurchase/function_feature_importance.py` & `py_predpurchase-0.1.2/src/py_predpurchase/function_feature_importance.py`

 * *Files identical despite different names*

### Comparing `py_predpurchase-0.1.1/src/py_predpurchase/function_model_cross_val.py` & `py_predpurchase-0.1.2/src/py_predpurchase/function_model_cross_val.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,22 +27,20 @@
     Returns:
     ----------
     dict
         Contains cross-validation results (mean and std of scores) for each specified model.
 
     Examples:
     --------
-    Assuming dataset is preprocessed and split into training and testing sets, 
-	with 'target' as the target column:
+    Assuming dataset is preprocessed and split into training and testing sets, with 'target' as the target column:
 
     >>> results = model_cross_validation(preprocessed_training_data, preprocessed_testing_data, 'target', k=5, gamma=0.1)
     >>> pd.DataFrame(results)
 
-    This will output the cross-validation results for each model, displaying the mean and 
-	standard deviation of the scores (also includes train scores).
+    This will output the cross-validation results for each model, displaying the mean and standard deviation of the scores (also includes train scores).
 
     Notes:
     -------
     The function assumes that the input data is already scaled and encoded.
     """
 
 	train_data = preprocessed_training_data
```

### Comparing `py_predpurchase-0.1.1/src/py_predpurchase/function_preprocessing.py` & `py_predpurchase-0.1.2/src/py_predpurchase/function_preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
    
     Examples:
     --------
     Assume you want to transform the following features and your data set has already been split
     into train and test
 
     >>> numeric_features = ['feature1', 'feature2']
-    >>> categorical_features = ['feature3', feature4']
+    >>> categorical_features = ['feature3', 'feature4']
     >>> train_transformed, test_transformed, transformed_columns = numerical_categorical_preprocess(
             X_train, X_test, y_train, y_test, numeric_features, categorical_features)
     
     The function will transform feature1,2,3,4 accordingly, carrying out scaling and one-hot encoding and 
     storing the preprocessed data in 'train_transformed' and 'test_transformed'. Column names will also be stored in 
     'transformed_columns'.
```

### Comparing `py_predpurchase-0.1.1/PKG-INFO` & `py_predpurchase-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_predpurchase
-Version: 0.1.1
+Version: 0.1.2
 Summary: ```py_predpurchase```is a package for predicting online shopper purchasing intentions, containing functions to aid with data analysis processes including conducting data preprocessing as well as calculating classification metrics, cross validation scores and feature importances.The package features functions that focus mainly on analyzing the data and evaluating model performance.
 License: MIT
 Author: Nour Abdelfattah, Sana Shams, Calvin Choi, Sai Pusuluri
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

