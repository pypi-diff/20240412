# Comparing `tmp/canalyst_candas-0.0.8.tar.gz` & `tmp/canalyst_candas-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canalyst_candas-0.0.8.tar", last modified: Mon Sep 20 19:06:48 2021, max compression
+gzip compressed data, was "canalyst_candas-0.0.9.tar", last modified: Tue Oct  5 12:21:04 2021, max compression
```

## Comparing `canalyst_candas-0.0.8.tar` & `canalyst_candas-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-20 19:06:48.885781 canalyst_candas-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)       57 2021-09-20 19:06:30.000000 canalyst_candas-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4964 2021-09-20 19:06:48.885781 canalyst_candas-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4353 2021-09-20 19:06:30.000000 canalyst_candas-0.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      104 2021-09-20 19:06:30.000000 canalyst_candas-0.0.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      219 2021-09-20 19:06:48.886781 canalyst_candas-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1715 2021-09-20 19:06:30.000000 canalyst_candas-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-20 19:06:48.877781 canalyst_candas-0.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-20 19:06:48.882781 canalyst_candas-0.0.8/src/canalyst_candas/
--rw-rw-rw-   0 root         (0) root         (0)      236 2021-09-20 19:06:30.000000 canalyst_candas-0.0.8/src/canalyst_candas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    68476 2021-09-20 19:06:30.000000 canalyst_candas-0.0.8/src/canalyst_candas/candas.py
--rw-rw-rw-   0 root         (0) root         (0)     7585 2021-09-20 19:06:30.000000 canalyst_candas-0.0.8/src/canalyst_candas/candas_datareader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-20 19:06:48.885781 canalyst_candas-0.0.8/src/canalyst_candas/configuration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-09-20 19:06:30.000000 canalyst_candas-0.0.8/src/canalyst_candas/configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8319 2021-09-20 19:06:30.000000 canalyst_candas-0.0.8/src/canalyst_candas/configuration/config.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2021-09-20 19:06:30.000000 canalyst_candas-0.0.8/src/canalyst_candas/configuration/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      962 2021-09-20 19:06:30.000000 canalyst_candas-0.0.8/src/canalyst_candas/connection.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2021-09-20 19:06:30.000000 canalyst_candas-0.0.8/src/canalyst_candas/settings.py
--rw-rw-rw-   0 root         (0) root         (0)    41103 2021-09-20 19:06:30.000000 canalyst_candas-0.0.8/src/canalyst_candas/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       48 2021-09-20 19:06:41.000000 canalyst_candas-0.0.8/src/canalyst_candas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-20 19:06:48.884781 canalyst_candas-0.0.8/src/canalyst_candas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4964 2021-09-20 19:06:48.000000 canalyst_candas-0.0.8/src/canalyst_candas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      632 2021-09-20 19:06:48.000000 canalyst_candas-0.0.8/src/canalyst_candas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-20 19:06:48.000000 canalyst_candas-0.0.8/src/canalyst_candas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      332 2021-09-20 19:06:48.000000 canalyst_candas-0.0.8/src/canalyst_candas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2021-09-20 19:06:48.000000 canalyst_candas-0.0.8/src/canalyst_candas.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-05 12:21:04.330901 canalyst_candas-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2021-10-05 12:20:46.000000 canalyst_candas-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4863 2021-10-05 12:21:04.330901 canalyst_candas-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4353 2021-10-05 12:20:46.000000 canalyst_candas-0.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      104 2021-10-05 12:20:46.000000 canalyst_candas-0.0.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      219 2021-10-05 12:21:04.331901 canalyst_candas-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2021-10-05 12:20:46.000000 canalyst_candas-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-05 12:21:04.323900 canalyst_candas-0.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-05 12:21:04.328900 canalyst_candas-0.0.9/src/canalyst_candas/
+-rw-rw-rw-   0 root         (0) root         (0)      236 2021-10-05 12:20:46.000000 canalyst_candas-0.0.9/src/canalyst_candas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    77950 2021-10-05 12:20:46.000000 canalyst_candas-0.0.9/src/canalyst_candas/candas.py
+-rw-rw-rw-   0 root         (0) root         (0)     7585 2021-10-05 12:20:46.000000 canalyst_candas-0.0.9/src/canalyst_candas/candas_datareader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-05 12:21:04.330901 canalyst_candas-0.0.9/src/canalyst_candas/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-10-05 12:20:46.000000 canalyst_candas-0.0.9/src/canalyst_candas/configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8319 2021-10-05 12:20:46.000000 canalyst_candas-0.0.9/src/canalyst_candas/configuration/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2021-10-05 12:20:46.000000 canalyst_candas-0.0.9/src/canalyst_candas/configuration/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      970 2021-10-05 12:20:46.000000 canalyst_candas-0.0.9/src/canalyst_candas/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1725 2021-10-05 12:20:46.000000 canalyst_candas-0.0.9/src/canalyst_candas/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    40905 2021-10-05 12:20:46.000000 canalyst_candas-0.0.9/src/canalyst_candas/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       48 2021-10-05 12:20:56.000000 canalyst_candas-0.0.9/src/canalyst_candas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-05 12:21:04.329901 canalyst_candas-0.0.9/src/canalyst_candas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4863 2021-10-05 12:21:04.000000 canalyst_candas-0.0.9/src/canalyst_candas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      632 2021-10-05 12:21:04.000000 canalyst_candas-0.0.9/src/canalyst_candas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-10-05 12:21:04.000000 canalyst_candas-0.0.9/src/canalyst_candas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      332 2021-10-05 12:21:04.000000 canalyst_candas-0.0.9/src/canalyst_candas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2021-10-05 12:21:04.000000 canalyst_candas-0.0.9/src/canalyst_candas.egg-info/top_level.txt
```

### Comparing `canalyst_candas-0.0.8/PKG-INFO` & `canalyst_candas-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: canalyst_candas
-Version: 0.0.8
+Version: 0.0.9
 Summary: The official Canalyst Software Development Kit (SDK) for our public API
