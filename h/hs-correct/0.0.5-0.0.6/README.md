# Comparing `tmp/hs_correct-0.0.5.tar.gz` & `tmp/hs_correct-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hs_correct-0.0.5.tar", last modified: Thu Apr 11 06:16:03 2024, max compression
+gzip compressed data, was "hs_correct-0.0.6.tar", last modified: Fri Apr 12 08:02:35 2024, max compression
```

## Comparing `hs_correct-0.0.5.tar` & `hs_correct-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.634563 hs_correct-0.0.5/
--rw-rw-rw-   0        0        0      213 2024-04-10 01:56:17.000000 hs_correct-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      272 2024-04-11 06:16:03.618939 hs_correct-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      100 2024-04-01 06:28:15.000000 hs_correct-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.618939 hs_correct-0.0.5/correct/
--rw-rw-rw-   0        0        0     2871 2024-04-11 06:14:35.000000 hs_correct-0.0.5/correct/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.618939 hs_correct-0.0.5/correct/exception/
--rw-rw-rw-   0        0        0      610 2024-04-02 06:36:33.000000 hs_correct-0.0.5/correct/exception/correct_exception.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.618939 hs_correct-0.0.5/correct/funcs/
--rw-rw-rw-   0        0        0    16537 2024-04-11 06:14:35.000000 hs_correct-0.0.5/correct/funcs/alignment.py
--rw-rw-rw-   0        0        0     2122 2024-04-11 06:14:35.000000 hs_correct-0.0.5/correct/funcs/correction.py
--rw-rw-rw-   0        0        0     7035 2024-04-10 02:06:54.000000 hs_correct-0.0.5/correct/funcs/data_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.618939 hs_correct-0.0.5/correct/logger/
--rw-rw-rw-   0        0        0     1791 2024-03-19 09:58:45.000000 hs_correct-0.0.5/correct/logger/logger.py
--rw-rw-rw-   0        0        0       24 2024-04-01 08:38:32.000000 hs_correct-0.0.5/correct/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.618939 hs_correct-0.0.5/correct/response/
--rw-rw-rw-   0        0        0     1210 2024-04-02 06:36:33.000000 hs_correct-0.0.5/correct/response/response.py
--rw-rw-rw-   0        0        0      186 2024-03-29 02:44:54.000000 hs_correct-0.0.5/correct/response/response_code.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.618939 hs_correct-0.0.5/correct/tools/
--rw-rw-rw-   0        0        0      461 2024-03-29 02:14:14.000000 hs_correct-0.0.5/correct/tools/constants.py
--rw-rw-rw-   0        0        0     1632 2024-04-08 06:46:25.000000 hs_correct-0.0.5/correct/tools/min_edit_distance.py
--rw-rw-rw-   0        0        0     1625 2024-03-27 06:56:01.000000 hs_correct-0.0.5/correct/tools/point_handle.py
--rw-rw-rw-   0        0        0     2655 2024-03-27 06:56:01.000000 hs_correct-0.0.5/correct/tools/rectangle_handle.py
--rw-rw-rw-   0        0        0     5281 2024-04-10 09:31:13.000000 hs_correct-0.0.5/correct/tools/str_tools.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:16:03.618939 hs_correct-0.0.5/hs_correct.egg-info/
--rw-rw-rw-   0        0        0      272 2024-04-11 06:16:03.000000 hs_correct-0.0.5/hs_correct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      623 2024-04-11 06:16:03.000000 hs_correct-0.0.5/hs_correct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 06:16:03.000000 hs_correct-0.0.5/hs_correct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-04-11 06:16:03.000000 hs_correct-0.0.5/hs_correct.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-11 06:16:03.000000 hs_correct-0.0.5/hs_correct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2024-04-10 01:56:17.000000 hs_correct-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 06:16:03.634563 hs_correct-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      731 2024-04-11 06:15:35.000000 hs_correct-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:02:35.363043 hs_correct-0.0.6/
+-rw-rw-rw-   0        0        0      213 2024-04-10 01:56:17.000000 hs_correct-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      272 2024-04-12 08:02:35.363043 hs_correct-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      100 2024-04-01 06:28:15.000000 hs_correct-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 08:02:35.352155 hs_correct-0.0.6/correct/
+-rw-rw-rw-   0        0        0     2871 2024-04-11 06:14:35.000000 hs_correct-0.0.6/correct/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:02:35.352155 hs_correct-0.0.6/correct/exception/
+-rw-rw-rw-   0        0        0      610 2024-04-02 06:36:33.000000 hs_correct-0.0.6/correct/exception/correct_exception.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:02:35.354250 hs_correct-0.0.6/correct/funcs/
+-rw-rw-rw-   0        0        0    16537 2024-04-12 01:36:50.000000 hs_correct-0.0.6/correct/funcs/alignment.py
+-rw-rw-rw-   0        0        0     2122 2024-04-11 06:14:35.000000 hs_correct-0.0.6/correct/funcs/correction.py
+-rw-rw-rw-   0        0        0     7035 2024-04-10 02:06:54.000000 hs_correct-0.0.6/correct/funcs/data_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:02:35.354250 hs_correct-0.0.6/correct/logger/
+-rw-rw-rw-   0        0        0     1791 2024-03-19 09:58:45.000000 hs_correct-0.0.6/correct/logger/logger.py
+-rw-rw-rw-   0        0        0       24 2024-04-01 08:38:32.000000 hs_correct-0.0.6/correct/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 08:02:35.356531 hs_correct-0.0.6/correct/response/
+-rw-rw-rw-   0        0        0     1210 2024-04-02 06:36:33.000000 hs_correct-0.0.6/correct/response/response.py
+-rw-rw-rw-   0        0        0      186 2024-03-29 02:44:54.000000 hs_correct-0.0.6/correct/response/response_code.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:02:35.358535 hs_correct-0.0.6/correct/tools/
+-rw-rw-rw-   0        0        0      461 2024-03-29 02:14:14.000000 hs_correct-0.0.6/correct/tools/constants.py
+-rw-rw-rw-   0        0        0     1632 2024-04-08 06:46:25.000000 hs_correct-0.0.6/correct/tools/min_edit_distance.py
+-rw-rw-rw-   0        0        0     1625 2024-03-27 06:56:01.000000 hs_correct-0.0.6/correct/tools/point_handle.py
+-rw-rw-rw-   0        0        0     2655 2024-03-27 06:56:01.000000 hs_correct-0.0.6/correct/tools/rectangle_handle.py
+-rw-rw-rw-   0        0        0     6542 2024-04-12 07:53:28.000000 hs_correct-0.0.6/correct/tools/str_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:02:35.361904 hs_correct-0.0.6/hs_correct.egg-info/
+-rw-rw-rw-   0        0        0      272 2024-04-12 08:02:35.000000 hs_correct-0.0.6/hs_correct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2024-04-12 08:02:35.000000 hs_correct-0.0.6/hs_correct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 08:02:35.000000 hs_correct-0.0.6/hs_correct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-12 08:02:35.000000 hs_correct-0.0.6/hs_correct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 08:02:35.000000 hs_correct-0.0.6/hs_correct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2024-04-10 01:56:17.000000 hs_correct-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 08:02:35.364256 hs_correct-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      731 2024-04-12 08:00:43.000000 hs_correct-0.0.6/setup.py
```

### Comparing `hs_correct-0.0.5/correct/__init__.py` & `hs_correct-0.0.6/correct/__init__.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.5/correct/exception/correct_exception.py` & `hs_correct-0.0.6/correct/exception/correct_exception.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.5/correct/funcs/alignment.py` & `hs_correct-0.0.6/correct/funcs/alignment.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.5/correct/funcs/correction.py` & `hs_correct-0.0.6/correct/funcs/correction.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.5/correct/funcs/data_handle.py` & `hs_correct-0.0.6/correct/funcs/data_handle.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.5/correct/logger/logger.py` & `hs_correct-0.0.6/correct/logger/logger.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.5/correct/response/response.py` & `hs_correct-0.0.6/correct/response/response.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.5/correct/tools/min_edit_distance.py` & `hs_correct-0.0.6/correct/tools/min_edit_distance.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.5/correct/tools/point_handle.py` & `hs_correct-0.0.6/correct/tools/point_handle.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.5/correct/tools/rectangle_handle.py` & `hs_correct-0.0.6/correct/tools/rectangle_handle.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.5/hs_correct.egg-info/SOURCES.txt` & `hs_correct-0.0.6/hs_correct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.5/setup.py` & `hs_correct-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def parse_requirements(filename):
     line_iter = (line.strip() for line in open(filename))
     return [line for line in line_iter if line and not line.startswith("#")]
 
 
 setup(
     name='hs_correct',
-    version='0.0.5',
+    version='0.0.6',
     description='hs-correct-module',
     classifiers=[],
     keywords='hs-correct-module',
     author='zgl',
     author_email='',
     url='',
     license='MIT',
```

