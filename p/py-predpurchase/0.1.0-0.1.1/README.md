# Comparing `tmp/py_predpurchase-0.1.0.tar.gz` & `tmp/py_predpurchase-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_predpurchase-0.1.0.tar", max compression
+gzip compressed data, was "py_predpurchase-0.1.1.tar", max compression
```

## Comparing `py_predpurchase-0.1.0.tar` & `py_predpurchase-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1114 2024-04-11 08:37:04.049363 py_predpurchase-0.1.0/LICENSE
--rw-r--r--   0        0        0     1060 2024-04-11 08:37:04.049363 py_predpurchase-0.1.0/README.md
--rw-r--r--   0        0        0     1404 2024-04-11 08:37:14.881362 py_predpurchase-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      117 2024-04-11 08:37:04.049363 py_predpurchase-0.1.0/src/py_predpurchase/__init__.py
--rw-r--r--   0        0        0     1209 2024-04-11 08:37:04.049363 py_predpurchase-0.1.0/src/py_predpurchase/function_classification_metrics.py
--rw-r--r--   0        0        0     1716 2024-04-11 08:37:04.049363 py_predpurchase-0.1.0/src/py_predpurchase/function_feature_importance.py
--rw-r--r--   0        0        0     2468 2024-04-11 08:37:04.049363 py_predpurchase-0.1.0/src/py_predpurchase/function_model_cross_val.py
--rw-r--r--   0        0        0     2392 2024-04-11 08:37:04.049363 py_predpurchase-0.1.0/src/py_predpurchase/function_preprocessing.py
--rw-r--r--   0        0        0     2164 1970-01-01 00:00:00.000000 py_predpurchase-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1114 2024-04-11 23:33:17.384827 py_predpurchase-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3403 2024-04-11 23:33:17.384827 py_predpurchase-0.1.1/README.md
+-rw-r--r--   0        0        0     1404 2024-04-11 23:33:27.580870 py_predpurchase-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-04-11 23:33:17.384827 py_predpurchase-0.1.1/src/py_predpurchase/__init__.py
+-rw-r--r--   0        0        0     1490 2024-04-11 23:33:17.384827 py_predpurchase-0.1.1/src/py_predpurchase/function_classification_metrics.py
+-rw-r--r--   0        0        0     1716 2024-04-11 23:33:17.384827 py_predpurchase-0.1.1/src/py_predpurchase/function_feature_importance.py
+-rw-r--r--   0        0        0     3139 2024-04-11 23:33:17.384827 py_predpurchase-0.1.1/src/py_predpurchase/function_model_cross_val.py
+-rw-r--r--   0        0        0     3202 2024-04-11 23:33:17.384827 py_predpurchase-0.1.1/src/py_predpurchase/function_preprocessing.py
+-rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 py_predpurchase-0.1.1/PKG-INFO
```

### Comparing `py_predpurchase-0.1.0/LICENSE` & `py_predpurchase-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_predpurchase-0.1.0/pyproject.toml` & `py_predpurchase-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py_predpurchase"
-version = "0.1.0"
+version = "0.1.1"
 description = "```py_predpurchase```is a package for predicting online shopper purchasing intentions, containing functions to aid with data analysis processes including conducting data preprocessing as well as calculating classification metrics, cross validation scores and feature importances.The package features functions that focus mainly on analyzing the data and evaluating model performance."
 authors = ["Nour Abdelfattah, Sana Shams, Calvin Choi, Sai Pusuluri"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `py_predpurchase-0.1.0/src/py_predpurchase/function_classification_metrics.py` & `py_predpurchase-0.1.1/src/py_predpurchase/function_classification_metrics.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 from sklearn.metrics import precision_score, recall_score, accuracy_score, f1_score
 import numpy as np
 
 def calculate_classification_metrics(y_true, y_pred):
     """
     Calculates classification metrics for model predictions including precision, 
-    recall, accuracy and F1 scores. 
+    recall, accuracy, and F1 scores. 
     
     Parameters:
-    - y_true: pd.Series, true target values in a dataset
-    - y_pred: pd.Series, predicted target values by the model.
+    ----------
+    y_true : array-like or pd.Series
+        True target values in a dataset.
+    y_pred : array-like or pd.Series
+        Predicted target values by the model.
     
     Returns:
-    - dict, containing precision, recall, accuracy, and F1 score.
+    ----------
+    dict
+        Contains precision, recall, accuracy, and F1 score.
+    
+    Examples:
+    --------
+
+    Assume `y_true` and `y_pred` are as follows:
+    >>> y_true = [0, 1, 2, 0, 1]
+    >>> y_pred = [0, 2, 1, 0, 0]
+    >>> calculate_classification_metrics(y_true, y_pred)
+
     """
 
     if not all(isinstance(y, (int, float, np.number)) for y in np.concatenate([y_true, y_pred])):
         raise TypeError("y_true and y_pred must contain numeric values only.")
 
     
     if len(y_true) != len(y_pred):
```

### Comparing `py_predpurchase-0.1.0/src/py_predpurchase/function_feature_importance.py` & `py_predpurchase-0.1.1/src/py_predpurchase/function_feature_importance.py`

 * *Files identical despite different names*

### Comparing `py_predpurchase-0.1.0/src/py_predpurchase/function_model_cross_val.py` & `py_predpurchase-0.1.1/src/py_predpurchase/function_model_cross_val.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,23 +8,46 @@
 
 def model_cross_validation(preprocessed_training_data, preprocessed_testing_data, target, k, gamma):
 	"""
 	Calculates the cross validation results for a four common off-the-shelf models (Dummy, KNN, SVM and RandomForests)
 	using preprocessed and cleaned training and testing datasets. Random forests and Dummy hyperparameters are fixed for simplicity sake.
 	
 	Parameters:
-	- preprocessed_training_data: DataFrame, cleaned and preprocessed training data 
-	- preprocessed_testing_data: DataFrame, cleaned and preprocessed testing data
-	- target: str target column name
-	- k: k value hyperparameter for KNearestNeighbours Int
-	- gamma: gamma value hyperparameter for SVM
-	
-	Returns:
-	- dictionary, containing cross validation results (mean and std of scores) from specified model
-	"""
+    ----------
+    preprocessed_training_data : DataFrame
+        Cleaned and preprocessed training data.
+    preprocessed_testing_data : DataFrame
+        Cleaned and preprocessed testing data.
+    target : str
+        Target column name in the dataset.
+    k : int
+        Hyperparameter 'k' value for KNearestNeighbours.
+    gamma : float
+        Hyperparameter 'gamma' value for SVM.
+
+    Returns:
+    ----------
+    dict
+        Contains cross-validation results (mean and std of scores) for each specified model.
+
+    Examples:
+    --------
+    Assuming dataset is preprocessed and split into training and testing sets, 
+	with 'target' as the target column:
+
+    >>> results = model_cross_validation(preprocessed_training_data, preprocessed_testing_data, 'target', k=5, gamma=0.1)
+    >>> pd.DataFrame(results)
+
+    This will output the cross-validation results for each model, displaying the mean and 
+	standard deviation of the scores (also includes train scores).
+
+    Notes:
+    -------
+    The function assumes that the input data is already scaled and encoded.
+    """
 
 	train_data = preprocessed_training_data
 	test_data = preprocessed_testing_data
 	X_train = train_data.drop(target, axis=1)
 	y_train = train_data[target]
 	X_test = test_data.drop(target, axis=1)
 	y_test = test_data[target]
```

### Comparing `py_predpurchase-0.1.0/src/py_predpurchase/function_preprocessing.py` & `py_predpurchase-0.1.1/src/py_predpurchase/function_preprocessing.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,24 +4,48 @@
 
 def numerical_categorical_preprocess(X_train, X_test, y_train, y_test, numeric_features, categorical_features):
     """
     Applies preprocessing transformations to the data, including scaling, encoding, and passing through features as specified.
     This function requires target data to be provided and includes it in the output DataFrames.
 
     Parameters:
-    - X_train: DataFrame, training feature data
-    - X_test: DataFrame, testing feature data
-    - y_train: DataFrame, training target data
-    - y_test: DataFrame, testing target data
-    - numeric_features: list, names of numeric features to scale
-    - categorical_features: list, names of categorical features to encode
-    
+    ----------
+    X_train : DataFrame
+        Training feature data.
+    X_test : DataFrame
+        Testing feature data.
+    y_train : DataFrame or Series
+        Training target data.
+    y_test : DataFrame or Series
+        Testing target data.
+    numeric_features : list
+        Names of numeric features to scale.
+    categorical_features : list
+        Names of categorical features to encode.
     
     Returns:
-    - Tuple containing preprocessed training and testing DataFrames including target data, and transformed column names
+    ----------
+    Tuple
+        Contains preprocessed training and testing DataFrames including target data, 
+        and transformed column names.
+   
+    Examples:
+    --------
+    Assume you want to transform the following features and your data set has already been split
+    into train and test
+
+    >>> numeric_features = ['feature1', 'feature2']
+    >>> categorical_features = ['feature3', feature4']
+    >>> train_transformed, test_transformed, transformed_columns = numerical_categorical_preprocess(
+            X_train, X_test, y_train, y_test, numeric_features, categorical_features)
+    
+    The function will transform feature1,2,3,4 accordingly, carrying out scaling and one-hot encoding and 
+    storing the preprocessed data in 'train_transformed' and 'test_transformed'. Column names will also be stored in 
+    'transformed_columns'.
+    
     """
     
     
     numeric_transformer = StandardScaler()
     categorical_transformer = OneHotEncoder(handle_unknown="ignore", sparse_output=False)
     
     # Defining preprocessor
```

