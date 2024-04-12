# Comparing `tmp/fastapi-easyauth-0.0.1.tar.gz` & `tmp/fastapi-easyauth-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-easyauth-0.0.1.tar", last modified: Fri Apr  5 16:09:21 2024, max compression
+gzip compressed data, was "fastapi-easyauth-0.0.2.tar", last modified: Fri Apr 12 16:41:40 2024, max compression
```

## Comparing `fastapi-easyauth-0.0.1.tar` & `fastapi-easyauth-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-04-05 16:09:21.128998 fastapi-easyauth-0.0.1/
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     3145 2024-04-05 16:09:21.129070 fastapi-easyauth-0.0.1/PKG-INFO
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     2565 2024-04-05 15:58:15.000000 fastapi-easyauth-0.0.1/README.md
-drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-04-05 16:09:21.128296 fastapi-easyauth-0.0.1/fastapi-easyauth/
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       73 2024-04-05 15:42:05.000000 fastapi-easyauth-0.0.1/fastapi-easyauth/__init__.py
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     1305 2024-04-05 15:54:13.000000 fastapi-easyauth-0.0.1/fastapi-easyauth/easyauth.py
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      233 2024-04-04 18:40:07.000000 fastapi-easyauth-0.0.1/fastapi-easyauth/exp.py
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     3251 2024-04-05 15:41:51.000000 fastapi-easyauth-0.0.1/fastapi-easyauth/jwt.py
-drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-04-05 16:09:21.128906 fastapi-easyauth-0.0.1/fastapi_easyauth.egg-info/
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     3145 2024-04-05 16:09:21.000000 fastapi-easyauth-0.0.1/fastapi_easyauth.egg-info/PKG-INFO
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      333 2024-04-05 16:09:21.000000 fastapi-easyauth-0.0.1/fastapi_easyauth.egg-info/SOURCES.txt
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)        1 2024-04-05 16:09:21.000000 fastapi-easyauth-0.0.1/fastapi_easyauth.egg-info/dependency_links.txt
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       29 2024-04-05 16:09:21.000000 fastapi-easyauth-0.0.1/fastapi_easyauth.egg-info/requires.txt
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       17 2024-04-05 16:09:21.000000 fastapi-easyauth-0.0.1/fastapi_easyauth.egg-info/top_level.txt
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       38 2024-04-05 16:09:21.129262 fastapi-easyauth-0.0.1/setup.cfg
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      885 2024-04-05 15:58:21.000000 fastapi-easyauth-0.0.1/setup.py
+drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-04-12 16:41:40.770972 fastapi-easyauth-0.0.2/
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     3145 2024-04-12 16:41:40.771038 fastapi-easyauth-0.0.2/PKG-INFO
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     2565 2024-04-12 16:40:03.000000 fastapi-easyauth-0.0.2/README.md
+drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-04-12 16:41:40.770360 fastapi-easyauth-0.0.2/fastapi_easyauth/
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       73 2024-04-12 16:38:49.000000 fastapi-easyauth-0.0.2/fastapi_easyauth/__init__.py
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     1305 2024-04-12 16:38:49.000000 fastapi-easyauth-0.0.2/fastapi_easyauth/easyauth.py
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      233 2024-04-12 16:38:49.000000 fastapi-easyauth-0.0.2/fastapi_easyauth/exp.py
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     3251 2024-04-12 16:38:49.000000 fastapi-easyauth-0.0.2/fastapi_easyauth/jwt.py
+drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-04-12 16:41:40.770879 fastapi-easyauth-0.0.2/fastapi_easyauth.egg-info/
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     3145 2024-04-12 16:41:40.000000 fastapi-easyauth-0.0.2/fastapi_easyauth.egg-info/PKG-INFO
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      333 2024-04-12 16:41:40.000000 fastapi-easyauth-0.0.2/fastapi_easyauth.egg-info/SOURCES.txt
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)        1 2024-04-12 16:41:40.000000 fastapi-easyauth-0.0.2/fastapi_easyauth.egg-info/dependency_links.txt
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       29 2024-04-12 16:41:40.000000 fastapi-easyauth-0.0.2/fastapi_easyauth.egg-info/requires.txt
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       17 2024-04-12 16:41:40.000000 fastapi-easyauth-0.0.2/fastapi_easyauth.egg-info/top_level.txt
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       38 2024-04-12 16:41:40.771236 fastapi-easyauth-0.0.2/setup.cfg
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      885 2024-04-12 16:38:49.000000 fastapi-easyauth-0.0.2/setup.py
```

### Comparing `fastapi-easyauth-0.0.1/PKG-INFO` & `fastapi-easyauth-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-easyauth
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for quickly creating authentication using JWT and Cookies
 Home-page: https://github.com/Trejgus/fastapi-easyauth
 Author: duckduck
 Author-email: dimondtp@gmail.com
 Project-URL: GitHub, https://github.com/Trejgus/fastapi-easyauth
 Keywords: fastapi fastapi-jwt fastapi-easyauth fastapi-auth
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `fastapi-easyauth-0.0.1/README.md` & `fastapi-easyauth-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-easyauth-0.0.1/fastapi-easyauth/easyauth.py` & `fastapi-easyauth-0.0.2/fastapi_easyauth/easyauth.py`

 * *Files identical despite different names*

### Comparing `fastapi-easyauth-0.0.1/fastapi-easyauth/jwt.py` & `fastapi-easyauth-0.0.2/fastapi_easyauth/jwt.py`

 * *Files identical despite different names*

### Comparing `fastapi-easyauth-0.0.1/fastapi_easyauth.egg-info/PKG-INFO` & `fastapi-easyauth-0.0.2/fastapi_easyauth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-easyauth
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for quickly creating authentication using JWT and Cookies
 Home-page: https://github.com/Trejgus/fastapi-easyauth
 Author: duckduck
 Author-email: dimondtp@gmail.com
 Project-URL: GitHub, https://github.com/Trejgus/fastapi-easyauth
 Keywords: fastapi fastapi-jwt fastapi-easyauth fastapi-auth
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `fastapi-easyauth-0.0.1/setup.py` & `fastapi-easyauth-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='fastapi-easyauth',
-  version='0.0.1',
+  version='0.0.2',
   author='duckduck',
   author_email='dimondtp@gmail.com',
   description='A library for quickly creating authentication using JWT and Cookies',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Trejgus/fastapi-easyauth',
   packages=find_packages(),
```

