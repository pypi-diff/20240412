# Comparing `tmp/pyco-types-1.1.7.tar.gz` & `tmp/pyco-types-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyco-types-1.1.7.tar", last modified: Thu Apr 11 04:38:10 2024, max compression
+gzip compressed data, was "dist/pyco-types-1.1.8.tar", last modified: Fri Apr 12 09:09:56 2024, max compression
```

## Comparing `pyco-types-1.1.7.tar` & `pyco-types-1.1.8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-11 04:38:10.607056 pyco-types-1.1.7/
--rw-r--r--   0 nico       (502) staff       (20)     7651 2023-09-12 06:46:27.000000 pyco-types-1.1.7/LICENSE.txt
--rw-r--r--   0 nico       (502) staff       (20)      781 2024-04-11 04:38:10.606312 pyco-types-1.1.7/PKG-INFO
--rw-r--r--   0 nico       (502) staff       (20)       42 2023-09-11 08:05:54.000000 pyco-types-1.1.7/README.md
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-11 04:38:10.603405 pyco-types-1.1.7/pyco_types/
--rw-r--r--   0 nico       (502) staff       (20)      327 2023-09-13 03:32:10.000000 pyco-types-1.1.7/pyco_types/__init__.py
--rw-r--r--   0 nico       (502) staff       (20)     3709 2024-01-05 13:47:40.000000 pyco-types-1.1.7/pyco_types/_common.py
--rw-r--r--   0 nico       (502) staff       (20)     2109 2024-01-05 13:12:01.000000 pyco-types-1.1.7/pyco_types/_convert_meta.py
--rw-r--r--   0 nico       (502) staff       (20)     3577 2024-01-05 10:16:54.000000 pyco-types-1.1.7/pyco_types/_factory.py
--rw-r--r--   0 nico       (502) staff       (20)     6233 2024-04-11 04:36:21.000000 pyco-types-1.1.7/pyco_types/_int_exts.py
--rw-r--r--   0 nico       (502) staff       (20)      185 2024-04-11 04:23:42.000000 pyco-types-1.1.7/pyco_types/_version.py
--rw-r--r--   0 nico       (502) staff       (20)     5931 2024-02-29 09:31:06.000000 pyco-types-1.1.7/pyco_types/co_datetime.py
--rw-r--r--   0 nico       (502) staff       (20)     2573 2024-04-11 02:14:39.000000 pyco-types-1.1.7/pyco_types/co_dict.py
--rw-r--r--   0 nico       (502) staff       (20)     2651 2024-04-11 04:25:38.000000 pyco-types-1.1.7/pyco_types/co_integer.py
--rw-r--r--   0 nico       (502) staff       (20)     3755 2024-01-05 13:43:50.000000 pyco-types-1.1.7/pyco_types/co_json.py
--rw-r--r--   0 nico       (502) staff       (20)     5156 2023-09-10 03:46:01.000000 pyco-types-1.1.7/pyco_types/co_regex.py
--rw-r--r--   0 nico       (502) staff       (20)     6473 2024-01-02 13:02:23.000000 pyco-types-1.1.7/pyco_types/const.py
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-11 04:38:10.605749 pyco-types-1.1.7/pyco_types.egg-info/
--rw-r--r--   0 nico       (502) staff       (20)      781 2024-04-11 04:38:10.000000 pyco-types-1.1.7/pyco_types.egg-info/PKG-INFO
--rw-r--r--   0 nico       (502) staff       (20)      480 2024-04-11 04:38:10.000000 pyco-types-1.1.7/pyco_types.egg-info/SOURCES.txt
--rw-r--r--   0 nico       (502) staff       (20)        1 2024-04-11 04:38:10.000000 pyco-types-1.1.7/pyco_types.egg-info/dependency_links.txt
--rw-r--r--   0 nico       (502) staff       (20)       23 2024-04-11 04:38:10.000000 pyco-types-1.1.7/pyco_types.egg-info/requires.txt
--rw-r--r--   0 nico       (502) staff       (20)       11 2024-04-11 04:38:10.000000 pyco-types-1.1.7/pyco_types.egg-info/top_level.txt
--rw-r--r--   0 nico       (502) staff       (20)       38 2024-04-11 04:38:10.607276 pyco-types-1.1.7/setup.cfg
--rw-r--r--   0 nico       (502) staff       (20)     1283 2024-01-01 11:35:19.000000 pyco-types-1.1.7/setup.py
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-12 09:09:56.878771 pyco-types-1.1.8/
+-rw-r--r--   0 nico       (502) staff       (20)     7651 2023-09-12 06:46:27.000000 pyco-types-1.1.8/LICENSE.txt
+-rw-r--r--   0 nico       (502) staff       (20)      781 2024-04-12 09:09:56.878407 pyco-types-1.1.8/PKG-INFO
+-rw-r--r--   0 nico       (502) staff       (20)       42 2023-09-11 08:05:54.000000 pyco-types-1.1.8/README.md
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-12 09:09:56.875002 pyco-types-1.1.8/pyco_types/
+-rw-r--r--   0 nico       (502) staff       (20)      327 2023-09-13 03:32:10.000000 pyco-types-1.1.8/pyco_types/__init__.py
+-rw-r--r--   0 nico       (502) staff       (20)     3709 2024-01-05 13:47:40.000000 pyco-types-1.1.8/pyco_types/_common.py
+-rw-r--r--   0 nico       (502) staff       (20)     2109 2024-01-05 13:12:01.000000 pyco-types-1.1.8/pyco_types/_convert_meta.py
+-rw-r--r--   0 nico       (502) staff       (20)     4111 2024-04-12 09:01:18.000000 pyco-types-1.1.8/pyco_types/_factory.py
+-rw-r--r--   0 nico       (502) staff       (20)     6233 2024-04-11 04:36:21.000000 pyco-types-1.1.8/pyco_types/_int_exts.py
+-rw-r--r--   0 nico       (502) staff       (20)      185 2024-04-12 09:05:39.000000 pyco-types-1.1.8/pyco_types/_version.py
+-rw-r--r--   0 nico       (502) staff       (20)     5931 2024-02-29 09:31:06.000000 pyco-types-1.1.8/pyco_types/co_datetime.py
+-rw-r--r--   0 nico       (502) staff       (20)     2573 2024-04-11 02:14:39.000000 pyco-types-1.1.8/pyco_types/co_dict.py
+-rw-r--r--   0 nico       (502) staff       (20)     3141 2024-04-12 09:07:04.000000 pyco-types-1.1.8/pyco_types/co_ext_base.py
+-rw-r--r--   0 nico       (502) staff       (20)     2651 2024-04-11 04:25:38.000000 pyco-types-1.1.8/pyco_types/co_integer.py
+-rw-r--r--   0 nico       (502) staff       (20)     3755 2024-01-05 13:43:50.000000 pyco-types-1.1.8/pyco_types/co_json.py
+-rw-r--r--   0 nico       (502) staff       (20)     5156 2023-09-10 03:46:01.000000 pyco-types-1.1.8/pyco_types/co_regex.py
+-rw-r--r--   0 nico       (502) staff       (20)     6473 2024-01-02 13:02:23.000000 pyco-types-1.1.8/pyco_types/const.py
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-12 09:09:56.877934 pyco-types-1.1.8/pyco_types.egg-info/
+-rw-r--r--   0 nico       (502) staff       (20)      781 2024-04-12 09:09:56.000000 pyco-types-1.1.8/pyco_types.egg-info/PKG-INFO
+-rw-r--r--   0 nico       (502) staff       (20)      506 2024-04-12 09:09:56.000000 pyco-types-1.1.8/pyco_types.egg-info/SOURCES.txt
+-rw-r--r--   0 nico       (502) staff       (20)        1 2024-04-12 09:09:56.000000 pyco-types-1.1.8/pyco_types.egg-info/dependency_links.txt
+-rw-r--r--   0 nico       (502) staff       (20)       23 2024-04-12 09:09:56.000000 pyco-types-1.1.8/pyco_types.egg-info/requires.txt
+-rw-r--r--   0 nico       (502) staff       (20)       11 2024-04-12 09:09:56.000000 pyco-types-1.1.8/pyco_types.egg-info/top_level.txt
+-rw-r--r--   0 nico       (502) staff       (20)       38 2024-04-12 09:09:56.878937 pyco-types-1.1.8/setup.cfg
+-rw-r--r--   0 nico       (502) staff       (20)     1283 2024-01-01 11:35:19.000000 pyco-types-1.1.8/setup.py
```

### Comparing `pyco-types-1.1.7/LICENSE.txt` & `pyco-types-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.7/PKG-INFO` & `pyco-types-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyco-types
-Version: 1.1.7
+Version: 1.1.8
 Summary: pyco types: Flexible Extensionable Python Types with Converter
 Home-page: https://github.com/vmicode/pyco-types
 Author: dodoru
 Author-email: dodoru@foxmail.com
 License: GNU LGPLv3
 Keywords: pyco-types,datetime,regex-patten,converter,type-formatter
 Platform: any
