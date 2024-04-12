# Comparing `tmp/pynyairbnb-0.1.0.tar.gz` & `tmp/pynyairbnb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynyairbnb-0.1.0.tar", max compression
+gzip compressed data, was "pynyairbnb-0.2.0.tar", max compression
```

## Comparing `pynyairbnb-0.1.0.tar` & `pynyairbnb-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1097 2024-04-07 22:02:51.053074 pynyairbnb-0.1.0/LICENSE
--rw-r--r--   0        0        0     1117 2024-04-11 22:01:14.392602 pynyairbnb-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2227 2024-04-11 23:00:51.766046 pynyairbnb-0.1.0/README.md
--rw-r--r--   0        0        0      114 2024-04-07 22:02:51.217230 pynyairbnb-0.1.0/src/pynyairbnb/__init__.py
--rw-r--r--   0        0        0     8934 2024-04-11 17:35:53.404398 pynyairbnb-0.1.0/src/pynyairbnb/data_preprocessing.py
--rw-r--r--   0        0        0    11152 2024-04-11 17:35:53.405592 pynyairbnb-0.1.0/src/pynyairbnb/plotting.py
--rw-r--r--   0        0        0     7946 2024-04-11 17:14:13.720721 pynyairbnb-0.1.0/src/pynyairbnb/pynyairbnb.py
--rw-r--r--   0        0        0     2931 1970-01-01 00:00:00.000000 pynyairbnb-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-12 04:29:43.062995 pynyairbnb-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3977 2024-04-12 04:29:43.062995 pynyairbnb-0.2.0/README.md
+-rw-r--r--   0        0        0     1102 2024-04-12 04:29:52.834974 pynyairbnb-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      112 2024-04-12 04:29:43.158995 pynyairbnb-0.2.0/src/pynyairbnb/__init__.py
+-rw-r--r--   0        0        0     8478 2024-04-12 04:29:43.158995 pynyairbnb-0.2.0/src/pynyairbnb/data_preprocessing.py
+-rw-r--r--   0        0        0    10902 2024-04-12 04:29:43.158995 pynyairbnb-0.2.0/src/pynyairbnb/plotting.py
+-rw-r--r--   0        0        0     8344 2024-04-12 04:29:43.158995 pynyairbnb-0.2.0/src/pynyairbnb/pynyairbnb.py
+-rw-r--r--   0        0        0     4734 1970-01-01 00:00:00.000000 pynyairbnb-0.2.0/PKG-INFO
```

### Comparing `pynyairbnb-0.1.0/LICENSE` & `pynyairbnb-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2024, DSCI 310 Group 9
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2024, DSCI 310 Group 9
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `pynyairbnb-0.1.0/src/pynyairbnb/data_preprocessing.py` & `pynyairbnb-0.2.0/src/pynyairbnb/data_preprocessing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,234 +1,231 @@
-#import click
-import pandas as pd
-from sklearn.model_selection import train_test_split
-import os
-
-def create_dir_if_not_exists(directory):
-    """Create the directory if it doesn't exist.
-
-    Checks if a directory exists at the specified path, and if not, it creates the directory along with any necessary parent directories.
-
-    Parameters
-    ----------
-    directory : str
-        The path of the directory to create.
-
-    Returns
-    -------
-    None
-
-    Examples
-    --------
-    >>> create_dir_if_not_exists('./data/processed')
-    # This will create the 'processed' directory within the 'data' directory if it does not already exist.
-    """
-
-    if not os.path.exists(directory):
-        os.makedirs(directory)
-
-def read_data(data_url, out_dir):
-    """Loads and saves the data for this project from a specified URL or file path.
-
-    The function reads a CSV file from the given URL or file path, then saves it to the specified output directory after creating the directory if it does not exist.
-
-    Parameters
-    ----------
-    data_url : str
-        URL or path to the dataset file.
-    out_dir : str
-        Output directory to save the downloaded data.
-
-    Returns
-    -------
-    pd.DataFrame
-        The DataFrame of the raw data.
-
-    Examples
-    --------
-    >>> read_data('https://example.com/airbnb_data.csv', './data/raw')
-    # Downloads the dataset from the specified URL and saves it as 'airbnb_data_2023.csv' in './data/raw'.
-    """
-    
-    create_dir_if_not_exists(out_dir)
-
-    data = pd.read_csv(data_url)
-    data.to_csv(os.path.join(out_dir, 'airbnb_data_2023.csv'), index=False)
-    return data
-
-def convert_missing_values(data):
-    """Fill missing values in specific columns and convert certain columns to string type.
-
-    Specifically, fills missing values in the 'reviews_per_month' column with 0 and converts 'id' and 'host_id' columns to strings.
-
-    Parameters
-    ----------
-    data : pd.DataFrame
-        The pandas DataFrame containing the data.
-
-    Returns
-    -------
-    pd.DataFrame
-        The DataFrame after filling missing values and converting column types.
-
-    Examples
-    --------
-    >>> df = pd.DataFrame({
-    ...     'id': [1, 2, None],
-    ...     'host_id': [None, 2, 3],
-    ...     'reviews_per_month': [1.5, None, 2.0]
-    ... })
-    >>> convert_missing_values(df)
-        id host_id  reviews_per_month
-    0   1    None                1.5
-    1   2       2                0.0
-    2  NaN       3                2.0
-    """
-    
-    if data is None or data.empty:
-        pass
-    else:
-        data['id'] = data['id'].astype(str)
-        data['host_id'] = data['host_id'].astype(str)
-        data['reviews_per_month'] = data['reviews_per_month'].fillna(0)
-    return data
-
-def split_data(data):
-    """Split the dataset into training and testing subsets.
-
-    The function splits the data into training and testing datasets with a default size of 20% for testing.
-
-    Parameters
-    ----------
-    data : pd.DataFrame
-        The DataFrame to be split.
-
-    Returns
-    -------
-    tuple
-        A tuple containing the training and testing DataFrames.
-
-    Examples
-    --------
-    >>> df = pd.DataFrame(np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]), columns=['a', 'b', 'c'])
-    >>> train, test = split_data(df)
-    >>> print(train.shape, test.shape)
-    # Output example: (2, 3) (1, 3), depending on the random split.
-    """
-    return train_test_split(data, test_size=0.2, shuffle=True)
-
-def save_dataframes(out_dir, train_df, test_df):
-    """Save the processed DataFrames to specified directory.
-
-    Saves the training and testing DataFrames to CSV files in the given directory. Additionally, splits the features and labels ('price_category') and saves them separately.
-
-    Parameters
-    ----------
-    out_dir : str
-        The output directory to save the dataframes.
-    train_df : pd.DataFrame
-        The training dataset DataFrame.
-    test_df : pd.DataFrame
-        The testing dataset DataFrame.
-
-    Returns
-    -------
-    None
-
-    Examples
-    --------
-    >>> train_df = pd.DataFrame({'price': [100, 150], 'price_category': ['100-150', '150-200']})
-    >>> test_df = pd.DataFrame({'price': [200], 'price_category': ['200-250']})
-    >>> save_dataframes('./data/processed', train_df, test_df)
-    # Saves 'train_df.csv', 'test_df.csv', 'X_train.csv', 'y_train.csv', 'X_test.csv', and 'y_test.csv' in './data/processed'.
-    """
-    train_df.to_csv(os.path.join(out_dir, 'train_df.csv'), index=False)
-    test_df.to_csv(os.path.join(out_dir, 'test_df.csv'), index=False)
-
-    X_train = train_df.drop(['price'], axis=1)
-    y_train = train_df['price_category']
-    X_test = test_df.drop(['price'], axis=1)
-    y_test = test_df['price_category']
-
-    X_train.to_csv(os.path.join(out_dir, 'X_train.csv'), index=False)
-    y_train.to_csv(os.path.join(out_dir, 'y_train.csv'), index=False)
-    X_test.to_csv(os.path.join(out_dir, 'X_test.csv'), index=False)
-    y_test.to_csv(os.path.join(out_dir, 'y_test.csv'), index=False)
-
-def add_price_category(data):
-    """
-    Adds a 'price_category' column to the DataFrame based on predefined price ranges, facilitating easier analysis of data by price segments.
-    
-    This function categorizes each entry into one of seven price ranges, thereby enabling quick insights into the distribution of prices. The categories are defined as follows: 
-    '0-50', '50-100', '100-150', '150-200', '200-250', '250-300', '300-350'. 
-    Each range captures the minimum inclusive and maximum exclusive price points for that category, except for the '0-50' range, which is inclusive of 50, and '300-350', which is inclusive of 350.
-    
-    Parameters:
-    -----------
-    - data (pd.DataFrame): A DataFrame containing at least a 'price' column with numeric values. The 'price' values should be integers or floats.
-    
-    Returns:
-    --------
-    - pd.DataFrame: The modified DataFrame with an additional column 'price_category'. This column contains categorical labels indicating the price range for each row.
-    
-    Examples:
-    ---------
-    >>> import pandas as pd
-    >>> data = pd.DataFrame({"price": [25, 75, 125, 175, 225, 275, 325, 375]})
-    >>> add_price_category(data)
-        price price_category
-    0     25           0-50
-    1     75         50-100
-    2    125       100-150
-    3    175       150-200
-    4    225       200-250
-    5    275       250-300
-    6    325       300-350
-    7    375           350+
-    
-    Notes:
-    ------
-    - The function directly modifies the input DataFrame by adding a new column 'price_category'.
-    - Prices are categorized based on predefined bins, which are set to be inclusive of the lower bound and exclusive of the upper bound for all categories except for the first ('0-50') and the last ('350+'), which includes all prices above 350.
-    - Negative price values are treated as errors in input data and will be categorized into the lowest bin ('0-50'), implying the need for data cleaning if such values exist.
-    """
-    categories = pd.cut(
-        data['price'],
-        bins=[-float('inf'), 50, 100, 150, 200, 250, 300, 350, float('inf')],
-        labels=['0-50', '50-100', '100-150', '150-200', '200-250', '250-300', '300-350', '350+'],
-        include_lowest=True
-    )
-    data['price_category'] = categories
-    return data
-
-# @click.command()
-# @click.option('--input_path', type=str, default="data/raw/airbnb_data_2023.csv", help='Path to input data')
-# @click.option('--out_dir', type=str, default="data/cleaned", help='Path to write the file')
-def data_preprocessing(input_path, out_dir):
-    """Main function orchestrating the data cleaning and preprocessing.
-
-    Reads data from a specified input path, performs cleaning operations including filling missing values and converting data types, splits the data into training and testing datasets, adds a 'price_category' column based on predefined price ranges, and saves the processed datasets to the specified output directory.
-
-    Parameters
-    ----------
-    input_path : str
-        Path to input data file.
-    out_dir : str
-        Path to directory where processed files will be saved.
-
-    Returns
-    -------
-    None
-
-    Examples
-    --------
-    >>> data_preprocessing('data/raw/airbnb_data_2023.csv', 'data/processed')
-    # Reads the raw data, processes it, and saves the processed data into the 'data/processed' directory.
-    """
-    create_dir_if_not_exists(out_dir)
-
-    data = read_data(input_path, out_dir)
-    data = convert_missing_values(data)
-    train_df, test_df = split_data(data)
-    train_df = add_price_category(train_df)
-    test_df = add_price_category(test_df)
+#import click
+import pandas as pd
+from sklearn.model_selection import train_test_split
+import os
+
+def create_dir_if_not_exists(directory):
+    """Create the directory if it doesn't exist.
+
+    Checks if a directory exists at the specified path, and if not, it creates the directory along with any necessary parent directories.
+
+    Parameters
+    ----------
+    directory : str
+        The path of the directory to create.
+
+    Returns
+    -------
+    None
+
+    Examples
+    --------
+    >>> create_dir_if_not_exists('./data/processed')
+    # This will create the 'processed' directory within the 'data' directory if it does not already exist.
+    """
+
+    if not os.path.exists(directory):
+        os.makedirs(directory)
+
+def read_data(data_url, out_dir):
+    """Loads and saves the data for this project from a specified URL or file path.
+
+    The function reads a CSV file from the given URL or file path, then saves it to the specified output directory after creating the directory if it does not exist.
+
+    Parameters
+    ----------
+    data_url : str
+        URL or path to the dataset file.
+    out_dir : str
+        Output directory to save the downloaded data.
+
+    Returns
+    -------
+    pd.DataFrame
+        The DataFrame of the raw data.
+
+    Examples
+    --------
+    >>> read_data('https://example.com/airbnb_data.csv', './data/raw')
+    # Downloads the dataset from the specified URL and saves it as 'airbnb_data_2023.csv' in './data/raw'.
+    """
+    
+    create_dir_if_not_exists(out_dir)
+
+    data = pd.read_csv(data_url)
+    data.to_csv(os.path.join(out_dir, 'airbnb_data_2023.csv'), index=False)
+    return data
+
+def convert_missing_values(data):
+    """Fill missing values in specific columns and convert certain columns to string type.
+
+    Specifically, fills missing values in the 'reviews_per_month' column with 0 and converts 'id' and 'host_id' columns to strings.
+
+    Parameters
+    ----------
+    data : pd.DataFrame
+        The pandas DataFrame containing the data.
+
+    Returns
+    -------
+    pd.DataFrame
+        The DataFrame after filling missing values and converting column types.
+
+    Examples
+    --------
+    >>> df = pd.DataFrame({
+    ...     'id': [1, 2, None],
+    ...     'host_id': [None, 2, 3],
+    ...     'reviews_per_month': [1.5, None, 2.0]
+    ... })
+    >>> convert_missing_values(df)
+        id host_id  reviews_per_month
+    0   1    None                1.5
+    1   2       2                0.0
+    2  NaN       3                2.0
+    """
+    
+    if data is None or data.empty:
+        pass
+    else:
+        data['id'] = data['id'].astype(str)
+        data['host_id'] = data['host_id'].astype(str)
+        data['reviews_per_month'] = data['reviews_per_month'].fillna(0)
+    return data
+
+def split_data(data):
+    """Split the dataset into training and testing subsets.
+
+    The function splits the data into training and testing datasets with a default size of 20% for testing.
+
+    Parameters
+    ----------
+    data : pd.DataFrame
+        The DataFrame to be split.
+
+    Returns
+    -------
+    tuple
+        A tuple containing the training and testing DataFrames.
+
+    Examples
+    --------
+    >>> df = pd.DataFrame(np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]), columns=['a', 'b', 'c'])
+    >>> train, test = split_data(df)
+    >>> print(train.shape, test.shape)
+    # Output example: (2, 3) (1, 3), depending on the random split.
+    """
+    return train_test_split(data, test_size=0.2, shuffle=True)
+
+def save_dataframes(out_dir, train_df, test_df):
+    """Save the processed DataFrames to specified directory.
+
+    Saves the training and testing DataFrames to CSV files in the given directory. Additionally, splits the features and labels ('price_category') and saves them separately.
+
+    Parameters
+    ----------
+    out_dir : str
+        The output directory to save the dataframes.
+    train_df : pd.DataFrame
+        The training dataset DataFrame.
+    test_df : pd.DataFrame
+        The testing dataset DataFrame.
+
+    Returns
+    -------
+    None
+
+    Examples
+    --------
+    >>> train_df = pd.DataFrame({'price': [100, 150], 'price_category': ['100-150', '150-200']})
+    >>> test_df = pd.DataFrame({'price': [200], 'price_category': ['200-250']})
+    >>> save_dataframes('./data/processed', train_df, test_df)
+    # Saves 'train_df.csv', 'test_df.csv', 'X_train.csv', 'y_train.csv', 'X_test.csv', and 'y_test.csv' in './data/processed'.
+    """
+    train_df.to_csv(os.path.join(out_dir, 'train_df.csv'), index=False)
+    test_df.to_csv(os.path.join(out_dir, 'test_df.csv'), index=False)
+
+    X_train = train_df.drop(['price'], axis=1)
+    y_train = train_df['price_category']
+    X_test = test_df.drop(['price'], axis=1)
+    y_test = test_df['price_category']
+
+    X_train.to_csv(os.path.join(out_dir, 'X_train.csv'), index=False)
+    y_train.to_csv(os.path.join(out_dir, 'y_train.csv'), index=False)
+    X_test.to_csv(os.path.join(out_dir, 'X_test.csv'), index=False)
+    y_test.to_csv(os.path.join(out_dir, 'y_test.csv'), index=False)
+
+def add_price_category(data):
+    """
+    Adds a 'price_category' column to the DataFrame based on predefined price ranges, facilitating easier analysis of data by price segments.
+    
+    This function categorizes each entry into one of seven price ranges, thereby enabling quick insights into the distribution of prices. The categories are defined as follows: 
+    '0-50', '50-100', '100-150', '150-200', '200-250', '250-300', '300-350'. 
+    Each range captures the minimum inclusive and maximum exclusive price points for that category, except for the '0-50' range, which is inclusive of 50, and '300-350', which is inclusive of 350.
+    
+    Parameters:
+    -----------
+    - data (pd.DataFrame): A DataFrame containing at least a 'price' column with numeric values. The 'price' values should be integers or floats.
+    
+    Returns:
+    --------
+    - pd.DataFrame: The modified DataFrame with an additional column 'price_category'. This column contains categorical labels indicating the price range for each row.
+    
+    Examples:
+    ---------
+    >>> import pandas as pd
+    >>> data = pd.DataFrame({"price": [25, 75, 125, 175, 225, 275, 325, 375]})
+    >>> add_price_category(data)
+        price price_category
+    0     25           0-50
+    1     75         50-100
+    2    125       100-150
+    3    175       150-200
+    4    225       200-250
+    5    275       250-300
+    6    325       300-350
+    7    375           350+
+    
+    Notes:
+    ------
+    - The function directly modifies the input DataFrame by adding a new column 'price_category'.
+    - Prices are categorized based on predefined bins, which are set to be inclusive of the lower bound and exclusive of the upper bound for all categories except for the first ('0-50') and the last ('350+'), which includes all prices above 350.
+    - Negative price values are treated as errors in input data and will be categorized into the lowest bin ('0-50'), implying the need for data cleaning if such values exist.
+    """
+    categories = pd.cut(
+        data['price'],
+        bins=[-float('inf'), 50, 100, 150, 200, 250, 300, 350, float('inf')],
+        labels=['0-50', '50-100', '100-150', '150-200', '200-250', '250-300', '300-350', '350+'],
+        include_lowest=True
+    )
+    data['price_category'] = categories
+    return data
+
+def data_preprocessing(input_path, out_dir):
+    """Main function orchestrating the data cleaning and preprocessing.
+
+    Reads data from a specified input path, performs cleaning operations including filling missing values and converting data types, splits the data into training and testing datasets, adds a 'price_category' column based on predefined price ranges, and saves the processed datasets to the specified output directory.
+
+    Parameters
+    ----------
+    input_path : str
+        Path to input data file.
+    out_dir : str
+        Path to directory where processed files will be saved.
+
+    Returns
+    -------
+    None
+
+    Examples
+    --------
+    >>> data_preprocessing('data/raw/airbnb_data_2023.csv', 'data/processed')
+    # Reads the raw data, processes it, and saves the processed data into the 'data/processed' directory.
+    """
+    create_dir_if_not_exists(out_dir)
+
+    data = read_data(input_path, out_dir)
+    data = convert_missing_values(data)
+    train_df, test_df = split_data(data)
+    train_df = add_price_category(train_df)
+    test_df = add_price_category(test_df)
     save_dataframes(out_dir, train_df, test_df)
```

