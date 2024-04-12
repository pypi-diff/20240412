# Comparing `tmp/pynyairbnb-0.2.0.tar.gz` & `tmp/pynyairbnb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynyairbnb-0.2.0.tar", max compression
+gzip compressed data, was "pynyairbnb-0.3.0.tar", max compression
```

## Comparing `pynyairbnb-0.2.0.tar` & `pynyairbnb-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1075 2024-04-12 04:29:43.062995 pynyairbnb-0.2.0/LICENSE
--rw-r--r--   0        0        0     3977 2024-04-12 04:29:43.062995 pynyairbnb-0.2.0/README.md
--rw-r--r--   0        0        0     1102 2024-04-12 04:29:52.834974 pynyairbnb-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      112 2024-04-12 04:29:43.158995 pynyairbnb-0.2.0/src/pynyairbnb/__init__.py
--rw-r--r--   0        0        0     8478 2024-04-12 04:29:43.158995 pynyairbnb-0.2.0/src/pynyairbnb/data_preprocessing.py
--rw-r--r--   0        0        0    10902 2024-04-12 04:29:43.158995 pynyairbnb-0.2.0/src/pynyairbnb/plotting.py
--rw-r--r--   0        0        0     8344 2024-04-12 04:29:43.158995 pynyairbnb-0.2.0/src/pynyairbnb/pynyairbnb.py
--rw-r--r--   0        0        0     4734 1970-01-01 00:00:00.000000 pynyairbnb-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-12 05:18:12.492941 pynyairbnb-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2176 2024-04-12 05:18:12.492941 pynyairbnb-0.3.0/README.md
+-rw-r--r--   0        0        0     1102 2024-04-12 05:18:22.460981 pynyairbnb-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      112 2024-04-12 05:18:12.592942 pynyairbnb-0.3.0/src/pynyairbnb/__init__.py
+-rw-r--r--   0        0        0     8591 2024-04-12 05:18:12.592942 pynyairbnb-0.3.0/src/pynyairbnb/data_preprocessing.py
+-rw-r--r--   0        0        0    10902 2024-04-12 05:18:12.592942 pynyairbnb-0.3.0/src/pynyairbnb/plotting.py
+-rw-r--r--   0        0        0     8344 2024-04-12 05:18:12.592942 pynyairbnb-0.3.0/src/pynyairbnb/pynyairbnb.py
+-rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 pynyairbnb-0.3.0/PKG-INFO
```

### Comparing `pynyairbnb-0.2.0/LICENSE` & `pynyairbnb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynyairbnb-0.2.0/pyproject.toml` & `pynyairbnb-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynyairbnb"
-version = "0.2.0"
+version = "0.3.0"
 description = "A package for DSCI 310 Group's Airbnb Analysis."
 authors = ["DSCI 310 Group 9"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `pynyairbnb-0.2.0/src/pynyairbnb/data_preprocessing.py` & `pynyairbnb-0.3.0/src/pynyairbnb/data_preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,36 +196,38 @@
         bins=[-float('inf'), 50, 100, 150, 200, 250, 300, 350, float('inf')],
         labels=['0-50', '50-100', '100-150', '150-200', '200-250', '250-300', '300-350', '350+'],
         include_lowest=True
     )
     data['price_category'] = categories
     return data
 
-def data_preprocessing(input_path, out_dir):
+def data_preprocessing(input_path, out_dir, raw_dir="./data/raw"):
     """Main function orchestrating the data cleaning and preprocessing.
 
     Reads data from a specified input path, performs cleaning operations including filling missing values and converting data types, splits the data into training and testing datasets, adds a 'price_category' column based on predefined price ranges, and saves the processed datasets to the specified output directory.
 
     Parameters
     ----------
     input_path : str
         Path to input data file.
     out_dir : str
         Path to directory where processed files will be saved.
+    raw_dir : str
+        Path to directory where raw data file will be saved.
 
     Returns
     -------
     None
 
     Examples
     --------
-    >>> data_preprocessing('data/raw/airbnb_data_2023.csv', 'data/processed')
+    >>> data_preprocessing('data/raw/airbnb_data_2023.csv', 'data/processed', 'data/raw')
     # Reads the raw data, processes it, and saves the processed data into the 'data/processed' directory.
     """
     create_dir_if_not_exists(out_dir)
 
-    data = read_data(input_path, out_dir)
+    data = read_data(input_path, raw_dir)
     data = convert_missing_values(data)
     train_df, test_df = split_data(data)
     train_df = add_price_category(train_df)
     test_df = add_price_category(test_df)
     save_dataframes(out_dir, train_df, test_df)
```

### Comparing `pynyairbnb-0.2.0/src/pynyairbnb/plotting.py` & `pynyairbnb-0.3.0/src/pynyairbnb/plotting.py`

 * *Files identical despite different names*

### Comparing `pynyairbnb-0.2.0/src/pynyairbnb/pynyairbnb.py` & `pynyairbnb-0.3.0/src/pynyairbnb/pynyairbnb.py`

 * *Files identical despite different names*

