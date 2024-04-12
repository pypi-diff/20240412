# Comparing `tmp/dgtl_pyqldb-0.1.0.tar.gz` & `tmp/dgtl_pyqldb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgtl_pyqldb-0.1.0.tar", last modified: Tue Mar  5 15:51:29 2024, max compression
+gzip compressed data, was "dgtl_pyqldb-0.1.1.tar", last modified: Fri Apr 12 14:06:01 2024, max compression
```

## Comparing `dgtl_pyqldb-0.1.0.tar` & `dgtl_pyqldb-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 olivierwitteman   (501) staff       (20)        0 2024-03-05 15:51:29.517366 dgtl_pyqldb-0.1.0/
--rw-r--r--   0 olivierwitteman   (501) staff       (20)     1079 2024-03-05 15:51:29.517017 dgtl_pyqldb-0.1.0/PKG-INFO
--rw-r--r--   0 olivierwitteman   (501) staff       (20)      828 2022-04-08 09:13:26.000000 dgtl_pyqldb-0.1.0/README.md
-drwxr-xr-x   0 olivierwitteman   (501) staff       (20)        0 2024-03-05 15:51:29.515424 dgtl_pyqldb-0.1.0/dgtl_pyqldb/
--rw-r--r--   0 olivierwitteman   (501) staff       (20)        0 2022-04-07 23:06:36.000000 dgtl_pyqldb-0.1.0/dgtl_pyqldb/__init__.py
--rw-r--r--   0 olivierwitteman   (501) staff       (20)     9677 2024-03-05 15:49:57.000000 dgtl_pyqldb-0.1.0/dgtl_pyqldb/ledger_helper.py
-drwxr-xr-x   0 olivierwitteman   (501) staff       (20)        0 2024-03-05 15:51:29.516751 dgtl_pyqldb-0.1.0/dgtl_pyqldb.egg-info/
--rw-r--r--   0 olivierwitteman   (501) staff       (20)     1079 2024-03-05 15:51:29.000000 dgtl_pyqldb-0.1.0/dgtl_pyqldb.egg-info/PKG-INFO
--rw-r--r--   0 olivierwitteman   (501) staff       (20)      245 2024-03-05 15:51:29.000000 dgtl_pyqldb-0.1.0/dgtl_pyqldb.egg-info/SOURCES.txt
--rw-r--r--   0 olivierwitteman   (501) staff       (20)        1 2024-03-05 15:51:29.000000 dgtl_pyqldb-0.1.0/dgtl_pyqldb.egg-info/dependency_links.txt
--rw-r--r--   0 olivierwitteman   (501) staff       (20)       20 2024-03-05 15:51:29.000000 dgtl_pyqldb-0.1.0/dgtl_pyqldb.egg-info/requires.txt
--rw-r--r--   0 olivierwitteman   (501) staff       (20)       12 2024-03-05 15:51:29.000000 dgtl_pyqldb-0.1.0/dgtl_pyqldb.egg-info/top_level.txt
--rw-r--r--   0 olivierwitteman   (501) staff       (20)       38 2024-03-05 15:51:29.517419 dgtl_pyqldb-0.1.0/setup.cfg
--rw-r--r--   0 olivierwitteman   (501) staff       (20)      563 2024-03-05 15:51:04.000000 dgtl_pyqldb-0.1.0/setup.py
+drwxr-xr-x   0 olivierwitteman   (501) staff       (20)        0 2024-04-12 14:06:01.106959 dgtl_pyqldb-0.1.1/
+-rw-r--r--   0 olivierwitteman   (501) staff       (20)     1079 2024-04-12 14:06:01.106609 dgtl_pyqldb-0.1.1/PKG-INFO
+-rw-r--r--   0 olivierwitteman   (501) staff       (20)      828 2022-04-08 09:13:26.000000 dgtl_pyqldb-0.1.1/README.md
+drwxr-xr-x   0 olivierwitteman   (501) staff       (20)        0 2024-04-12 14:06:01.102909 dgtl_pyqldb-0.1.1/dgtl_pyqldb/
+-rw-r--r--   0 olivierwitteman   (501) staff       (20)        0 2022-04-07 23:06:36.000000 dgtl_pyqldb-0.1.1/dgtl_pyqldb/__init__.py
+-rw-r--r--   0 olivierwitteman   (501) staff       (20)     9680 2024-04-12 14:04:49.000000 dgtl_pyqldb-0.1.1/dgtl_pyqldb/ledger_helper.py
+drwxr-xr-x   0 olivierwitteman   (501) staff       (20)        0 2024-04-12 14:06:01.106031 dgtl_pyqldb-0.1.1/dgtl_pyqldb.egg-info/
+-rw-r--r--   0 olivierwitteman   (501) staff       (20)     1079 2024-04-12 14:06:01.000000 dgtl_pyqldb-0.1.1/dgtl_pyqldb.egg-info/PKG-INFO
+-rw-r--r--   0 olivierwitteman   (501) staff       (20)      245 2024-04-12 14:06:01.000000 dgtl_pyqldb-0.1.1/dgtl_pyqldb.egg-info/SOURCES.txt
+-rw-r--r--   0 olivierwitteman   (501) staff       (20)        1 2024-04-12 14:06:01.000000 dgtl_pyqldb-0.1.1/dgtl_pyqldb.egg-info/dependency_links.txt
+-rw-r--r--   0 olivierwitteman   (501) staff       (20)       20 2024-04-12 14:06:01.000000 dgtl_pyqldb-0.1.1/dgtl_pyqldb.egg-info/requires.txt
+-rw-r--r--   0 olivierwitteman   (501) staff       (20)       12 2024-04-12 14:06:01.000000 dgtl_pyqldb-0.1.1/dgtl_pyqldb.egg-info/top_level.txt
+-rw-r--r--   0 olivierwitteman   (501) staff       (20)       38 2024-04-12 14:06:01.107019 dgtl_pyqldb-0.1.1/setup.cfg
+-rw-r--r--   0 olivierwitteman   (501) staff       (20)      563 2024-04-12 14:05:48.000000 dgtl_pyqldb-0.1.1/setup.py
```

### Comparing `dgtl_pyqldb-0.1.0/PKG-INFO` & `dgtl_pyqldb-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgtl_pyqldb
-Version: 0.1.0
+Version: 0.1.1
 Summary: AWS Quantum Ledger Database python wrapper
 Author: Olivier Witteman
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: pyqldb
 Requires-Dist: boto3
 Requires-Dist: pandas
