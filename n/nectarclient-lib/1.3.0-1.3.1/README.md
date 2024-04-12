# Comparing `tmp/nectarclient-lib-1.3.0.tar.gz` & `tmp/nectarclient-lib-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nectarclient-lib-1.3.0.tar", last modified: Thu Mar 28 02:56:35 2024, max compression
+gzip compressed data, was "nectarclient-lib-1.3.1.tar", last modified: Fri Apr 12 01:02:05 2024, max compression
```

## Comparing `nectarclient-lib-1.3.0.tar` & `nectarclient-lib-1.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-03-28 02:56:35.010579 nectarclient-lib-1.3.0/
--rw-rw-r--   0 sam       (1000) sam       (1000)    10143 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/LICENSE
--rw-rw-r--   0 sam       (1000) sam       (1000)      134 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/MANIFEST.in
--rw-rw-r--   0 sam       (1000) sam       (1000)      434 2024-03-28 02:56:35.010579 nectarclient-lib-1.3.0/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)       81 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/README.md
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-03-28 02:56:35.006579 nectarclient-lib-1.3.0/nectarclient_lib/
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    15779 2024-03-28 02:45:12.000000 nectarclient-lib-1.3.0/nectarclient_lib/base.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     5462 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/exceptions.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-03-28 02:56:35.006579 nectarclient-lib-1.3.0/nectarclient_lib/osc/
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/osc/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1476 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/osc/utils.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-03-28 02:56:35.006579 nectarclient-lib-1.3.0/nectarclient_lib/tests/
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/tests/__init__.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-03-28 02:56:35.010579 nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     6548 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/fakes.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     5935 2023-12-13 23:45:59.000000 nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/test_base.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1148 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/test_exceptions.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     3132 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/utils.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-03-28 02:56:35.006579 nectarclient-lib-1.3.0/nectarclient_lib.egg-info/
--rw-rw-r--   0 sam       (1000) sam       (1000)      434 2024-03-28 02:56:35.000000 nectarclient-lib-1.3.0/nectarclient_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)      688 2024-03-28 02:56:35.000000 nectarclient-lib-1.3.0/nectarclient_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2024-03-28 02:56:35.000000 nectarclient-lib-1.3.0/nectarclient_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-11-09 00:03:28.000000 nectarclient-lib-1.3.0/nectarclient_lib.egg-info/not-zip-safe
--rw-rw-r--   0 sam       (1000) sam       (1000)       20 2024-03-28 02:56:35.000000 nectarclient-lib-1.3.0/nectarclient_lib.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       17 2024-03-28 02:56:35.000000 nectarclient-lib-1.3.0/nectarclient_lib.egg-info/top_level.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       20 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.0/requirements.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       61 2024-03-28 02:56:35.010579 nectarclient-lib-1.3.0/setup.cfg
--rw-rw-r--   0 sam       (1000) sam       (1000)     1279 2024-03-28 02:45:12.000000 nectarclient-lib-1.3.0/setup.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-04-12 01:02:05.265826 nectarclient-lib-1.3.1/
+-rw-rw-r--   0 sam       (1000) sam       (1000)    10143 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.1/LICENSE
+-rw-rw-r--   0 sam       (1000) sam       (1000)      134 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.1/MANIFEST.in
+-rw-rw-r--   0 sam       (1000) sam       (1000)      434 2024-04-12 01:02:05.265826 nectarclient-lib-1.3.1/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)       81 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.1/README.md
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-04-12 01:02:05.261826 nectarclient-lib-1.3.1/nectarclient_lib/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.1/nectarclient_lib/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    15797 2024-04-02 23:48:32.000000 nectarclient-lib-1.3.1/nectarclient_lib/base.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     5462 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.1/nectarclient_lib/exceptions.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-04-12 01:02:05.265826 nectarclient-lib-1.3.1/nectarclient_lib/osc/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.1/nectarclient_lib/osc/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1476 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.1/nectarclient_lib/osc/utils.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-04-12 01:02:05.265826 nectarclient-lib-1.3.1/nectarclient_lib/tests/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.1/nectarclient_lib/tests/__init__.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-04-12 01:02:05.265826 nectarclient-lib-1.3.1/nectarclient_lib/tests/unit/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.1/nectarclient_lib/tests/unit/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     6548 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.1/nectarclient_lib/tests/unit/fakes.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     5935 2023-12-13 23:45:59.000000 nectarclient-lib-1.3.1/nectarclient_lib/tests/unit/test_base.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1148 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.1/nectarclient_lib/tests/unit/test_exceptions.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3132 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.1/nectarclient_lib/tests/unit/utils.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-04-12 01:02:05.265826 nectarclient-lib-1.3.1/nectarclient_lib.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      434 2024-04-12 01:02:05.000000 nectarclient-lib-1.3.1/nectarclient_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      688 2024-04-12 01:02:05.000000 nectarclient-lib-1.3.1/nectarclient_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2024-04-12 01:02:05.000000 nectarclient-lib-1.3.1/nectarclient_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-11-09 00:03:28.000000 nectarclient-lib-1.3.1/nectarclient_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 sam       (1000) sam       (1000)       20 2024-04-12 01:02:05.000000 nectarclient-lib-1.3.1/nectarclient_lib.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       17 2024-04-12 01:02:05.000000 nectarclient-lib-1.3.1/nectarclient_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       20 2023-12-13 22:55:35.000000 nectarclient-lib-1.3.1/requirements.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       61 2024-04-12 01:02:05.265826 nectarclient-lib-1.3.1/setup.cfg
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1279 2024-04-02 23:48:32.000000 nectarclient-lib-1.3.1/setup.py
```

### Comparing `nectarclient-lib-1.3.0/LICENSE` & `nectarclient-lib-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nectarclient-lib-1.3.0/nectarclient_lib/base.py` & `nectarclient-lib-1.3.1/nectarclient_lib/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
         self._add_details(info)
         self._loaded = loaded
         self.request_ids_setup()
         self.append_request_ids(resp)
 
     def _add_details(self, info):
         for (k, v) in info.items():
