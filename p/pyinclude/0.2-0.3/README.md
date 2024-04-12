# Comparing `tmp/pyinclude-0.2.tar.gz` & `tmp/pyinclude-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinclude-0.2.tar", last modified: Fri Apr 12 12:29:07 2024, max compression
+gzip compressed data, was "pyinclude-0.3.tar", last modified: Fri Apr 12 12:38:01 2024, max compression
```

## Comparing `pyinclude-0.2.tar` & `pyinclude-0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 12:29:07.003830 pyinclude-0.2/
--rw-rw-rw-   0        0        0    27030 2024-04-07 15:39:33.000000 pyinclude-0.2/LICENSE
--rw-rw-rw-   0        0        0      960 2024-04-12 12:29:06.964368 pyinclude-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      545 2024-04-07 06:07:55.000000 pyinclude-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 12:29:06.932519 pyinclude-0.2/pyinclude/
--rw-rw-rw-   0        0        0     1525 2024-04-08 06:11:37.000000 pyinclude-0.2/pyinclude/__init__.py
--rw-rw-rw-   0        0        0     2181 2024-04-06 14:49:24.000000 pyinclude-0.2/pyinclude/date.py
--rw-rw-rw-   0        0        0     2154 2024-04-08 10:14:30.000000 pyinclude-0.2/pyinclude/explorer.py
--rw-rw-rw-   0        0        0     2450 2024-04-07 06:05:12.000000 pyinclude-0.2/pyinclude/math.py
--rw-rw-rw-   0        0        0     1567 2024-04-07 15:36:35.000000 pyinclude-0.2/pyinclude/savedata.py
-drwxrwxrwx   0        0        0        0 2024-04-12 12:29:06.964368 pyinclude-0.2/pyinclude.egg-info/
--rw-rw-rw-   0        0        0      960 2024-04-12 12:29:06.000000 pyinclude-0.2/pyinclude.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-12 12:29:06.000000 pyinclude-0.2/pyinclude.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 12:29:06.000000 pyinclude-0.2/pyinclude.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-12 12:29:06.000000 pyinclude-0.2/pyinclude.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-12 12:29:06.000000 pyinclude-0.2/pyinclude.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 12:29:07.003830 pyinclude-0.2/setup.cfg
--rw-rw-rw-   0        0        0      654 2024-04-12 12:28:54.000000 pyinclude-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:38:01.038997 pyinclude-0.3/
+-rw-rw-rw-   0        0        0    27030 2024-04-07 15:39:33.000000 pyinclude-0.3/LICENSE
+-rw-rw-rw-   0        0        0      960 2024-04-12 12:38:01.035400 pyinclude-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2024-04-07 06:07:55.000000 pyinclude-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 12:38:00.987033 pyinclude-0.3/pyinclude/
+-rw-rw-rw-   0        0        0     1525 2024-04-08 06:11:37.000000 pyinclude-0.3/pyinclude/__init__.py
+-rw-rw-rw-   0        0        0     2181 2024-04-06 14:49:24.000000 pyinclude-0.3/pyinclude/date.py
+-rw-rw-rw-   0        0        0     2154 2024-04-08 10:14:30.000000 pyinclude-0.3/pyinclude/explorer.py
+-rw-rw-rw-   0        0        0     2450 2024-04-07 06:05:12.000000 pyinclude-0.3/pyinclude/math.py
+-rw-rw-rw-   0        0        0     1567 2024-04-07 15:36:35.000000 pyinclude-0.3/pyinclude/savedata.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:38:01.030246 pyinclude-0.3/pyinclude.egg-info/
+-rw-rw-rw-   0        0        0      960 2024-04-12 12:38:00.000000 pyinclude-0.3/pyinclude.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-12 12:38:00.000000 pyinclude-0.3/pyinclude.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 12:38:00.000000 pyinclude-0.3/pyinclude.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-12 12:38:00.000000 pyinclude-0.3/pyinclude.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-12 12:38:00.000000 pyinclude-0.3/pyinclude.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 12:38:01.038997 pyinclude-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      587 2024-04-12 12:37:51.000000 pyinclude-0.3/setup.py
```

### Comparing `pyinclude-0.2/LICENSE` & `pyinclude-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyinclude-0.2/PKG-INFO` & `pyinclude-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinclude
-Version: 0.2
+Version: 0.3
 Summary: A collection of python codes to be easy as possible
 Home-page: https://github.com/harrymkt/pyinclude
 Author: Harry Min Khant
 Author-email: harrymk64@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyinclude-0.2/README.md` & `pyinclude-0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyinclude-0.2/pyinclude/__init__.py` & `pyinclude-0.3/pyinclude/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinclude-0.2/pyinclude/date.py` & `pyinclude-0.3/pyinclude/date.py`

 * *Files identical despite different names*

### Comparing `pyinclude-0.2/pyinclude/explorer.py` & `pyinclude-0.3/pyinclude/explorer.py`

 * *Files identical despite different names*

### Comparing `pyinclude-0.2/pyinclude/math.py` & `pyinclude-0.3/pyinclude/math.py`

 * *Files identical despite different names*

### Comparing `pyinclude-0.2/pyinclude/savedata.py` & `pyinclude-0.3/pyinclude/savedata.py`

 * *Files identical despite different names*

### Comparing `pyinclude-0.2/pyinclude.egg-info/PKG-INFO` & `pyinclude-0.3/pyinclude.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinclude
-Version: 0.2
+Version: 0.3
 Summary: A collection of python codes to be easy as possible
 Home-page: https://github.com/harrymkt/pyinclude
 Author: Harry Min Khant
 Author-email: harrymk64@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

