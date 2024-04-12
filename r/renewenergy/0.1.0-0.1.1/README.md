# Comparing `tmp/renewenergy-0.1.0.tar.gz` & `tmp/renewenergy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renewenergy-0.1.0.tar", max compression
+gzip compressed data, was "renewenergy-0.1.1.tar", max compression
```

## Comparing `renewenergy-0.1.0.tar` & `renewenergy-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rwxr-xr-x   0        0        0     1108 2024-04-05 23:16:56.371666 renewenergy-0.1.0/LICENSE
--rw-r--r--   0        0        0     1273 2024-04-08 00:14:13.223028 renewenergy-0.1.0/README.md
--rw-r--r--   0        0        0     1074 2024-04-09 18:38:05.756543 renewenergy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      113 2024-04-05 23:16:56.393918 renewenergy-0.1.0/src/renewenergy/__init__.py
--rw-r--r--   0        0        0     1226 2024-04-07 19:56:46.722418 renewenergy-0.1.0/src/renewenergy/clean_data.py
--rw-r--r--   0        0        0     1401 2024-04-07 23:10:11.710780 renewenergy-0.1.0/src/renewenergy/eda.py
--rw-r--r--   0        0        0     1174 2024-04-06 00:06:28.171100 renewenergy-0.1.0/src/renewenergy/functionread.py
--rw-r--r--   0        0        0      923 2024-04-06 00:11:42.920773 renewenergy-0.1.0/src/renewenergy/impute_split.py
--rw-r--r--   0        0        0     2103 2024-04-07 07:44:54.956104 renewenergy-0.1.0/src/renewenergy/linear_regression.py
--rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 renewenergy-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1108 2024-04-12 00:07:54.847276 renewenergy-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1428 2024-04-12 00:07:54.847276 renewenergy-0.1.1/README.md
+-rw-r--r--   0        0        0     1074 2024-04-12 00:08:05.247416 renewenergy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      113 2024-04-12 00:07:54.911276 renewenergy-0.1.1/src/renewenergy/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-12 00:07:54.911276 renewenergy-0.1.1/src/renewenergy/clean_data.py
+-rw-r--r--   0        0        0     1453 2024-04-12 00:07:54.911276 renewenergy-0.1.1/src/renewenergy/create_scatter_plots.py
+-rw-r--r--   0        0        0      923 2024-04-12 00:07:54.911276 renewenergy-0.1.1/src/renewenergy/impute_split.py
+-rw-r--r--   0        0        0     3403 2024-04-12 00:07:54.911276 renewenergy-0.1.1/src/renewenergy/plot_rmse.py
+-rw-r--r--   0        0        0     1809 2024-04-12 00:07:54.911276 renewenergy-0.1.1/src/renewenergy/reading_data.py
+-rw-r--r--   0        0        0     1077 2024-04-12 00:07:54.911276 renewenergy-0.1.1/src/renewenergy/split_xy_columns.py
+-rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 renewenergy-0.1.1/PKG-INFO
```

### Comparing `renewenergy-0.1.0/LICENSE` & `renewenergy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `renewenergy-0.1.0/README.md` & `renewenergy-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # renewenergy
 
 A great package to run aanalysis to help predict the renewable energy output of a country.
 
+[![Documentation Status](https://readthedocs.org/projects/renewenergy/badge/?version=latest)](https://renewenergy.readthedocs.io/en/latest/?badge=latest)
+
 ## Installation
 
 ```bash
 $ pip install renewenergy
 ```
 
 ## Usage
```

