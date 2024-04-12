# Comparing `tmp/spark_dataframe_tools-0.6.5.tar.gz` & `tmp/spark_dataframe_tools-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_dataframe_tools-0.6.5.tar", last modified: Fri Apr 12 08:29:36 2024, max compression
+gzip compressed data, was "spark_dataframe_tools-0.6.6.tar", last modified: Fri Apr 12 09:05:40 2024, max compression
```

## Comparing `spark_dataframe_tools-0.6.5.tar` & `spark_dataframe_tools-0.6.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 08:29:36.320881 spark_dataframe_tools-0.6.5/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.5/LICENSE
--rw-rw-rw-   0        0        0       47 2023-05-22 08:45:59.000000 spark_dataframe_tools-0.6.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2747 2024-04-12 08:29:36.320881 spark_dataframe_tools-0.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     1975 2023-05-22 05:38:16.000000 spark_dataframe_tools-0.6.5/README.md
--rw-rw-rw-   0        0        0      673 2023-10-01 22:03:27.000000 spark_dataframe_tools-0.6.5/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-04-12 08:29:36.320881 spark_dataframe_tools-0.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1177 2024-04-12 08:29:35.000000 spark_dataframe_tools-0.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:29:36.304238 spark_dataframe_tools-0.6.5/spark_dataframe_tools/
--rw-rw-rw-   0        0        0     2115 2023-10-01 23:43:22.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:29:36.320881 spark_dataframe_tools-0.6.5/spark_dataframe_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools/functions/__init__.py
--rw-rw-rw-   0        0        0     3190 2023-05-22 05:14:31.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:29:36.320881 spark_dataframe_tools-0.6.5/spark_dataframe_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:29:36.320881 spark_dataframe_tools-0.6.5/spark_dataframe_tools/utils/templates/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools/utils/templates/__init__.py
--rw-rw-rw-   0        0        0     1861 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools/utils/templates/table.html
--rw-rw-rw-   0        0        0      416 2023-09-08 22:42:23.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools/utils/utils_color.py
--rw-rw-rw-   0        0        0      370 2023-10-01 22:49:46.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools/utils/utils_enviroment.py
--rw-rw-rw-   0        0        0     3390 2024-04-12 08:29:35.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools/utils/utils_faker.py
--rw-rw-rw-   0        0        0     4777 2024-03-04 02:51:11.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools/utils/utils_reformat_type.py
--rw-rw-rw-   0        0        0     3652 2024-04-03 18:19:12.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools/utils/utils_session_retry.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:29:36.320881 spark_dataframe_tools-0.6.5/spark_dataframe_tools.egg-info/
--rw-rw-rw-   0        0        0     2747 2024-04-12 08:29:36.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      785 2024-04-12 08:29:36.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 08:29:36.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      195 2024-04-12 08:29:36.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-12 08:29:36.000000 spark_dataframe_tools-0.6.5/spark_dataframe_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 09:05:40.528272 spark_dataframe_tools-0.6.6/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.6/LICENSE
+-rw-rw-rw-   0        0        0       47 2023-05-22 08:45:59.000000 spark_dataframe_tools-0.6.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2747 2024-04-12 09:05:40.528272 spark_dataframe_tools-0.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1975 2023-05-22 05:38:16.000000 spark_dataframe_tools-0.6.6/README.md
+-rw-rw-rw-   0        0        0      673 2023-10-01 22:03:27.000000 spark_dataframe_tools-0.6.6/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-04-12 09:05:40.528272 spark_dataframe_tools-0.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2024-04-12 09:05:39.000000 spark_dataframe_tools-0.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:05:40.511808 spark_dataframe_tools-0.6.6/spark_dataframe_tools/
+-rw-rw-rw-   0        0        0     2115 2023-10-01 23:43:22.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:05:40.528272 spark_dataframe_tools-0.6.6/spark_dataframe_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0     3190 2023-05-22 05:14:31.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:05:40.528272 spark_dataframe_tools-0.6.6/spark_dataframe_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:05:40.528272 spark_dataframe_tools-0.6.6/spark_dataframe_tools/utils/templates/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools/utils/templates/__init__.py
+-rw-rw-rw-   0        0        0     1861 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools/utils/templates/table.html
+-rw-rw-rw-   0        0        0      416 2023-09-08 22:42:23.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools/utils/utils_color.py
+-rw-rw-rw-   0        0        0      370 2023-10-01 22:49:46.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools/utils/utils_enviroment.py
+-rw-rw-rw-   0        0        0     3686 2024-04-12 09:05:17.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools/utils/utils_faker.py
+-rw-rw-rw-   0        0        0     4777 2024-03-04 02:51:11.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools/utils/utils_reformat_type.py
+-rw-rw-rw-   0        0        0     3652 2024-04-03 18:19:12.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools/utils/utils_session_retry.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:05:40.528272 spark_dataframe_tools-0.6.6/spark_dataframe_tools.egg-info/
+-rw-rw-rw-   0        0        0     2747 2024-04-12 09:05:40.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2024-04-12 09:05:40.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 09:05:40.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      195 2024-04-12 09:05:40.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-12 09:05:40.000000 spark_dataframe_tools-0.6.6/spark_dataframe_tools.egg-info/top_level.txt
```

### Comparing `spark_dataframe_tools-0.6.5/LICENSE` & `spark_dataframe_tools-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.5/PKG-INFO` & `spark_dataframe_tools-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_dataframe_tools
-Version: 0.6.5
+Version: 0.6.6
 Summary: spark_dataframe_tools
 Home-page: https://github.com/jonaqp/spark_dataframe_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dataframe_tools/archive/main.zip
 Keywords: spark,dataframe
