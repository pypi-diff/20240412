# Comparing `tmp/pyinclude-0.1.tar.gz` & `tmp/pyinclude-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinclude-0.1.tar", last modified: Fri Apr 12 12:06:27 2024, max compression
+gzip compressed data, was "pyinclude-0.2.tar", last modified: Fri Apr 12 12:29:07 2024, max compression
```

## Comparing `pyinclude-0.1.tar` & `pyinclude-0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 12:06:27.185630 pyinclude-0.1/
--rw-rw-rw-   0        0        0    27030 2024-04-07 15:39:33.000000 pyinclude-0.1/LICENSE
--rw-rw-rw-   0        0        0      960 2024-04-12 12:06:27.182623 pyinclude-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      545 2024-04-07 06:07:55.000000 pyinclude-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 12:06:27.141697 pyinclude-0.1/pyinclude/
--rw-rw-rw-   0        0        0     1525 2024-04-08 06:11:37.000000 pyinclude-0.1/pyinclude/__init__.py
--rw-rw-rw-   0        0        0     2181 2024-04-06 14:49:24.000000 pyinclude-0.1/pyinclude/date.py
--rw-rw-rw-   0        0        0     2154 2024-04-08 10:14:30.000000 pyinclude-0.1/pyinclude/explorer.py
--rw-rw-rw-   0        0        0     2450 2024-04-07 06:05:12.000000 pyinclude-0.1/pyinclude/math.py
--rw-rw-rw-   0        0        0     1567 2024-04-07 15:36:35.000000 pyinclude-0.1/pyinclude/savedata.py
-drwxrwxrwx   0        0        0        0 2024-04-12 12:06:27.175015 pyinclude-0.1/pyinclude.egg-info/
--rw-rw-rw-   0        0        0      960 2024-04-12 12:06:26.000000 pyinclude-0.1/pyinclude.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-12 12:06:27.000000 pyinclude-0.1/pyinclude.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 12:06:26.000000 pyinclude-0.1/pyinclude.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-12 12:06:26.000000 pyinclude-0.1/pyinclude.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-12 12:06:26.000000 pyinclude-0.1/pyinclude.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 12:06:27.185630 pyinclude-0.1/setup.cfg
--rw-rw-rw-   0        0        0      654 2024-04-12 11:39:50.000000 pyinclude-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:29:07.003830 pyinclude-0.2/
+-rw-rw-rw-   0        0        0    27030 2024-04-07 15:39:33.000000 pyinclude-0.2/LICENSE
+-rw-rw-rw-   0        0        0      960 2024-04-12 12:29:06.964368 pyinclude-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2024-04-07 06:07:55.000000 pyinclude-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 12:29:06.932519 pyinclude-0.2/pyinclude/
+-rw-rw-rw-   0        0        0     1525 2024-04-08 06:11:37.000000 pyinclude-0.2/pyinclude/__init__.py
+-rw-rw-rw-   0        0        0     2181 2024-04-06 14:49:24.000000 pyinclude-0.2/pyinclude/date.py
+-rw-rw-rw-   0        0        0     2154 2024-04-08 10:14:30.000000 pyinclude-0.2/pyinclude/explorer.py
+-rw-rw-rw-   0        0        0     2450 2024-04-07 06:05:12.000000 pyinclude-0.2/pyinclude/math.py
+-rw-rw-rw-   0        0        0     1567 2024-04-07 15:36:35.000000 pyinclude-0.2/pyinclude/savedata.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:29:06.964368 pyinclude-0.2/pyinclude.egg-info/
+-rw-rw-rw-   0        0        0      960 2024-04-12 12:29:06.000000 pyinclude-0.2/pyinclude.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-12 12:29:06.000000 pyinclude-0.2/pyinclude.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 12:29:06.000000 pyinclude-0.2/pyinclude.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-12 12:29:06.000000 pyinclude-0.2/pyinclude.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-12 12:29:06.000000 pyinclude-0.2/pyinclude.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 12:29:07.003830 pyinclude-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      654 2024-04-12 12:28:54.000000 pyinclude-0.2/setup.py
```

### Comparing `pyinclude-0.1/LICENSE` & `pyinclude-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyinclude-0.1/PKG-INFO` & `pyinclude-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinclude
-Version: 0.1
+Version: 0.2
 Summary: A collection of python codes to be easy as possible
 Home-page: https://github.com/harrymkt/pyinclude
 Author: Harry Min Khant
 Author-email: harrymk64@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyinclude-0.1/README.md` & `pyinclude-0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyinclude-0.1/pyinclude/__init__.py` & `pyinclude-0.2/pyinclude/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinclude-0.1/pyinclude/date.py` & `pyinclude-0.2/pyinclude/date.py`

 * *Files identical despite different names*

### Comparing `pyinclude-0.1/pyinclude/explorer.py` & `pyinclude-0.2/pyinclude/explorer.py`

 * *Files identical despite different names*

### Comparing `pyinclude-0.1/pyinclude/math.py` & `pyinclude-0.2/pyinclude/math.py`

 * *Files identical despite different names*

### Comparing `pyinclude-0.1/pyinclude/savedata.py` & `pyinclude-0.2/pyinclude/savedata.py`

 * *Files identical despite different names*

### Comparing `pyinclude-0.1/pyinclude.egg-info/PKG-INFO` & `pyinclude-0.2/pyinclude.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinclude
-Version: 0.1
+Version: 0.2
 Summary: A collection of python codes to be easy as possible
 Home-page: https://github.com/harrymkt/pyinclude
 Author: Harry Min Khant
 Author-email: harrymk64@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyinclude-0.1/setup.py` & `pyinclude-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the requirements from requirements.txt
 with open("requirements.txt") as f:
 	requirements = f.read().splitlines()
 
 setup(
 	name="pyinclude",
-	version="0.1",
+	version="0.2",
 	packages=find_packages(),
 	install_requires=requirements,
 	author="Harry Min Khant",
 	author_email="harrymk64@gmail.com",
 	description="A collection of python codes to be easy as possible",
 	long_description=open("README.md").read(),
 	long_description_content_type="text/markdown",
```
