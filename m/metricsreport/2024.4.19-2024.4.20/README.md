# Comparing `tmp/metricsreport-2024.4.19.tar.gz` & `tmp/metricsreport-2024.4.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metricsreport-2024.4.19.tar", max compression
+gzip compressed data, was "metricsreport-2024.4.20.tar", max compression
```

## Comparing `metricsreport-2024.4.19.tar` & `metricsreport-2024.4.20.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2024-04-05 14:51:42.426099 metricsreport-2024.4.19/LICENSE
--rw-r--r--   0        0        0     2322 2024-04-05 19:03:59.359773 metricsreport-2024.4.19/README.md
--rw-r--r--   0        0        0       99 2024-04-05 19:09:40.541449 metricsreport-2024.4.19/metricsreport/__init__.py
--rw-r--r--   0        0        0     2749 2024-04-05 14:51:42.450099 metricsreport-2024.4.19/metricsreport/custom_metrics.py
--rw-r--r--   0        0        0    29481 2024-04-05 19:09:21.833357 metricsreport-2024.4.19/metricsreport/metricsreport.py
--rw-r--r--   0        0        0      577 2024-04-05 19:09:34.109417 metricsreport-2024.4.19/pyproject.toml
--rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 metricsreport-2024.4.19/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-12 13:44:26.925841 metricsreport-2024.4.20/LICENSE
+-rw-r--r--   0        0        0     2322 2024-04-12 13:44:26.925841 metricsreport-2024.4.20/README.md
+-rw-r--r--   0        0        0       99 2024-04-12 14:13:35.841878 metricsreport-2024.4.20/metricsreport/__init__.py
+-rw-r--r--   0        0        0     2749 2024-04-12 13:44:26.949841 metricsreport-2024.4.20/metricsreport/custom_metrics.py
+-rw-r--r--   0        0        0    30080 2024-04-12 14:09:44.817364 metricsreport-2024.4.20/metricsreport/metricsreport.py
+-rw-r--r--   0        0        0      577 2024-04-12 14:13:26.421857 metricsreport-2024.4.20/pyproject.toml
+-rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 metricsreport-2024.4.20/PKG-INFO
```

### Comparing `metricsreport-2024.4.19/LICENSE` & `metricsreport-2024.4.20/LICENSE`

 * *Files identical despite different names*

### Comparing `metricsreport-2024.4.19/README.md` & `metricsreport-2024.4.20/README.md`

 * *Files identical despite different names*

### Comparing `metricsreport-2024.4.19/metricsreport/custom_metrics.py` & `metricsreport-2024.4.20/metricsreport/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `metricsreport-2024.4.19/metricsreport/metricsreport.py` & `metricsreport-2024.4.20/metricsreport/metricsreport.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,36 +46,43 @@
         task_type: Type of task, either "classification" or "regression".
         y_true: A list of true target values.
         y_pred: A list of predicted target values.
         threshold: Threshold for generating binary classification metrics.
         metrics: A dictionary containing all metrics generated.
         target_info: A dictionary containing information about the target variable.
     """
-    def __init__(self, y_true, y_pred, threshold: float = 0.5):
+    def __init__(self, y_true, y_pred, threshold: float = 0.5, verbose=0):
         """
         Initializes the MetricsReport object.
 
         Args:
             y_true: A list of true target values.
             y_pred: A list of predicted target values.
             threshold: Threshold for generating binary classification metrics.
+            verbose: Verbosity level.
 
         Returns:
             None
         """
         self.task_type = self._determine_task_type(y_true)
-        print(f'Detecting {self.task_type} task type')
+        #print(f'Detecting {self.task_type} task type')
         self.y_true = np.array(y_true)
         self.y_pred = np.array(y_pred)
         self.threshold = threshold
         self.metrics = {}
         self.target_info = {}
 
         if self.task_type == "classification":
             self.y_pred_binary = (self.y_pred > self.threshold).astype(int)
+            if sum(self.y_true) == 0:
+                raise ValueError("For classification tasks, y_true should contain at least one True value.")
+            
+            if sum(self.y_pred_binary) == 0:
+                print(f"Warning: For classification tasks threshold {self.threshold}, sum y_pred: 0, -> should contain at least one True value.")
+            
             # fix for skplt
             self.probas_reval = pd.DataFrame(data={"proba_0": 1 - self.y_pred.ravel(), "proba_1": self.y_pred.ravel()})
             self.metrics = self._generate_classification_metrics()
         else:
             # assuming y_pred is a numpy array
             self.y_pred_nonnegative = np.maximum(self.y_pred, 0)
             self.metrics = self._generate_regression_metrics()
@@ -120,15 +127,17 @@
     def _generate_classification_metrics(self) -> dict:
         """
         Generates a dictionary of classification metrics.
 
         Returns:
             A dictionary of classification metrics.
         """
-        tn, fp, fn, tp = confusion_matrix(y_true=self.y_true, y_pred=self.y_pred_binary).ravel()
+        #tn, fp, fn, tp = confusion_matrix(y_true=self.y_true, y_pred=self.y_pred_binary).ravel()
+        cm = confusion_matrix(y_true=self.y_true, y_pred=self.y_pred_binary).ravel()
+        tn, fp, fn, tp = (cm if cm.size == 4 else [0, 0, 0, 0])  # Default to 0 if not all present
         report = classification_report(
             y_true=self.y_true, 
             y_pred=self.y_pred_binary, 
             output_dict=True, 
             labels=[0, 1], 
             target_names=['negative', 'positive'], 
             zero_division='warn'
```

### Comparing `metricsreport-2024.4.19/pyproject.toml` & `metricsreport-2024.4.20/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metricsreport"
-version = "2024.4.19"
+version = "2024.4.20"
 description = "Generating reports on metrics for Machine Learning models"
 authors = ["Alex Lekov <11148364-AlexLekov@users.noreply.gitlab.com>"]
 repository = 'https://github.com/Alex-Lekov/metricsreport'
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `metricsreport-2024.4.19/PKG-INFO` & `metricsreport-2024.4.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metricsreport
-Version: 2024.4.19
+Version: 2024.4.20
 Summary: Generating reports on metrics for Machine Learning models
 Home-page: https://github.com/Alex-Lekov/metricsreport
 Author: Alex Lekov
 Author-email: 11148364-AlexLekov@users.noreply.gitlab.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

