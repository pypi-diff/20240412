# Comparing `tmp/spark_dataframe_tools-0.6.3.tar.gz` & `tmp/spark_dataframe_tools-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_dataframe_tools-0.6.3.tar", last modified: Wed Apr  3 19:16:56 2024, max compression
+gzip compressed data, was "spark_dataframe_tools-0.6.4.tar", last modified: Fri Apr 12 08:22:33 2024, max compression
```

## Comparing `spark_dataframe_tools-0.6.3.tar` & `spark_dataframe_tools-0.6.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:56.501481 spark_dataframe_tools-0.6.3/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.3/LICENSE
--rw-rw-rw-   0        0        0       47 2023-05-22 08:45:59.000000 spark_dataframe_tools-0.6.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2747 2024-04-03 19:16:56.501481 spark_dataframe_tools-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     1975 2023-05-22 05:38:16.000000 spark_dataframe_tools-0.6.3/README.md
--rw-rw-rw-   0        0        0      673 2023-10-01 22:03:27.000000 spark_dataframe_tools-0.6.3/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-04-03 19:16:56.501481 spark_dataframe_tools-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1177 2024-04-03 19:16:55.000000 spark_dataframe_tools-0.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:56.485854 spark_dataframe_tools-0.6.3/spark_dataframe_tools/
--rw-rw-rw-   0        0        0     2115 2023-10-01 23:43:22.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:56.501481 spark_dataframe_tools-0.6.3/spark_dataframe_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/functions/__init__.py
--rw-rw-rw-   0        0        0     3190 2023-05-22 05:14:31.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:56.501481 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:56.501481 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/templates/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/templates/__init__.py
--rw-rw-rw-   0        0        0     1861 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/templates/table.html
--rw-rw-rw-   0        0        0      416 2023-09-08 22:42:23.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_color.py
--rw-rw-rw-   0        0        0      370 2023-10-01 22:49:46.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_enviroment.py
--rw-rw-rw-   0        0        0     3244 2024-04-03 19:16:55.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_faker.py
--rw-rw-rw-   0        0        0     4777 2024-03-04 02:51:11.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_reformat_type.py
--rw-rw-rw-   0        0        0     3652 2024-04-03 18:19:12.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_session_retry.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:56.501481 spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/
--rw-rw-rw-   0        0        0     2747 2024-04-03 19:16:56.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      785 2024-04-03 19:16:56.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 19:16:56.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      195 2024-04-03 19:16:56.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-03 19:16:56.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 08:22:33.411564 spark_dataframe_tools-0.6.4/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.4/LICENSE
+-rw-rw-rw-   0        0        0       47 2023-05-22 08:45:59.000000 spark_dataframe_tools-0.6.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2747 2024-04-12 08:22:33.411564 spark_dataframe_tools-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1975 2023-05-22 05:38:16.000000 spark_dataframe_tools-0.6.4/README.md
+-rw-rw-rw-   0        0        0      673 2023-10-01 22:03:27.000000 spark_dataframe_tools-0.6.4/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-04-12 08:22:33.412566 spark_dataframe_tools-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2024-04-12 08:22:10.000000 spark_dataframe_tools-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:22:33.349892 spark_dataframe_tools-0.6.4/spark_dataframe_tools/
+-rw-rw-rw-   0        0        0     2115 2023-10-01 23:43:22.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:22:33.365364 spark_dataframe_tools-0.6.4/spark_dataframe_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0     3190 2023-05-22 05:14:31.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:22:33.405099 spark_dataframe_tools-0.6.4/spark_dataframe_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:22:33.411564 spark_dataframe_tools-0.6.4/spark_dataframe_tools/utils/templates/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools/utils/templates/__init__.py
+-rw-rw-rw-   0        0        0     1861 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools/utils/templates/table.html
+-rw-rw-rw-   0        0        0      416 2023-09-08 22:42:23.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools/utils/utils_color.py
+-rw-rw-rw-   0        0        0      370 2023-10-01 22:49:46.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools/utils/utils_enviroment.py
+-rw-rw-rw-   0        0        0     3385 2024-04-12 08:22:10.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools/utils/utils_faker.py
+-rw-rw-rw-   0        0        0     4777 2024-03-04 02:51:11.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools/utils/utils_reformat_type.py
+-rw-rw-rw-   0        0        0     3652 2024-04-03 18:19:12.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools/utils/utils_session_retry.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:22:33.365364 spark_dataframe_tools-0.6.4/spark_dataframe_tools.egg-info/
+-rw-rw-rw-   0        0        0     2747 2024-04-12 08:22:33.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2024-04-12 08:22:33.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 08:22:33.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      195 2024-04-12 08:22:33.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-12 08:22:33.000000 spark_dataframe_tools-0.6.4/spark_dataframe_tools.egg-info/top_level.txt
```

### Comparing `spark_dataframe_tools-0.6.3/LICENSE` & `spark_dataframe_tools-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.3/PKG-INFO` & `spark_dataframe_tools-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_dataframe_tools
-Version: 0.6.3
+Version: 0.6.4
 Summary: spark_dataframe_tools
 Home-page: https://github.com/jonaqp/spark_dataframe_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dataframe_tools/archive/main.zip
 Keywords: spark,dataframe
