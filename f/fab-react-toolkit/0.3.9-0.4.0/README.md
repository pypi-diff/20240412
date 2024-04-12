# Comparing `tmp/fab-react-toolkit-0.3.9.tar.gz` & `tmp/fab-react-toolkit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fab-react-toolkit-0.3.9.tar", last modified: Fri Apr 12 07:31:18 2024, max compression
+gzip compressed data, was "fab-react-toolkit-0.4.0.tar", last modified: Fri Apr 12 10:57:34 2024, max compression
```

## Comparing `fab-react-toolkit-0.3.9.tar` & `fab-react-toolkit-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:31:18.040207 fab-react-toolkit-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 07:31:18.040207 fab-react-toolkit-0.3.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:31:18.036207 fab-react-toolkit-0.3.9/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:31:18.036207 fab-react-toolkit-0.3.9/example/app/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/example/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/example/app/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/example/app/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/example/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/example/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/example/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/example/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:31:18.036207 fab-react-toolkit-0.3.9/fab_react_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:31:18.036207 fab-react-toolkit-0.3.9/fab_react_toolkit/api/
--rw-r--r--   0 runner    (1001) docker     (127)    20853 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/api/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:31:18.040207 fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 07:31:18.000000 fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-12 07:31:18.000000 fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:31:18.000000 fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 07:31:18.000000 fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 07:31:18.000000 fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:31:18.040207 fab-react-toolkit-0.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:34.490649 fab-react-toolkit-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 10:57:34.490649 fab-react-toolkit-0.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:34.486649 fab-react-toolkit-0.4.0/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:34.486649 fab-react-toolkit-0.4.0/example/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/example/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/example/app/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/example/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/example/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/example/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/example/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:34.486649 fab-react-toolkit-0.4.0/fab_react_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/fab_react_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:34.486649 fab-react-toolkit-0.4.0/fab_react_toolkit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    21804 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/fab_react_toolkit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/fab_react_toolkit/api/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/fab_react_toolkit/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/fab_react_toolkit/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/fab_react_toolkit/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/fab_react_toolkit/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/fab_react_toolkit/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/fab_react_toolkit/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:34.490649 fab-react-toolkit-0.4.0/fab_react_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 10:57:34.000000 fab-react-toolkit-0.4.0/fab_react_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-12 10:57:34.000000 fab-react-toolkit-0.4.0/fab_react_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:57:34.000000 fab-react-toolkit-0.4.0/fab_react_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 10:57:34.000000 fab-react-toolkit-0.4.0/fab_react_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 10:57:34.000000 fab-react-toolkit-0.4.0/fab_react_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-12 10:57:22.000000 fab-react-toolkit-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:57:34.490649 fab-react-toolkit-0.4.0/setup.cfg
```

### Comparing `fab-react-toolkit-0.3.9/LICENSE` & `fab-react-toolkit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.9/PKG-INFO` & `fab-react-toolkit-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.3.9
+Version: 0.4.0
 Summary: A small example package
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fab-react-toolkit-0.3.9/example/app/__init__.py` & `fab-react-toolkit-0.4.0/example/app/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.9/example/app/apis.py` & `fab-react-toolkit-0.4.0/example/app/apis.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.9/example/app/config.py` & `fab-react-toolkit-0.4.0/example/app/config.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.9/example/app/models.py` & `fab-react-toolkit-0.4.0/example/app/models.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.9/example/run.py` & `fab-react-toolkit-0.4.0/example/run.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.9/fab_react_toolkit/__init__.py` & `fab-react-toolkit-0.4.0/fab_react_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.9/fab_react_toolkit/api/__init__.py` & `fab-react-toolkit-0.4.0/fab_react_toolkit/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import urllib
 from typing import Any, Callable, Optional, Dict
 import jsonschema
 import prison as prison
 from flask_appbuilder.api import BaseApi, ModelRestApi as FABModelRestApi, merge_response_func, expose, safe, rison, get_info_schema, get_item_schema
 from flask_appbuilder._compat import as_unicode
+from .utils import generate_report
 
 from flask_appbuilder.const import (
     API_ADD_COLUMNS_RES_KEY,
     API_ADD_COLUMNS_RIS_KEY,
     API_ADD_TITLE_RES_KEY,
     API_ADD_TITLE_RIS_KEY,
     API_DESCRIPTION_COLUMNS_RES_KEY,
@@ -412,14 +413,37 @@
             Returns:
                 The response from the bulk operation.
 
             """
             id_list = request.get_json()
             bulk_func = getattr(self, f"bulk_{handler}")
             return bulk_func(id_list)
+    
+    @expose("/download", methods=["POST"])
+    @protect(allow_browser_login=True)
+    @safe
+    def download(self):
+        query_params = request.json.get("queryParams", "")
+
+        query = self.datamodel.session.query(self.datamodel.obj)
+
+        
+        self._filters.clear_filters()
+
+        self._filters.rest_add_filters(query_params['filters'])
+        filters = self._filters.get_joined_filters(self._base_filters)
+
+        inner_filters = self.datamodel.get_inner_filters(filters)
+        query = self.datamodel.apply_filters(query, inner_filters)
+        result = query.yield_per(100)
+
+        response = Response(generate_report(result,self.list_columns, self.label_columns), mimetype='text/csv')
+        response.headers['Content-Type'] = 'application/octet-stream'
+        response.headers['Content-Disposition'] = 'attachment; filename={name}.csv'.format(name='appbybu')
+        return response
 
 
     @expose("/<pk>", methods=["GET"])
     @protect()
     @safe
     @permission_name("get")
     @rison(get_item_schema)
```

### Comparing `fab-react-toolkit-0.3.9/fab_react_toolkit/api/convert.py` & `fab-react-toolkit-0.4.0/fab_react_toolkit/api/convert.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.9/fab_react_toolkit/apis.py` & `fab-react-toolkit-0.4.0/fab_react_toolkit/apis.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.9/fab_react_toolkit/filters.py` & `fab-react-toolkit-0.4.0/fab_react_toolkit/filters.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.9/fab_react_toolkit/views.py` & `fab-react-toolkit-0.4.0/fab_react_toolkit/views.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/PKG-INFO` & `fab-react-toolkit-0.4.0/fab_react_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.3.9
+Version: 0.4.0
 Summary: A small example package
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/SOURCES.txt` & `fab-react-toolkit-0.4.0/fab_react_toolkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 fab_react_toolkit.egg-info/PKG-INFO
 fab_react_toolkit.egg-info/SOURCES.txt
 fab_react_toolkit.egg-info/dependency_links.txt
 fab_react_toolkit.egg-info/requires.txt
 fab_react_toolkit.egg-info/top_level.txt
 fab_react_toolkit/api/__init__.py
 fab_react_toolkit/api/convert.py
-fab_react_toolkit/api/decorators.py
+fab_react_toolkit/api/decorators.py
+fab_react_toolkit/api/utils.py
```

### Comparing `fab-react-toolkit-0.3.9/pyproject.toml` & `fab-react-toolkit-0.4.0/pyproject.toml`

 * *Files identical despite different names*