```

### Comparing `spark_dataframe_tools-0.6.5/README.md` & `spark_dataframe_tools-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.5/pyproject.toml` & `spark_dataframe_tools-0.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.5/setup.py` & `spark_dataframe_tools-0.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_dataframe_tools',
     packages=find_packages(),
-    version='0.6.5',
+    version='0.6.6',
     description='spark_dataframe_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_dataframe_tools/',
     download_url='https://github.com/jonaqp/spark_dataframe_tools/archive/main.zip',
```

### Comparing `spark_dataframe_tools-0.6.5/spark_dataframe_tools/__init__.py` & `spark_dataframe_tools-0.6.6/spark_dataframe_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.5/spark_dataframe_tools/functions/generator.py` & `spark_dataframe_tools-0.6.6/spark_dataframe_tools/functions/generator.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.5/spark_dataframe_tools/utils/templates/table.html` & `spark_dataframe_tools-0.6.6/spark_dataframe_tools/utils/templates/table.html`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.5/spark_dataframe_tools/utils/utils_faker.py` & `spark_dataframe_tools-0.6.6/spark_dataframe_tools/utils/utils_faker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import numpy as np
+
+
 def faker_generated_data(naming=None,
                          format=None,
                          parentheses=None,
                          columns_integer_default=None,
                          columns_date_default=None,
                          columns_string_default=None,
                          columns_decimal_default=None
@@ -61,10 +64,18 @@
             _fake = fake.bothify(text='PE0011')
         elif naming in ("gf_frequency_type", "frequency_type"):
             _fake = fake.bothify(text='?', letters='DM')
         elif naming in list(columns_string_default.keys()):
             new_text = columns_string_default[naming]
             _fake = fake.bothify(text=new_text)
         else:
-            new_int = random.randint(1, int(parentheses))
+            parentheses2 = 5
+            if parentheses in ("", None, np.NaN, 0, "0"):
+                parentheses2 = 5
+            if int(parentheses) > parentheses2:
+                parentheses2 = 5
+            else:
+                parentheses2 = parentheses
+
+            new_int = random.randint(1, int(parentheses2))
             _fake = ''.join(random.choices(string.ascii_letters + string.digits, k=int(new_int)))
     return _fake
```

### Comparing `spark_dataframe_tools-0.6.5/spark_dataframe_tools/utils/utils_reformat_type.py` & `spark_dataframe_tools-0.6.6/spark_dataframe_tools/utils/utils_reformat_type.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.5/spark_dataframe_tools/utils/utils_session_retry.py` & `spark_dataframe_tools-0.6.6/spark_dataframe_tools/utils/utils_session_retry.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.5/spark_dataframe_tools.egg-info/PKG-INFO` & `spark_dataframe_tools-0.6.6/spark_dataframe_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-dataframe-tools
-Version: 0.6.5
+Version: 0.6.6
 Summary: spark_dataframe_tools
 Home-page: https://github.com/jonaqp/spark_dataframe_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dataframe_tools/archive/main.zip
 Keywords: spark,dataframe
```

### Comparing `spark_dataframe_tools-0.6.5/spark_dataframe_tools.egg-info/SOURCES.txt` & `spark_dataframe_tools-0.6.6/spark_dataframe_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

