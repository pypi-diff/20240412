# Comparing `tmp/pyconfman2-0.0.8.tar.gz` & `tmp/pyconfman2-0.0.9.tar.gz`

## Comparing `pyconfman2-0.0.8.tar` & `pyconfman2-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/Devs.md
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/setup.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/.github/workflows/build-and-publish-to-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/src/pyconfman2/Exceptions.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/src/pyconfman2/Schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/src/pyconfman2/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/tests/config.yaml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/tests/config.yml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/tests/test_default_config.yml
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/tests/test_schema.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/tests/test_schema_config.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/LICENSE
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pyconfman2-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/Devs.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/setup.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/.github/workflows/build-and-publish-to-pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/src/pyconfman2/Exceptions.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/src/pyconfman2/Schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/src/pyconfman2/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/tests/config.yaml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/tests/config.yml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/tests/test_default_config.yml
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/tests/test_schema.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/tests/test_schema_config.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/README.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/PKG-INFO
```

### Comparing `pyconfman2-0.0.8/src/pyconfman2/Schema.py` & `pyconfman2-0.0.9/src/pyconfman2/Schema.py`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.0.8/tests/test_schema.py` & `pyconfman2-0.0.9/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.0.8/LICENSE` & `pyconfman2-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.0.8/README.md` & `pyconfman2-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.0.8/pyproject.toml` & `pyconfman2-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyconfman2"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Phillyp Henning", email="phillyp.henning@gmail.com" },
 ]
 description = "A python package for managing YAML configuration"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pyconfman2-0.0.8/PKG-INFO` & `pyconfman2-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyconfman2
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python package for managing YAML configuration
 Project-URL: Homepage, https://github.com/PhillypHenning/python-config-parser
 Project-URL: Issues, https://github.com/PhillypHenning/python-config-parser/issues
 Author-email: Phillyp Henning <phillyp.henning@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

