# Comparing `tmp/pyconfman2-0.0.9.tar.gz` & `tmp/pyconfman2-0.1.0.tar.gz`

## Comparing `pyconfman2-0.0.9.tar` & `pyconfman2-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/Devs.md
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/setup.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/.github/workflows/build-and-publish-to-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/src/pyconfman2/Exceptions.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/src/pyconfman2/Schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/src/pyconfman2/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/tests/__init__.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/tests/config.yaml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/tests/config.yml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/tests/test_default_config.yml
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/tests/test_schema.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/tests/test_schema_config.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/LICENSE
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pyconfman2-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/Devs.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/setup.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/.github/workflows/build-and-publish-to-pypi.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/src/pyconfman2/Exceptions.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/src/pyconfman2/Schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/src/pyconfman2/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/tests/config.yaml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/tests/config.yml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/tests/test_default_config.yml
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/tests/test_schema.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/tests/test_schema_config.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/README.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 pyconfman2-0.1.0/PKG-INFO
```

### Comparing `pyconfman2-0.0.9/.github/workflows/build-and-publish-to-pypi.yml` & `pyconfman2-0.1.0/.github/workflows/build-and-publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.0.9/src/pyconfman2/Schema.py` & `pyconfman2-0.1.0/src/pyconfman2/Schema.py`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.0.9/tests/test_schema.py` & `pyconfman2-0.1.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.0.9/LICENSE` & `pyconfman2-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.0.9/README.md` & `pyconfman2-0.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -11,37 +11,37 @@
 
 ### Basic
 In it's most basic form, a Schema can be created which will load a local "config.yaml" or "config.yml" file present.
 
 ```python
 from pyconfman2 import Schema
 
-config=Schema()
+config=ConfigSchema()
 ```
 
 ### Provide a default config
 ```python
 from pyconfman2 import Schema
 
-config=Schema({"foo": "bar"})
+config=ConfigSchema({"foo": "bar"})
 ```
 
 ### Specify the default config file to load
 ```python
 from pyconfman2 import Schema
 
-config=Schema(default_config="default_config.yaml")
+config=ConfigSchema(default_config="default_config.yaml")
 ```
 
 
 ### Specify the config file to load
 ```python
 from pyconfman2 import Schema
 
-config=Schema(filepath="another_config.yaml")
+config=ConfigSchema(filepath="another_config.yaml")
 ```
 
 
 ## Schema Loading breakdown
 __init__
   1. Load the hard-coded defaults
   2. Load (and override) using the "default config" file if present
```

### Comparing `pyconfman2-0.0.9/pyproject.toml` & `pyconfman2-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyconfman2"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Phillyp Henning", email="phillyp.henning@gmail.com" },
 ]
 description = "A python package for managing YAML configuration"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pyconfman2-0.0.9/PKG-INFO` & `pyconfman2-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyconfman2
-Version: 0.0.9
+Version: 0.1.0
 Summary: A python package for managing YAML configuration
 Project-URL: Homepage, https://github.com/PhillypHenning/python-config-parser
 Project-URL: Issues, https://github.com/PhillypHenning/python-config-parser/issues
 Author-email: Phillyp Henning <phillyp.henning@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,37 +25,37 @@
 
 ### Basic
 In it's most basic form, a Schema can be created which will load a local "config.yaml" or "config.yml" file present.
 
 ```python
 from pyconfman2 import Schema
 
-config=Schema()
+config=ConfigSchema()
 ```
 
 ### Provide a default config
 ```python
 from pyconfman2 import Schema
 
-config=Schema({"foo": "bar"})
+config=ConfigSchema({"foo": "bar"})
 ```
 
 ### Specify the default config file to load
 ```python
 from pyconfman2 import Schema
 
-config=Schema(default_config="default_config.yaml")
+config=ConfigSchema(default_config="default_config.yaml")
 ```
 
 
 ### Specify the config file to load
 ```python
 from pyconfman2 import Schema
 
-config=Schema(filepath="another_config.yaml")
+config=ConfigSchema(filepath="another_config.yaml")
 ```
 
 
 ## Schema Loading breakdown
 __init__
   1. Load the hard-coded defaults
   2. Load (and override) using the "default config" file if present
```