### Comparing `pynyairbnb-0.1.0/src/pynyairbnb/plotting.py` & `pynyairbnb-0.2.0/src/pynyairbnb/plotting.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-import pandas as pd
-import matplotlib.pyplot as plt
-import seaborn as sns
-import numpy as np
-import matplotlib.image as mpimg
-import os
-#import sys
-#sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
-from pynyairbnb.data_preprocessing import create_dir_if_not_exists
-
-def rank_correlations(corr_matrix):
-    """Rank the correlations present in the given correlation matrix, excluding self-correlations.
-
-    This function takes a correlation matrix, flattens it to include only unique pairings of variables, and then sorts these pairs by the absolute value of their correlation in descending order. Finally, it filters out repeated correlations to provide a concise list of the top correlations.
-
-    Parameters
-    ----------
-    corr_matrix : pd.DataFrame
-        A DataFrame representing a correlation matrix where both rows and columns are variables.
-
-    Returns
-    -------
-    pd.DataFrame
-        A DataFrame containing the top 10 unique variable pairings sorted by their absolute correlation value, excluding self-correlations.
-
-    Examples
-    --------
-    >>> import pandas as pd
-    >>> data = pd.DataFrame({"A": [1, 2, 3], "B": [3, 2, 1], "C": [1, 3, 2]})
-    >>> corr_matrix = data.corr()
-    >>> print(rank_correlations(corr_matrix))
-    """
-    # flattening matrix
-    flattened_matrix = corr_matrix.stack().reset_index()
-    #renaming columns
-    flattened_matrix.columns = ['Variable_1', 'Variable_2', 'Correlation']
-    # removing duplicate variable names
-    flattened_matrix = flattened_matrix.loc[flattened_matrix['Variable_1'] != flattened_matrix['Variable_2']]
-    corr_column = flattened_matrix['Correlation']
-    flattened_matrix = flattened_matrix.iloc[abs(corr_column).argsort()[::-1]]
-    flattened_matrix = flattened_matrix.loc[flattened_matrix['Correlation'].duplicated()]
-    #print(f'Top 10 Variable Correlations: \n{flattened_matrix.head(10)}')
-    return flattened_matrix.head(10)
-
-def sns_plotting(plot_type, data, x='number_of_reviews', y='price', figlength=14, figheight=7):
-    """
-    Generates a plot from the seaborn library with the provided plot type, the x-variable, and the y-variable from provided data.
-
-    This function does so by using matplotlib pyplot subplots and setting the figsize to the provided figlength and figheight.
-    
-    Parameters:
-    -----------
-    - plot_type (str): Type of plot to generate - one of 'scatterplot', 'boxplot', 'histplot' or 'heatmap'.
-    - data (pd.DataFrame): A DataFrame containing at least 2 columns.
-    - x (str): x-variable present in data. (Not applicable for 'heatmap')
-    - y (str): y-variable present in data. (Not applicable for 'heatmap')
-    - figlength (int): The length of the plotting area in inches.
-    - figheight (int): The height of the plotting area in inches.
-    
-    Returns:
-    --------
-    - matplotlib.figure.Figure: The matplotlib figure containing the plot.
-    
-    Examples:
-    ---------
-    >>> import pandas as pd
-    >>> import numpy as np
-    >>> import seaborn as sns
-    >>> import matplotlib.pyplot as plt
-    >>> data = pd.DataFrame({"price": [25, 75, 125, 175, 225, 275, 325, 375],
-                            "number_of_reviews": [2, 0, 1, 15, 22, 7, 5, 3]})
-    >>> figure = sns_plotting('scatterplot', data, x='number_of_reviews', y='price', figlength=12, figheight=6)
-    >>> figure.tight_layout
-    
-    Notes:
-    ------
-    - The function directly modifies the input DataFrame to what is necessary for the plot.
-    """
-    if plot_type == "heatmap":
-
-        corr_matrix = data.select_dtypes(include=["int64", "float64"]).corr()
-        train_corr = corr_matrix.corr(method = 'pearson')
-        mask = np.zeros_like(train_corr, dtype=bool)
-        mask[np.triu_indices_from(mask)] = True
-
-        fig, ax = plt.subplots(figsize=(7, 5))
-
-        sns.heatmap(train_corr, mask=mask, vmin=-1, vmax=1, center=0, linewidths=.5, cmap="vlag")
-        fig.suptitle('Correlation Heat Map of Numeric Predictors', fontsize=12)
-
-    elif plot_type == "scatterplot":
-
-        fig, ax = plt.subplots(nrows=1,ncols=2,figsize=(figlength, figheight))
-
-        sns.scatterplot(data=data, x=x, y=y, hue='room_type', ax=ax[0])
-        if x == 'number_of_reviews':
-            ax[0].set_title("Price vs Number of Reviews Coloured by Room Type")
-            ax[0].set(xlabel="# of Reviews", ylabel="Price")
-        elif x == 'reviews_per_month':
-            ax[0].set_title("Price vs Reviews Per Month Coloured by Room Type")
-            ax[0].set(xlabel="# of Reviews Per Month", ylabel="Price")
-
-        sns.scatterplot(data=data, x=x, y=y, hue='room_type', ax=ax[1])
-        ax[1].set_ylim(-100, 5000)
-        if x == 'number_of_reviews':
-            ax[1].set_title("Price (< 5000) vs Number of Reviews For Clarity")
-            ax[1].set(xlabel="# of Reviews", ylabel="Price")
-        elif x == 'reviews_per_month':
-            ax[1].set_title("Price (< 5000) vs Reviews Per Month For Clarity")
-            ax[1].set(xlabel="# of Reviews Per Month", ylabel="Price")
-
-    elif plot_type == "boxplot":
-
-        fig, ax = plt.subplots(nrows=1,ncols=2,figsize=(figlength, figheight))
-        
-        sns.boxplot(data=data, x=x, y=np.log(data[y]), ax=ax[0])
-        if x == 'neighbourhood_group':
-            ax[0].set_title("Log Price by Neighbourhood Group")
-            ax[0].set(xlabel="Neighbourhood Group", ylabel="Log Price")
-        elif x == 'room_type':
-            ax[0].set_title("Log Price by Room Type")
-            ax[0].set(xlabel="Room Type", ylabel="Log Price")
-
-        sns.boxplot(data=data, x=x, y=np.log(data[y]), showfliers=False, ax=ax[1])
-        if x == 'neighbourhood_group':
-            ax[1].set_title("Price by Neighbourhood Group (Outliers Removed)")
-            ax[1].set(xlabel="Neighbourhood Group", ylabel="Price")
-        elif x == 'room_type':
-            ax[1].set_title("Price by Room Type (Outliers Removed)")
-            ax[1].set(xlabel="Room Type", ylabel="Price")
-    
-    elif plot_type == "histplot":
-        Q1 = data[y].quantile(0.25)
-        Q3 = data[y].quantile(0.75)
-        IQR = Q3 - Q1
-        lower_bound = Q1 - 1.5 * IQR
-        upper_bound = Q3 + 1.5 * IQR
-        filtered_train_df = data[(data[y] >= lower_bound) & (data[y] <= upper_bound)]
-
-        fig, ax = plt.subplots(figsize=(figlength, figheight))
-
-        sns.histplot(data=filtered_train_df, x=y)
-        fig.suptitle('Price Distribution without Outliers')
-        plt.xlabel('Price')
-        plt.ylabel('Frequency')
-
-    else: raise Exception("plot_type must be one of scatterplot, boxplot, histplot or heatmap")
-    
-    return fig
-
-def plot_pynyairbnb(input_file, viz_out_dir, tbl_out_dir):
-    """Creates and saves visualizations and tables for pynyairbnb data analysis.
-
-    This function orchestrates the creation of various plots and tables as part of the data analysis process for the pynyairbnb project. It reads the dataset from the given input file, generates specified visualizations (e.g., heatmaps, scatter plots, box plots), and then saves these figures to the specified output directory for visualizations. It also ranks correlations among variables and saves this information as a table in the specified output directory for tables.
-
-    Parameters
-    ----------
-    input_file : str
-        Path to the dataset CSV file.
-    viz_out_dir : str
-        Output directory to save the generated figures.
-    tbl_out_dir : str
-        Output directory to save the generated tables.
-
-    Returns
-    -------
-    None
-
-    Examples
-    --------
-    >>> plot_pynyairbnb('data/raw/airbnb_data_nyc.csv', 'data/figures', 'data/tables')
-    
-    Notes
-    -----
-    - This function assumes that the input file is a CSV containing the required columns for the specified visualizations and tables.
-    - The directories specified by `viz_out_dir` and `tbl_out_dir` will be created if they do not already exist, using the `create_dir_if_not_exists` function.
-    """
-    
-    create_dir_if_not_exists(viz_out_dir)
-    create_dir_if_not_exists(tbl_out_dir)
-    
-    data = pd.read_csv(input_file)
-
-    # Fig. 1 Correlation Heat Map of Numerical Predictors
-
-    fig1 = sns_plotting('heatmap', data, 7, 5)
-    fig1.tight_layout()
-    fig1.savefig(os.path.join(viz_out_dir, 'corr_heat_map.jpg'))
-
-    # Fig. 2 Map with Distribution of Listings by Location and Price
-
-    fig2, ax2 = plt.subplots(nrows=1,ncols=2,figsize=(14, 6))
-
-    vmin, vmax = 0, 400 # Setting color limits to more typical range, e.g., 0 to 400
-
-    ax2[0].scatter(data['longitude'], data['latitude'], c=data['price'], #cmap='viridis',
-                s=10, alpha=0.6, vmin=vmin, vmax=vmax)
-    fig2.colorbar(plt.scatter(data['longitude'], data['latitude'], c=data['price'], #cmap='viridis',
-                s=10, alpha=0.6, vmin=vmin, vmax=vmax), label='Price', ax=ax2[0])
-    ax2[0].grid(True, which='both', linestyle='--', linewidth=0.5)
-    ax2[0].set_title('Distribution of Listings by Location and Price')
-    ax2[0].set(xlabel='Longitude', ylabel='Latitude')
-
-    img_path = 'src/images/New_York_City_Map.jpg'
-    try:
-        img = mpimg.imread(img_path)
-
-        ax2[1].imshow(img)
-        ax2[1].set_title('Map of New York City')
-        ax2[1].axis("off")
-
-        fig2.savefig(os.path.join(viz_out_dir, 'listing_locations.jpg'))
-    
-    except FileNotFoundError:
-        print("Image file not found. Please check the file path.")
-
-    # Fig. 3 Price vs Number of Reviews Coloured by Room Type Scatterplot
-    
-    fig3 = sns_plotting('scatterplot', data, x='number_of_reviews', y='price', figlength=20, figheight=6)
-    fig3.tight_layout
-    fig3.savefig(os.path.join(viz_out_dir, 'price_vs_reviews.jpg'))
-
-    # Fig. 4 Price vs Reviews Per Month Coloured by Room Type Scatterplot
-
-    fig4 = sns_plotting('scatterplot', data, x='reviews_per_month', y='price', figlength=20, figheight=6)
-    fig4.tight_layout
-    fig4.savefig(os.path.join(viz_out_dir, 'price_vs_reviews_per_month.jpg'))
-    
-    # Fig. 5 Log Price and Price by Neighbourhood Group Boxplot
-
-    fig5 = sns_plotting('boxplot', data, x='neighbourhood_group', y='price', figlength=12, figheight=6)
-    fig5.tight_layout
-    fig5.savefig(os.path.join(viz_out_dir, 'neighbourhood_groups_boxplots.jpg'))
-
-    # Fig. 6 Log Price and Price by Room Type Boxplot
-
-    fig6 = sns_plotting('boxplot', data, x='room_type', y='price', figlength=12, figheight=6)
-    fig6.tight_layout
-    fig6.savefig(os.path.join(viz_out_dir, 'room_type_boxplots.jpg'))
-
-    # Fig. 7 Price Histogram (Outliers Removed)
-
-    fig7 = sns_plotting('histplot', data, y='price', figlength=7, figheight=5)
-    fig7.tight_layout
-    fig7.savefig(os.path.join(viz_out_dir, 'price_histogram.jpg'))
-    
-    # Table 1: Correlations Ranked
-
-    corr_matrix = data.select_dtypes(include=["int64", "float64"]).corr()
-    table1 = rank_correlations(corr_matrix)
+import pandas as pd
+import matplotlib.pyplot as plt
+import seaborn as sns
+import numpy as np
+import matplotlib.image as mpimg
+import os
+#import sys
+#sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+from pynyairbnb.data_preprocessing import create_dir_if_not_exists
+
+def rank_correlations(corr_matrix):
+    """Rank the correlations present in the given correlation matrix, excluding self-correlations.
+
+    This function takes a correlation matrix, flattens it to include only unique pairings of variables, and then sorts these pairs by the absolute value of their correlation in descending order. Finally, it filters out repeated correlations to provide a concise list of the top correlations.
+
+    Parameters
+    ----------
+    corr_matrix : pd.DataFrame
+        A DataFrame representing a correlation matrix where both rows and columns are variables.
+
+    Returns
+    -------
+    pd.DataFrame
+        A DataFrame containing the top 10 unique variable pairings sorted by their absolute correlation value, excluding self-correlations.
+
+    Examples
+    --------
+    >>> import pandas as pd
+    >>> data = pd.DataFrame({"A": [1, 2, 3], "B": [3, 2, 1], "C": [1, 3, 2]})
+    >>> corr_matrix = data.corr()
+    >>> print(rank_correlations(corr_matrix))
+    """
+    # flattening matrix
+    flattened_matrix = corr_matrix.stack().reset_index()
+    #renaming columns
+    flattened_matrix.columns = ['Variable_1', 'Variable_2', 'Correlation']
+    # removing duplicate variable names
+    flattened_matrix = flattened_matrix.loc[flattened_matrix['Variable_1'] != flattened_matrix['Variable_2']]
+    corr_column = flattened_matrix['Correlation']
+    flattened_matrix = flattened_matrix.iloc[abs(corr_column).argsort()[::-1]]
+    flattened_matrix = flattened_matrix.loc[flattened_matrix['Correlation'].duplicated()]
+    #print(f'Top 10 Variable Correlations: \n{flattened_matrix.head(10)}')
+    return flattened_matrix.head(10)
+
+def sns_plotting(plot_type, data, x='number_of_reviews', y='price', figlength=14, figheight=7):
+    """
+    Generates a plot from the seaborn library with the provided plot type, the x-variable, and the y-variable from provided data.
+
+    This function does so by using matplotlib pyplot subplots and setting the figsize to the provided figlength and figheight.
+    
+    Parameters:
+    -----------
+    - plot_type (str): Type of plot to generate - one of 'scatterplot', 'boxplot', 'histplot' or 'heatmap'.
+    - data (pd.DataFrame): A DataFrame containing at least 2 columns.
+    - x (str): x-variable present in data. (Not applicable for 'heatmap')
+    - y (str): y-variable present in data. (Not applicable for 'heatmap')
+    - figlength (int): The length of the plotting area in inches.
+    - figheight (int): The height of the plotting area in inches.
+    
+    Returns:
+    --------
+    - matplotlib.figure.Figure: The matplotlib figure containing the plot.
+    
+    Examples:
+    ---------
+    >>> import pandas as pd
+    >>> import numpy as np
+    >>> import seaborn as sns
+    >>> import matplotlib.pyplot as plt
+    >>> data = pd.DataFrame({"price": [25, 75, 125, 175, 225, 275, 325, 375],
+                            "number_of_reviews": [2, 0, 1, 15, 22, 7, 5, 3]})
+    >>> figure = sns_plotting('scatterplot', data, x='number_of_reviews', y='price', figlength=12, figheight=6)
+    >>> figure.tight_layout
+    
+    Notes:
+    ------
+    - The function directly modifies the input DataFrame to what is necessary for the plot.
+    """
+    if plot_type == "heatmap":
+
+        corr_matrix = data.select_dtypes(include=["int64", "float64"]).corr()
+        train_corr = corr_matrix.corr(method = 'pearson')
+        mask = np.zeros_like(train_corr, dtype=bool)
+        mask[np.triu_indices_from(mask)] = True
+
+        fig, ax = plt.subplots(figsize=(7, 5))
+
+        sns.heatmap(train_corr, mask=mask, vmin=-1, vmax=1, center=0, linewidths=.5, cmap="vlag")
+        fig.suptitle('Correlation Heat Map of Numeric Predictors', fontsize=12)
+
+    elif plot_type == "scatterplot":
+
+        fig, ax = plt.subplots(nrows=1,ncols=2,figsize=(figlength, figheight))
+
+        sns.scatterplot(data=data, x=x, y=y, hue='room_type', ax=ax[0])
+        if x == 'number_of_reviews':
+            ax[0].set_title("Price vs Number of Reviews Coloured by Room Type")
+            ax[0].set(xlabel="# of Reviews", ylabel="Price")
+        elif x == 'reviews_per_month':
+            ax[0].set_title("Price vs Reviews Per Month Coloured by Room Type")
+            ax[0].set(xlabel="# of Reviews Per Month", ylabel="Price")
+
+        sns.scatterplot(data=data, x=x, y=y, hue='room_type', ax=ax[1])
+        ax[1].set_ylim(-100, 5000)
+        if x == 'number_of_reviews':
+            ax[1].set_title("Price (< 5000) vs Number of Reviews For Clarity")
+            ax[1].set(xlabel="# of Reviews", ylabel="Price")
+        elif x == 'reviews_per_month':
+            ax[1].set_title("Price (< 5000) vs Reviews Per Month For Clarity")
+            ax[1].set(xlabel="# of Reviews Per Month", ylabel="Price")
+
+    elif plot_type == "boxplot":
+
+        fig, ax = plt.subplots(nrows=1,ncols=2,figsize=(figlength, figheight))
+        
+        sns.boxplot(data=data, x=x, y=np.log(data[y]), ax=ax[0])
+        if x == 'neighbourhood_group':
+            ax[0].set_title("Log Price by Neighbourhood Group")
+            ax[0].set(xlabel="Neighbourhood Group", ylabel="Log Price")
+        elif x == 'room_type':
+            ax[0].set_title("Log Price by Room Type")
+            ax[0].set(xlabel="Room Type", ylabel="Log Price")
+
+        sns.boxplot(data=data, x=x, y=np.log(data[y]), showfliers=False, ax=ax[1])
+        if x == 'neighbourhood_group':
+            ax[1].set_title("Price by Neighbourhood Group (Outliers Removed)")
+            ax[1].set(xlabel="Neighbourhood Group", ylabel="Price")
+        elif x == 'room_type':
+            ax[1].set_title("Price by Room Type (Outliers Removed)")
+            ax[1].set(xlabel="Room Type", ylabel="Price")
+    
+    elif plot_type == "histplot":
+        Q1 = data[y].quantile(0.25)
+        Q3 = data[y].quantile(0.75)
+        IQR = Q3 - Q1
+        lower_bound = Q1 - 1.5 * IQR
+        upper_bound = Q3 + 1.5 * IQR
+        filtered_train_df = data[(data[y] >= lower_bound) & (data[y] <= upper_bound)]
+
+        fig, ax = plt.subplots(figsize=(figlength, figheight))
+
+        sns.histplot(data=filtered_train_df, x=y)
+        fig.suptitle('Price Distribution without Outliers')
+        plt.xlabel('Price')
+        plt.ylabel('Frequency')
+
+    else: raise Exception("plot_type must be one of scatterplot, boxplot, histplot or heatmap")
+    
+    return fig
+
+def plot_pynyairbnb(input_file, viz_out_dir, tbl_out_dir):
+    """Creates and saves visualizations and tables for pynyairbnb data analysis.
+
+    This function orchestrates the creation of various plots and tables as part of the data analysis process for the pynyairbnb project. It reads the dataset from the given input file, generates specified visualizations (e.g., heatmaps, scatter plots, box plots), and then saves these figures to the specified output directory for visualizations. It also ranks correlations among variables and saves this information as a table in the specified output directory for tables.
+
+    Parameters
+    ----------
+    input_file : str
+        Path to the dataset CSV file.
+    viz_out_dir : str
+        Output directory to save the generated figures.
+    tbl_out_dir : str
+        Output directory to save the generated tables.
+
+    Returns
+    -------
+    None
+
+    Examples
+    --------
+    >>> plot_pynyairbnb('data/raw/airbnb_data_nyc.csv', 'data/figures', 'data/tables')
+    
+    Notes
+    -----
+    - This function assumes that the input file is a CSV containing the required columns for the specified visualizations and tables.
+    - The directories specified by `viz_out_dir` and `tbl_out_dir` will be created if they do not already exist, using the `create_dir_if_not_exists` function.
+    """
+    
+    create_dir_if_not_exists(viz_out_dir)
+    create_dir_if_not_exists(tbl_out_dir)
+    
+    data = pd.read_csv(input_file)
+
+    # Fig. 1 Correlation Heat Map of Numerical Predictors
+
+    fig1 = sns_plotting('heatmap', data, 7, 5)
+    fig1.tight_layout()
+    fig1.savefig(os.path.join(viz_out_dir, 'corr_heat_map.jpg'))
+
+    # Fig. 2 Map with Distribution of Listings by Location and Price
+
+    fig2, ax2 = plt.subplots(nrows=1,ncols=2,figsize=(14, 6))
+
+    vmin, vmax = 0, 400 # Setting color limits to more typical range, e.g., 0 to 400
+
+    ax2[0].scatter(data['longitude'], data['latitude'], c=data['price'], #cmap='viridis',
+                s=10, alpha=0.6, vmin=vmin, vmax=vmax)
+    fig2.colorbar(plt.scatter(data['longitude'], data['latitude'], c=data['price'], #cmap='viridis',
+                s=10, alpha=0.6, vmin=vmin, vmax=vmax), label='Price', ax=ax2[0])
+    ax2[0].grid(True, which='both', linestyle='--', linewidth=0.5)
+    ax2[0].set_title('Distribution of Listings by Location and Price')
+    ax2[0].set(xlabel='Longitude', ylabel='Latitude')
+
+    img_path = 'src/images/New_York_City_Map.jpg'
+    try:
+        img = mpimg.imread(img_path)
+
+        ax2[1].imshow(img)
+        ax2[1].set_title('Map of New York City')
+        ax2[1].axis("off")
+
+        fig2.savefig(os.path.join(viz_out_dir, 'listing_locations.jpg'))
+    
+    except FileNotFoundError:
+        print("Image file not found. Please check the file path.")
+
+    # Fig. 3 Price vs Number of Reviews Coloured by Room Type Scatterplot
+    
+    fig3 = sns_plotting('scatterplot', data, x='number_of_reviews', y='price', figlength=20, figheight=6)
+    fig3.tight_layout
+    fig3.savefig(os.path.join(viz_out_dir, 'price_vs_reviews.jpg'))
+
+    # Fig. 4 Price vs Reviews Per Month Coloured by Room Type Scatterplot
+
+    fig4 = sns_plotting('scatterplot', data, x='reviews_per_month', y='price', figlength=20, figheight=6)
+    fig4.tight_layout
+    fig4.savefig(os.path.join(viz_out_dir, 'price_vs_reviews_per_month.jpg'))
+    
+    # Fig. 5 Log Price and Price by Neighbourhood Group Boxplot
+
+    fig5 = sns_plotting('boxplot', data, x='neighbourhood_group', y='price', figlength=12, figheight=6)
+    fig5.tight_layout
+    fig5.savefig(os.path.join(viz_out_dir, 'neighbourhood_groups_boxplots.jpg'))
+
+    # Fig. 6 Log Price and Price by Room Type Boxplot
+
+    fig6 = sns_plotting('boxplot', data, x='room_type', y='price', figlength=12, figheight=6)
+    fig6.tight_layout
+    fig6.savefig(os.path.join(viz_out_dir, 'room_type_boxplots.jpg'))
+
+    # Fig. 7 Price Histogram (Outliers Removed)
+
+    fig7 = sns_plotting('histplot', data, y='price', figlength=7, figheight=5)
+    fig7.tight_layout
+    fig7.savefig(os.path.join(viz_out_dir, 'price_histogram.jpg'))
+    
+    # Table 1: Correlations Ranked
+
+    corr_matrix = data.select_dtypes(include=["int64", "float64"]).corr()
+    table1 = rank_correlations(corr_matrix)
     table1.to_csv(os.path.join(tbl_out_dir, 'correlations_ranked.csv'), index=False)
