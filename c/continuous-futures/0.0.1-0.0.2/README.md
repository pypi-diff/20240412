# Comparing `tmp/continuous_futures-0.0.1.tar.gz` & `tmp/continuous_futures-0.0.2.tar.gz`

## Comparing `continuous_futures-0.0.1.tar` & `continuous_futures-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 continuous_futures-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 continuous_futures-0.0.1/src/continuous_futures/__init__.py
--rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 continuous_futures-0.0.1/src/continuous_futures/continuous_futures.py
--rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 continuous_futures-0.0.1/tests/test_continuous.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 continuous_futures-0.0.1/tests/test_documentation.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 continuous_futures-0.0.1/tests/test_rollover_indexes.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 continuous_futures-0.0.1/.gitignore
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 continuous_futures-0.0.1/LICENSE
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 continuous_futures-0.0.1/README.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 continuous_futures-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 continuous_futures-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 continuous_futures-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 continuous_futures-0.0.2/src/continuous_futures/__init__.py
+-rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 continuous_futures-0.0.2/src/continuous_futures/continuous_futures.py
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 continuous_futures-0.0.2/tests/test_continuous.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 continuous_futures-0.0.2/tests/test_documentation.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 continuous_futures-0.0.2/tests/test_rollover_indexes.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 continuous_futures-0.0.2/.gitignore
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 continuous_futures-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 continuous_futures-0.0.2/README.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 continuous_futures-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 continuous_futures-0.0.2/PKG-INFO
```

### Comparing `continuous_futures-0.0.1/src/continuous_futures/continuous_futures.py` & `continuous_futures-0.0.2/src/continuous_futures/continuous_futures.py`

 * *Files identical despite different names*

### Comparing `continuous_futures-0.0.1/tests/test_continuous.py` & `continuous_futures-0.0.2/tests/test_continuous.py`

 * *Files identical despite different names*

### Comparing `continuous_futures-0.0.1/tests/test_documentation.py` & `continuous_futures-0.0.2/tests/test_documentation.py`

 * *Files identical despite different names*

### Comparing `continuous_futures-0.0.1/tests/test_rollover_indexes.py` & `continuous_futures-0.0.2/tests/test_rollover_indexes.py`

 * *Files identical despite different names*

### Comparing `continuous_futures-0.0.1/.gitignore` & `continuous_futures-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `continuous_futures-0.0.1/LICENSE` & `continuous_futures-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `continuous_futures-0.0.1/README.md` & `continuous_futures-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `continuous_futures-0.0.1/pyproject.toml` & `continuous_futures-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "continuous_futures"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Felix Steiner", email="f@fxstr.com" },
 ]
 description = "Converts single future contracts to a continuous contract (ratio back-adjusted)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `continuous_futures-0.0.1/PKG-INFO` & `continuous_futures-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: continuous_futures
-Version: 0.0.1
+Version: 0.0.2
 Summary: Converts single future contracts to a continuous contract (ratio back-adjusted)
 Project-URL: Homepage, https://github.com/fxstr/continuous_futures
 Project-URL: Bug Tracker, https://github.com/fxstr/continuous_futures/issues
 Author-email: Felix Steiner <f@fxstr.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
```

