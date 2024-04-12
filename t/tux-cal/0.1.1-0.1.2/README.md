# Comparing `tmp/tux_cal-0.1.1.tar.gz` & `tmp/tux_cal-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tux_cal-0.1.1.tar", max compression
+gzip compressed data, was "tux_cal-0.1.2.tar", max compression
```

## Comparing `tux_cal-0.1.1.tar` & `tux_cal-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       21 2024-04-12 21:10:26.816422 tux_cal-0.1.1/cal/__init__.py
--rw-r--r--   0        0        0     2002 2024-04-12 20:22:16.466545 tux_cal-0.1.1/cal/cal.py
--rw-r--r--   0        0        0      434 2024-04-12 21:24:23.786692 tux_cal-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      751 2024-04-12 20:53:41.019436 tux_cal-0.1.1/README.md
--rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 tux_cal-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       21 2024-04-12 21:10:26.816422 tux_cal-0.1.2/cal/__init__.py
+-rw-r--r--   0        0        0     2002 2024-04-12 20:22:16.466545 tux_cal-0.1.2/cal/cal.py
+-rw-r--r--   0        0        0      434 2024-04-12 21:26:01.474247 tux_cal-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      757 2024-04-12 21:25:57.194982 tux_cal-0.1.2/README.md
+-rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 tux_cal-0.1.2/PKG-INFO
```

### Comparing `tux_cal-0.1.1/cal/cal.py` & `tux_cal-0.1.2/cal/cal.py`

 * *Files identical despite different names*

### Comparing `tux_cal-0.1.1/README.md` & `tux_cal-0.1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 ## Installation
 
 Install Cal-Tool via pip with the following command:
 
 ```bash
 pip install cal-tool
+````
 
 # Usage
 ```bash
 cal
 ```
 
 ```bash
```

### Comparing `tux_cal-0.1.1/PKG-INFO` & `tux_cal-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tux-cal
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple calendar tool mimicking Unix 'cal' command.
 License: MIT
 Author: Estevao Fonseca
 Author-email: estevaopfon@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,15 @@
 
 ## Installation
 
 Install Cal-Tool via pip with the following command:
 
 ```bash
 pip install cal-tool
+````
 
 # Usage
 ```bash
 cal
 ```
 
 ```bash
```