```

### Comparing `pynyairbnb-0.1.0/src/pynyairbnb/pynyairbnb.py` & `pynyairbnb-0.2.0/src/pynyairbnb/pynyairbnb.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,164 +1,179 @@
-import pandas as pd
-import os
-import sys
-from sklearn.pipeline import make_pipeline
-from sklearn.dummy import DummyClassifier
-from sklearn.metrics import classification_report
-from sklearn.compose import make_column_transformer
-from sklearn.preprocessing import OrdinalEncoder
-from sklearn.preprocessing import OneHotEncoder, StandardScaler
-from sklearn.feature_extraction.text import CountVectorizer
-from sklearn.neighbors import KNeighborsClassifier
-from sklearn.model_selection import RandomizedSearchCV
-from scipy.stats import randint
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
-# from src.function_build_preprocessor import build_preprocessor
-from pynyairbnb.data_preprocessing import create_dir_if_not_exists
-
-def build_preprocessor(numerical_data, text_data, categorical_data):
-    """_summary_
-    Builds a preprocessor for numerical, text, and categorical data with the following transformations: Standard scaler, One hot encoding, and count Vectorizer
-    Args:
-        numerical_data (_type_): numeric data
-        text_data (_type_): text data 
-        categorical_data (_type_): cateogorical data 
-
-    Returns:
-        _type_: _description_
-    """
-    # Numerical Transformer
-    numerical_transformer = StandardScaler()
-
-    # Categorical Transformer
-    categorical_transformer = OneHotEncoder(handle_unknown='ignore')
-
-    # Text Data Transformer
-    text_transformer = CountVectorizer()
-    
-    # Making Our Preprocessor
-    preprocessor = make_column_transformer(
-        (numerical_transformer, numerical_data),
-        (categorical_transformer, categorical_data),
-        (text_transformer, text_data),
-        remainder='drop'
-    )
-    
-    return preprocessor
-
-def build_clf_model(model, preprocessor, tbl_out_dir, X_train, y_train, X_test, y_test, replacement_dict, clf_report_file_name):
-    """_summary_
-    Builds a classification model with X_train, y_train, X_test, y_test and saves the classification report to clf_saved_fp 
-    Args:
-        model (_type_): classification model specified 
-        preprocessor (_type_): preprocessor with data transformations
-        tbl_out_dir (_type_): path to save our classification report tables
-        X_train (_type_): training data input features
-        y_train (_type_): training data target variable
-        X_test (_type_): testing data input features
-        y_test (_type_): testing data target variable
-        replacement_dict (_type_): Dictionary with proper Formatting for classification report 
-        clf_saved_fp (_type_): File name to save classification report
-    
-    Returns:
-        Model that has been trained on our training data
-        Classification report that is saved to Csv file (output)
-    """
-    model_pipe = make_pipeline(preprocessor, model)
-    model = model_pipe.fit(X_train, y_train)
-    predictions = model.predict(X_test)
-    
-    clf_report = classification_report(y_test, predictions, output_dict=True)
-    #clf_report = dict((replacement_dict[key], value) for (key, value) in clf_report.items())
-    clf_report = {replacement_dict.get(key, key): value for (key, value) in clf_report.items()}
-    clf_report = pd.DataFrame(clf_report).transpose()
-    
-    # Saving table
-    clf_report.to_csv(os.path.join(tbl_out_dir, clf_report_file_name))
-    
-    return model 
-
-    
-def knn_param_optimization(knn_model, tbl_out_dir, X_train, y_train, X_test, y_test,replacement_dict):
-    # KNN Hyperparameter Optimization
-    param_dist = {
-        'kneighborsclassifier__n_neighbors': randint(1, 30),
-        'kneighborsclassifier__weights': ['uniform', 'distance'],
-        'kneighborsclassifier__p': [1, 2]  
-    }
-
-    try:
-        rand_search = RandomizedSearchCV(knn_model, param_distributions=param_dist, n_iter=5,  
-                                        n_jobs=1,  
-                                        scoring='accuracy', cv=3, 
-                                        verbose=1, random_state=42, pre_dispatch='2*n_jobs')  
-    except Exception as e:
-        print(f"Error with rand_search: {e}")
-        rand_search = RandomizedSearchCV(knn_model, param_distributions=param_dist, n_iter=5,
-                                        scoring='accuracy', cv=3, verbose=1, random_state=42)
-
-    rand_search.fit(X_train, y_train)
-
-    # Classification Report After Hyperparameter Optimization
-    rand_search_predictions = rand_search.predict(X_test)
-    hyperparam_clf_report = classification_report(y_test, rand_search_predictions, output_dict=True)
-    hyperparam_clf_report = dict((replacement_dict[key], value) for (key, value) in hyperparam_clf_report.items())
-    hyperparam_clf_report = pd.DataFrame(hyperparam_clf_report).transpose()
-
-    # Saving table
-    hyperparam_clf_report.to_csv(os.path.join(tbl_out_dir, 'hyperparam_classification_report.csv'))
-
-
-def nyairbnb_analysis(input_dir, tbl_out_dir):
-    """Creates model and saves tables to src/tables."""
-    
-    create_dir_if_not_exists(tbl_out_dir)
-    
-    replacement_dict = {'0.0':'0-50', '1.0':'50-100', '2.0':'100-150', '3.0':'150-200', '4.0':'200-250','5.0':'250-300',
-                '6.0':'300-350', '7.0':'350+', 'accuracy':'accuracy', 'macro avg':'macro avg', 'weighted avg':'weighted avg'}
-    
-    X_train = pd.read_csv(os.path.join(input_dir, 'X_train.csv'))
-    y_train = pd.read_csv(os.path.join(input_dir, 'y_train.csv'))
-    X_test = pd.read_csv(os.path.join(input_dir, 'X_test.csv'))
-    y_test = pd.read_csv(os.path.join(input_dir, 'y_test.csv'))
-
-    # numeric data
-    numerical_data = ['latitude', 'longitude', 'minimum_nights', 'number_of_reviews', 'reviews_per_month',
-                    'calculated_host_listings_count', 'availability_365', 'number_of_reviews_ltm']
-
-    # text data
-    text_data = "name"
-
-    # Categorical Data
-    categorical_data = ['neighbourhood_group', 'neighbourhood', 'room_type']
-
-    # Encoding our y_train & y_test with ordinal encoder
-    categories = [['0-50', '50-100', '100-150', '150-200', '200-250', '250-300', '300-350', '350+']]
-    ordinal_encoder = OrdinalEncoder(categories=categories)
-    y_train_encoded = ordinal_encoder.fit_transform(y_train.values.reshape(-1, 1)).ravel()
-    y_test_encoded = ordinal_encoder.transform(y_test.values.reshape(-1, 1)).ravel()
-    
-    # Making Our Preprocessor
-    preprocessor = build_preprocessor(numerical_data=numerical_data, text_data=text_data, categorical_data=categorical_data)
-    
-
-    # Implementing a Dummy Regressor model as a baseline to assess our model with and saving results to csv file
-    try:
-        build_clf_model(model=DummyClassifier(), preprocessor=preprocessor, tbl_out_dir=tbl_out_dir, X_train=X_train,
-                    y_train=y_train_encoded, X_test=X_test, y_test=y_test_encoded, replacement_dict=replacement_dict, clf_report_file_name='dummy_classification_report.csv')
-    except Exception as e:
-        print(f"Error creating dummy model: {e}")
-
-    # implementing knn model and saving results to a csv file
-    try:
-        knn_model = build_clf_model(model = KNeighborsClassifier(), preprocessor=preprocessor, tbl_out_dir=tbl_out_dir, X_train=X_train, 
-                    y_train=y_train_encoded, X_test=X_test, y_test=y_test_encoded,replacement_dict=replacement_dict, clf_report_file_name='knn_classification_report.csv')
-    except Exception as e:
-        print(f"Error creating KNN model: {e}")
-
-
-    # performing hyperparameter optimization with our knn model and saving classification report results to csv
-    try:
-        knn_param_optimization(knn_model=knn_model, tbl_out_dir=tbl_out_dir, X_train=X_train, y_train=y_train_encoded, X_test=X_test, 
-                            y_test=y_test_encoded,replacement_dict=replacement_dict)
-    except Exception as e: 
+import pandas as pd
+import os
+import sys
+from sklearn.pipeline import make_pipeline
+from sklearn.dummy import DummyClassifier
+from sklearn.metrics import classification_report
+from sklearn.compose import make_column_transformer
+from sklearn.preprocessing import OrdinalEncoder
+from sklearn.preprocessing import OneHotEncoder, StandardScaler
+from sklearn.feature_extraction.text import CountVectorizer
+from sklearn.neighbors import KNeighborsClassifier
+from sklearn.model_selection import RandomizedSearchCV
+from scipy.stats import randint
+#sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+# from src.function_build_preprocessor import build_preprocessor
+from pynyairbnb.data_preprocessing import create_dir_if_not_exists
+
+def build_preprocessor(numerical_data, text_data, categorical_data):
+    """_summary_
+    Builds a preprocessor for numerical, text, and categorical data with the following transformations: Standard scaler, One hot encoding, and count Vectorizer
+    Args:
+        numerical_data (_type_): numeric data
+        text_data (_type_): text data 
+        categorical_data (_type_): cateogorical data 
+
+    Returns:
+        _type_: _description_
+    """
+    # Numerical Transformer
+    numerical_transformer = StandardScaler()
+
+    # Categorical Transformer
+    categorical_transformer = OneHotEncoder(handle_unknown='ignore')
+
+    # Text Data Transformer
+    text_transformer = CountVectorizer()
+    
+    # Making Our Preprocessor
+    preprocessor = make_column_transformer(
+        (numerical_transformer, numerical_data),
+        (categorical_transformer, categorical_data),
+        (text_transformer, text_data),
+        remainder='drop'
+    )
+    
+    return preprocessor
+
+def build_clf_model(model, preprocessor, tbl_out_dir, X_train, y_train, X_test, y_test, replacement_dict, clf_report_file_name):
+    """_summary_
+    Builds a classification model with X_train, y_train, X_test, y_test and saves the classification report to clf_saved_fp 
+    Args:
+        model (_type_): classification model specified 
+        preprocessor (_type_): preprocessor with data transformations
+        tbl_out_dir (_type_): path to save our classification report tables
+        X_train (_type_): training data input features
+        y_train (_type_): training data target variable
+        X_test (_type_): testing data input features
+        y_test (_type_): testing data target variable
+        replacement_dict (_type_): Dictionary with proper Formatting for classification report 
+        clf_saved_fp (_type_): File name to save classification report
+    
+    Returns:
+        Model that has been trained on our training data
+        Classification report that is saved to Csv file (output)
+    """
+    model_pipe = make_pipeline(preprocessor, model)
+    model = model_pipe.fit(X_train, y_train)
+    predictions = model.predict(X_test)
+    
+    clf_report = classification_report(y_test, predictions, output_dict=True)
+    clf_report = {replacement_dict.get(key, key): value for (key, value) in clf_report.items()}
+    clf_report = pd.DataFrame(clf_report).transpose()
+    
+    # Saving table
+    clf_report.to_csv(os.path.join(tbl_out_dir, clf_report_file_name))
+    
+    return model 
+
+    
+def knn_param_optimization(knn_model, tbl_out_dir, X_train, y_train, X_test, y_test,replacement_dict):
+    """_summary_
+    Performs Hyperparameter optimization for KNN model 
+    Args:
+        knn_model (_type_): KNN Model Built with Sklearn Library 
+        tbl_out_dir (_type_): Data Input
+        X_train (_type_): training data input features
+        y_train (_type_): training data target variable
+        X_test (_type_): testing data input features
+        y_test (_type_): testing data target variable
+        replacement_dict (_type_): Dictionary with proper Formatting for classification report 
+        output_file_name (str): The name to save the output as, will be a .csv file 
+        
+        
+    Output:
+    Saves output of model to csv file defined in output_file_name
+    """
+    # KNN Hyperparameter Optimization
+    param_dist = {
+        'n_neighbors': randint(1, 30),
+        'weights': ['uniform', 'distance'],
+        'p': [1, 2]  
+    }
+
+    try:
+        rand_search = RandomizedSearchCV(knn_model, param_distributions=param_dist, n_iter=5,  
+                                        n_jobs=1,  
+                                        scoring='accuracy', cv=3, 
+                                        verbose=1, random_state=42, pre_dispatch='2*n_jobs')  
+    except Exception as e:
+        print(f"Error with rand_search: {e}")
+        rand_search = RandomizedSearchCV(knn_model, param_distributions=param_dist, n_iter=5,
+                                        scoring='accuracy', cv=3, verbose=1, random_state=42)
+
+    rand_search.fit(X_train, y_train)
+
+    # Classification Report After Hyperparameter Optimization
+    rand_search_predictions = rand_search.predict(X_test)
+    hyperparam_clf_report = classification_report(y_test, rand_search_predictions, output_dict=True)
+    hyperparam_clf_report = dict((replacement_dict[key], value) for (key, value) in hyperparam_clf_report.items() if key in replacement_dict)
+    hyperparam_clf_report = pd.DataFrame(hyperparam_clf_report).transpose()
+
+    # Saving table
+    hyperparam_clf_report.to_csv(os.path.join(tbl_out_dir, 'hyperparam_classification_report.csv'))
+
+
+def nyairbnb_analysis(input_dir, tbl_out_dir):
+    """Creates model and saves tables to src/tables."""
+    
+    create_dir_if_not_exists(tbl_out_dir)
+    
+    replacement_dict = {'0.0':'0-50', '1.0':'50-100', '2.0':'100-150', '3.0':'150-200', '4.0':'200-250','5.0':'250-300',
+                '6.0':'300-350', '7.0':'350+', 'accuracy':'accuracy', 'macro avg':'macro avg', 'weighted avg':'weighted avg'}
+    
+    X_train = pd.read_csv(os.path.join(input_dir, 'X_train.csv'))
+    y_train = pd.read_csv(os.path.join(input_dir, 'y_train.csv'))
+    X_test = pd.read_csv(os.path.join(input_dir, 'X_test.csv'))
+    y_test = pd.read_csv(os.path.join(input_dir, 'y_test.csv'))
+
+    # numeric data
+    numerical_data = ['latitude', 'longitude', 'minimum_nights', 'number_of_reviews', 'reviews_per_month',
+                    'calculated_host_listings_count', 'availability_365', 'number_of_reviews_ltm']
+
+    # text data
+    text_data = "name"
+
+    # Categorical Data
+    categorical_data = ['neighbourhood_group', 'neighbourhood', 'room_type']
+
+    # Encoding our y_train & y_test with ordinal encoder
+    categories = [['0-50', '50-100', '100-150', '150-200', '200-250', '250-300', '300-350', '350+']]
+    ordinal_encoder = OrdinalEncoder(categories=categories)
+    y_train_encoded = ordinal_encoder.fit_transform(y_train.values.reshape(-1, 1)).ravel()
+    y_test_encoded = ordinal_encoder.transform(y_test.values.reshape(-1, 1)).ravel()
+    
+    # Making Our Preprocessor
+    preprocessor = build_preprocessor(numerical_data=numerical_data, text_data=text_data, categorical_data=categorical_data)
+    
+
+    # Implementing a Dummy Regressor model as a baseline to assess our model with and saving results to csv file
+    try:
+        build_clf_model(model=DummyClassifier(), preprocessor=preprocessor, tbl_out_dir=tbl_out_dir, X_train=X_train,
+                    y_train=y_train_encoded, X_test=X_test, y_test=y_test_encoded, replacement_dict=replacement_dict, clf_report_file_name='dummy_classification_report.csv')
+    except Exception as e:
+        print(f"Error creating dummy model: {e}")
+
+    # implementing knn model and saving results to a csv file
+    try:
+        knn_model = build_clf_model(model = KNeighborsClassifier(), preprocessor=preprocessor, tbl_out_dir=tbl_out_dir, X_train=X_train, 
+                    y_train=y_train_encoded, X_test=X_test, y_test=y_test_encoded,replacement_dict=replacement_dict, clf_report_file_name='knn_classification_report.csv')
+    except Exception as e:
+        print(f"Error creating KNN model: {e}")
+
+
+    # performing hyperparameter optimization with our knn model and saving classification report results to csv
+    try:
+        knn_param_optimization(knn_model=knn_model, tbl_out_dir=tbl_out_dir, X_train=X_train, y_train=y_train_encoded, X_test=X_test, 
+                            y_test=y_test_encoded,replacement_dict=replacement_dict)
+    except Exception as e: 
         print(f'Error performing hyperparameter optimization: {e}')
```

