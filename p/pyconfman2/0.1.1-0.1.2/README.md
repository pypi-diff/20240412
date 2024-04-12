# Comparing `tmp/pyconfman2-0.1.1.tar.gz` & `tmp/pyconfman2-0.1.2.tar.gz`

## Comparing `pyconfman2-0.1.1.tar` & `pyconfman2-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/Devs.md
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/setup.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/.github/workflows/build-and-publish-to-pypi.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/src/pyconfman2/Exceptions.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/src/pyconfman2/Schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/src/pyconfman2/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/tests/config.yaml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/tests/config.yml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/tests/test_default_config.yml
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/tests/test_schema.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/tests/test_schema_config.yml
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/LICENSE
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 pyconfman2-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/Devs.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/setup.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/.github/workflows/build-and-publish-to-pypi.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/src/pyconfman2/Exceptions.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/src/pyconfman2/Schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/src/pyconfman2/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/tests/config.yaml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/tests/config.yml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/tests/test_default_config.yml
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/tests/test_schema.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/tests/test_schema_config.yml
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/README.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pyconfman2-0.1.2/PKG-INFO
```

### Comparing `pyconfman2-0.1.1/.github/workflows/build-and-publish-to-pypi.yml` & `pyconfman2-0.1.2/.github/workflows/build-and-publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.1/src/pyconfman2/Schema.py` & `pyconfman2-0.1.2/src/pyconfman2/Schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,7 +57,11 @@
         if not os.path.exists(filepath):
             raise FileNotFoundException
         
         with open(filepath, "r") as fh:
             config_file = yaml.safe_load(fh)
         
         self.add(config_file)
+
+    def load_as_constants(self):
+        for k in self.properties:
+            globals()[k.upper()] = self.properties[k]
```

### Comparing `pyconfman2-0.1.1/tests/test_schema.py` & `pyconfman2-0.1.2/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.1/LICENSE` & `pyconfman2-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.1/README.md` & `pyconfman2-0.1.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -9,40 +9,43 @@
 
 ## Usage
 
 ### Basic
 In it's most basic form, a Schema can be created which will load a local "config.yaml" or "config.yml" file present.
 
 ```python
-from pyconfman2 import Schema
-
-config=ConfigSchema()
+>>> from pyconfman2 import Schema
+>>> config = Schema.ConfigSchema()
+>>> print(config)
+{}
 ```
 
 ### Provide a default config
 ```python
-from pyconfman2 import Schema
-
-config=ConfigSchema({"foo": "bar"})
+>>> from pyconfman2 import Schema
+>>> config=Schema.ConfigSchema({"foo": "bar"})
+>>> print(config)
+{'foo': 'bar'}
 ```
 
 ### Specify the default config file to load
 ```python
-from pyconfman2 import Schema
-
-config=ConfigSchema(default_config="default_config.yaml")
+>>> from pyconfman2 import Schema
+>>> config=Schema.ConfigSchema(default_config="default_config.yaml")
+>>> print(config)
+{'foo': 'bar', 'zoo': {'jar': ['car', 'far']}}
 ```
 
 
 ### Specify the config file to load
 ```python
-from pyconfman2 import Schema
-
-config=ConfigSchema(filepath="another_config.yaml")
+>>> from pyconfman2 import Schema
+>>> config=Schema.ConfigSchema(default_config="default_config.yaml", filepath="another_config.yaml")
+>>> print(config)
+{'foo': 'overwritten_by_another_config', 'zoo': {'jar': ['car', 'far']}}
 ```
 
 
 ## Schema Loading breakdown
-__init__
-  1. Load the hard-coded defaults
-  2. Load (and override) using the "default config" file if present
-  3. Load (and override) using the config file if present
+1. Load the hard-coded defaults
+2. Load (and override) using the "default config" file if present
+3. Load (and override) using the config file if present
```

### Comparing `pyconfman2-0.1.1/pyproject.toml` & `pyconfman2-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyconfman2"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Phillyp Henning", email="phillyp.henning@gmail.com" },
 ]
 description = "A python package for managing YAML configuration"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pyconfman2-0.1.1/PKG-INFO` & `pyconfman2-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyconfman2
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python package for managing YAML configuration
 Project-URL: Homepage, https://github.com/PhillypHenning/python-config-parser
 Project-URL: Issues, https://github.com/PhillypHenning/python-config-parser/issues
 Author-email: Phillyp Henning <phillyp.henning@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,40 +23,43 @@
 
 ## Usage
 
 ### Basic
 In it's most basic form, a Schema can be created which will load a local "config.yaml" or "config.yml" file present.
 
 ```python
-from pyconfman2 import Schema
-
-config=ConfigSchema()
+>>> from pyconfman2 import Schema
+>>> config = Schema.ConfigSchema()
+>>> print(config)
+{}
 ```
 
 ### Provide a default config
 ```python
-from pyconfman2 import Schema
-
-config=ConfigSchema({"foo": "bar"})
+>>> from pyconfman2 import Schema
+>>> config=Schema.ConfigSchema({"foo": "bar"})
+>>> print(config)
+{'foo': 'bar'}
 ```
 
 ### Specify the default config file to load
 ```python
-from pyconfman2 import Schema
-
-config=ConfigSchema(default_config="default_config.yaml")
+>>> from pyconfman2 import Schema
+>>> config=Schema.ConfigSchema(default_config="default_config.yaml")
+>>> print(config)
+{'foo': 'bar', 'zoo': {'jar': ['car', 'far']}}
 ```
 
 
 ### Specify the config file to load
 ```python
-from pyconfman2 import Schema
-
-config=ConfigSchema(filepath="another_config.yaml")
+>>> from pyconfman2 import Schema
+>>> config=Schema.ConfigSchema(default_config="default_config.yaml", filepath="another_config.yaml")
+>>> print(config)
+{'foo': 'overwritten_by_another_config', 'zoo': {'jar': ['car', 'far']}}
 ```
 
 
 ## Schema Loading breakdown
-__init__
-  1. Load the hard-coded defaults
-  2. Load (and override) using the "default config" file if present
-  3. Load (and override) using the config file if present
+1. Load the hard-coded defaults
+2. Load (and override) using the "default config" file if present
+3. Load (and override) using the config file if present
```

