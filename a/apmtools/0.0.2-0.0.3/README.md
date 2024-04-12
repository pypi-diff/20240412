# Comparing `tmp/apmtools-0.0.2.tar.gz` & `tmp/apmtools-0.0.3.tar.gz`

## Comparing `apmtools-0.0.2.tar` & `apmtools-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apmtools-0.0.2/src/apmtools/__init__.py
--rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 apmtools-0.0.2/src/apmtools/classes.py
--rw-r--r--   0        0        0    17727 2020-02-02 00:00:00.000000 apmtools-0.0.2/src/apmtools/data_processing.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 apmtools-0.0.2/src/apmtools/functions.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 apmtools-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 apmtools-0.0.2/LICENSE
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 apmtools-0.0.2/README.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 apmtools-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 apmtools-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apmtools-0.0.3/src/apmtools/__init__.py
+-rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 apmtools-0.0.3/src/apmtools/classes.py
+-rw-r--r--   0        0        0    17737 2020-02-02 00:00:00.000000 apmtools-0.0.3/src/apmtools/data_processing.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 apmtools-0.0.3/src/apmtools/functions.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 apmtools-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 apmtools-0.0.3/LICENSE
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 apmtools-0.0.3/README.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 apmtools-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 apmtools-0.0.3/PKG-INFO
```

### Comparing `apmtools-0.0.2/src/apmtools/classes.py` & `apmtools-0.0.3/src/apmtools/classes.py`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.2/src/apmtools/data_processing.py` & `apmtools-0.0.3/src/apmtools/data_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -488,15 +488,15 @@
                'p_2_5_um_b',
                'p_5_0_um_b',
                'p_10_0_um_b']
     files = [i for i in os.listdir(directory) if i.split(".")[-1] == "csv"]
     if len(files)==0:
         print("there are no csv files in directory "+directory)
         return
-    files = [pd.read_csv(i) for i in files]
+    files = [pd.read_csv(directory+i) for i in files]
     df = pd.concat(files)
     if len(df["mac_address"].value_counts()) != 1:
         print("there is more than one or less than one mac address on directory "+directory)
         return
     df['UTCDateTime'] = df['UTCDateTime'].map(to_datetime)
     df.set_index('UTCDateTime', inplace=True)
     if df.index.value_counts().max() != 1:
```

### Comparing `apmtools-0.0.2/src/apmtools/functions.py` & `apmtools-0.0.3/src/apmtools/functions.py`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.2/LICENSE` & `apmtools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.2/pyproject.toml` & `apmtools-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "apmtools"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Federico Lorenzetti", email="lorenzetti.federico@gmail.com" },
 ]
 description = "A collection of tools for processing air pollution monitoring data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `apmtools-0.0.2/PKG-INFO` & `apmtools-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: apmtools
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of tools for processing air pollution monitoring data
 Project-URL: Homepage, https://github.com/federlorenz/apmtools
 Author-email: Federico Lorenzetti <lorenzetti.federico@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

