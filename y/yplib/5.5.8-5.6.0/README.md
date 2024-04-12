# Comparing `tmp/yplib-5.5.8.tar.gz` & `tmp/yplib-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-5.5.8.tar", last modified: Wed Apr 10 06:44:51 2024, max compression
+gzip compressed data, was "dist\yplib-5.6.0.tar", last modified: Fri Apr 12 03:56:59 2024, max compression
```

## Comparing `yplib-5.5.8.tar` & `yplib-5.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 06:44:51.503811 yplib-5.5.8/
--rw-rw-rw-   0        0        0      400 2024-04-10 06:44:51.503811 yplib-5.5.8/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.5.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 06:44:51.504811 yplib-5.5.8/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-04-10 06:44:44.000000 yplib-5.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 06:44:51.496810 yplib-5.5.8/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 02:25:38.000000 yplib-5.5.8/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.5.8/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.5.8/yplib/chart_html.py
--rw-rw-rw-   0        0        0    10134 2024-03-26 08:38:02.000000 yplib-5.5.8/yplib/db.py
--rw-rw-rw-   0        0        0     5292 2023-07-17 06:31:43.000000 yplib-5.5.8/yplib/file.py
--rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.5.8/yplib/http_util.py
--rw-rw-rw-   0        0        0    40804 2024-04-10 06:44:07.000000 yplib-5.5.8/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.5.8/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.5.8/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.5.8/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.5.8/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-04-10 06:44:51.501809 yplib-5.5.8/yplib.egg-info/
--rw-rw-rw-   0        0        0      400 2024-04-10 06:44:51.000000 yplib-5.5.8/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-04-10 06:44:51.000000 yplib-5.5.8/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 06:44:51.000000 yplib-5.5.8/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-10 06:44:51.000000 yplib-5.5.8/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 03:56:59.880433 yplib-5.6.0/
+-rw-rw-rw-   0        0        0      400 2024-04-12 03:56:59.879437 yplib-5.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 03:56:59.880433 yplib-5.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-04-12 03:56:22.000000 yplib-5.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 03:56:59.872437 yplib-5.6.0/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 02:25:38.000000 yplib-5.6.0/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.6.0/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.6.0/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    10190 2024-04-12 03:50:53.000000 yplib-5.6.0/yplib/db.py
+-rw-rw-rw-   0        0        0     5292 2023-07-17 06:31:43.000000 yplib-5.6.0/yplib/file.py
+-rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.6.0/yplib/http_util.py
+-rw-rw-rw-   0        0        0    40804 2024-04-10 06:44:07.000000 yplib-5.6.0/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.6.0/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.6.0/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.6.0/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.6.0/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-04-12 03:56:59.877433 yplib-5.6.0/yplib.egg-info/
+-rw-rw-rw-   0        0        0      400 2024-04-12 03:56:59.000000 yplib-5.6.0/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-04-12 03:56:59.000000 yplib-5.6.0/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 03:56:59.000000 yplib-5.6.0/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-12 03:56:59.000000 yplib-5.6.0/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.5.8/setup.py` & `yplib-5.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.5.8",
+    version="5.6.0",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.5.8/yplib/__init__.py` & `yplib-5.6.0/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.8/yplib/chart.py` & `yplib-5.6.0/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.8/yplib/chart_html.py` & `yplib-5.6.0/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.8/yplib/db.py` & `yplib-5.6.0/yplib/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from yplib.index import *
 from yplib.http_util import *
 import pymysql
 
 
 # 有关数据库操作的类
-def get_connect(db='MoneyKing', user='moneyking_uer', passwd='3^qp3Xqt4bG7', charset='utf8mb4', port=3306, host='192.168.40.230'):
-    return pymysql.connect(db=db, user=user, passwd=passwd, charset=charset, port=port, host=host)
+def get_connect(database='MoneyKing', user='moneyking_uer', password='3^qp3Xqt4bG7', charset='utf8mb4', port=3306, host='192.168.40.230'):
+    return pymysql.connect(database=database, user=user, password=password, charset=charset, port=port, host=host)
 
 
 # 执行 sql 语句, 并且提交, 默认值提交的了
 def exec_sql(sql='', db_conn=None, db_config='stock_db', commit=True, is_log=False):
     if db_conn is None:
         config_db = get_config_data(db_config)
-        db_conn = get_connect(db=config_db['db'], user=config_db['user'], passwd=config_db['passwd'], port=config_db['port'], host=config_db['host'])
+        db_conn = get_connect(database=config_db['database'], user=config_db['user'], password=config_db['password'], port=config_db['port'], host=config_db['host'])
     if db_conn is None or sql is None or sql == '':
         if is_log:
             to_log_file("db_conn is None or sql is None or sql == '', so return")
         return
     db_cursor = db_conn.cursor()
     if isinstance(sql, list) or isinstance(sql, set):
         for s in sql:
@@ -36,15 +36,15 @@
     exec_sql(sql=sql, db_conn=db_conn, commit=False)
 
 
 # 执行 sql 获得 数据
 def get_data_from_sql(sql='', db_conn=None, db_config='stock_db', is_log=False):
     if db_conn is None:
         config_db = get_config_data(db_config)
-        db_conn = get_connect(db=config_db['db'], user=config_db['user'], passwd=config_db['passwd'], port=config_db['port'], host=config_db['host'])
+        db_conn = get_connect(database=config_db['database'], user=config_db['user'], password=config_db['password'], port=config_db['port'], host=config_db['host'])
     if db_conn is None or sql is None or sql == '':
         if is_log:
             to_log_file("db_conn is None or sql is None or sql == '', so return")
         return
     db_cursor = db_conn.cursor()
     if is_log:
         to_log_file(sql)
```

### Comparing `yplib-5.5.8/yplib/file.py` & `yplib-5.6.0/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.8/yplib/http_util.py` & `yplib-5.6.0/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.8/yplib/index.py` & `yplib-5.6.0/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.8/yplib/mail.py` & `yplib-5.6.0/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.8/yplib/mail_html.py` & `yplib-5.6.0/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.5.8/yplib/markdown.py` & `yplib-5.6.0/yplib/markdown.py`

 * *Files identical despite different names*

