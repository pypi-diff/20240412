# Comparing `tmp/iaptoolkit-0.0.4.1.tar.gz` & `tmp/iaptoolkit-0.0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iaptoolkit-0.0.4.1.tar", max compression
+gzip compressed data, was "iaptoolkit-0.0.4.2.tar", max compression
```

## Comparing `iaptoolkit-0.0.4.1.tar` & `iaptoolkit-0.0.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2024-03-21 07:21:57.322489 iaptoolkit-0.0.4.1/LICENSE
--rwxr-xr-x   0        0        0     1343 2024-03-21 07:21:57.322489 iaptoolkit-0.0.4.1/README.md
--rwxr-xr-x   0        0        0     1014 2024-03-21 07:21:57.322489 iaptoolkit-0.0.4.1/pyproject.toml
--rw-r--r--   0        0        0       77 2024-03-21 07:21:57.322489 iaptoolkit-0.0.4.1/src/iaptoolkit/__init__.py
--rw-r--r--   0        0        0      522 2024-03-21 07:21:57.322489 iaptoolkit-0.0.4.1/src/iaptoolkit/constants.py
--rw-r--r--   0        0        0     1507 2024-03-21 07:21:57.322489 iaptoolkit-0.0.4.1/src/iaptoolkit/exceptions.py
--rw-r--r--   0        0        0     4041 2024-03-21 07:21:57.322489 iaptoolkit-0.0.4.1/src/iaptoolkit/headers.py
--rw-r--r--   0        0        0      931 2024-03-21 07:21:57.322489 iaptoolkit-0.0.4.1/src/iaptoolkit/tokens/__init__.py
--rw-r--r--   0        0        0     7750 2024-03-21 07:21:57.322489 iaptoolkit-0.0.4.1/src/iaptoolkit/tokens/service_account.py
--rw-r--r--   0        0        0     1330 2024-03-21 07:21:57.322489 iaptoolkit-0.0.4.1/src/iaptoolkit/tokens/structs.py
--rw-r--r--   0        0        0     2689 2024-03-21 07:21:57.322489 iaptoolkit-0.0.4.1/src/iaptoolkit/tokens/token_datastore.py
--rw-r--r--   0        0        0        0 2024-03-21 07:21:57.322489 iaptoolkit-0.0.4.1/src/iaptoolkit/utils/__init__.py
--rw-r--r--   0        0        0     1477 2024-03-21 07:21:57.322489 iaptoolkit-0.0.4.1/src/iaptoolkit/utils/urls.py
--rw-r--r--   0        0        0      817 2024-03-21 07:21:57.322489 iaptoolkit-0.0.4.1/src/iaptoolkit/vars.py
--rw-r--r--   0        0        0     1934 1970-01-01 00:00:00.000000 iaptoolkit-0.0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-12 13:39:53.792785 iaptoolkit-0.0.4.2/LICENSE
+-rwxr-xr-x   0        0        0     1343 2024-04-12 13:39:53.792785 iaptoolkit-0.0.4.2/README.md
+-rwxr-xr-x   0        0        0     1014 2024-04-12 13:39:53.792785 iaptoolkit-0.0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       77 2024-04-12 13:39:53.792785 iaptoolkit-0.0.4.2/src/iaptoolkit/__init__.py
+-rw-r--r--   0        0        0      522 2024-04-12 13:39:53.792785 iaptoolkit-0.0.4.2/src/iaptoolkit/constants.py
+-rw-r--r--   0        0        0     1507 2024-04-12 13:39:53.792785 iaptoolkit-0.0.4.2/src/iaptoolkit/exceptions.py
+-rw-r--r--   0        0        0     4041 2024-04-12 13:39:53.792785 iaptoolkit-0.0.4.2/src/iaptoolkit/headers.py
+-rw-r--r--   0        0        0      931 2024-04-12 13:39:53.792785 iaptoolkit-0.0.4.2/src/iaptoolkit/tokens/__init__.py
+-rw-r--r--   0        0        0     7750 2024-04-12 13:39:53.792785 iaptoolkit-0.0.4.2/src/iaptoolkit/tokens/service_account.py
+-rw-r--r--   0        0        0     1330 2024-04-12 13:39:53.792785 iaptoolkit-0.0.4.2/src/iaptoolkit/tokens/structs.py
+-rw-r--r--   0        0        0     2689 2024-04-12 13:39:53.792785 iaptoolkit-0.0.4.2/src/iaptoolkit/tokens/token_datastore.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:39:53.792785 iaptoolkit-0.0.4.2/src/iaptoolkit/utils/__init__.py
+-rw-r--r--   0        0        0     1477 2024-04-12 13:39:53.792785 iaptoolkit-0.0.4.2/src/iaptoolkit/utils/urls.py
+-rw-r--r--   0        0        0      817 2024-04-12 13:39:53.792785 iaptoolkit-0.0.4.2/src/iaptoolkit/vars.py
+-rw-r--r--   0        0        0     1934 1970-01-01 00:00:00.000000 iaptoolkit-0.0.4.2/PKG-INFO
```

### Comparing `iaptoolkit-0.0.4.1/LICENSE` & `iaptoolkit-0.0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.1/README.md` & `iaptoolkit-0.0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.1/pyproject.toml` & `iaptoolkit-0.0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iaptoolkit"
-version = "0.0.4.1"
+version = "0.0.4.2"
 description = "Library of common utils for interacting with Identity-Aware Proxies"
 authors = ["Rob Voigt <code@ravoigt.com>"]
 readme = "README.md"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `iaptoolkit-0.0.4.1/src/iaptoolkit/constants.py` & `iaptoolkit-0.0.4.2/src/iaptoolkit/constants.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.1/src/iaptoolkit/exceptions.py` & `iaptoolkit-0.0.4.2/src/iaptoolkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.1/src/iaptoolkit/headers.py` & `iaptoolkit-0.0.4.2/src/iaptoolkit/headers.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.1/src/iaptoolkit/tokens/__init__.py` & `iaptoolkit-0.0.4.2/src/iaptoolkit/tokens/__init__.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.1/src/iaptoolkit/tokens/service_account.py` & `iaptoolkit-0.0.4.2/src/iaptoolkit/tokens/service_account.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.1/src/iaptoolkit/tokens/structs.py` & `iaptoolkit-0.0.4.2/src/iaptoolkit/tokens/structs.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.1/src/iaptoolkit/tokens/token_datastore.py` & `iaptoolkit-0.0.4.2/src/iaptoolkit/tokens/token_datastore.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.1/src/iaptoolkit/utils/urls.py` & `iaptoolkit-0.0.4.2/src/iaptoolkit/utils/urls.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.1/src/iaptoolkit/vars.py` & `iaptoolkit-0.0.4.2/src/iaptoolkit/vars.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.1/PKG-INFO` & `iaptoolkit-0.0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iaptoolkit
-Version: 0.0.4.1
+Version: 0.0.4.2
 Summary: Library of common utils for interacting with Identity-Aware Proxies
 Author: Rob Voigt
 Author-email: code@ravoigt.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

