# Comparing `tmp/geoglows-1.0.4.tar.gz` & `tmp/geoglows-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.0.4.tar", last modified: Wed Apr 10 22:46:23 2024, max compression
+gzip compressed data, was "geoglows-1.1.tar", last modified: Fri Apr 12 18:20:01 2024, max compression
```

## Comparing `geoglows-1.0.4.tar` & `geoglows-1.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:46:23.158525 geoglows-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-10 22:46:19.000000 geoglows-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-10 22:46:19.000000 geoglows-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-10 22:46:23.154525 geoglows-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-10 22:46:19.000000 geoglows-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:46:23.154525 geoglows-1.0.4/geoglows/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-10 22:46:19.000000 geoglows-1.0.4/geoglows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-10 22:46:19.000000 geoglows-1.0.4/geoglows/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:46:23.154525 geoglows-1.0.4/geoglows/_plots/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-10 22:46:19.000000 geoglows-1.0.4/geoglows/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-10 22:46:19.000000 geoglows-1.0.4/geoglows/_plots/format_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-10 22:46:19.000000 geoglows-1.0.4/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-10 22:46:19.000000 geoglows-1.0.4/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-10 22:46:19.000000 geoglows-1.0.4/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-10 22:46:19.000000 geoglows-1.0.4/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-10 22:46:19.000000 geoglows-1.0.4/geoglows/_plots/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-10 22:46:19.000000 geoglows-1.0.4/geoglows/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-10 22:46:19.000000 geoglows-1.0.4/geoglows/bias.py
--rw-r--r--   0 runner    (1001) docker     (127)    13590 2024-04-10 22:46:19.000000 geoglows-1.0.4/geoglows/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-10 22:46:19.000000 geoglows-1.0.4/geoglows/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-10 22:46:19.000000 geoglows-1.0.4/geoglows/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:46:23.154525 geoglows-1.0.4/geoglows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-10 22:46:23.000000 geoglows-1.0.4/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-10 22:46:23.000000 geoglows-1.0.4/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 22:46:23.000000 geoglows-1.0.4/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-10 22:46:23.000000 geoglows-1.0.4/geoglows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 22:46:23.000000 geoglows-1.0.4/geoglows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-10 22:46:19.000000 geoglows-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 22:46:23.158525 geoglows-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-10 22:46:19.000000 geoglows-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:20:01.776823 geoglows-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-12 18:19:53.000000 geoglows-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-12 18:19:53.000000 geoglows-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-12 18:20:01.776823 geoglows-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-12 18:19:53.000000 geoglows-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:20:01.772823 geoglows-1.1/geoglows/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:20:01.776823 geoglows-1.1/geoglows/_plots/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_plots/format_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/_plots/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/streamflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-12 18:19:53.000000 geoglows-1.1/geoglows/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:20:01.776823 geoglows-1.1/geoglows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-12 18:20:01.000000 geoglows-1.1/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-12 18:20:01.000000 geoglows-1.1/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:20:01.000000 geoglows-1.1/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 18:20:01.000000 geoglows-1.1/geoglows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 18:20:01.000000 geoglows-1.1/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-12 18:19:53.000000 geoglows-1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:20:01.776823 geoglows-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-12 18:19:53.000000 geoglows-1.1/setup.py
```

### Comparing `geoglows-1.0.4/LICENSE` & `geoglows-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.4/PKG-INFO` & `geoglows-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.4
+Version: 1.1.0
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.0.4/README.md` & `geoglows-1.1/README.md`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.4/geoglows/_plots/format_tools.py` & `geoglows-1.1/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.4/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.1/geoglows/_plots/plotly_bias_corrected.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.4/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.1/geoglows/_plots/plotly_forecasts.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.4/geoglows/_plots/plotly_helpers.py` & `geoglows-1.1/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.4/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.1/geoglows/_plots/plotly_retrospective.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.4/geoglows/_plots/plots.py` & `geoglows-1.1/geoglows/_plots/plots.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.4/geoglows/analyze.py` & `geoglows-1.1/geoglows/analyze.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.4/geoglows/bias.py` & `geoglows-1.1/geoglows/bias.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.4/geoglows/data.py` & `geoglows-1.1/geoglows/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 def _forecast_endpoint_decorator(function):
     def from_aws(*args, **kwargs):
         product_name = function.__name__.replace("_", "").lower()
         if product_name == 'forecastrecords':
             warnings.warn('forecast_records are not available from the AWS Open Data Program.')
             return from_rest(*args, **kwargs)
 
-        reach_id = kwargs.get('reach_id', '')
-        reach_id = args[0] if len(args) > 0 else None
+        river_id = kwargs.get('river_id', '')
+        river_id = args[0] if len(args) > 0 else None
 
         s3 = s3fs.S3FileSystem(anon=True, client_kwargs=dict(region_name=ODP_S3_BUCKET_REGION))
         if kwargs.get('date', '') and not product_name == 'dates':
             date = kwargs['date']
             if len(date) == 8:
                 date = f'{date}00.zarr'
             elif len(date) == 10:
@@ -64,22 +64,22 @@
             dates = [x.split('.')[0] for x in dates if x.endswith('.zarr')]  # ignore the index.html file
             dates = [x.replace('00.zarr', '') for x in dates]
             if product_name == 'dates':
                 return pd.DataFrame(dict(dates=dates))
             date = dates[-1]
         s3store = s3fs.S3Map(root=f'{ODP_FORECAST_S3_BUCKET_URI}/{date}', s3=s3, check=False)
 
-        df = xr.open_zarr(s3store).sel(rivid=reach_id).to_dataframe().round(2).reset_index()
+        df = xr.open_zarr(s3store).sel(rivid=river_id).to_dataframe().round(2).reset_index()
 
         # rename columns to match the REST API
-        if isinstance(reach_id, int):
+        if isinstance(river_id, int):
             df = df.pivot(index='time', columns='ensemble', values='Qout')
         else:
             df = df.pivot(index=['time', 'rivid'], columns='ensemble', values='Qout')
-            df.index.names = ['time', 'LINKNO']
+            df.index.names = ['time', 'river_id']
         df = df[sorted(df.columns)]
         df.columns = [f'ensemble_{str(x).zfill(2)}' for x in df.columns]
 
         if product_name == 'forecastensembles':
             return df
         elif product_name == 'forecaststats':
             return calc_forecast_stats(df)
@@ -98,25 +98,32 @@
         # parse out the information necessary to build a request url
         endpoint = kwargs.get('endpoint', DEFAULT_REST_ENDPOINT)
         endpoint = endpoint[:-1] if endpoint[-1] == '/' else endpoint
         endpoint = endpoint + '/api' if not endpoint.endswith('/api') else endpoint
         endpoint = f'https://{endpoint}' if not endpoint.startswith(('https://', 'http://')) else endpoint
 
         version = kwargs.get('version', DEFAULT_REST_ENDPOINT_VERSION)
+        assert version in ('v1', 'v2', ), ValueError(f'Unrecognized model version parameter: {version}')
 
         product_name = function.__name__.replace("_", "").lower()
 
-        reach_id = args[0] if len(args) > 0 else None
-        reach_id = kwargs.get('reach_id', '') if not reach_id else reach_id
+        river_id = args[0] if len(args) > 0 else None
+        river_id = kwargs.get('river_id', '') if not river_id else river_id
+        if isinstance(river_id, list):
+            raise ValueError('Multiple river_ids are not available via REST API or on v1. '
+                             'Use data_source="aws" and version="v2" for multiple river_ids.')
+        river_id = int(river_id) if river_id else None
+        if river_id and version == 'v2':
+            assert river_id < 1_000_000_000 and river_id >= 110_000_000, ValueError('River ID must be a 9 digit integer')
 
         return_format = kwargs.get('return_format', 'csv')
         assert return_format in ('csv', 'json', 'url'), f'Unsupported return format requested: {return_format}'
 
         # request parameter validation before submitting
-        for key in ('endpoint', 'version', 'reach_id'):
+        for key in ('endpoint', 'version', 'river_id'):
             if key in kwargs:
                 del kwargs[key]
         for key, value in kwargs.items():
             if value is None:
                 del kwargs[key]
         for date in ('date', 'start_date', 'end_date'):
             if date in kwargs:
@@ -125,15 +132,15 @@
         if 'format' in kwargs and kwargs['format'] != 'json':
             del kwargs['format']
         kwargs['source'] = kwargs.get('source', 'pygeoglows')  # allow using default for specific apps which override
         params = '&'.join([f'{key}={value}' for key, value in kwargs.items()])
 
         # piece together the request url
         request_url = f'{endpoint}/{version}/{product_name}'  # build the base url
-        request_url = f'{request_url}/{reach_id}' if reach_id else request_url  # add the reach_id if it exists
+        request_url = f'{request_url}/{river_id}' if river_id else request_url  # add the river_id if it exists
         request_url = f'{request_url}?{params}'  # add the query parameters
 
         if return_url:
             return request_url.replace(f'source={kwargs["source"]}', '')
 
         response = requests.get(request_url)
 
@@ -154,14 +161,15 @@
     def main(*args, **kwargs):
         source = kwargs.get('data_source', 'aws')
         assert source in ('rest', 'aws'), ValueError(f'Unrecognized data source requested: {source}')
         if source == 'rest':
             return from_rest(*args, **kwargs)
         else:
             return from_aws(*args, **kwargs)
+    main.__doc__ = function.__doc__  # necessary for code documentation auto generators
     return main
 
 
 # Forecast data and derived products
 @_forecast_endpoint_decorator
 def dates(**kwargs) -> dict or str:
     """
@@ -177,165 +185,166 @@
         the csv is a single column with a header of 'available_dates' and 1 row per date, sorted oldest to newest
         The dictionary structure is {'available_dates': ['list', 'of', 'dates', 'YYYYMMDD', 'format']}
     """
     pass
 
 
 @_forecast_endpoint_decorator
-def forecast(*, reach_id: int, date: str, return_format: str, data_source: str,
+def forecast(*, river_id: int, date: str, return_format: str, data_source: str,
              **kwargs) -> pd.DataFrame or dict or str:
     """
-    Gets the average forecasted flow for a certain reach_id on a certain date
+    Gets the average forecasted flow for a certain river_id on a certain date
 
     Keyword Args:
-        reach_id: the ID of a stream, should be a 9 digit integer
-        date: a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
-        return_format: csv, json, or url, default csv
-        data_source: location to query for data, either 'rest' or 'aws'. default is aws.
+        river_id (str): the ID of a stream, should be a 9 digit integer
+        date (str): a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
+        return_format (str): csv, json, or url, default csv
+        data_source (str): location to query for data, either 'rest' or 'aws'. default is aws.
+        version (str): the version of the API and model data to retrieve. default is 'v2'. should be 'v1' or 'v2'
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
 @_forecast_endpoint_decorator
-def forecast_stats(*, reach_id: int, date: str, return_format: str, data_source: str,
+def forecast_stats(*, river_id: int, date: str, return_format: str, data_source: str,
                    **kwargs) -> pd.DataFrame or dict or str:
     """
-    Retrieves the min, 25%, mean, median, 75%, and max river discharge of the 51 ensembles members for a reach_id
+    Retrieves the min, 25%, mean, median, 75%, and max river discharge of the 51 ensembles members for a river_id
     The 52nd higher resolution member is excluded
 
     Keyword Args:
-        reach_id: the ID of a stream, should be a 9 digit integer
+        river_id: the ID of a stream, should be a 9 digit integer
         date: a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
         return_format: csv, json, or url, default csv
         data_source: location to query for data, either 'rest' or 'aws'. default is aws.
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
 @_forecast_endpoint_decorator
-def forecast_ensembles(*, reach_id: int, date: str, return_format: str, data_source: str,
+def forecast_ensembles(*, river_id: int, date: str, return_format: str, data_source: str,
                        **kwargs) -> pd.DataFrame or dict or str:
     """
-    Retrieves each of 52 time series of forecasted discharge for a reach_id on a certain date
+    Retrieves each of 52 time series of forecasted discharge for a river_id on a certain date
 
     Keyword Args:
-        reach_id: the ID of a stream, should be a 9 digit integer
+        river_id: the ID of a stream, should be a 9 digit integer
         date: a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
         return_format: csv, json, or url, default csv
         data_source: location to query for data, either 'rest' or 'aws'. default is aws.
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
 @_forecast_endpoint_decorator
-def forecast_records(*, reach_id: int, start_date: str, end_date: str, return_format: str, data_source: str,
+def forecast_records(*, river_id: int, start_date: str, end_date: str, return_format: str, data_source: str,
                      **kwargs) -> pd.DataFrame or dict or str:
     """
     Retrieves a csv showing the ensemble average forecasted flow for the year from January 1 to the current date
 
     Keyword Args:
-        reach_id: the ID of a stream, should be a 9 digit integer
+        river_id: the ID of a stream, should be a 9 digit integer
         start_date: a YYYYMMDD string giving the earliest date this year to include, defaults to 14 days ago.
         end_date: a YYYYMMDD string giving the latest date this year to include, defaults to latest available
         data_source: location to query for data, either 'rest' or 'aws'. default is aws.
         return_format: csv, json, or url, default csv
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
 # Retrospective simulation and derived products
-def retrospective(reach_id: int or list) -> pd.DataFrame:
+def retrospective(river_id: int or list) -> pd.DataFrame:
     """
-    Retrieves the retrospective simulation of streamflow for a given reach_id from the
+    Retrieves the retrospective simulation of streamflow for a given river_id from the
     AWS Open Data Program GEOGloWS V2 S3 bucket
 
     Args:
-        reach_id: the ID of a stream, should be a 9 digit integer
+        river_id: the ID of a stream, should be a 9 digit integer
 
     Returns:
         pd.DataFrame
     """
     s3 = s3fs.S3FileSystem(anon=True, client_kwargs=dict(region_name=ODP_S3_BUCKET_REGION))
     s3store = s3fs.S3Map(root=f'{ODP_RETROSPECTIVE_S3_BUCKET_URI}/retrospective.zarr', s3=s3, check=False)
-    return (xr.open_zarr(s3store).sel(rivid=reach_id).to_dataframe().reset_index().set_index('time')
+    return (xr.open_zarr(s3store).sel(rivid=river_id).to_dataframe().reset_index().set_index('time')
             .pivot(columns='rivid', values='Qout'))
 
 
 def historical(*args, **kwargs):
     """Alias for retrospective"""
     return retrospective(*args, **kwargs)
 
 
-def daily_averages(reach_id: int or list) -> pd.DataFrame:
+def daily_averages(river_id: int or list) -> pd.DataFrame:
     """
-    Retrieves daily average streamflow for a given reach_id
+    Retrieves daily average streamflow for a given river_id
 
     Args:
-        reach_id: the ID of a stream, should be a 9 digit integer
+        river_id: the ID of a stream, should be a 9 digit integer
 
     Returns:
         pd.DataFrame
     """
-    df = retrospective(reach_id)
+    df = retrospective(river_id)
     return calc_daily_averages(df)
 
 
-def monthly_averages(reach_id: int or list) -> pd.DataFrame:
+def monthly_averages(river_id: int or list) -> pd.DataFrame:
     """
-    Retrieves monthly average streamflow for a given reach_id
+    Retrieves monthly average streamflow for a given river_id
 
     Args:
-        reach_id: the ID of a stream, should be a 9 digit integer
+        river_id: the ID of a stream, should be a 9 digit integer
 
     Returns:
         pd.DataFrame
     """
-    df = retrospective(reach_id)
+    df = retrospective(river_id)
     return calc_monthly_averages(df)
 
 
-def annual_averages(reach_id: int or list) -> pd.DataFrame:
+def annual_averages(river_id: int or list) -> pd.DataFrame:
     """
-    Retrieves annual average streamflow for a given reach_id
+    Retrieves annual average streamflow for a given river_id
 
     Args:
-        reach_id: the ID of a stream, should be a 9 digit integer
+        river_id: the ID of a stream, should be a 9 digit integer
 
     Returns:
         pd.DataFrame
     """
-    df = retrospective(reach_id)
+    df = retrospective(river_id)
     return calc_annual_averages(df)
 
 
-def return_periods(reach_id: int or list) -> pd.DataFrame:
+def return_periods(river_id: int or list) -> pd.DataFrame:
     """
-    Retrieves the return period thresholds based on a specified historic simulation forcing on a certain reach_id.
+    Retrieves the return period thresholds based on a specified historic simulation forcing on a certain river_id.
 
     Args:
-        reach_id: the ID of a stream, should be a 9 digit integer
+        river_id: the ID of a stream, should be a 9 digit integer
 
     Returns:
         pd.DataFrame
     """
     s3 = s3fs.S3FileSystem(anon=True, client_kwargs=dict(region_name=ODP_S3_BUCKET_REGION))
     s3store = s3fs.S3Map(root=f'{ODP_RETROSPECTIVE_S3_BUCKET_URI}/return-periods.zarr', s3=s3, check=False)
-    return (xr.open_zarr(s3store).sel(rivid=reach_id)['return_period_flow'].to_dataframe().reset_index()
+    return (xr.open_zarr(s3store).sel(rivid=river_id)['return_period_flow'].to_dataframe().reset_index()
             .pivot(index='rivid', columns='return_period', values='return_period_flow'))
 
 
 # model config and supplementary data
 def metadata_tables(columns: list = None) -> pd.DataFrame:
     """
     Retrieves the master table of stream reaches with all metadata and properties as a pandas DataFrame
```

