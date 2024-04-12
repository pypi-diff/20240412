# Comparing `tmp/m3-rest-gar-1.0.8.tar.gz` & `tmp/m3-rest-gar-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3-rest-gar-1.0.8.tar", last modified: Thu Oct 21 16:51:21 2021, max compression
+gzip compressed data, was "m3-rest-gar-1.0.9.tar", last modified: Fri Oct 29 22:35:27 2021, max compression
```

## Comparing `m3-rest-gar-1.0.8.tar` & `m3-rest-gar-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-21 16:51:21.728630 m3-rest-gar-1.0.8/
--rw-r--r--   0 root         (0) root         (0)       24 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    30809 2021-10-21 16:51:21.728630 m3-rest-gar-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    30257 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-21 16:51:21.727630 m3-rest-gar-1.0.8/m3_rest_gar/
--rw-r--r--   0 root         (0) root         (0)        0 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.8/m3_rest_gar/__init__.py
--rw-r--r--   0 root         (0) root         (0)      316 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.8/m3_rest_gar/consts.py
--rw-r--r--   0 root         (0) root         (0)     3319 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.8/m3_rest_gar/filters.py
--rw-r--r--   0 root         (0) root         (0)     1563 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.8/m3_rest_gar/mixins.py
--rw-r--r--   0 root         (0) root         (0)     6961 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.8/m3_rest_gar/serializers.py
--rw-r--r--   0 root         (0) root         (0)      557 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.8/m3_rest_gar/urls.py
--rw-r--r--   0 root         (0) root         (0)     2807 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.8/m3_rest_gar/util.py
--rw-r--r--   0 root         (0) root         (0)     1819 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.8/m3_rest_gar/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-21 16:51:21.728630 m3-rest-gar-1.0.8/m3_rest_gar.egg-info/
--rw-r--r--   0 root         (0) root         (0)    30809 2021-10-21 16:51:21.000000 m3-rest-gar-1.0.8/m3_rest_gar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      401 2021-10-21 16:51:21.000000 m3-rest-gar-1.0.8/m3_rest_gar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-21 16:51:21.000000 m3-rest-gar-1.0.8/m3_rest_gar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2021-10-21 16:51:21.000000 m3-rest-gar-1.0.8/m3_rest_gar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2021-10-21 16:51:21.000000 m3-rest-gar-1.0.8/m3_rest_gar.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      105 2021-10-21 16:51:12.000000 m3-rest-gar-1.0.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-10-21 16:51:21.729630 m3-rest-gar-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      855 2021-10-21 16:51:12.000000 m3-rest-gar-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 22:35:27.572208 m3-rest-gar-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)       24 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    30809 2021-10-29 22:35:27.572208 m3-rest-gar-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    30257 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 22:35:27.569208 m3-rest-gar-1.0.9/m3_rest_gar/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.9/m3_rest_gar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      316 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.9/m3_rest_gar/consts.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.9/m3_rest_gar/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.9/m3_rest_gar/mixins.py
+-rw-r--r--   0 root         (0) root         (0)     6961 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.9/m3_rest_gar/serializers.py
+-rw-r--r--   0 root         (0) root         (0)      557 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.9/m3_rest_gar/urls.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.9/m3_rest_gar/util.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2021-10-21 16:32:21.000000 m3-rest-gar-1.0.9/m3_rest_gar/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 22:35:27.571208 m3-rest-gar-1.0.9/m3_rest_gar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    30809 2021-10-29 22:35:27.000000 m3-rest-gar-1.0.9/m3_rest_gar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      401 2021-10-29 22:35:27.000000 m3-rest-gar-1.0.9/m3_rest_gar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-10-29 22:35:27.000000 m3-rest-gar-1.0.9/m3_rest_gar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2021-10-29 22:35:27.000000 m3-rest-gar-1.0.9/m3_rest_gar.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2021-10-29 22:35:27.000000 m3-rest-gar-1.0.9/m3_rest_gar.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2021-10-29 22:35:19.000000 m3-rest-gar-1.0.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-10-29 22:35:27.572208 m3-rest-gar-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      855 2021-10-29 22:35:19.000000 m3-rest-gar-1.0.9/setup.py
```

### Comparing `m3-rest-gar-1.0.8/PKG-INFO` & `m3-rest-gar-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3-rest-gar
-Version: 1.0.8
+Version: 1.0.9
 Summary: REST-service for GAR.
 Home-page: UNKNOWN
 Author: BARS Group
 Author-email: bars@bars.group
 License: MIT
 Keywords: django rest gar
 Platform: UNKNOWN
```

### Comparing `m3-rest-gar-1.0.8/README.rst` & `m3-rest-gar-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `m3-rest-gar-1.0.8/m3_rest_gar/filters.py` & `m3-rest-gar-1.0.9/m3_rest_gar/filters.py`

 * *Files identical despite different names*

### Comparing `m3-rest-gar-1.0.8/m3_rest_gar/mixins.py` & `m3-rest-gar-1.0.9/m3_rest_gar/mixins.py`

 * *Files identical despite different names*

### Comparing `m3-rest-gar-1.0.8/m3_rest_gar/serializers.py` & `m3-rest-gar-1.0.9/m3_rest_gar/serializers.py`

 * *Files identical despite different names*

### Comparing `m3-rest-gar-1.0.8/m3_rest_gar/urls.py` & `m3-rest-gar-1.0.9/m3_rest_gar/urls.py`

 * *Files identical despite different names*

### Comparing `m3-rest-gar-1.0.8/m3_rest_gar/util.py` & `m3-rest-gar-1.0.9/m3_rest_gar/util.py`

 * *Files identical despite different names*

### Comparing `m3-rest-gar-1.0.8/m3_rest_gar/views.py` & `m3-rest-gar-1.0.9/m3_rest_gar/views.py`

 * *Files identical despite different names*

### Comparing `m3-rest-gar-1.0.8/m3_rest_gar.egg-info/PKG-INFO` & `m3-rest-gar-1.0.9/m3_rest_gar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3-rest-gar
-Version: 1.0.8
+Version: 1.0.9
 Summary: REST-service for GAR.
 Home-page: UNKNOWN
 Author: BARS Group
 Author-email: bars@bars.group
 License: MIT
 Keywords: django rest gar
 Platform: UNKNOWN
```

### Comparing `m3-rest-gar-1.0.8/setup.py` & `m3-rest-gar-1.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def read(fn):
     return codecs.open(Path(__file__).resolve().parent / fn).read()
 
 
 setup(
     name='m3-rest-gar',
-    version='1.0.8',
+    version='1.0.9',
     description=("REST-service for GAR."),
     author='BARS Group',
     author_email='bars@bars.group',
     license="MIT",
     keywords="django rest gar",
     long_description=read('README.rst'),
     packages=['m3_rest_gar'],
```