### Comparing `renewenergy-0.1.0/pyproject.toml` & `renewenergy-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "renewenergy"
-version = "0.1.0"
+version = "0.1.1"
 description = "A great package to run aanalysis to help predict the renewable energy output of a country."
 authors = ["Neha Menon, Caden Chan, Peter Chen, Tak Sripratak"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `renewenergy-0.1.0/src/renewenergy/eda.py` & `renewenergy-0.1.1/src/renewenergy/create_scatter_plots.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from matplotlib import pyplot as plt
+import click
+import numpy as np
+import pandas as pd
 
 def create_scatter_plots(data, x_columns, y_column, nrows, ncols, figsize=(32, 17)):
     """
     Create scatter plots for given columns against a common y-column.
 
     Parameters:
     - data (DataFrame): The data to plot.
```

### Comparing `renewenergy-0.1.0/src/renewenergy/functionread.py` & `renewenergy-0.1.1/src/renewenergy/reading_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,44 @@
 # import urllib.request as urllib2
 import pandas as pd
 import os
 from zipfile import ZipFile
 from urllib.request import urlopen
 import pathlib
 
-def reading_datain(url, data_file, data_path, file_name):
+def reading_data(url, data_file, data_path, file_name):
+    """
+    Read a specified data file in from a URL containing a zip file.
+
+    Parameters
+    ----------
+    url : str
+        URL of link containing zip file. 
+    
+    data_file: str
+        Specified file in .ZIP that data is to be extracted from. 
+    
+    data_path: str
+        Directory to which the imported data should be saved to. 
+    
+    file_name: str
+        Name of file that imported data will be saved to. 
+    
+
+    Returns
+    -------
+    file_name.csv
+        CSV file that data is saved to. 
+
+    Examples
+    --------
+    >>> reading_datain("url", "WDICSV.csv", "data/raw", "downloaded_data.csv" )
+    
+    """
+
     """Simple program that reads in the data from a URL, and selects a file from the .zip."""
     request= requests.get(url)
 
     if request.status_code !=200:
         raise ValueError('The inputed URL does not exist.')
     
     if url[-4:] !=".zip":
```

### Comparing `renewenergy-0.1.0/src/renewenergy/impute_split.py` & `renewenergy-0.1.1/src/renewenergy/impute_split.py`

 * *Files identical despite different names*

### Comparing `renewenergy-0.1.0/src/renewenergy/linear_regression.py` & `renewenergy-0.1.1/src/renewenergy/plot_rmse.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,29 +4,83 @@
 from sklearn.model_selection import train_test_split
 from sklearn.linear_model import LinearRegression
 from sklearn.metrics import mean_squared_error
 from sklearn import set_config
 from sklearn.metrics import mean_squared_error
 
 
-def split_xy_columns(dataset):
-    #splitting the x and y columns of the data
-    dataset_x = dataset
-    dataset_x = dataset_x.drop('Renewable electricity output (% of total electricity output)', axis=1)
-    dataset_x = dataset_x.drop('Country Name', axis=1)
-    dataset_y = dataset[["Renewable electricity output (% of total electricity output)"]]
+# def split_xy_columns(dataset):
+#     """
+#     Read a specified data file in from a URL containing a zip file.
+
+#     Parameters
+#     ----------
+#     url : str
+#         URL of link containing zip file. 
+    
+#     data_file: str
+#         Specified file in .ZIP that data is to be extracted from. 
+    
+#     data_path: str
+#         Directory to which the imported data should be saved to. 
+    
+#     file_name: str
+#         Name of file that imported data will be saved to. 
+    
+
+#     Returns
+#     -------
+#     file_name.csv
+#         CSV file that data is saved to. 
+
+#     Examples
+#     --------
+#     >>> reading_datain("url", "WDICSV.csv", "data/raw", "downloaded_data.csv" )
+    
+#     """
+
+#     #splitting the x and y columns of the data
+#     dataset_x = dataset
+#     dataset_x = dataset_x.drop('Renewable electricity output (% of total electricity output)', axis=1)
+#     dataset_x = dataset_x.drop('Country Name', axis=1)
+#     dataset_y = dataset[["Renewable electricity output (% of total electricity output)"]]
 
-    return dataset_x, dataset_y
+#     return dataset_x, dataset_y
 
 #@click.command()
 #@click.option('--training_data_path', help='path of training set data (csv) to read', type=str)
 #@click.option('--test_data_path', help='path of test set data (csv) to read', type=str)
 #@click.option('--output_path', help='folder path to save the results, need to end with.png', type=str)
 
 def plot_rmse(training_data_path, test_data_path, output_path):
+    """
+    Perform linear regression and plot the results on a graph containing Expected vs Predicted. 
+
+    Parameters
+    ----------
+    training_data_path: str
+        Path to training data .csv file
+    
+    test_data_path: str
+        Path to test data .csv file
+    
+    output_path: str
+        Directory to which the figure should be saved to. 
+    
+    
+    Returns
+    -------
+    results.png
+        Figure containing the Predicted vs Expected Values of the linear regression.
+
+    Examples
+    --------
+    >>> plot_rmse("data/energy_train.csv", "data/energy_test.csv", "results/" )
+    
+    """
     #read clean train and test dataset
 
     energy_train = pd.read_csv(training_data_path)
     energy_test = pd.read_csv(test_data_path)
 
     #splitting the x and y columns of the data
```

### Comparing `renewenergy-0.1.0/PKG-INFO` & `renewenergy-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renewenergy
-Version: 0.1.0
+Version: 0.1.1
 Summary: A great package to run aanalysis to help predict the renewable energy output of a country.
 License: MIT
 Author: Neha Menon, Caden Chan, Peter Chen, Tak Sripratak
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -16,14 +16,16 @@
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # renewenergy
 
 A great package to run aanalysis to help predict the renewable energy output of a country.
 
+[![Documentation Status](https://readthedocs.org/projects/renewenergy/badge/?version=latest)](https://renewenergy.readthedocs.io/en/latest/?badge=latest)
+
 ## Installation
 
 ```bash
 $ pip install renewenergy
 ```
 
 ## Usage
```