### Comparing `geoglows-1.0.4/geoglows/streams.py` & `geoglows-1.1/geoglows/streams.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import numpy as np
 
 from .data import metadata_tables
 
-__all__ = ['reach_to_vpu', 'latlon_to_reach', 'reach_to_latlon', ]
+__all__ = ['river_to_vpu', 'latlon_to_river', 'river_to_latlon', ]
 
 
-def reach_to_vpu(reach_id: int) -> str or int:
+def river_to_vpu(reach_id: int) -> str or int:
     return (
         metadata_tables(columns=['LINKNO', 'VPUCode'])
         .loc[lambda x: x['LINKNO'] == reach_id, 'VPUCode']
         .values[0]
     )
 
 
-def latlon_to_reach(lat: float, lon: float) -> int:
+def latlon_to_river(lat: float, lon: float) -> int:
     df = metadata_tables(columns=['LINKNO', 'lat', 'lon'])
     df['dist'] = ((df['lat'] - lat) ** 2 + (df['lon'] - lon) ** 2) ** 0.5
     return df.loc[lambda x: x['dist'] == df['dist'].min(), 'LINKNO'].values[0]
 
 
-def reach_to_latlon(reach_id: int) -> np.ndarray:
+def river_to_latlon(reach_id: int) -> np.ndarray:
     return (
         metadata_tables(columns=['LINKNO', 'lat', 'lon'])
         .loc[lambda x: x['LINKNO'] == reach_id, ['lat', 'lon']]
         .values[0]
     )
```

### Comparing `geoglows-1.0.4/geoglows/tables.py` & `geoglows-1.1/geoglows/tables.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.4/geoglows.egg-info/PKG-INFO` & `geoglows-1.1/geoglows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.4
+Version: 1.1.0
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.0.4/geoglows.egg-info/SOURCES.txt` & `geoglows-1.1/geoglows.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 requirements.txt
 setup.py
 geoglows/__init__.py
 geoglows/_constants.py
 geoglows/analyze.py
 geoglows/bias.py
 geoglows/data.py
+geoglows/streamflow.py
 geoglows/streams.py
 geoglows/tables.py
 geoglows.egg-info/PKG-INFO
 geoglows.egg-info/SOURCES.txt
 geoglows.egg-info/dependency_links.txt
 geoglows.egg-info/requires.txt
 geoglows.egg-info/top_level.txt
```

### Comparing `geoglows-1.0.4/setup.py` & `geoglows-1.1/setup.py`

 * *Files identical despite different names*

