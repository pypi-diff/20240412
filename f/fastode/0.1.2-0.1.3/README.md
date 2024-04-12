# Comparing `tmp/fastode-0.1.2.tar.gz` & `tmp/fastode-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fastode-0.1.2.tar", last modified: Mon Feb 13 13:13:30 2023, max compression
+gzip compressed data, was "dist\fastode-0.1.3.tar", last modified: Fri Apr 12 02:54:19 2024, max compression
```

## Comparing `fastode-0.1.2.tar` & `fastode-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-02-13 13:13:30.000000 fastode-0.1.2/
--rw-rw-rw-   0        0        0     1085 2022-09-14 07:08:58.000000 fastode-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1278 2023-02-13 13:13:30.000000 fastode-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      828 2022-09-21 09:17:46.000000 fastode-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-13 13:13:29.000000 fastode-0.1.2/fastapi/
--rw-rw-rw-   0        0        0      213 2022-11-10 07:06:52.000000 fastode-0.1.2/fastapi/__init__.py
--rw-rw-rw-   0        0        0     1360 2022-11-10 07:27:46.000000 fastode-0.1.2/fastapi/fast_baidu_translate.py
-drwxrwxrwx   0        0        0        0 2023-02-13 13:13:29.000000 fastode-0.1.2/fastode/
--rw-rw-rw-   0        0        0      370 2023-02-01 06:48:07.000000 fastode-0.1.2/fastode/__init__.py
--rw-rw-rw-   0        0        0     1938 2022-11-01 10:51:32.000000 fastode-0.1.2/fastode/fast_color.py
--rw-rw-rw-   0        0        0      364 2022-09-14 07:15:36.000000 fastode-0.1.2/fastode/fast_config.py
--rw-rw-rw-   0        0        0      790 2023-02-01 06:38:00.000000 fastode-0.1.2/fastode/fast_list.py
--rw-rw-rw-   0        0        0     1523 2022-09-14 06:57:44.000000 fastode-0.1.2/fastode/fast_log.py
--rw-rw-rw-   0        0        0     3223 2023-02-13 13:12:57.000000 fastode-0.1.2/fastode/fast_xml.py
--rw-rw-rw-   0        0        0      257 2022-10-21 05:28:16.000000 fastode-0.1.2/fastode/fast_zip.py
-drwxrwxrwx   0        0        0        0 2023-02-13 13:13:30.000000 fastode-0.1.2/fastode.egg-info/
--rw-rw-rw-   0        0        0     1278 2023-02-13 13:13:29.000000 fastode-0.1.2/fastode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-02-13 13:13:29.000000 fastode-0.1.2/fastode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-13 13:13:29.000000 fastode-0.1.2/fastode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-02-13 13:13:29.000000 fastode-0.1.2/fastode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-02-13 13:13:29.000000 fastode-0.1.2/fastode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-13 13:13:30.000000 fastode-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-02-13 13:13:17.000000 fastode-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 02:54:19.000000 fastode-0.1.3/
+-rw-rw-rw-   0        0        0     1085 2022-09-14 07:08:58.000000 fastode-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1278 2024-04-12 02:54:19.000000 fastode-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      828 2022-09-21 09:17:46.000000 fastode-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 02:54:19.000000 fastode-0.1.3/fastapi/
+-rw-rw-rw-   0        0        0      213 2022-11-10 07:06:52.000000 fastode-0.1.3/fastapi/__init__.py
+-rw-rw-rw-   0        0        0     1360 2022-11-10 07:27:46.000000 fastode-0.1.3/fastapi/fast_baidu_translate.py
+drwxrwxrwx   0        0        0        0 2024-04-12 02:54:19.000000 fastode-0.1.3/fastode/
+-rw-rw-rw-   0        0        0      370 2023-02-01 06:48:07.000000 fastode-0.1.3/fastode/__init__.py
+-rw-rw-rw-   0        0        0     1938 2022-11-01 10:51:32.000000 fastode-0.1.3/fastode/fast_color.py
+-rw-rw-rw-   0        0        0      364 2022-09-14 07:15:36.000000 fastode-0.1.3/fastode/fast_config.py
+-rw-rw-rw-   0        0        0      790 2023-02-01 06:38:00.000000 fastode-0.1.3/fastode/fast_list.py
+-rw-rw-rw-   0        0        0     1523 2022-09-14 06:57:44.000000 fastode-0.1.3/fastode/fast_log.py
+-rw-rw-rw-   0        0        0      791 2023-02-14 06:51:22.000000 fastode-0.1.3/fastode/fast_numerous_file.py
+-rw-rw-rw-   0        0        0      634 2024-04-12 02:53:28.000000 fastode-0.1.3/fastode/fast_plot.py
+-rw-rw-rw-   0        0        0     3223 2023-02-13 13:12:57.000000 fastode-0.1.3/fastode/fast_xml.py
+-rw-rw-rw-   0        0        0      305 2023-02-20 07:50:50.000000 fastode-0.1.3/fastode/fast_zip.py
+drwxrwxrwx   0        0        0        0 2024-04-12 02:54:19.000000 fastode-0.1.3/fastode.egg-info/
+-rw-rw-rw-   0        0        0     1278 2024-04-12 02:54:18.000000 fastode-0.1.3/fastode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2024-04-12 02:54:18.000000 fastode-0.1.3/fastode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 02:54:18.000000 fastode-0.1.3/fastode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-12 02:54:18.000000 fastode-0.1.3/fastode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-12 02:54:18.000000 fastode-0.1.3/fastode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 02:54:19.000000 fastode-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2024-04-12 02:54:15.000000 fastode-0.1.3/setup.py
```

### Comparing `fastode-0.1.2/LICENSE` & `fastode-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastode-0.1.2/PKG-INFO` & `fastode-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastode
-Version: 0.1.2
+Version: 0.1.3
 Summary: A toolset to help make python coding faster
 Home-page: https://github.com/zbc0315/fastode
 Author: zhang
 Author-email: zhangbc0315@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fastode-0.1.2/README.md` & `fastode-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fastode-0.1.2/fastapi/fast_baidu_translate.py` & `fastode-0.1.3/fastapi/fast_baidu_translate.py`

 * *Files identical despite different names*

### Comparing `fastode-0.1.2/fastode/fast_color.py` & `fastode-0.1.3/fastode/fast_color.py`

 * *Files identical despite different names*

### Comparing `fastode-0.1.2/fastode/fast_list.py` & `fastode-0.1.3/fastode/fast_list.py`

 * *Files identical despite different names*

### Comparing `fastode-0.1.2/fastode/fast_log.py` & `fastode-0.1.3/fastode/fast_log.py`

 * *Files identical despite different names*

### Comparing `fastode-0.1.2/fastode/fast_xml.py` & `fastode-0.1.3/fastode/fast_xml.py`

 * *Files identical despite different names*

### Comparing `fastode-0.1.2/fastode.egg-info/PKG-INFO` & `fastode-0.1.3/fastode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastode
-Version: 0.1.2
+Version: 0.1.3
 Summary: A toolset to help make python coding faster
 Home-page: https://github.com/zbc0315/fastode
 Author: zhang
 Author-email: zhangbc0315@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fastode-0.1.2/setup.py` & `fastode-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8')as f:
     long_description = f.read()
 
 setup(
     name='fastode',
-    version='0.1.2',
+    version='0.1.3',
     author='zhang',
     author_email='zhangbc0315@outlook.com',
     url='https://github.com/zbc0315/fastode',
     description=u'A toolset to help make python coding faster',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['fastode', 'fastapi'],
```

