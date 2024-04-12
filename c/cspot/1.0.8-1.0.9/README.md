# Comparing `tmp/cspot-1.0.8.tar.gz` & `tmp/cspot-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cspot-1.0.8.tar", max compression
+gzip compressed data, was "cspot-1.0.9.tar", max compression
```

## Comparing `cspot-1.0.8.tar` & `cspot-1.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1907 2023-06-04 22:13:27.495922 cspot-1.0.8/README.md
--rw-r--r--   0        0        0     8196 2023-06-03 14:50:07.931359 cspot-1.0.8/cspot/.DS_Store
--rw-r--r--   0        0        0    32012 2023-03-20 20:58:58.000000 cspot-1.0.8/cspot/UNet.py
--rw-r--r--   0        0        0      567 2023-06-03 00:49:31.038091 cspot-1.0.8/cspot/__init__.py
--rw-r--r--   0        0        0     6447 2023-06-04 14:04:52.928156 cspot-1.0.8/cspot/addPredictions.py
--rw-r--r--   0        0        0    30831 2023-02-04 00:24:05.000000 cspot-1.0.8/cspot/archives/UNet-02032023.py
--rw-r--r--   0        0        0    35278 2023-01-27 16:37:48.000000 cspot-1.0.8/cspot/archives/gator-01272023.py
--rw-r--r--   0        0        0      727 2023-02-03 20:50:23.000000 cspot-1.0.8/cspot/archives/toolbox-02032023/GPUselect.py
--rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.000000 cspot-1.0.8/cspot/archives/toolbox-02032023/PartitionOfImage.py
--rw-r--r--   0        0        0     6075 2023-02-03 20:50:23.000000 cspot-1.0.8/cspot/archives/toolbox-02032023/PartitionOfImageOM.py
--rw-r--r--   0        0        0      804 2023-02-04 00:05:31.000000 cspot-1.0.8/cspot/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc
--rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.000000 cspot-1.0.8/cspot/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc
--rw-r--r--   0        0        0     2062 2023-02-04 00:05:31.000000 cspot-1.0.8/cspot/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc
--rw-r--r--   0        0        0     9960 2023-02-04 00:25:40.000000 cspot-1.0.8/cspot/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc
--rw-r--r--   0        0        0     1408 2023-02-03 20:50:23.000000 cspot-1.0.8/cspot/archives/toolbox-02032023/ftools.py
--rw-r--r--   0        0        0    10892 2023-02-04 00:25:24.000000 cspot-1.0.8/cspot/archives/toolbox-02032023/imtools.py
--rw-r--r--   0        0        0     7197 2023-02-03 20:50:23.000000 cspot-1.0.8/cspot/archives/toolbox-02032023/toolbox.py
--rw-r--r--   0        0        0     9983 2023-06-03 23:29:17.205882 cspot-1.0.8/cspot/cloneFolder.py
--rw-r--r--   0        0        0     5516 2023-06-06 17:24:19.305517 cspot-1.0.8/cspot/csExport.py
--rw-r--r--   0        0        0    12214 2023-06-04 01:49:29.376512 cspot-1.0.8/cspot/csObject.py
--rw-r--r--   0        0        0    21466 2023-06-04 13:57:25.098445 cspot-1.0.8/cspot/csPhenotype.py
--rw-r--r--   0        0        0    17791 2023-06-04 00:09:38.907372 cspot-1.0.8/cspot/csPipeline.py
--rw-r--r--   0        0        0    12655 2023-06-04 01:03:32.130826 cspot-1.0.8/cspot/csPredict.py
--rw-r--r--   0        0        0    11491 2023-06-03 23:36:08.727326 cspot-1.0.8/cspot/csTrain.py
--rw-r--r--   0        0        0    41377 2023-06-04 01:56:09.635845 cspot-1.0.8/cspot/cspot.py
--rw-r--r--   0        0        0     7236 2023-06-04 01:37:29.786489 cspot-1.0.8/cspot/generateCSScore.py
--rw-r--r--   0        0        0    27169 2023-10-25 17:33:31.000000 cspot-1.0.8/cspot/generateThumbnails.py
--rw-r--r--   0        0        0    13523 2023-06-03 23:32:52.946563 cspot-1.0.8/cspot/generateTrainTestSplit.py
--rw-r--r--   0        0        0     8633 2023-06-04 02:03:45.337949 cspot-1.0.8/cspot/mergecsObject.py
--rw-r--r--   0        0        0    10237 2023-06-04 00:13:46.879038 cspot-1.0.8/cspot/scatterPlot.py
--rw-r--r--   0        0        0      727 2023-02-03 20:50:23.000000 cspot-1.0.8/cspot/toolbox/GPUselect.py
--rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.000000 cspot-1.0.8/cspot/toolbox/PartitionOfImage.py
--rw-r--r--   0        0        0      196 2023-03-10 02:36:16.000000 cspot-1.0.8/cspot/toolbox/__init__.py
--rw-r--r--   0        0        0      804 2023-02-04 00:05:31.000000 cspot-1.0.8/cspot/toolbox/__pycache__/GPUselect.cpython-39.pyc
--rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.000000 cspot-1.0.8/cspot/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc
--rw-r--r--   0        0        0      477 2023-03-10 02:39:18.000000 cspot-1.0.8/cspot/toolbox/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      711 2023-02-04 00:52:32.000000 cspot-1.0.8/cspot/toolbox/__pycache__/ftools.cpython-39.pyc
--rw-r--r--   0        0        0     1017 2023-02-04 00:52:32.000000 cspot-1.0.8/cspot/toolbox/__pycache__/imtools.cpython-39.pyc
--rw-r--r--   0        0        0      361 2023-02-04 00:50:12.000000 cspot-1.0.8/cspot/toolbox/ftools.py
--rw-r--r--   0        0        0      671 2023-02-04 00:46:01.000000 cspot-1.0.8/cspot/toolbox/imtools.py
--rw-r--r--   0        0        0     1166 2023-10-25 18:18:20.457189 cspot-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     3465 1970-01-01 00:00:00.000000 cspot-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1907 2023-06-04 22:13:27.495922 cspot-1.0.9/README.md
+-rw-r--r--   0        0        0     8196 2023-06-03 14:50:07.931359 cspot-1.0.9/cspot/.DS_Store
+-rw-r--r--   0        0        0    32012 2023-03-20 20:58:58.000000 cspot-1.0.9/cspot/UNet.py
+-rw-r--r--   0        0        0      567 2023-06-03 00:49:31.038091 cspot-1.0.9/cspot/__init__.py
+-rw-r--r--   0        0        0     6447 2023-06-04 14:04:52.928156 cspot-1.0.9/cspot/addPredictions.py
+-rw-r--r--   0        0        0    30831 2023-02-04 00:24:05.000000 cspot-1.0.9/cspot/archives/UNet-02032023.py
+-rw-r--r--   0        0        0    35278 2023-01-27 16:37:48.000000 cspot-1.0.9/cspot/archives/gator-01272023.py
+-rw-r--r--   0        0        0      727 2023-02-03 20:50:23.000000 cspot-1.0.9/cspot/archives/toolbox-02032023/GPUselect.py
+-rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.000000 cspot-1.0.9/cspot/archives/toolbox-02032023/PartitionOfImage.py
+-rw-r--r--   0        0        0     6075 2023-02-03 20:50:23.000000 cspot-1.0.9/cspot/archives/toolbox-02032023/PartitionOfImageOM.py
+-rw-r--r--   0        0        0      804 2023-02-04 00:05:31.000000 cspot-1.0.9/cspot/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc
+-rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.000000 cspot-1.0.9/cspot/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc
+-rw-r--r--   0        0        0     2062 2023-02-04 00:05:31.000000 cspot-1.0.9/cspot/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc
+-rw-r--r--   0        0        0     9960 2023-02-04 00:25:40.000000 cspot-1.0.9/cspot/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc
+-rw-r--r--   0        0        0     1408 2023-02-03 20:50:23.000000 cspot-1.0.9/cspot/archives/toolbox-02032023/ftools.py
+-rw-r--r--   0        0        0    10892 2023-02-04 00:25:24.000000 cspot-1.0.9/cspot/archives/toolbox-02032023/imtools.py
+-rw-r--r--   0        0        0     7197 2023-02-03 20:50:23.000000 cspot-1.0.9/cspot/archives/toolbox-02032023/toolbox.py
+-rw-r--r--   0        0        0     9983 2023-06-03 23:29:17.205882 cspot-1.0.9/cspot/cloneFolder.py
+-rw-r--r--   0        0        0     5516 2023-06-06 17:24:19.305517 cspot-1.0.9/cspot/csExport.py
+-rw-r--r--   0        0        0    12214 2023-06-04 01:49:29.376512 cspot-1.0.9/cspot/csObject.py
+-rw-r--r--   0        0        0    21466 2023-06-04 13:57:25.098445 cspot-1.0.9/cspot/csPhenotype.py
+-rw-r--r--   0        0        0    17791 2023-06-04 00:09:38.907372 cspot-1.0.9/cspot/csPipeline.py
+-rw-r--r--   0        0        0    12655 2023-06-04 01:03:32.130826 cspot-1.0.9/cspot/csPredict.py
+-rw-r--r--   0        0        0    11491 2023-06-03 23:36:08.727326 cspot-1.0.9/cspot/csTrain.py
+-rw-r--r--   0        0        0    43066 2024-01-09 04:09:51.843110 cspot-1.0.9/cspot/cspot.py
+-rw-r--r--   0        0        0     7236 2023-06-04 01:37:29.786489 cspot-1.0.9/cspot/generateCSScore.py
+-rw-r--r--   0        0        0    27169 2023-10-25 17:33:31.000000 cspot-1.0.9/cspot/generateThumbnails.py
+-rw-r--r--   0        0        0    13523 2023-06-03 23:32:52.946563 cspot-1.0.9/cspot/generateTrainTestSplit.py
+-rw-r--r--   0        0        0     8633 2023-06-04 02:03:45.337949 cspot-1.0.9/cspot/mergecsObject.py
+-rw-r--r--   0        0        0    10237 2023-06-04 00:13:46.879038 cspot-1.0.9/cspot/scatterPlot.py
+-rw-r--r--   0        0        0      727 2023-02-03 20:50:23.000000 cspot-1.0.9/cspot/toolbox/GPUselect.py
+-rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.000000 cspot-1.0.9/cspot/toolbox/PartitionOfImage.py
+-rw-r--r--   0        0        0      196 2023-03-10 02:36:16.000000 cspot-1.0.9/cspot/toolbox/__init__.py
+-rw-r--r--   0        0        0      804 2023-02-04 00:05:31.000000 cspot-1.0.9/cspot/toolbox/__pycache__/GPUselect.cpython-39.pyc
+-rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.000000 cspot-1.0.9/cspot/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc
+-rw-r--r--   0        0        0      477 2023-03-10 02:39:18.000000 cspot-1.0.9/cspot/toolbox/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      711 2023-02-04 00:52:32.000000 cspot-1.0.9/cspot/toolbox/__pycache__/ftools.cpython-39.pyc
+-rw-r--r--   0        0        0     1017 2023-02-04 00:52:32.000000 cspot-1.0.9/cspot/toolbox/__pycache__/imtools.cpython-39.pyc
+-rw-r--r--   0        0        0      361 2023-02-04 00:50:12.000000 cspot-1.0.9/cspot/toolbox/ftools.py
+-rw-r--r--   0        0        0      671 2023-02-04 00:46:01.000000 cspot-1.0.9/cspot/toolbox/imtools.py
+-rw-r--r--   0        0        0     1166 2024-01-09 04:09:11.582035 cspot-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3465 1970-01-01 00:00:00.000000 cspot-1.0.9/PKG-INFO
```

### Comparing `cspot-1.0.8/README.md` & `cspot-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/.DS_Store` & `cspot-1.0.9/cspot/.DS_Store`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/UNet.py` & `cspot-1.0.9/cspot/UNet.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/__init__.py` & `cspot-1.0.9/cspot/__init__.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/addPredictions.py` & `cspot-1.0.9/cspot/addPredictions.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/archives/UNet-02032023.py` & `cspot-1.0.9/cspot/archives/UNet-02032023.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/archives/gator-01272023.py` & `cspot-1.0.9/cspot/archives/gator-01272023.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/archives/toolbox-02032023/GPUselect.py` & `cspot-1.0.9/cspot/archives/toolbox-02032023/GPUselect.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/archives/toolbox-02032023/PartitionOfImage.py` & `cspot-1.0.9/cspot/archives/toolbox-02032023/PartitionOfImage.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/archives/toolbox-02032023/PartitionOfImageOM.py` & `cspot-1.0.9/cspot/archives/toolbox-02032023/PartitionOfImageOM.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc` & `cspot-1.0.9/cspot/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc` & `cspot-1.0.9/cspot/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc` & `cspot-1.0.9/cspot/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc` & `cspot-1.0.9/cspot/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/archives/toolbox-02032023/ftools.py` & `cspot-1.0.9/cspot/archives/toolbox-02032023/ftools.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/archives/toolbox-02032023/imtools.py` & `cspot-1.0.9/cspot/archives/toolbox-02032023/imtools.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/archives/toolbox-02032023/toolbox.py` & `cspot-1.0.9/cspot/archives/toolbox-02032023/toolbox.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/cloneFolder.py` & `cspot-1.0.9/cspot/cloneFolder.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/csExport.py` & `cspot-1.0.9/cspot/csExport.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/csObject.py` & `cspot-1.0.9/cspot/csObject.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/csPhenotype.py` & `cspot-1.0.9/cspot/csPhenotype.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/csPipeline.py` & `cspot-1.0.9/cspot/csPipeline.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/csPredict.py` & `cspot-1.0.9/cspot/csPredict.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/csTrain.py` & `cspot-1.0.9/cspot/csTrain.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/cspot.py` & `cspot-1.0.9/cspot/cspot.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,20 @@
             --csObject /Users/aj/Documents/cspotExampleData/CSPOT/csObject/exampleImage_cspotPredict.ome.h5ad \
             --projectDir /Users/aj/Documents/cspotExampleData
                 
         
         ```
 
     """
+    
+    # testing
+    #csObject= '/Users/aj/Dropbox (Partners HealthCare)/nirmal lab/resources/exemplarData/cspotExampleData/CSPOT/csObject/exampleImage_cspotPredict.ome.h5ad'
+    #csScore='csScore'; minAbundance=0.005; percentiles=[1, 20, 80, 99]; dropMarkers = None
+    #RobustScale=False; log=True; stringentThreshold=False; x_coordinate='X_centroid'; y_coordinate='Y_centroid'
+    #imageid='imageid'; random_state=0; rescaleMethod='minmax'; label='cspotOutput'; verbose=True; projectDir=None
 
     # Load the andata object
     if isinstance(csObject, str):
         adata = ad.read(csObject)
         csObject = [csObject]
         csObjectPath = [pathlib.Path(p) for p in csObject]
     else:
@@ -324,25 +330,27 @@
       return sorted_data[midpoint_index]
 
     # Used for reassigning some of the wrong 'nes' and 'pos' within data given a midpoint
     def modify_negatives_vectorized(data, labels, midpoint):
       # Convert data and labels to NumPy arrays
       data = np.array(data)
       labels = np.array(labels)
+      # Calculating the mean of 'neg' instances  (used to replace wrongly assigned pos instances)
+      neg_mean = np.mean(data[labels == 'neg'])
       # Get the indices that would sort the data and labels arrays
       sort_indices = np.argsort(data)
       # Sort the data and labels arrays using the sort indices
       sorted_data = data[sort_indices]
       sorted_labels = labels[sort_indices]
       # Find the index where the sorted data is greater than or equal to the midpoint value
       midpoint_index = np.argmax(sorted_data >= midpoint)
       # Find all the elements in the sorted labels array with a value of 'neg' after the midpoint index
       neg_mask = np.logical_and(sorted_labels == 'neg', np.arange(len(sorted_data)) >= midpoint_index)
       # Modify the value of the elements to be equal to the midpoint value
-      sorted_data[neg_mask] = midpoint
+      sorted_data[neg_mask] = neg_mean
       # Find all the elements in the sorted labels array with a value of 'pos' before the midpoint index
       pos_mask = np.logical_and(sorted_labels == 'pos', np.arange(len(sorted_data)) < midpoint_index)
       # Modify the value of the elements to be equal to the midpoint value plus 0.1
       sorted_data[pos_mask] = midpoint + 0.1
       # Reorder the data array to the original order
       reordered_data = sorted_data[np.argsort(sort_indices)]
       # Return the modified data
@@ -569,15 +577,15 @@
     
 
 
     ###########################################################################
     # step-5 : Generate training data for the Gradient Boost Classifier
     ###########################################################################
 
-    # bonafide_cells_result = bonafide_cells_result[2]
+    # bonafide_cells_result = bonafide_cells_result[8]
     def trainingData (bonafide_cells_result, pre_processed_data, RobustScale):
         # uravel the data
         marker = bonafide_cells_result[0]
         pos = bonafide_cells_result[1]
         neg = bonafide_cells_result[2]
         PD = pre_processed_data.copy()
 
@@ -700,43 +708,71 @@
         midpoints_dict[markerOrder[i]] = csClassifier_result[i][3]
 
     ###########################################################################
     # step-8 : Final cleaning of predicted results with UNET results
     ###########################################################################
 
     # bonafide_cells_result_copy = bonafide_cells_result.copy()
-    # bonafide_cells_result = bonafide_cells_result[0]
+    # bonafide_cells_result = bonafide_cells_result[8]
 
     def anomalyDetector (pre_processed_data, bonafide_cells_result, prediction_results):
         # unravel data
         marker = bonafide_cells_result[0]
         pos = bonafide_cells_result[1]
         neg = bonafide_cells_result[2]
 
         if verbose is True:
             print("Processing: " + str(marker))
         # prepare data
         X = pre_processed_data.drop(marker, axis=1)
         # scale data
         scaler = StandardScaler()
         X_scaled = scaler.fit_transform(X)
+        
         # model data
-        model = LocalOutlierFactor(n_neighbors=20)
-        model.fit(X_scaled)
-        outlier_scores = model.negative_outlier_factor_
-        outliers = pre_processed_data[outlier_scores < -1].index
+        #model = LocalOutlierFactor(n_neighbors=20)
+        #model.fit(X_scaled)
+        #outlier_scores = model.negative_outlier_factor_
+        #outliers = pre_processed_data[outlier_scores < -1].index
+
+        # Initialize LocalOutlierFactor with parallel processing
+        model = LocalOutlierFactor(n_neighbors=20, n_jobs=-1)
+        
+        # Define batch size and prepare for batch processing
+        batch_size = 50000  # Adjust this based on your system's memory capacity
+        n_batches = int(np.ceil(X_scaled.shape[0] / batch_size))
+        
+        outlier_scores = np.array([])
+        
+        # Process in batches
+        for i in range(n_batches):
+            start_index = i * batch_size
+            end_index = start_index + batch_size
+            batch = X_scaled[start_index:end_index]
+        
+            # Fit the model on the batch
+            model.fit(batch)
+            
+            # Append the batch's outlier scores
+            batch_scores = model.negative_outlier_factor_
+            outlier_scores = np.concatenate((outlier_scores, batch_scores))
+        
+        # Identifying outliers
+        threshold = -1 
+        outliers = pre_processed_data[outlier_scores < threshold].index
+                
 
         # common elements betwenn outliers and true neg
         posttoneg = list(set(outliers).intersection(set(neg)))
         # similarly is there any cells in negative that needs to be relocated to positive?
         negtopos = list(set(pos).intersection(set(prediction_results[prediction_results[marker]=='neg'].index)))
 
         # mutate the prediction results
-        prediction_results.loc[posttoneg, marker] = 'neg'
         prediction_results.loc[negtopos, marker] = 'pos'
+        prediction_results.loc[posttoneg, marker] = 'neg'
 
         # results
         results = prediction_results[[marker]]
         return results
 
     # Run the function
     if verbose is True:
```

### Comparing `cspot-1.0.8/cspot/generateCSScore.py` & `cspot-1.0.9/cspot/generateCSScore.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/generateThumbnails.py` & `cspot-1.0.9/cspot/generateThumbnails.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/generateTrainTestSplit.py` & `cspot-1.0.9/cspot/generateTrainTestSplit.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/mergecsObject.py` & `cspot-1.0.9/cspot/mergecsObject.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/scatterPlot.py` & `cspot-1.0.9/cspot/scatterPlot.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/toolbox/GPUselect.py` & `cspot-1.0.9/cspot/toolbox/GPUselect.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/toolbox/PartitionOfImage.py` & `cspot-1.0.9/cspot/toolbox/PartitionOfImage.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/toolbox/__pycache__/GPUselect.cpython-39.pyc` & `cspot-1.0.9/cspot/toolbox/__pycache__/GPUselect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc` & `cspot-1.0.9/cspot/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/toolbox/__pycache__/ftools.cpython-39.pyc` & `cspot-1.0.9/cspot/toolbox/__pycache__/ftools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/toolbox/__pycache__/imtools.cpython-39.pyc` & `cspot-1.0.9/cspot/toolbox/__pycache__/imtools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/cspot/toolbox/imtools.py` & `cspot-1.0.9/cspot/toolbox/imtools.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.8/pyproject.toml` & `cspot-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cspot"
-version = "1.0.8"
+version = "1.0.9"
 description = "CELL SPOTTER (CSPOT): A scalable framework for automated processing of highly multiplexed tissue images"
 authors = ["Ajit Johnson Nirmal <ajitjohnson.n@gmail.com>"]
 readme = "README.md"
 
 keywords = ["image analysis","multiplex imaging","single cell analysis"]
 
 homepage = "https://pypi.org/project/cspot/"
```

### Comparing `cspot-1.0.8/PKG-INFO` & `cspot-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cspot
-Version: 1.0.8
+Version: 1.0.9
 Summary: CELL SPOTTER (CSPOT): A scalable framework for automated processing of highly multiplexed tissue images
 Home-page: https://pypi.org/project/cspot/
 Keywords: image analysis,multiplex imaging,single cell analysis
 Author: Ajit Johnson Nirmal
 Author-email: ajitjohnson.n@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
```