```

### Comparing `pyco-types-1.1.7/pyco_types/_common.py` & `pyco-types-1.1.8/pyco_types/_common.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.7/pyco_types/_convert_meta.py` & `pyco-types-1.1.8/pyco_types/_convert_meta.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.7/pyco_types/_factory.py` & `pyco-types-1.1.8/pyco_types/_factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -99,7 +99,27 @@
         orig_vars.pop('__dict__', None)
         orig_vars.pop('__weakref__', None)
         if hasattr(cls, '__qualname__'):
             orig_vars['__qualname__'] = cls.__qualname__
         return metaclass(cls.__name__, cls.__bases__, orig_vars)
 
     return wrapper
+
+
+def wrap_base_class(*base_class):
+    """
+    @wrap_base_class(BaseClass)
+    class ParentClass():
+        def __init__(self, *args, **kwargs):
+            print("ParentClass __init__ called")
+    """
+
+    def decorator(cls):
+        class WrappedClass(cls, *base_class):
+            def __init__(self, *args, **kwargs):
+                base_class.__init__(self, *args, **kwargs)
+                if hasattr(cls, '__init__'):
+                    cls.__init__(self, *args, **kwargs)
+
+        return WrappedClass
+
+    return decorator
```

### Comparing `pyco-types-1.1.7/pyco_types/_int_exts.py` & `pyco-types-1.1.8/pyco_types/_int_exts.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.7/pyco_types/co_datetime.py` & `pyco-types-1.1.8/pyco_types/co_datetime.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.7/pyco_types/co_dict.py` & `pyco-types-1.1.8/pyco_types/co_dict.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.7/pyco_types/co_integer.py` & `pyco-types-1.1.8/pyco_types/co_integer.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.7/pyco_types/co_json.py` & `pyco-types-1.1.8/pyco_types/co_json.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.7/pyco_types/co_regex.py` & `pyco-types-1.1.8/pyco_types/co_regex.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.7/pyco_types/const.py` & `pyco-types-1.1.8/pyco_types/const.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.7/pyco_types.egg-info/PKG-INFO` & `pyco-types-1.1.8/pyco_types.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyco-types
-Version: 1.1.7
+Version: 1.1.8
 Summary: pyco types: Flexible Extensionable Python Types with Converter
 Home-page: https://github.com/vmicode/pyco-types
 Author: dodoru
 Author-email: dodoru@foxmail.com
 License: GNU LGPLv3
 Keywords: pyco-types,datetime,regex-patten,converter,type-formatter
 Platform: any
```

### Comparing `pyco-types-1.1.7/setup.py` & `pyco-types-1.1.8/setup.py`

 * *Files identical despite different names*

