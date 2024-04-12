# Comparing `tmp/spark_dummy_tools-0.8.2.tar.gz` & `tmp/spark_dummy_tools-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_dummy_tools-0.8.2.tar", last modified: Wed Apr  3 18:20:55 2024, max compression
+gzip compressed data, was "spark_dummy_tools-0.8.3.tar", last modified: Fri Apr 12 08:13:09 2024, max compression
```

## Comparing `spark_dummy_tools-0.8.2.tar` & `spark_dummy_tools-0.8.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 18:20:55.423539 spark_dummy_tools-0.8.2/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_dummy_tools-0.8.2/LICENSE
--rw-rw-rw-   0        0        0        4 2023-06-26 03:19:39.000000 spark_dummy_tools-0.8.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4822 2024-04-03 18:20:55.423539 spark_dummy_tools-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     4063 2023-10-02 01:12:40.000000 spark_dummy_tools-0.8.2/README.md
--rw-rw-rw-   0        0        0      471 2024-04-03 18:19:40.000000 spark_dummy_tools-0.8.2/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-04-03 18:20:55.423539 spark_dummy_tools-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-04-03 18:20:44.000000 spark_dummy_tools-0.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:20:55.392287 spark_dummy_tools-0.8.2/spark_dummy_tools/
--rw-rw-rw-   0        0        0      620 2023-08-31 23:23:15.000000 spark_dummy_tools-0.8.2/spark_dummy_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:20:55.423539 spark_dummy_tools-0.8.2/spark_dummy_tools/functions/
--rw-rw-rw-   0        0        0       75 2024-03-04 07:12:57.000000 spark_dummy_tools-0.8.2/spark_dummy_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    12861 2024-04-03 18:18:16.000000 spark_dummy_tools-0.8.2/spark_dummy_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:20:55.407913 spark_dummy_tools-0.8.2/spark_dummy_tools.egg-info/
--rw-rw-rw-   0        0        0     4822 2024-04-03 18:20:55.000000 spark_dummy_tools-0.8.2/spark_dummy_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2024-04-03 18:20:55.000000 spark_dummy_tools-0.8.2/spark_dummy_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 18:20:55.000000 spark_dummy_tools-0.8.2/spark_dummy_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-03 18:20:55.000000 spark_dummy_tools-0.8.2/spark_dummy_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-03 18:20:55.000000 spark_dummy_tools-0.8.2/spark_dummy_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 08:13:09.203852 spark_dummy_tools-0.8.3/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_dummy_tools-0.8.3/LICENSE
+-rw-rw-rw-   0        0        0        4 2023-06-26 03:19:39.000000 spark_dummy_tools-0.8.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4822 2024-04-12 08:13:09.219476 spark_dummy_tools-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4063 2023-10-02 01:12:40.000000 spark_dummy_tools-0.8.3/README.md
+-rw-rw-rw-   0        0        0      471 2024-04-04 07:10:25.000000 spark_dummy_tools-0.8.3/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-04-12 08:13:09.220469 spark_dummy_tools-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-04-12 08:13:07.000000 spark_dummy_tools-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:13:09.187047 spark_dummy_tools-0.8.3/spark_dummy_tools/
+-rw-rw-rw-   0        0        0      620 2023-08-31 23:23:15.000000 spark_dummy_tools-0.8.3/spark_dummy_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:13:09.203852 spark_dummy_tools-0.8.3/spark_dummy_tools/functions/
+-rw-rw-rw-   0        0        0       75 2024-03-04 07:12:57.000000 spark_dummy_tools-0.8.3/spark_dummy_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    13082 2024-04-12 08:13:07.000000 spark_dummy_tools-0.8.3/spark_dummy_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:13:09.203852 spark_dummy_tools-0.8.3/spark_dummy_tools.egg-info/
+-rw-rw-rw-   0        0        0     4822 2024-04-12 08:13:09.000000 spark_dummy_tools-0.8.3/spark_dummy_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2024-04-12 08:13:09.000000 spark_dummy_tools-0.8.3/spark_dummy_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 08:13:09.000000 spark_dummy_tools-0.8.3/spark_dummy_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-12 08:13:09.000000 spark_dummy_tools-0.8.3/spark_dummy_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-12 08:13:09.000000 spark_dummy_tools-0.8.3/spark_dummy_tools.egg-info/top_level.txt
```

### Comparing `spark_dummy_tools-0.8.2/LICENSE` & `spark_dummy_tools-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_dummy_tools-0.8.2/PKG-INFO` & `spark_dummy_tools-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_dummy_tools
-Version: 0.8.2
+Version: 0.8.3
 Summary: spark_dummy_tools
 Home-page: https://github.com/jonaqp/spark_dummy_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dummy_tools/archive/main.zip
 Keywords: spark,datax,schema
```

### Comparing `spark_dummy_tools-0.8.2/README.md` & `spark_dummy_tools-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `spark_dummy_tools-0.8.2/setup.py` & `spark_dummy_tools-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_dummy_tools',
     packages=find_packages(),
-    version='0.8.2',
+    version='0.8.3',
     description='spark_dummy_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_dummy_tools/',
     download_url='https://github.com/jonaqp/spark_dummy_tools/archive/main.zip',
```

### Comparing `spark_dummy_tools-0.8.2/spark_dummy_tools/__init__.py` & `spark_dummy_tools-0.8.3/spark_dummy_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_dummy_tools-0.8.2/spark_dummy_tools/functions/generator.py` & `spark_dummy_tools-0.8.3/spark_dummy_tools/functions/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     spark_schema_string = types.StructType(struct_string_list)
     return spark_schema, spark_schema_string
 
 
 def generated_dummy_table_artifactory(spark=None,
                                       uuaa_name=None,
                                       table_name=None,
+                                      table_conf=None,
                                       env="work",
                                       phase="master",
                                       code_country="pe",
                                       is_uuaa_tag=False,
                                       is_sandbox=False,
                                       token_artifactory=None,
                                       partition_colum=None,
@@ -90,19 +91,25 @@
     is_windows = sys.platform.startswith('win')
     spark.conf.set("spark.sql.debug.maxToStringFields", 5000)
     requests_environ_artifactory()
 
     path = request_path_schema_artifactory(
         table_name=table_name, uuaa_name=uuaa_name, env=env, phase=phase, code_country=code_country,
         is_uuaa_tag=is_uuaa_tag, is_sandbox=is_sandbox, token_artifactory=token_artifactory)
+    print(path)
     if path is not None:
         with open(f"{table_name}.txt", 'wb') as f:
             f.write(path.content)
-        with open(f"{table_name}.txt") as f:
-            artifactory_json = json.load(f)
+        if not table_conf:
+            with open(f"{table_name}.txt") as f:
+                artifactory_json = json.load(f)
+        else:
+            with open(f"{table_conf}") as f:
+                artifactory_json = json.load(f)
+
         table_name = artifactory_json.get("name")
         _partition_colum = artifactory_json.get("partitions")
         if _partition_colum in ("", None, np.nan, np.NaN, " "):
             _partition_colum = partition_colum or ["cutoff_date"]
         output = list()
         for _ in range(sample_parquet):
             columns_dict = dict()
```

### Comparing `spark_dummy_tools-0.8.2/spark_dummy_tools.egg-info/PKG-INFO` & `spark_dummy_tools-0.8.3/spark_dummy_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-dummy-tools
-Version: 0.8.2
+Version: 0.8.3
 Summary: spark_dummy_tools
 Home-page: https://github.com/jonaqp/spark_dummy_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dummy_tools/archive/main.zip
 Keywords: spark,datax,schema
```