-Home-page: https://github.com/pypa/sampleproject
+Home-page: UNKNOWN
 Author: Canalyst
 Author-email: support+api@canalyst.com
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `canalyst_candas-0.0.8/README.md` & `canalyst_candas-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `canalyst_candas-0.0.8/setup.py` & `canalyst_candas-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,14 @@
     name="canalyst_candas",
     version=__version__,
     author="Canalyst",
     author_email="support+api@canalyst.com",
     description="The official Canalyst Software Development Kit (SDK) for our public API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/pypa/sampleproject",
-    project_urls={"Bug Tracker": "https://github.com/pypa/sampleproject/issues"},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `canalyst_candas-0.0.8/src/canalyst_candas/candas.py` & `canalyst_candas-0.0.9/src/canalyst_candas/candas.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     get_scenario_url_data,
     json_to_df,
     map_scenario_urls,
     read_json,
     save_guidance_csv,
     send_scenario,
     calendar_quarter,
+    get_excel_model,
 )
 import __main__
 from pyvis.network import Network
 from functools import reduce
 import networkx as nx
 import plotly.express as px
 from statistics import stdev
@@ -88,14 +89,143 @@
     def func_multiply(self):
         return float(self.value) * float(self.argument)
 
     def func_subtract(self):
         return float(self.value) - float(self.argument)
 
 
+class Search:
+    def __init__(self, config: Config = None):
+        self.config = config
+        self.df_search = None
+        self.df_guidance = None
+
+    def help(self):
+        print("search_time_series syntax:")
+        print(
+            "ticker (Bloomberg ticker),sector,time_series_name,time_series_description,category,is_driver,unit_type"
+        )
+        print("unit types:currency, percentage, count, ratio, time")
+        print("search_guidance_time_series syntax:")
+        print(
+            "ticker (Bloomberg ticker),sector,item (time series description),item_name (time series name),most_recent (True or blank)"
+        )
+        return
+
+    def search_guidance_time_series(
+        self,
+        ticker="",
+        sector="",
+        Type="",
+        item="",
+        item_name="",
+        most_recent="",
+    ):
+        if self.df_guidance is None:
+            print("Building guidance index...")
+            self.df_guidance = Getter(config=self.config).get_csv_from_s3(
+                f"DATA/df_guidance.csv"
+            )
+            print("Done")
+
+        df = self.df_guidance
+
+        if most_recent == True:
+            df = df.sort_values(["ticker", "Date"], ascending=False)
+            df = df.groupby(["ticker", "Item"]).first().reset_index()
+
+        if type(ticker) == list:
+            df = df.loc[df["ticker"].isin(ticker)]
+        elif ticker != "":
+            df = df.loc[df["ticker"].str.contains(ticker, case=True, regex=True)]
+
+        if sector != "":
+            df = df.loc[df["Path"].str.contains(sector, case=True, regex=True)]
+        if item != "":
+            df = df.loc[df["Item"].str.contains(item, case=False, regex=True)]
+        if item_name != "":
+            df = df.loc[df["item_name"].str.contains(item_name, case=False)]
+        return df[
+            [
+                "ticker",
+                "Path",
+                "Item",
+                "Item Name",
+                "Fiscal Period",
+                "Low",
+                "Mid",
+                "High",
+                "Type.1",
+                "Date",
+                "Link",
+            ]
+        ].sort_values(["ticker", "Date", "Item"])
+
+    def search_time_series(
+        self,
+        ticker="",
+        sector="",
+        time_series_name="",
+        time_series_description="",
+        category="",
+        is_driver="",
+        unit_type="",
+    ):
+        if self.df_search is None:
+            print("Building search index...")
+            self.df_search = Getter(config=self.config).get_csv_from_s3(
+                f"DATA/df_search.csv"
+            )
+            print("Done")
+
+        df = self.df_search
+        if type(ticker) == list:
+            df = df.loc[df["ticker"].isin(ticker)]
+        elif ticker != "":
+            df = df.loc[df["ticker"].str.contains(ticker, case=True, regex=True)]
+
+        if sector != "":
+            df = df.loc[df["Path"].str.contains(sector, case=True, regex=True)]
+        if category != "":
+            df = df.loc[df["category"].str.contains(category, case=True, regex=True)]
+        if time_series_name != "":
+            df = df.loc[
+                df["time_series_name"].str.contains(
+                    time_series_name, case=False, regex=True
+                )
+            ]
+        if time_series_description != "":
+            df = df.loc[
+                df["time_series_description"].str.contains(
+                    time_series_description, case=False
+                )
+            ]
+        if is_driver != "":
+            df = df.loc[df["is_driver"] == is_driver]
+        if unit_type != "":
+            df = df.loc[
+                df["unit_type"] == unit_type
+            ]  # currency, percentage, count, ratio, time
+        df["fiscal_or_annual"] = np.where(
+            df["value"].isna(), "fiscal_year", "fiscal_quarter"
+        )
+        return df[
+            [
+                "ticker",
+                "Path",
+                "category",
+                "time_series_description",
+                "time_series_name",
+                "fiscal_or_annual",
+                "unit_type",
+                "is_driver",
+            ]
+        ].sort_values(["ticker", "time_series_description"])
+
+
 # WIP Class for parsing json revenue builds in graph structure (as opposed to tree)
 # class FormulaGraph:
 # def __init__(
 #     self,
 #     file_name=None,
 #     ticker=None,
 #     auto_parse=True,
@@ -563,31 +693,101 @@
         self.api_headers = get_api_headers(self.config.canalyst_api_key)
 
         self.get_featurelibrary()  # set self._features
 
         if type(ticker_list) is str:
             ticker_list = [ticker_list]
 
+    def help(self, function_name=""):
+        dict_help = {
+            "create_model_map": "Create a model map.  params: ticker, col_for_labels = 'time_series_name', time_series_name = 'MO_RIS_REV', tree = True, notebook = True",
+            "create_time_series_chart": "Create a time series chart.  params: ticker, time_series_name",
+            "guidance": "Return guidance from a mmodel.  params: ticker",
+            "mrq": "Return most recent quarter from a mmodel.  params: ticker",
+            "time_series_search": "Return time series regex match. params: time_series_name",
+            "driver_search": "Return driver regex match. params: driver_name",
+            "model_frame": "Return a dataframe of the full modelset. params: time_series_name,period_name,is_driver='',pivot=False,mrq=False,period_duration_type='',is_historical='',n_periods='',mrq_notation=False",
+            "forecast_frame": "Return a params dataframe for use in the fit function. params: time_series_name, n_periods, function_name='value', function_value='' where function name can be add, subtract, multiply, divide, or value",
+            "fit": "Return a return series for a fitted model. params: params dataframe, return_series.  params dataframe columns are: ticker period time_series_name value new_value",
+        }
+        if function_name != "":
+            return dict_help[function_name]
+        else:
+            df = pd.DataFrame(dict_help, index=[0]).T
+            df.columns = ["help"]
+            return df
+
     # shows a tree for the given ticker and time series
     def create_model_map(
         self,
         ticker,
         col_for_labels="time_series_name",
         time_series_name="MO_RIS_REV",
         tree=True,
         notebook=True,
     ):
-        model = self.models[ticker]
-        return model.create_model_map(
-            time_series_name=time_series_name,
-            tree=tree,
-            col_for_labels=col_for_labels,
-            notebook=notebook,
-            common_time_series_names=self._common_time_series_names,
-        )
+        if type(ticker) == list:
+            print("Please request one ticker at a time.")
+            return
+
+        if ticker in self.ticker_list:
+            model = self.models[ticker]
+            return model.create_model_map(
+                time_series_name=time_series_name,
+                tree=tree,
+                col_for_labels=col_for_labels,
+                notebook=notebook,
+                common_time_series_names=self._common_time_series_names,
+            )
+        else:
+            print("Please choose a ticker in this ModelSet's ticker list")
+            return
+
+    def create_time_series_chart(self, ticker, time_series_name):
+        if type(ticker) == list:
+            print("Please request one ticker at a time.")
+            return
+
+        if ticker in self.ticker_list:
+            self.models[df].create_time_series_chart(time_series_name)
+
+        else:
+            print("Please choose a ticker in this ModelSet's ticker list")
+        return
+
+    def guidance(self, ticker):
+        if type(ticker) == list:
+            list_df = []
+            for t in ticker:
+                if ticker in self.ticker_list:
+                    df = self.models[ticker].guidance()
+                    list_df.append(df)
+            return pd.concat(list_df)
+        else:
+            if ticker in self.ticker_list:
+                return self.models[ticker].guidance()
+            else:
+                print("Please choose a ticker in this ModelSet's ticker list")
+        return
+
+    def mrq(self, ticker):
+        if type(ticker) == list:
+            list_df = []
+            for t in ticker:
+                if ticker in self.ticker_list:
+                    df = self.models[ticker].mrq()
+                    df["ticker"] = t
+                    list_df.append(df)
+            return pd.concat(list_df)
+        else:
+            if ticker in self.ticker_list:
+                return self.models[ticker].mrq()
+            else:
+                print("Please choose a ticker in this ModelSet's ticker list")
+        return
 
     # get a list of time series from the default dataframe
     def time_series_names(self):
         df = self._features
         df = (
             df.groupby(["time_series_name"])
             .first()
@@ -693,31 +893,37 @@
             self._features = df
             if self.extract_drivers == True:
                 self.drivers = df[df["is_driver"] == 1]
             return
         return
 
     # allows for filtering and shaping the default dataframe
-    # MODEL model_frame
+    # MODELSET model_frame
     def model_frame(
         self,
         time_series_name="",
         period_name="",
         is_driver="",
         pivot=False,
         mrq=False,
         period_duration_type="",
         is_historical="",
         n_periods="",
         mrq_notation=False,
         warning=True,
+        ticker="",
     ):
 
+        if ticker != "":
+            df = self.models[ticker]._model_frame
+        else:
+            df = self._features
+
         return filter_dataset(
-            self._features,  # this is the core dataset of the modelset class
+            df,  # this is the core dataset of the modelset class
             time_series_name,
             period_name,
             is_driver,
             pivot,
             mrq,
             period_duration_type,
             is_historical,
@@ -933,15 +1139,20 @@
         self.complexity = None
         self.mean_end_node_distance = 0
         self.max_end_node_distance = 0
         self.std_dev_node_distance = 0
 
         # Create dataframe for precedent/dependent tree, graph of the tree, and a network of that graph (for visualization)
         self.df = self.load_data()
-        self.network = self.create_model()
+        try:
+            self.network = self.create_model()
+        except:
+            print(
+                "Canalyst-Candas error creating modelmap.  Possible permissions issue with your Canalyst login, please contact us."
+            )
 
         self.fig = None
 
     # helper function to load data from candas:
     # loads model_frame for chosen ticker and create a dot file
     def load_data(self) -> pd.DataFrame:
         if self.model:
@@ -1249,17 +1460,20 @@
         self.log = LogFile(default_dir=self.config.default_dir)
 
         self.set_new_uuid()
 
         if self.force == True:
             print("model_frame")
 
-        self.csin, self.latest_version = get_company_info_from_ticker(
-            self.ticker, self.api_headers, self.config.mds_host
-        )
+        try:
+            self.csin, self.latest_version = get_company_info_from_ticker(
+                self.ticker, self.api_headers, self.config.mds_host
+            )
+        except:
+            print("Canalyst-Candas: Error on API Key.  Perhaps missing key.")
 
         self.get_model_frame()
 
         if self.extract_drivers == True:
             self.apply_drivers(self.force)
 
         if self.force == True:
@@ -1277,14 +1491,64 @@
             except:
                 self.log.write("failed to create drivers")
 
         if self.force == True:
             print("guidance")
             self.create_guidance_csv()
 
+        self._model_name = self.get_excel_model_name()
+        self._model_frame["model_name"] = self._model_name
+
+    def get_excel_model_name(self):
+
+        csin = self.csin
+        auth_headers = self.api_headers
+        mds_host = self.config.mds_host
+        wp_host = self.config.wp_host
+
+        from python_graphql_client import GraphqlClient
+
+        client = GraphqlClient(endpoint=f"{wp_host}/model-workbooks")
+
+        # Create the query string and variables required for the request.
+        query = """
+        query driversWorksheetByCSIN($csin: ID!) {
+            modelSeries(id: $csin) {
+            latestModel {
+                id
+                name
+                publishedAt
+                variantsByDimensions(
+                    driversWorksheets: [STANDARD_FCF],
+                    periodOrder: [CHRONOLOGICAL],
+                ) {
+                id
+                downloadUrl
+                variantDimensions {
+                    driversWorksheets
+                    periodOrder
+                }
+                }
+            }
+            }
+        }
+        """
+        variables = {"csin": csin}
+
+        # Synchronous request
+        data = client.execute(
+            query=query, variables=variables, headers=auth_headers, verify=False
+        )
+        url = data["data"]["modelSeries"]["latestModel"]["variantsByDimensions"][0][
+            "downloadUrl"
+        ]
+        file_ticker = self.ticker.split(" ")[0]
+        file_name = data["data"]["modelSeries"]["latestModel"]["name"]
+        return file_name
+
     def key_driver_map(self, time_series_name):
         # defaulting to MO_RIS_REV, but you could choose another time_series_name as a starting point like MO_RIS_EBIT
         model_map = self.create_model_map(
             time_series_name=time_series_name, col_for_labels="time_series_name"
         )
 
         # list all the nodes in the model map
```

