# Comparing `tmp/pyinclude-0.3.tar.gz` & `tmp/pyinclude-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinclude-0.3.tar", last modified: Fri Apr 12 12:38:01 2024, max compression
+gzip compressed data, was "pyinclude-0.4.tar", last modified: Fri Apr 12 12:40:40 2024, max compression
```

## Comparing `pyinclude-0.3.tar` & `pyinclude-0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 12:38:01.038997 pyinclude-0.3/
--rw-rw-rw-   0        0        0    27030 2024-04-07 15:39:33.000000 pyinclude-0.3/LICENSE
--rw-rw-rw-   0        0        0      960 2024-04-12 12:38:01.035400 pyinclude-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      545 2024-04-07 06:07:55.000000 pyinclude-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 12:38:00.987033 pyinclude-0.3/pyinclude/
--rw-rw-rw-   0        0        0     1525 2024-04-08 06:11:37.000000 pyinclude-0.3/pyinclude/__init__.py
--rw-rw-rw-   0        0        0     2181 2024-04-06 14:49:24.000000 pyinclude-0.3/pyinclude/date.py
--rw-rw-rw-   0        0        0     2154 2024-04-08 10:14:30.000000 pyinclude-0.3/pyinclude/explorer.py
--rw-rw-rw-   0        0        0     2450 2024-04-07 06:05:12.000000 pyinclude-0.3/pyinclude/math.py
--rw-rw-rw-   0        0        0     1567 2024-04-07 15:36:35.000000 pyinclude-0.3/pyinclude/savedata.py
-drwxrwxrwx   0        0        0        0 2024-04-12 12:38:01.030246 pyinclude-0.3/pyinclude.egg-info/
--rw-rw-rw-   0        0        0      960 2024-04-12 12:38:00.000000 pyinclude-0.3/pyinclude.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-12 12:38:00.000000 pyinclude-0.3/pyinclude.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 12:38:00.000000 pyinclude-0.3/pyinclude.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-12 12:38:00.000000 pyinclude-0.3/pyinclude.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-12 12:38:00.000000 pyinclude-0.3/pyinclude.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 12:38:01.038997 pyinclude-0.3/setup.cfg
--rw-rw-rw-   0        0        0      587 2024-04-12 12:37:51.000000 pyinclude-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:40:40.520685 pyinclude-0.4/
+-rw-rw-rw-   0        0        0    27030 2024-04-07 15:39:33.000000 pyinclude-0.4/LICENSE
+-rw-rw-rw-   0        0        0      960 2024-04-12 12:40:40.514352 pyinclude-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2024-04-07 06:07:55.000000 pyinclude-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 12:40:40.483150 pyinclude-0.4/pyinclude/
+-rw-rw-rw-   0        0        0     1525 2024-04-08 06:11:37.000000 pyinclude-0.4/pyinclude/__init__.py
+-rw-rw-rw-   0        0        0     2181 2024-04-06 14:49:24.000000 pyinclude-0.4/pyinclude/date.py
+-rw-rw-rw-   0        0        0     2154 2024-04-08 10:14:30.000000 pyinclude-0.4/pyinclude/explorer.py
+-rw-rw-rw-   0        0        0     2450 2024-04-07 06:05:12.000000 pyinclude-0.4/pyinclude/math.py
+-rw-rw-rw-   0        0        0     1567 2024-04-07 15:36:35.000000 pyinclude-0.4/pyinclude/savedata.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:40:40.511017 pyinclude-0.4/pyinclude.egg-info/
+-rw-rw-rw-   0        0        0      960 2024-04-12 12:40:40.000000 pyinclude-0.4/pyinclude.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-12 12:40:40.000000 pyinclude-0.4/pyinclude.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 12:40:40.000000 pyinclude-0.4/pyinclude.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-12 12:40:40.000000 pyinclude-0.4/pyinclude.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-12 12:40:40.000000 pyinclude-0.4/pyinclude.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 12:40:40.520685 pyinclude-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      587 2024-04-12 12:40:33.000000 pyinclude-0.4/setup.py
```

### Comparing `pyinclude-0.3/LICENSE` & `pyinclude-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyinclude-0.3/PKG-INFO` & `pyinclude-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinclude
-Version: 0.3
+Version: 0.4
 Summary: A collection of python codes to be easy as possible
 Home-page: https://github.com/harrymkt/pyinclude
 Author: Harry Min Khant
 Author-email: harrymk64@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyinclude-0.3/README.md` & `pyinclude-0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyinclude-0.3/pyinclude/__init__.py` & `pyinclude-0.4/pyinclude/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinclude-0.3/pyinclude/date.py` & `pyinclude-0.4/pyinclude/date.py`

 * *Files identical despite different names*

### Comparing `pyinclude-0.3/pyinclude/explorer.py` & `pyinclude-0.4/pyinclude/explorer.py`

 * *Files identical despite different names*

### Comparing `pyinclude-0.3/pyinclude/math.py` & `pyinclude-0.4/pyinclude/math.py`

 * *Files identical despite different names*

### Comparing `pyinclude-0.3/pyinclude/savedata.py` & `pyinclude-0.4/pyinclude/savedata.py`

 * *Files identical despite different names*

### Comparing `pyinclude-0.3/pyinclude.egg-info/PKG-INFO` & `pyinclude-0.4/pyinclude.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinclude
-Version: 0.3
+Version: 0.4
 Summary: A collection of python codes to be easy as possible
 Home-page: https://github.com/harrymkt/pyinclude
 Author: Harry Min Khant
 Author-email: harrymk64@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyinclude-0.3/setup.py` & `pyinclude-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements=[
 	"ctypes",
 	"inflect",
 	"wxpython"
 	]
 setup(
 	name="pyinclude",
-	version="0.3",
+	version="0.4",
 	packages=find_packages(),
 	install_requires=requirements,
 	author="Harry Min Khant",
 	author_email="harrymk64@gmail.com",
 	description="A collection of python codes to be easy as possible",
 	long_description=open("README.md").read(),
 	long_description_content_type="text/markdown",
```

