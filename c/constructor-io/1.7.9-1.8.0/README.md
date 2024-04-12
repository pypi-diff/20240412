# Comparing `tmp/constructor-io-1.7.9.tar.gz` & `tmp/constructor-io-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constructor-io-1.7.9.tar", last modified: Thu Oct 26 13:49:50 2023, max compression
+gzip compressed data, was "constructor-io-1.8.0.tar", last modified: Fri Apr 12 15:22:08 2024, max compression
```

## Comparing `constructor-io-1.7.9.tar` & `constructor-io-1.8.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-10-26 13:49:50.009337 constructor-io-1.7.9/
--rw-r--r--   0 enes       (502) staff       (20)     1086 2021-09-21 17:57:12.000000 constructor-io-1.7.9/LICENSE
--rw-r--r--   0 enes       (502) staff       (20)     2562 2023-10-26 13:49:50.009170 constructor-io-1.7.9/PKG-INFO
--rw-r--r--   0 enes       (502) staff       (20)     2198 2022-10-03 13:13:47.000000 constructor-io-1.7.9/README.md
-drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-10-26 13:49:50.005418 constructor-io-1.7.9/constructor_io/
--rw-r--r--   0 enes       (502) staff       (20)       41 2023-10-26 13:49:33.000000 constructor-io-1.7.9/constructor_io/__init__.py
--rw-r--r--   0 enes       (502) staff       (20)     2324 2023-06-08 14:52:00.000000 constructor-io-1.7.9/constructor_io/constructor_io.py
-drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-10-26 13:49:50.006696 constructor-io-1.7.9/constructor_io/helpers/
--rw-r--r--   0 enes       (502) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.7.9/constructor_io/helpers/__init__.py
--rw-r--r--   0 enes       (502) staff       (20)      481 2021-11-18 19:33:38.000000 constructor-io-1.7.9/constructor_io/helpers/exception.py
--rw-r--r--   0 enes       (502) staff       (20)     4795 2023-05-10 19:05:41.000000 constructor-io-1.7.9/constructor_io/helpers/utils.py
-drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-10-26 13:49:50.008861 constructor-io-1.7.9/constructor_io/modules/
--rw-r--r--   0 enes       (502) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.7.9/constructor_io/modules/__init__.py
--rw-r--r--   0 enes       (502) staff       (20)     3976 2022-10-03 13:13:47.000000 constructor-io-1.7.9/constructor_io/modules/autocomplete.py
--rw-r--r--   0 enes       (502) staff       (20)    14881 2022-10-03 13:13:47.000000 constructor-io-1.7.9/constructor_io/modules/browse.py
--rw-r--r--   0 enes       (502) staff       (20)    17262 2022-10-21 17:16:45.000000 constructor-io-1.7.9/constructor_io/modules/catalog.py
--rw-r--r--   0 enes       (502) staff       (20)     6762 2023-04-13 18:25:13.000000 constructor-io-1.7.9/constructor_io/modules/quizzes.py
--rw-r--r--   0 enes       (502) staff       (20)     4167 2022-10-03 13:13:47.000000 constructor-io-1.7.9/constructor_io/modules/recommendations.py
--rw-r--r--   0 enes       (502) staff       (20)     4164 2023-05-10 18:53:45.000000 constructor-io-1.7.9/constructor_io/modules/search.py
--rw-r--r--   0 enes       (502) staff       (20)     3880 2023-06-21 16:51:54.000000 constructor-io-1.7.9/constructor_io/modules/tasks.py
-drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-10-26 13:49:50.006201 constructor-io-1.7.9/constructor_io.egg-info/
--rw-r--r--   0 enes       (502) staff       (20)     2562 2023-10-26 13:49:49.000000 constructor-io-1.7.9/constructor_io.egg-info/PKG-INFO
--rw-r--r--   0 enes       (502) staff       (20)      660 2023-10-26 13:49:49.000000 constructor-io-1.7.9/constructor_io.egg-info/SOURCES.txt
--rw-r--r--   0 enes       (502) staff       (20)        1 2023-10-26 13:49:49.000000 constructor-io-1.7.9/constructor_io.egg-info/dependency_links.txt
--rw-r--r--   0 enes       (502) staff       (20)       15 2023-10-26 13:49:49.000000 constructor-io-1.7.9/constructor_io.egg-info/requires.txt
--rw-r--r--   0 enes       (502) staff       (20)       15 2023-10-26 13:49:49.000000 constructor-io-1.7.9/constructor_io.egg-info/top_level.txt
--rw-r--r--   0 enes       (502) staff       (20)       38 2023-10-26 13:49:50.009385 constructor-io-1.7.9/setup.cfg
--rw-r--r--   0 enes       (502) staff       (20)      745 2022-01-10 22:25:09.000000 constructor-io-1.7.9/setup.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2024-04-12 15:22:08.429680 constructor-io-1.8.0/
+-rw-r--r--   0 enes       (502) staff       (20)     1086 2021-09-21 17:57:12.000000 constructor-io-1.8.0/LICENSE
+-rw-r--r--   0 enes       (502) staff       (20)     2562 2024-04-12 15:22:08.429479 constructor-io-1.8.0/PKG-INFO
+-rw-r--r--   0 enes       (502) staff       (20)     2198 2022-10-03 13:13:47.000000 constructor-io-1.8.0/README.md
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2024-04-12 15:22:08.424511 constructor-io-1.8.0/constructor_io/
+-rw-r--r--   0 enes       (502) staff       (20)       41 2024-04-12 15:21:54.000000 constructor-io-1.8.0/constructor_io/__init__.py
+-rw-r--r--   0 enes       (502) staff       (20)     2324 2023-06-08 14:52:00.000000 constructor-io-1.8.0/constructor_io/constructor_io.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2024-04-12 15:22:08.426334 constructor-io-1.8.0/constructor_io/helpers/
+-rw-r--r--   0 enes       (502) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.8.0/constructor_io/helpers/__init__.py
+-rw-r--r--   0 enes       (502) staff       (20)      481 2021-11-18 19:33:38.000000 constructor-io-1.8.0/constructor_io/helpers/exception.py
+-rw-r--r--   0 enes       (502) staff       (20)     4795 2023-05-10 19:05:41.000000 constructor-io-1.8.0/constructor_io/helpers/utils.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2024-04-12 15:22:08.429097 constructor-io-1.8.0/constructor_io/modules/
+-rw-r--r--   0 enes       (502) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.8.0/constructor_io/modules/__init__.py
+-rw-r--r--   0 enes       (502) staff       (20)     4767 2024-04-12 15:21:14.000000 constructor-io-1.8.0/constructor_io/modules/autocomplete.py
+-rw-r--r--   0 enes       (502) staff       (20)    14881 2022-10-03 13:13:47.000000 constructor-io-1.8.0/constructor_io/modules/browse.py
+-rw-r--r--   0 enes       (502) staff       (20)    17262 2022-10-21 17:16:45.000000 constructor-io-1.8.0/constructor_io/modules/catalog.py
+-rw-r--r--   0 enes       (502) staff       (20)     6762 2023-04-13 18:25:13.000000 constructor-io-1.8.0/constructor_io/modules/quizzes.py
+-rw-r--r--   0 enes       (502) staff       (20)     4167 2022-10-03 13:13:47.000000 constructor-io-1.8.0/constructor_io/modules/recommendations.py
+-rw-r--r--   0 enes       (502) staff       (20)     4164 2023-05-10 18:53:45.000000 constructor-io-1.8.0/constructor_io/modules/search.py
+-rw-r--r--   0 enes       (502) staff       (20)     3880 2023-06-21 16:51:54.000000 constructor-io-1.8.0/constructor_io/modules/tasks.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2024-04-12 15:22:08.425672 constructor-io-1.8.0/constructor_io.egg-info/
+-rw-r--r--   0 enes       (502) staff       (20)     2562 2024-04-12 15:22:08.000000 constructor-io-1.8.0/constructor_io.egg-info/PKG-INFO
+-rw-r--r--   0 enes       (502) staff       (20)      660 2024-04-12 15:22:08.000000 constructor-io-1.8.0/constructor_io.egg-info/SOURCES.txt
+-rw-r--r--   0 enes       (502) staff       (20)        1 2024-04-12 15:22:08.000000 constructor-io-1.8.0/constructor_io.egg-info/dependency_links.txt
+-rw-r--r--   0 enes       (502) staff       (20)       15 2024-04-12 15:22:08.000000 constructor-io-1.8.0/constructor_io.egg-info/requires.txt
+-rw-r--r--   0 enes       (502) staff       (20)       15 2024-04-12 15:22:08.000000 constructor-io-1.8.0/constructor_io.egg-info/top_level.txt
+-rw-r--r--   0 enes       (502) staff       (20)       38 2024-04-12 15:22:08.429762 constructor-io-1.8.0/setup.cfg
+-rw-r--r--   0 enes       (502) staff       (20)      745 2022-01-10 22:25:09.000000 constructor-io-1.8.0/setup.py
```

### Comparing `constructor-io-1.7.9/LICENSE` & `constructor-io-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.9/PKG-INFO` & `constructor-io-1.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: constructor-io
-Version: 1.7.9
+Version: 1.8.0
 Summary: Constructor.IO Python Client
 Home-page: https://www.constructor.io
 Author: Constructor.io
 Author-email: info@constructor.io
 License: MIT
-Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.7.9
+Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.8.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Constructor.io Python Client
 
 [![Version](https://img.shields.io/pypi/v/constructor-io.svg)](https://pypi.python.org/pypi/constructor-io)
```

### Comparing `constructor-io-1.7.9/README.md` & `constructor-io-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.9/constructor_io/constructor_io.py` & `constructor-io-1.8.0/constructor_io/constructor_io.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.9/constructor_io/helpers/utils.py` & `constructor-io-1.8.0/constructor_io/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.9/constructor_io/modules/autocomplete.py` & `constructor-io-1.8.0/constructor_io/modules/recommendations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,64 @@
-'''Autocomplete Module'''
+'''Recommendations Module'''
 
 from time import time
 from urllib.parse import quote, urlencode
 
 import requests as r
 
 from constructor_io.helpers.exception import ConstructorException
 from constructor_io.helpers.utils import (clean_params, create_auth_header,
                                           create_request_headers,
                                           create_shared_query_params,
                                           throw_http_exception_from_response)
 
 
-def _create_autocomplete_url(query, parameters, user_parameters, options):
-    # pylint: disable=too-many-branches
-    '''Create URL from supplied query (term) and parameters'''
+def _create_recommendations_url(pod_id, parameters, user_parameters, options):
+    '''Create URL from supplied parameters'''
 
     query_params = create_shared_query_params(options, parameters, user_parameters)
 
-    if not query or not isinstance(query, str):
-        raise ConstructorException('query is a required parameter of type string')
+    if not pod_id or not isinstance(pod_id, str):
+        raise ConstructorException('pod_id is a required parameter of type string')
 
     if parameters:
         if parameters.get('num_results'):
             query_params['num_results'] = parameters.get('num_results')
 
-        if parameters.get('results_per_section'):
-            for key, value in parameters.get('results_per_section').items():
-                query_params[f'num_results_{key}'] = value
+        if parameters.get('item_ids'):
+            query_params['item_id'] = parameters.get('item_ids')
+
+        if parameters.get('term'):
+            query_params['term'] = parameters.get('term')
 
     query_params['_dt'] = int(time()*1000.0)
     query_params = clean_params(query_params)
     query_string = urlencode(query_params, doseq=True)
 
-    return f'{options.get("service_url")}/autocomplete/{quote(query)}?{query_string}'
+    return f'{options.get("service_url")}/recommendations/v1/pods/{quote(pod_id)}?{query_string}'
+
+
 
-class Autocomplete:
-    # pylint: disable=too-few-public-methods
-    '''Autocomplete Class'''
+class Recommendations:
+    '''Recommendations Class'''
 
     def __init__(self, options):
         self.__options = options or {}
 
-    def get_autocomplete_results(self, query, parameters=None, user_parameters=None):
+    def get_recommendation_results(self, pod_id, parameters=None, user_parameters=None):
         '''
-        Retrieve autocomplete results from API
+        Retrieve recommendation results from API
 
-        :param str query: Autocomplete query
+        :param str pod_id: Recommendation pod identifier
         :param dict parameters: Additional parameters to refine result set
         :param int parameters.num_results: The total number of results to return
-        :param dict parameters.filters: Filters used to refine search
-        :param dict parameters.results_per_section: Number of results to return per section
-        :param list parameters.hidden_fields: Hidden metadata fields to return
+        :param str|list parameters.item_ids: Item ID(s) to retrieve recommendations for (strategy specific)
+        :param str parameters.term: The term to use to refine results (strategy specific)
+        :param dict parameters.filters: Key / value mapping of filters used to refine results
+        :param str parameters.section: The section to return results from
         :param dict parameters.variations_map: The variations map dictionary to aggregate variations. Please refer to https://docs.constructor.io/rest_api/variations_mapping for details
         :param dict user_parameters: Parameters relevant to the user request
         :param int user_parameters.session_id: Session ID, utilized to personalize results
         :param str user_parameters.client_id: Client ID, utilized to personalize results
         :param str user_parameters.user_id: User ID, utilized to personalize results
         :param str user_parameters.segments: User segments
         :param dict user_parameters.test_cells: User test cells
@@ -66,30 +69,33 @@
         '''
 
         if not parameters:
             parameters = {}
         if not user_parameters:
             user_parameters = {}
 
-        request_url = _create_autocomplete_url(query, parameters, user_parameters, self.__options)
+        request_url = _create_recommendations_url(pod_id, parameters, user_parameters, self.__options)
         requests = self.__options.get('requests') or r
 
         response = requests.get(
             request_url,
             auth=create_auth_header(self.__options),
             headers=create_request_headers(self.__options, user_parameters)
         )
 
         if not response.ok:
             throw_http_exception_from_response(response)
 
         json = response.json()
+        json_response = json.get('response')
 
-        if json.get('sections'):
-            if json.get('result_id'):
-                for section_items in json.get('sections').values():
-                    for item in section_items:
-                        item['result_id'] = json.get('result_id')
+        if json_response:
+            if json_response.get('results') or json_response.get('results') == []:
+                result_id = json.get('result_id')
+
+                if result_id:
+                    for result in json_response.get('results'):
+                        result['result_id'] = result_id
 
             return json
 
-        raise ConstructorException('get_autocomplete_results response data is malformed')
+        raise ConstructorException('get_recommendation_results response data is malformed')
```

### Comparing `constructor-io-1.7.9/constructor_io/modules/browse.py` & `constructor-io-1.8.0/constructor_io/modules/browse.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.9/constructor_io/modules/catalog.py` & `constructor-io-1.8.0/constructor_io/modules/catalog.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.9/constructor_io/modules/quizzes.py` & `constructor-io-1.8.0/constructor_io/modules/quizzes.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.9/constructor_io/modules/recommendations.py` & `constructor-io-1.8.0/constructor_io/modules/autocomplete.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,77 @@
-'''Recommendations Module'''
+'''Autocomplete Module'''
 
 from time import time
 from urllib.parse import quote, urlencode
 
 import requests as r
 
 from constructor_io.helpers.exception import ConstructorException
 from constructor_io.helpers.utils import (clean_params, create_auth_header,
                                           create_request_headers,
                                           create_shared_query_params,
                                           throw_http_exception_from_response)
 
 
-def _create_recommendations_url(pod_id, parameters, user_parameters, options):
-    '''Create URL from supplied parameters'''
+def _create_autocomplete_url(query, parameters, user_parameters, options):
+    # pylint: disable=too-many-branches
+    '''Create URL from supplied query (term) and parameters'''
 
     query_params = create_shared_query_params(options, parameters, user_parameters)
 
-    if not pod_id or not isinstance(pod_id, str):
-        raise ConstructorException('pod_id is a required parameter of type string')
+    if not query or not isinstance(query, str):
+        raise ConstructorException('query is a required parameter of type string')
 
     if parameters:
         if parameters.get('num_results'):
             query_params['num_results'] = parameters.get('num_results')
 
-        if parameters.get('item_ids'):
-            query_params['item_id'] = parameters.get('item_ids')
-
-        if parameters.get('term'):
-            query_params['term'] = parameters.get('term')
+        if parameters.get('results_per_section'):
+            for key, value in parameters.get('results_per_section').items():
+                query_params[f'num_results_{key}'] = value
+
+        if parameters.get('filters_by_section'):
+            filters = parameters.get('filters_by_section')
+            _create_autocomplete_url_filters_by_section(query_params, filters)
 
     query_params['_dt'] = int(time()*1000.0)
     query_params = clean_params(query_params)
     query_string = urlencode(query_params, doseq=True)
 
-    return f'{options.get("service_url")}/recommendations/v1/pods/{quote(pod_id)}?{query_string}'
-
-
+    return f'{options.get("service_url")}/autocomplete/{quote(query)}?{query_string}'
 
-class Recommendations:
-    '''Recommendations Class'''
+def _create_autocomplete_url_filters_by_section(query_params, filters):
+    if isinstance(filters, dict):
+        for key, value in filters.items():
+            if isinstance(value, dict):
+                for inner_key, inner_value in value.items():
+                    query_params[f'filters[{key}][{inner_key}]'] = inner_value
+            else:
+                raise ConstructorException('section\'s filters must be a dictionary')
+    else:
+        raise ConstructorException('filters must be a dictionary')
+
+class Autocomplete:
+    # pylint: disable=too-few-public-methods
+    '''Autocomplete Class'''
 
     def __init__(self, options):
         self.__options = options or {}
 
-    def get_recommendation_results(self, pod_id, parameters=None, user_parameters=None):
+    def get_autocomplete_results(self, query, parameters=None, user_parameters=None):
         '''
-        Retrieve recommendation results from API
+        Retrieve autocomplete results from API
 
-        :param str pod_id: Recommendation pod identifier
+        :param str query: Autocomplete query
         :param dict parameters: Additional parameters to refine result set
         :param int parameters.num_results: The total number of results to return
-        :param str|list parameters.item_ids: Item ID(s) to retrieve recommendations for (strategy specific)
-        :param str parameters.term: The term to use to refine results (strategy specific)
-        :param dict parameters.filters: Key / value mapping of filters used to refine results
-        :param str parameters.section: The section to return results from
+        :param dict parameters.filters: Filters used to refine search
+        :param dict parameters.filters_by_section: Filters used to refine search by section
+        :param dict parameters.results_per_section: Number of results to return per section
+        :param list parameters.hidden_fields: Hidden metadata fields to return
         :param dict parameters.variations_map: The variations map dictionary to aggregate variations. Please refer to https://docs.constructor.io/rest_api/variations_mapping for details
         :param dict user_parameters: Parameters relevant to the user request
         :param int user_parameters.session_id: Session ID, utilized to personalize results
         :param str user_parameters.client_id: Client ID, utilized to personalize results
         :param str user_parameters.user_id: User ID, utilized to personalize results
         :param str user_parameters.segments: User segments
         :param dict user_parameters.test_cells: User test cells
@@ -69,33 +82,30 @@
         '''
 
         if not parameters:
             parameters = {}
         if not user_parameters:
             user_parameters = {}
 
-        request_url = _create_recommendations_url(pod_id, parameters, user_parameters, self.__options)
+        request_url = _create_autocomplete_url(query, parameters, user_parameters, self.__options)
         requests = self.__options.get('requests') or r
 
         response = requests.get(
             request_url,
             auth=create_auth_header(self.__options),
             headers=create_request_headers(self.__options, user_parameters)
         )
 
         if not response.ok:
             throw_http_exception_from_response(response)
 
         json = response.json()
-        json_response = json.get('response')
 
-        if json_response:
-            if json_response.get('results') or json_response.get('results') == []:
-                result_id = json.get('result_id')
-
-                if result_id:
-                    for result in json_response.get('results'):
-                        result['result_id'] = result_id
+        if json.get('sections'):
+            if json.get('result_id'):
+                for section_items in json.get('sections').values():
+                    for item in section_items:
+                        item['result_id'] = json.get('result_id')
 
             return json
 
-        raise ConstructorException('get_recommendation_results response data is malformed')
+        raise ConstructorException('get_autocomplete_results response data is malformed')
```

### Comparing `constructor-io-1.7.9/constructor_io/modules/search.py` & `constructor-io-1.8.0/constructor_io/modules/search.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.9/constructor_io/modules/tasks.py` & `constructor-io-1.8.0/constructor_io/modules/tasks.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.9/constructor_io.egg-info/PKG-INFO` & `constructor-io-1.8.0/constructor_io.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: constructor-io
-Version: 1.7.9
+Version: 1.8.0
 Summary: Constructor.IO Python Client
 Home-page: https://www.constructor.io
 Author: Constructor.io
 Author-email: info@constructor.io
 License: MIT
-Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.7.9
+Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.8.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Constructor.io Python Client
 
 [![Version](https://img.shields.io/pypi/v/constructor-io.svg)](https://pypi.python.org/pypi/constructor-io)
```

### Comparing `constructor-io-1.7.9/constructor_io.egg-info/SOURCES.txt` & `constructor-io-1.8.0/constructor_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.9/setup.py` & `constructor-io-1.8.0/setup.py`

 * *Files identical despite different names*

