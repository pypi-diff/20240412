# Comparing `tmp/darrow-poc-0.1.7.tar.gz` & `tmp/darrow-poc-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darrow-poc-0.1.7.tar", last modified: Tue Mar 26 08:56:26 2024, max compression
+gzip compressed data, was "darrow-poc-0.1.8.tar", last modified: Fri Apr 12 11:54:21 2024, max compression
```

## Comparing `darrow-poc-0.1.7.tar` & `darrow-poc-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:56:26.255088 darrow-poc-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-26 08:56:20.000000 darrow-poc-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19629 2024-03-26 08:56:26.255088 darrow-poc-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18619 2024-03-26 08:56:20.000000 darrow-poc-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:56:26.251088 darrow-poc-0.1.7/darrow_poc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 08:56:20.000000 darrow-poc-0.1.7/darrow_poc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-26 08:56:20.000000 darrow-poc-0.1.7/darrow_poc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:56:26.251088 darrow-poc-0.1.7/darrow_poc/models/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-26 08:56:20.000000 darrow-poc-0.1.7/darrow_poc/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-03-26 08:56:20.000000 darrow-poc-0.1.7/darrow_poc/models/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-03-26 08:56:20.000000 darrow-poc-0.1.7/darrow_poc/models/linear_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-03-26 08:56:20.000000 darrow-poc-0.1.7/darrow_poc/models/poc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-03-26 08:56:20.000000 darrow-poc-0.1.7/darrow_poc/models/validation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:56:26.255088 darrow-poc-0.1.7/darrow_poc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19629 2024-03-26 08:56:26.000000 darrow-poc-0.1.7/darrow_poc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-26 08:56:26.000000 darrow-poc-0.1.7/darrow_poc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 08:56:26.000000 darrow-poc-0.1.7/darrow_poc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-26 08:56:26.000000 darrow-poc-0.1.7/darrow_poc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-26 08:56:26.000000 darrow-poc-0.1.7/darrow_poc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-26 08:56:20.000000 darrow-poc-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-26 08:56:20.000000 darrow-poc-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 08:56:26.255088 darrow-poc-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:56:26.255088 darrow-poc-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-26 08:56:20.000000 darrow-poc-0.1.7/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-26 08:56:20.000000 darrow-poc-0.1.7/tests/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:54:21.780513 darrow-poc-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-12 11:54:18.000000 darrow-poc-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19629 2024-04-12 11:54:21.780513 darrow-poc-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18619 2024-04-12 11:54:18.000000 darrow-poc-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:54:21.780513 darrow-poc-0.1.8/darrow_poc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:54:18.000000 darrow-poc-0.1.8/darrow_poc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 11:54:18.000000 darrow-poc-0.1.8/darrow_poc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:54:21.780513 darrow-poc-0.1.8/darrow_poc/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 11:54:18.000000 darrow-poc-0.1.8/darrow_poc/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-12 11:54:18.000000 darrow-poc-0.1.8/darrow_poc/models/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-12 11:54:18.000000 darrow-poc-0.1.8/darrow_poc/models/linear_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-12 11:54:18.000000 darrow-poc-0.1.8/darrow_poc/models/poc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-04-12 11:54:18.000000 darrow-poc-0.1.8/darrow_poc/models/validation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:54:21.780513 darrow-poc-0.1.8/darrow_poc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19629 2024-04-12 11:54:21.000000 darrow-poc-0.1.8/darrow_poc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-12 11:54:21.000000 darrow-poc-0.1.8/darrow_poc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:54:21.000000 darrow-poc-0.1.8/darrow_poc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-12 11:54:21.000000 darrow-poc-0.1.8/darrow_poc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 11:54:21.000000 darrow-poc-0.1.8/darrow_poc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-12 11:54:18.000000 darrow-poc-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-12 11:54:18.000000 darrow-poc-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:54:21.780513 darrow-poc-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:54:21.780513 darrow-poc-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-12 11:54:18.000000 darrow-poc-0.1.8/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-12 11:54:18.000000 darrow-poc-0.1.8/tests/test_interface.py
```

### Comparing `darrow-poc-0.1.7/LICENSE` & `darrow-poc-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `darrow-poc-0.1.7/PKG-INFO` & `darrow-poc-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darrow-poc
-Version: 0.1.7
+Version: 0.1.8
 Summary: Proof of concept for twinn-ml-interface with model pipeline for predicting water throughput in ruhr river.
 License: MIT
 Project-URL: homepage, https://github.com/RoyalHaskoningDHV/darrow-poc
 Project-URL: issues, https://github.com/RoyalHaskoningDHV/darrow-poc/issues
 Project-URL: discussions, https://github.com/RoyalHaskoningDHV/darrow-poc/discussions
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `darrow-poc-0.1.7/README.md` & `darrow-poc-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `darrow-poc-0.1.7/darrow_poc/models/anomaly_detection.py` & `darrow-poc-0.1.8/darrow_poc/models/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `darrow-poc-0.1.7/darrow_poc/models/linear_quantile_regressor.py` & `darrow-poc-0.1.8/darrow_poc/models/linear_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `darrow-poc-0.1.7/darrow_poc/models/poc.py` & `darrow-poc-0.1.8/darrow_poc/models/poc.py`

 * *Files 5% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 
         train = pd.concat(input_data.values(), axis=1)
         validator = ValidationModel(
             train,
             model_type="lasso",
             n_features=5,
             use_precipitation_features=False,
-            training_end_date="2010-01-04 00:00:00",
+            training_end_date=((input_data.max_datetime - input_data.min_datetime) // 2) + input_data.min_datetime,
         )
         _, num_obs, _, r2_by_target = validator.fit_and_evaluate(str(self.target))
         r2_by_missing_sensor = validator._flatten_output(r2_by_target, "r2")
         r2_log = {prep_string_for_mlflow(k): prep_string_for_mlflow(v) for k, v in r2_by_missing_sensor.items()}
         self.logger.log_params(r2_log)  # This will be logged to mlflow
         self.logger.log_params({f"samples_{prep_string_for_mlflow(k)}": str(v) for k, v in num_obs.items()})
```

### Comparing `darrow-poc-0.1.7/darrow_poc/models/validation_model.py` & `darrow-poc-0.1.8/darrow_poc/models/validation_model.py`

 * *Files identical despite different names*

### Comparing `darrow-poc-0.1.7/darrow_poc.egg-info/PKG-INFO` & `darrow-poc-0.1.8/darrow_poc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darrow-poc
-Version: 0.1.7
+Version: 0.1.8
 Summary: Proof of concept for twinn-ml-interface with model pipeline for predicting water throughput in ruhr river.
 License: MIT
 Project-URL: homepage, https://github.com/RoyalHaskoningDHV/darrow-poc
 Project-URL: issues, https://github.com/RoyalHaskoningDHV/darrow-poc/issues
 Project-URL: discussions, https://github.com/RoyalHaskoningDHV/darrow-poc/discussions
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `darrow-poc-0.1.7/pyproject.toml` & `darrow-poc-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `darrow-poc-0.1.7/tests/test_executor.py` & `darrow-poc-0.1.8/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `darrow-poc-0.1.7/tests/test_interface.py` & `darrow-poc-0.1.8/tests/test_interface.py`

 * *Files identical despite different names*