-            if k in self.date_fields:
+            if k in self.date_fields and v is not None:
                 parsed = False
                 for dt_format in self.DATE_FORMATS:
                     try:
                         dt = datetime.strptime(v, dt_format)
                         if dt.tzinfo:
                             dt = dt.astimezone(LOCAL_TIMEZONE)
                         setattr(self, k, dt)
```

### Comparing `nectarclient-lib-1.3.0/nectarclient_lib/exceptions.py` & `nectarclient-lib-1.3.1/nectarclient_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `nectarclient-lib-1.3.0/nectarclient_lib/osc/utils.py` & `nectarclient-lib-1.3.1/nectarclient_lib/osc/utils.py`

 * *Files identical despite different names*

### Comparing `nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/fakes.py` & `nectarclient-lib-1.3.1/nectarclient_lib/tests/unit/fakes.py`

 * *Files identical despite different names*

### Comparing `nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/test_base.py` & `nectarclient-lib-1.3.1/nectarclient_lib/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/test_exceptions.py` & `nectarclient-lib-1.3.1/nectarclient_lib/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `nectarclient-lib-1.3.0/nectarclient_lib/tests/unit/utils.py` & `nectarclient-lib-1.3.1/nectarclient_lib/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `nectarclient-lib-1.3.0/nectarclient_lib.egg-info/SOURCES.txt` & `nectarclient-lib-1.3.1/nectarclient_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nectarclient-lib-1.3.0/setup.py` & `nectarclient-lib-1.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import setuptools
 
 from pbr.packaging import parse_requirements
 
 setuptools.setup(
     name='nectarclient-lib',
-    version='1.3.0',
+    version='1.3.1',
     description=('Common lib for nectar clients'),
     author='Sam Morrison',
     author_email='sorrison@gmail.com',
     url='https://github.com/NeCTAR-RC/nectarclient-lib',
     packages=[
         'nectarclient_lib',
     ],
```

