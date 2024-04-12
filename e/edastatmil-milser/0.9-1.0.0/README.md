# Comparing `tmp/edastatmil_milser-0.9.tar.gz` & `tmp/edastatmil_milser-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edastatmil_milser-0.9.tar", last modified: Mon Apr  8 16:37:28 2024, max compression
+gzip compressed data, was "edastatmil_milser-1.0.0.tar", last modified: Fri Apr 12 16:36:54 2024, max compression
```

## Comparing `edastatmil_milser-0.9.tar` & `edastatmil_milser-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 16:37:28.908364 edastatmil_milser-0.9/
--rw-rw-rw-   0        0        0    11558 2024-04-06 18:06:27.000000 edastatmil_milser-0.9/LICENSE
--rw-rw-rw-   0        0        0       70 2024-04-06 18:06:27.000000 edastatmil_milser-0.9/MANIFEST.in
--rw-rw-rw-   0        0        0      630 2024-04-08 16:37:28.907365 edastatmil_milser-0.9/PKG-INFO
--rw-rw-rw-   0        0        0      517 2024-04-08 16:37:02.000000 edastatmil_milser-0.9/pyproject.toml
--rw-rw-rw-   0        0        0      538 2024-04-08 16:37:28.913366 edastatmil_milser-0.9/setup.cfg
--rw-rw-rw-   0        0        0      613 2024-04-08 16:36:59.000000 edastatmil_milser-0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:37:28.820320 edastatmil_milser-0.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 16:37:28.879342 edastatmil_milser-0.9/src/edastatmil_milser/
--rw-rw-rw-   0        0        0       63 2024-04-06 18:06:27.000000 edastatmil_milser-0.9/src/edastatmil_milser/__init__.py
--rw-rw-rw-   0        0        0      277 2024-04-06 18:11:47.000000 edastatmil_milser-0.9/src/edastatmil_milser/commandline.py
--rw-rw-rw-   0        0        0    26328 2024-04-08 16:36:38.000000 edastatmil_milser-0.9/src/edastatmil_milser/edas_tatmil.py
--rw-rw-rw-   0        0        0      175 2024-04-08 16:36:55.000000 edastatmil_milser-0.9/src/edastatmil_milser/version.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:37:28.906365 edastatmil_milser-0.9/src/edastatmil_milser.egg-info/
--rw-rw-rw-   0        0        0      630 2024-04-08 16:37:28.000000 edastatmil_milser-0.9/src/edastatmil_milser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-04-08 16:37:28.000000 edastatmil_milser-0.9/src/edastatmil_milser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 16:37:28.000000 edastatmil_milser-0.9/src/edastatmil_milser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-08 16:37:28.000000 edastatmil_milser-0.9/src/edastatmil_milser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 16:36:54.680206 edastatmil_milser-1.0.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-12 16:32:09.000000 edastatmil_milser-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       70 2024-04-12 16:32:09.000000 edastatmil_milser-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    16331 2024-04-12 16:36:54.679206 edastatmil_milser-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    15697 2024-04-12 16:19:55.000000 edastatmil_milser-1.0.0/README.md
+-rw-rw-rw-   0        0        0      519 2024-04-12 16:32:09.000000 edastatmil_milser-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      540 2024-04-12 16:36:54.682216 edastatmil_milser-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      615 2024-04-12 16:36:00.000000 edastatmil_milser-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:36:54.637196 edastatmil_milser-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 16:36:54.653201 edastatmil_milser-1.0.0/src/edastatmil_milser/
+-rw-rw-rw-   0        0        0       63 2024-04-12 16:30:31.000000 edastatmil_milser-1.0.0/src/edastatmil_milser/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-04-12 16:30:30.000000 edastatmil_milser-1.0.0/src/edastatmil_milser/commandline.py
+-rw-rw-rw-   0        0        0    27991 2024-04-12 16:30:30.000000 edastatmil_milser-1.0.0/src/edastatmil_milser/edas_tatmil.py
+-rw-rw-rw-   0        0        0      177 2024-04-12 16:30:30.000000 edastatmil_milser-1.0.0/src/edastatmil_milser/version.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:36:54.677204 edastatmil_milser-1.0.0/src/edastatmil_milser.egg-info/
+-rw-rw-rw-   0        0        0    16331 2024-04-12 16:36:54.000000 edastatmil_milser-1.0.0/src/edastatmil_milser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2024-04-12 16:36:54.000000 edastatmil_milser-1.0.0/src/edastatmil_milser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 16:36:54.000000 edastatmil_milser-1.0.0/src/edastatmil_milser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-12 16:36:54.000000 edastatmil_milser-1.0.0/src/edastatmil_milser.egg-info/top_level.txt
```

### Comparing `edastatmil_milser-0.9/LICENSE` & `edastatmil_milser-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edastatmil_milser-0.9/pyproject.toml` & `edastatmil_milser-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "edastatmil_milser"
-version = "0.9"
+version = "1.0.0"
 authors = [
   { name="TatianaCC y milser", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `edastatmil_milser-0.9/setup.cfg` & `edastatmil_milser-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6461 7374 6174 6d69 6c5f 6d69   = edastatmil_mi
 00000020: 6c73 6572 0d0a 7665 7273 696f 6e20 3d20  lser..version = 
-00000030: 302e 390d 0a61 7574 686f 7220 3d20 5461  0.9..author = Ta
-00000040: 7469 616e 6143 4320 7920 6d69 6c73 6572  tianaCC y milser
-00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
-00000060: 2061 7574 686f 7240 6578 616d 706c 652e   author@example.
-00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
-00000080: 203d 2041 2073 6d61 6c6c 2065 7861 6d70   = A small examp
-00000090: 6c65 2070 6163 6b61 6765 0d0a 6c6f 6e67  le package..long
-000000a0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-000000b0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-000000c0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000d0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-000000e0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
-000000f0: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
-00000100: 6875 622e 636f 6d2f 6d69 6c73 6572 2f65  hub.com/milser/e
-00000110: 6461 735f 7461 7469 616e 616d 696c 7365  das_tatianamilse
-00000120: 720d 0a63 6c61 7373 6966 6965 7273 203d  r..classifiers =
-00000130: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
-00000140: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000150: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
-00000160: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000170: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-00000180: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-00000190: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
-000001a0: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
-000001b0: 735d 0d0a 7061 636b 6167 6573 203d 2066  s]..packages = f
-000001c0: 696e 643a 0d0a 0d0a 5b6f 7074 696f 6e73  ind:....[options
-000001d0: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-000001e0: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
-000001f0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000200: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000210: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000030: 312e 302e 300d 0a61 7574 686f 7220 3d20  1.0.0..author = 
+00000040: 5461 7469 616e 6143 4320 7920 6d69 6c73  TatianaCC y mils
+00000050: 6572 0d0a 6175 7468 6f72 5f65 6d61 696c  er..author_email
+00000060: 203d 2061 7574 686f 7240 6578 616d 706c   = author@exampl
+00000070: 652e 636f 6d0d 0a64 6573 6372 6970 7469  e.com..descripti
+00000080: 6f6e 203d 2041 2073 6d61 6c6c 2065 7861  on = A small exa
+00000090: 6d70 6c65 2070 6163 6b61 6765 0d0a 6c6f  mple package..lo
+000000a0: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
+000000b0: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
+000000c0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000000d0: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+000000e0: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
+000000f0: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
+00000100: 6974 6875 622e 636f 6d2f 6d69 6c73 6572  ithub.com/milser
+00000110: 2f65 6461 735f 7461 7469 616e 616d 696c  /edas_tatianamil
+00000120: 7365 720d 0a63 6c61 7373 6966 6965 7273  ser..classifiers
+00000130: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
+00000140: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000150: 7468 6f6e 203a 3a20 330d 0a09 4c69 6365  thon :: 3...Lice
+00000160: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000170: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+00000180: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
+00000190: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+000001a0: 7065 6e64 656e 740d 0a0d 0a5b 6f70 7469  pendent....[opti
+000001b0: 6f6e 735d 0d0a 7061 636b 6167 6573 203d  ons]..packages =
+000001c0: 2066 696e 643a 0d0a 0d0a 5b6f 7074 696f   find:....[optio
+000001d0: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
+000001e0: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
+000001f0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000200: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000210: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `edastatmil_milser-0.9/setup.py` & `edastatmil_milser-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='edastatmil_milser',
-    version='0.9',
+    version='1.0.0',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     author='Tatiana Cazorla y Rubén Serrano',
     description='Tu EDA mas sencillo',
     url='https://github.com/milser/edas_tatianamilser',
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `edastatmil_milser-0.9/src/edastatmil_milser/edas_tatmil.py` & `edastatmil_milser-1.0.0/src/edastatmil_milser/edas_tatmil.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ############################################################################
-#                       Functions for complete EDA                         #
+#                       Functions for complete EDA   V1.0.0                 #
 # ------------------------------------------------------------------------ #
+#   - build_directory for create necessary files structure.
 #   - get_column_type for discrimine variables in numerical or categorical #
 #   - explore for get basic info and both list of numerical and            #
 #     categorical variables                                                #
 #   - FindDuplicates for find and drop (or not) duplicates based in one    #
 #     given variable                                                       #
 #   - univariate_hist for plot histograms of a list of variables_          #
 #   - univariate_histbox for plot histograms and boxplotof a list of       #
@@ -29,34 +30,56 @@
 ###############################Imports#####################################
 import pandas as pd
 import matplotlib.pyplot as plt
 import seaborn as sns
 import os
 import math
 import importlib
-import tabulate
+import numpy as np
+
+from tabulate import tabulate
+from enum import Enum
 from typing import List, Tuple, Literal, Union, Dict
 
 ############################################################################
 
+def build_directory(data_root: str) -> None:
+    """
+    Create the folder structure that this library recommends for storing files.
+
+    Parameters::
+
+        data_root (str): main folder for data.
+
+    Returns::
+    
+        None
+    """
+    data_root_ = data_root.copy()
+    directory_end =['processed/','processed/factorized_mapping/','processed/NonSplit/','processed/SplitData/','processed/SplitData/FeatureSel/','processed/SplitData/NormData/']
+    for d in directory_end:
+        destino_ = data_root_ + d
+        if not os.path.exists(destino_):
+            os.makedirs(destino_)
+                
 
-def get_column_type(series: str) -> Literal['Numeric','Categorical']:
+def get_column_type(series: str) -> Literal['Numerical','Categorical']:
     """
     Determines the column type of a pandas series.
 
     This function takes a pandas series as input and determines whether the data
-    in the series are `numeric` or `categorical`.
+    in the series are `Numerical` or `categorical`.
 
     Parameters::
 
         series (pandas.Series): The pandas series from which the column type will be determined.
 
     Returns::
     
-        str: 'Numeric': If they are numeric.
+        str: 'Numerical': If they are Numerical.
              'Categorical': If they are categorical.
     """
     series_ = series.copy()
     
     if pd.api.types.is_numeric_dtype(series_):
         return 'Numerical'
     else:
@@ -64,24 +87,24 @@
 
 def explore(data_frame: pd.DataFrame) -> Tuple[List[str], List[str]]:
     """
     Explores a pandas DataFrame and prints information about its characteristics.
 
     This function `prints` useful `information` about the provided pandas DataFrame,
     including the number of `rows` and `columns`, the count of `null` and `non-null` values,
-    the `data type` of each column, and whether each column is `categorical` or `numeric`.
+    the `data type` of each column, and whether each column is `categorical` or `numerical`.
 
     Parameters::
 
         data_frame (pandas.DataFrame): The pandas DataFrame to be explored.
 
     Returns:
 
         tuple: A tuple containing two lists. The first list contains the names of categorical columns.
-        The second list contains the names of numeric columns.
+        The second list contains the names of Numerical columns.
     """
     data_frame_ = data_frame.copy()
     
     # Get shape
     num_rows_, num_columns_ = data_frame_.shape
     print('Rows:', num_rows_)
     print('Columns:', num_columns_)
@@ -94,15 +117,15 @@
     }) 
     # Add if a variable is categorical or numerical  
     column_data_['Data Category'] = data_frame_.apply(get_column_type)
     print(tabulate(column_data_, headers='keys', tablefmt='pretty'))
 
     # Get list of categorical and numerical variables_
     categorical_columns_ = list(column_data_[column_data_['Data Category'] == 'Categorical'].index)
-    numeric_columns_ = list(column_data_[column_data_['Data Category'] == 'Numeric'].index)
+    numeric_columns_ = list(column_data_[column_data_['Data Category'] == 'Numerical'].index)
     
     return categorical_columns_, numeric_columns_
 
 def FindDuplicates(data_frame: pd.DataFrame, id_col: str, Drop: bool = False) -> Union[pd.DataFrame, int]:
     """
     Finds and handles duplicates in a pandas DataFrame.
 
@@ -205,27 +228,27 @@
     color_ = color
     kde_ = kde
     
     
     num_plots_ = len(variables_)
     num_rows_ = (num_plots_ - 1) // 3 + 1  # N rows
     
-    fig_, axes_ = plt.subplots(num_rows_, 3, figsize=(15, 5*num_rows_))
-    axes_ = axes_.flatten()  
+    fig_, axs_ = plt.subplots(num_rows_, 3, figsize=(15, 5*num_rows_))
+    axs_ = axs_.flatten()  
 
     for i_, var_ in enumerate(variables_):
-        ax_ = axes_[i_]
+        ax_ = axs_[i_]
         sns.histplot(data_frame_[var_], ax=ax_, kde=kde_, color=color_)
         ax_.set_title(var_)
         ax_.set_xlabel('')
         ax_.set_ylabel('')
         
-    # Remove empty axes_
-    for j_ in range(i_+1, len(axes_)):
-        fig_.delaxes(axes_[j_])
+    # Remove empty axs_
+    for j_ in range(i_+1, len(axs_)):
+        fig_.delaxes(axs_[j_])
     
     plt.tight_layout()
 
 def univariate_histbox(variables: List[str], data_frame: pd.DataFrame, color: str = '#1295a6') -> None:
     """
     Creates a univariate histogram and boxplot for each specified variable in a pandas DataFrame.
 
@@ -261,62 +284,65 @@
     if num_variables_ % 3 != 0:
         for j_ in range(num_variables_ % 3, 3):
             axis_[num_rows_ * 2 - 1, j_].remove()
             axis_[num_rows_ * 2 - 2, j_].remove()
 
     plt.tight_layout()
 
-def multivariate_barplots(df: pd.DataFrame, variable_lists: List[List[str]], y: str = 'count', palette: str = 'Set2') -> None:
+def multivariate_barplots(df: pd.DataFrame, variable_lists: Union[List[str], List[List[str]]], y: str = 'count', palette: str = 'Set2') -> None:
     """
     Creates multivariate bar plots for the specified variables in a pandas DataFrame.
 
     This function creates `multivariate` bar plots for the specified variables in the provided pandas DataFrame.
     The plots are displayed one below the other.
 
     Parameters::
 
         df (pandas.DataFrame): The pandas DataFrame containing the data.
-        variable_lists (List[List[str]]): List of lists containing variable names.
-        Each sublist should contain three elements: the x variable, the y variable, and the hue variable.
+        variable_lists (Union[List[str], List[List[str]]]): List of lists containing variable names,
+        or a single list containing variable names. Each sublist should contain three elements:
+        the x variable, the y variable, and the hue variable.
         y (str, optional): Specifies whether to compute y values as 'count' or 'mean'. Default is 'count'.
         palette (str, optional): Color palette to use in the plots. Default is 'Set2'.
 
     Returns::
 
         None
     """
     df_ = df.copy()
     variable_lists_ = variable_lists.copy()
+    if isinstance(variable_lists_[0], str):
+        variable_lists_ = [variable_lists_]
     y_ = y
     palette_ = palette
         
     num_plots_ = len(variable_lists_)
-    _, axes_ = plt.subplots(num_plots_, 1, figsize=(10, 5 * num_plots_))
+    _, axs_ = plt.subplots(num_plots_, 1, figsize=(10, 5 * num_plots_))
 
-    for i_, variables_ in enumerate(variable_lists_):
+    for i, variables_ in enumerate(variable_lists_):
         if y_ == 'count':
             df_ = df_.groupby(variables_).size().reset_index(name='count')
-
             x_, hue_ = variables_[0], variables_[2]
-            ax_ = axes_[i_]
-            sns.barplot(data=df_, x=x_, y='count', hue=hue_, ax=ax_,palette=palette_,errorbar=None)
+            ax_ = axs_[i] if num_plots_ > 1 else axs_  # Acceder al eje correspondiente
+            sns.barplot(data=df_, x=x_, y='count', hue=hue_, ax=ax_, palette=palette_, errorbar=None)
             ax_.set_xlabel(variables_[0])
             ax_.set_ylabel('Count')
         elif y_ == 'mean':
             try:
                 mean_ = df_.groupby([variables_[0], variables_[2]])[variables_[1]].mean().reset_index()
                 x_, hue_ = variables_[0], variables_[2]
-                ax_ = axes_[i_]
-                sns.barplot(data=mean_, x=x_, y=variables_[1], hue=hue_, ax=ax_,palette=palette_,errorbar=None)
+                ax_ = axs_[i] if num_plots_ > 1 else axs_  # Acceder al eje correspondiente
+                sns.barplot(data=mean_, x=x_, y=variables_[1], hue=hue_, ax=ax_, palette=palette_, errorbar=None)
                 ax_.set_xlabel(variables_[0])
                 ax_.set_ylabel('Mean')
             except:
                 print('y variable is not numerical')
     plt.tight_layout()
 
+
 def factorize_categorical(df: pd.DataFrame, cols_to_factor: List[str]) -> pd.DataFrame:
     """
     Factorizes categorical variables in a pandas DataFrame and saves the mappings to CSV files.
 
     This function `factorizes` the categorical `variables` specified in a pandas DataFrame, assigning a unique integer number to each unique value of the variable.
     Additionally, it saves the mappings between the original values and the factorized values to CSV files in
         >>> ..\\data\\processed\\factorized_mapping\\
@@ -352,37 +378,43 @@
         mappings_df = pd.concat([mappings_df, mappings])
         mappings_df = mappings_df.drop_duplicates(subset=['Original_Value', 'Factorized_Value'])
         
         mappings_df.to_csv(os.path.join(mapping_dir, f'{col_}_mappings.csv'), index=False)
 
     return df_
 
-def correlation_matrix(df: pd.DataFrame, variables_list: List[str]) -> None:
+def correlation_matrix(df: pd.DataFrame, variables_list: List[str], size: Tuple[int,int]=(20,16)) -> None: 
     """
     Creates a correlation matrix for the specified variables in a pandas DataFrame.
 
     This function creates a `correlation` matrix for the specified variables in the provided pandas DataFrame.
     CATEGORICAL variables are FACTORIZED before calculating the correlation.
 
     Parameters::
 
         df (pandas.DataFrame): The pandas DataFrame containing the data.
         variables_list (List[str]): List of variable names for which correlation will be calculated.
+        size (Tupla(int)): Tupla with figure's width and height.
 
     Returns::
 
         pd.DataFrame: The pandas DataFrame with the factorized categorical variables.
+        pd.DataFrame: The pandas DataFrame with the factorized categorical variables and categorical variables.        
     """
     df_ = df.copy()
     variables_list_ = variables_list.copy()
+    size_ = size
     
     fz_df_ = factorize_categorical(df_, variables_list_)
-    sns.heatmap(fz_df_.corr(), annot = True, fmt = ".2f")
+    fz_df = fz_df_.copy()
+    fz_df_numcol_ = fz_df[df_.columns]
+    plt.figure(figsize=size_)
+    sns.heatmap(fz_df_numcol_.corr(), annot = True, fmt = ".2f")
 
-    return fz_df_
+    return fz_df_, fz_df_numcol_
 
 def numerical_box(variables: List[str], data_frame: pd.DataFrame, color: str = '#1295a6') -> None:
     """
     Crea diagramas de caja para variables numéricas en un DataFrame de pandas.
 
     Esta función crea `diagramas` de caja para variables `numéricas` en el DataFrame de pandas proporcionado.
     Los diagramas se muestran en una cuadrícula, con hasta 3 gráficos por fila.
@@ -400,47 +432,54 @@
     variables_ = variables.copy()
     data_frame_ = data_frame.copy()
     color_ = color
     
     num_plots_ = len(variables_)
     num_rows_ = (num_plots_ - 1) // 3 + 1  # N rows
     
-    fig_, axes_ = plt.subplots(num_rows_, 3, figsize=(15, 5*num_rows_))
-    axes_ = axes_.flatten()  
+    fig_, axs_ = plt.subplots(num_rows_, 3, figsize=(15, 5*num_rows_))
+    axs_ = axs_.flatten()  
 
     for i_, var_ in enumerate(variables_):
-        ax_ = axes_[i_]
+        ax_ = axs_[i_]
         sns.boxplot(x=data_frame_[var_], ax=ax_, color=color_)
         ax_.set_title(var_)
         ax_.set_xlabel('')
         ax_.set_ylabel('')
 
-    for j_ in range(i_+1, len(axes_)):
-        fig_.delaxes(axes_[j_])
+    for j_ in range(i_+1, len(axs_)):
+        fig_.delaxes(axs_[j_])
     
     plt.tight_layout()
 
-def outliers_iqr(df: pd.DataFrame, var: str, sigma: float, Do: str = 'nothing') -> Tuple[pd.DataFrame, pd.DataFrame]:
+class Do_enum(Enum):
+    NOTHING = "nothing"
+    DROP = "drop"
+    MODE = "mode"
+    MEAN = "mean"
+    MEDIAN = "median"
+
+def outliers_iqr(df: pd.DataFrame, var: str, sigma: float, Do: Do_enum.NOTHING) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """
     Identifies and handles outliers of a variable in a pandas DataFrame using the interquartile range (IQR).
 
     This function identifies `outliers` of a variable in a pandas DataFrame using the interquartile range (IQR).
     Optionally, outliers can be `removed` or `replaced` with the `mode`, `mean`, or `median` value.
 
     Parameters::
 
         df (pandas.DataFrame): The pandas DataFrame containing the data.
         var (str): Name of the variable for which outliers will be identified.
         sigma (float): Tolerance for the interquartile range (IQR).
-        Do (str, optional): Action to take with the outliers.
-            'nothing' (default): No action is taken.
-            'drop': Outliers are DROPPED.
-            'mode': Outliers are REPLACED by the MODE.
-            'mean': Outliers are REPLACED by the MEAN.
-            'median': Outliers are REPLACED by the MEDIAN.
+        Do (Enum, optional): Action to take with the outliers.
+            'NOTHING' (default): No action is taken.
+            'DROP': Outliers are DROPPED.
+            'MODE': Outliers are REPLACED by the MODE.
+            'MEAN': Outliers are REPLACED by the MEAN.
+            'MEDIAN': Outliers are REPLACED by the MEDIAN.
 
     Returns::
 
         tuple: A tuple containing two DataFrames.
                The first DataFrame contains the identified outliers.
                The second DataFrame contains the original data with outliers treated according to the option specified in 'Do'.
     """    
@@ -455,29 +494,28 @@
     upper_l_ = descr_["75%"] + sigma_*iqr_
     lower_l_ = descr_["25%"] - sigma_*iqr_
     print(upper_l_, lower_l_)
 
     outliers_ = df_[(df_[var_] >= upper_l_) | (df_[var_] < lower_l_)]
     num_outliers_ = outliers_.shape[0]     
 
-    if Do_ == 'nothing':
+    if Do_ == Do_enum.NOTHING:
         print(str(num_outliers_)+' outliers have been found')
-        pass
     else:
-        if Do_ != 'drop':
-            if Do_ == 'mode':
-                replacer_ = df_[var_].mode()                    
-            elif Do_ == 'mean':
+        if Do_ != Do_enum.DROP:
+            if Do_ == Do_enum.MODE:
+                replacer_ = df_[var_].mode()[0]                    
+            elif Do_ == Do_enum.MEAN:
                 replacer_ = df_[var_].mean()
-            elif Do_ == 'median':
+            elif Do_ == Do_enum.MEDIAN:
                 replacer_ = df_[var_].median()
 
-            replace_func_ = lambda x_: x_ if lower_l_ <= x_ < upper_l_ else replacer_
+            replace_func_ = lambda x: x if lower_l_ <= x < upper_l_ else replacer_
             df_[var_] = df_[var_].apply(replace_func_)        
-            print(str(num_outliers_) + ' outliers have been treated by replacing them with the ' + Do_)
+            print(str(num_outliers_) + ' outliers have been treated by replacing them with the ' + Do_.value)
         else:
             df_ = df_[var_].between(lower_l_, upper_l_)
             print(str(num_outliers_)+' outliers have been treated by dropping')
     return outliers_, df_
     
 def splitter(origin_root: str, predictors: List[str], target: str) -> Dict[str, pd.DataFrame]:
     """
@@ -570,27 +608,27 @@
     
     for df_root_ in csv_files_:
         if '_X' in str(df_root_):
             df_ = pd.read_csv(df_root_)
 
             scaler_.fit(df_)
             scaler_df_ = scaler_.transform(df_)
-            scaler_df_ = pd.DataFrame(scaler_df_, index = df_.index_, columns = predictors_)
+            scaler_df_ = pd.DataFrame(scaler_df_, index = df_.index, columns = predictors_)
             
             name_ = (df_root_.split('/'))[-1].split('.')[0]       
             destino_ =origin_root_+'NormData/'
             if not os.path.exists(destino_): os.makedirs(destino_)
 
             scaler_df_.to_csv(destino_ + name_ + '_norm.csv', index=False)
             normalized_datasets_[name_ + '_norm'] = scaler_df_
     
     return normalized_datasets_
 
 
-def feature_sel(X_train: pd.DataFrame, y_train: pd.Series, k: int, file_name: str, method: str = 'SelectKBest', test: str = 'mutual_info_classif') -> pd.DataFrame:
+def feature_sel(X_train: pd.DataFrame, y_train: pd.Series, k: int, file_name: str, method: str = 'SelectKBest', test: str = 'mutual_info_classif') -> tuple[pd.DataFrame, list[str]]:
     """
     Performs feature selection and saves the selected dataset to a CSV file in
     >>> \\data\\processed\\SplitData\\FeatureSel\\
 
     This function performs feature selection using a specified `method` and a `feature selection test`,
     and saves the selected dataset to a CSV file.
 
@@ -602,14 +640,15 @@
         file_name (str): Name of the resulting CSV file.
         method (str, optional): Feature selection method. Default is 'SelectKBest'.
         test (str, optional): Feature selection test. Default is 'mutual_info_classif'.
 
     Returns::
 
         pd.DataFrame: Selected dataset.
+        list(Str): Selected columns.
     """
     X_train_ = X_train.copy()
     y_train_ = y_train.copy()
     k_ = k
     file_name_ = file_name
     method_ = method
     test_ = test
@@ -618,13 +657,13 @@
     method_ = getattr(module_, method_)
     test_ = getattr(module_, test_)
         
     selection_model_ = method_(test_, k = k_)
     selection_model_.fit(X_train_, y_train_)
     ix_ = selection_model_.get_support()
     X_train_sel_ = pd.DataFrame(selection_model_.transform(X_train_), columns = X_train_.columns.values[ix_])
+    keys_sel_ = list(X_train_sel_.keys())
 
     if not os.path.exists('../data/processed/SplitData/FeatureSel/'):
             os.makedirs('../data/processed/SplitData/FeatureSel/')
     X_train_sel_.to_csv('../data/processed/SplitData/FeatureSel/'+str(file_name_)+'_FeatureSel.csv', index=False)
-
-    return X_train_sel_
+    return X_train_sel_ , keys_sel_
```