```

### Comparing `dgtl_pyqldb-0.1.0/README.md` & `dgtl_pyqldb-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dgtl_pyqldb-0.1.0/dgtl_pyqldb/ledger_helper.py` & `dgtl_pyqldb-0.1.1/dgtl_pyqldb/ledger_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
             index = (self.index_name, data[self.index_name])
             index_value = self.convert_index(index=index)
             del data[self.index_name]
         else:
             index_value = self.convert_index(index=index)
 
         for key, value in data.items():
-            logging.info("updating ", key, value)
+            logging.info(f"updating {key}: {value}")
             self.execute_query(f"UPDATE {self.table_name} SET {key} = ? WHERE {index[0]} IN ({index_value})", query_arg=value)
 
     def remove_entry(self, data: tuple = None):
         """
          Remove an entry from the table based on the specified index.
 
          :param data: A tuple specifying the index of the entry to be removed.
```

### Comparing `dgtl_pyqldb-0.1.0/dgtl_pyqldb.egg-info/PKG-INFO` & `dgtl_pyqldb-0.1.1/dgtl_pyqldb.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgtl_pyqldb
-Version: 0.1.0
+Version: 0.1.1
 Summary: AWS Quantum Ledger Database python wrapper
 Author: Olivier Witteman
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: pyqldb
 Requires-Dist: boto3
 Requires-Dist: pandas
```

### Comparing `dgtl_pyqldb-0.1.0/setup.py` & `dgtl_pyqldb-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="dgtl_pyqldb",
-    version="0.1.0",
+    version="0.1.1",
     description="AWS Quantum Ledger Database python wrapper",
     author="Olivier Witteman",
     license="MIT",
     packages=["dgtl_pyqldb"],
     install_requires=["pyqldb",
                       "boto3",
                       "pandas"],
```