### Comparing `canalyst_candas-0.0.8/src/canalyst_candas/candas_datareader.py` & `canalyst_candas-0.0.9/src/canalyst_candas/candas_datareader.py`

 * *Files identical despite different names*

### Comparing `canalyst_candas-0.0.8/src/canalyst_candas/configuration/config.py` & `canalyst_candas-0.0.9/src/canalyst_candas/configuration/config.py`

 * *Files identical despite different names*

### Comparing `canalyst_candas-0.0.8/src/canalyst_candas/connection.py` & `canalyst_candas-0.0.9/src/canalyst_candas/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Connection module
 """
 from typing import Any
-from canalyst_candas.candas import Model, ModelMap, ModelSet
+from canalyst_candas.candas import Model, ModelMap, ModelSet, Search
 from canalyst_candas.configuration.config import Config, resolve_config
 
 
 class Connection:
     """
     Connection uses configuration and shares them across the library
     """
```

### Comparing `canalyst_candas-0.0.8/src/canalyst_candas/settings.py` & `canalyst_candas-0.0.9/src/canalyst_candas/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             "fred_key": "",
             "default_dir": "",
             "mds_host": "",
             "wp_host": "",
         }
         config_file.write_text(json.dumps(config_file_json))
         print(
-            "Bad configuration. A configuration file has been created for you in \n"
+            "A configuration file has been created for you in \n"
             f"{config_file}. For Excel file downloads and scenario \n"
             "mapping, you'll need to add an API key to the 'canalyst_api_key' \n"
             "value. Visit https://app.canalyst.com/settings/api-tokens to create \n"
             "and retrieve your API key. You will also need to retrieve your \n"
             "S3 Access ID and Secret Key and fill in 'canalyst_s3_id' and \n"
             "'canalyst_s3_key' with those values, respectively. If using a \n"
             "Jupyter Notebook, stop and restart the notebook for the changes to \n"
```

### Comparing `canalyst_candas-0.0.8/src/canalyst_candas/utils.py` & `canalyst_candas-0.0.9/src/canalyst_candas/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,18 +425,19 @@
                 list_values = [
                     val
                     for val in model_sheet.iter_rows(min_row=int(row), max_row=int(row))
                 ][0]
             except:
                 log.write(f"error: {defined_name}")
                 continue
-            i_toggle = 0
+
             dict_values = {}
 
             for index, item in enumerate(list_values):
+                i_toggle = 0
                 if type(item.value) == float or type(item.value) == int:
                     dict_values = {}
                     num = (
                         "$"
                         + n2a(index)
                         + str(named_ranges[defined_name]).replace("$", "")
                     )
@@ -1069,28 +1070,30 @@
     cols = list(df.groupby("n").first().reset_index()["n"])
 
     df = pd.pivot_table(
         df,
         values="value",
         index=[
             "name_index",
+            "model_name",
             "ticker",
             "category",
             "time_series_name",
             "time_series_description",
             "is_driver",
             "MRQ",
         ],
         columns=["n"],
         aggfunc=np.sum,
     ).reset_index()
     list_cols = []
 
     name_cols = [
         "name_index",
+        "model_name",
         "ticker",
         "category",
         "time_series_name",
         "time_series_description",
         "is_driver",
         "MRQ",
     ]
@@ -1106,30 +1109,19 @@
 
 def pivot_df(df, mrq_notation):
 
     if mrq_notation == True:
         df = mrq_df(df)
         return df
 
-    cols1 = [
-        "ticker",
-        "name_index",
-        "category",
-        "time_series_name",
-        "time_series_description",
-        "is_driver",
-    ]
-    cols1.extend(list(df["period_name"]))
-    cols2 = []
-    [cols2.append(x) for x in cols1 if x not in cols2]
-
     df = pd.pivot_table(
         df,
         values="value",
         index=[
+            "model_name",
             "ticker",
             "name_index",
             "category",
             "time_series_name",
             "time_series_description",
             "is_driver",
         ],
```

### Comparing `canalyst_candas-0.0.8/src/canalyst_candas.egg-info/PKG-INFO` & `canalyst_candas-0.0.9/src/canalyst_candas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: canalyst-candas
-Version: 0.0.8
+Version: 0.0.9
 Summary: The official Canalyst Software Development Kit (SDK) for our public API
-Home-page: https://github.com/pypa/sampleproject
+Home-page: UNKNOWN
 Author: Canalyst
 Author-email: support+api@canalyst.com
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `canalyst_candas-0.0.8/src/canalyst_candas.egg-info/SOURCES.txt` & `canalyst_candas-0.0.9/src/canalyst_candas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