```

### Comparing `spark_dataframe_tools-0.6.3/README.md` & `spark_dataframe_tools-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.3/pyproject.toml` & `spark_dataframe_tools-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.3/setup.py` & `spark_dataframe_tools-0.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_dataframe_tools',
     packages=find_packages(),
-    version='0.6.3',
+    version='0.6.4',
     description='spark_dataframe_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_dataframe_tools/',
     download_url='https://github.com/jonaqp/spark_dataframe_tools/archive/main.zip',
```

### Comparing `spark_dataframe_tools-0.6.3/spark_dataframe_tools/__init__.py` & `spark_dataframe_tools-0.6.4/spark_dataframe_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.3/spark_dataframe_tools/functions/generator.py` & `spark_dataframe_tools-0.6.4/spark_dataframe_tools/functions/generator.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/templates/table.html` & `spark_dataframe_tools-0.6.4/spark_dataframe_tools/utils/templates/table.html`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_faker.py` & `spark_dataframe_tools-0.6.4/spark_dataframe_tools/utils/utils_faker.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,15 +53,18 @@
         else:
             d2 = datetime.today()
             d1 = d2 - relativedelta(months=1)
             _fake = str(fake.date_between(start_date=d1, end_date=d2))
     elif format.startswith("STRING"):
         if naming in ("g_entific_id",):
             _fake = fake.bothify(text='PE')
+        elif naming in ("g_entity_id",):
+            _fake = fake.bothify(text='PE0011')
         elif naming in ("gf_frequency_type", "frequency_type"):
             _fake = fake.bothify(text='?', letters='DM')
         elif naming in list(columns_string_default.keys()):
             new_text = columns_string_default[naming]
             _fake = fake.bothify(text=new_text)
         else:
-            _fake = ''.join(random.choices(string.ascii_letters + string.digits, k=int(parentheses)))
+            new_int = random.randint(1, parentheses)
+            _fake = ''.join(random.choices(string.ascii_letters + string.digits, k=int(new_int)))
     return _fake
```

### Comparing `spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_reformat_type.py` & `spark_dataframe_tools-0.6.4/spark_dataframe_tools/utils/utils_reformat_type.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_session_retry.py` & `spark_dataframe_tools-0.6.4/spark_dataframe_tools/utils/utils_session_retry.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/PKG-INFO` & `spark_dataframe_tools-0.6.4/spark_dataframe_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-dataframe-tools
-Version: 0.6.3
+Version: 0.6.4
 Summary: spark_dataframe_tools
 Home-page: https://github.com/jonaqp/spark_dataframe_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dataframe_tools/archive/main.zip
 Keywords: spark,dataframe
```

### Comparing `spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/SOURCES.txt` & `spark_dataframe_tools-0.6.4/spark_dataframe_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

