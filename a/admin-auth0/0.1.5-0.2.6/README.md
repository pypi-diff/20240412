# Comparing `tmp/admin_auth0-0.1.5.tar.gz` & `tmp/admin_auth0-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admin_auth0-0.1.5.tar", max compression
+gzip compressed data, was "admin_auth0-0.2.6.tar", max compression
```

## Comparing `admin_auth0-0.1.5.tar` & `admin_auth0-0.2.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      258 2024-02-06 19:26:25.373020 admin_auth0-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-02-06 19:26:25.373020 admin_auth0-0.1.5/admin_auth0/__init__.py
--rw-r--r--   0        0        0      632 2024-02-06 19:26:25.373020 admin_auth0-0.1.5/admin_auth0/auth0.py
--rw-r--r--   0        0        0     2127 2024-02-06 19:26:25.373020 admin_auth0-0.1.5/admin_auth0/authentication.py
--rw-r--r--   0        0        0      236 2024-02-06 19:26:25.373020 admin_auth0-0.1.5/admin_auth0/urls.py
--rw-r--r--   0        0        0     1344 2024-02-06 19:26:25.373020 admin_auth0-0.1.5/admin_auth0/views.py
--rw-r--r--   0        0        0      395 2024-02-06 19:26:25.373020 admin_auth0-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 admin_auth0-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      258 2024-04-12 15:04:26.711020 admin_auth0-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 15:04:26.711020 admin_auth0-0.2.6/admin_auth0/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-12 15:04:26.711020 admin_auth0-0.2.6/admin_auth0/auth0.py
+-rw-r--r--   0        0        0     2127 2024-04-12 15:04:26.711020 admin_auth0-0.2.6/admin_auth0/authentication.py
+-rw-r--r--   0        0        0      236 2024-04-12 15:04:26.711020 admin_auth0-0.2.6/admin_auth0/urls.py
+-rw-r--r--   0        0        0     1344 2024-04-12 15:04:26.711020 admin_auth0-0.2.6/admin_auth0/views.py
+-rw-r--r--   0        0        0      393 2024-04-12 15:04:26.711020 admin_auth0-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 admin_auth0-0.2.6/PKG-INFO
```

### Comparing `admin_auth0-0.1.5/admin_auth0/auth0.py` & `admin_auth0-0.2.6/admin_auth0/auth0.py`

 * *Files identical despite different names*

### Comparing `admin_auth0-0.1.5/admin_auth0/authentication.py` & `admin_auth0-0.2.6/admin_auth0/authentication.py`

 * *Files identical despite different names*

### Comparing `admin_auth0-0.1.5/admin_auth0/views.py` & `admin_auth0-0.2.6/admin_auth0/views.py`

 * *Files identical despite different names*

### Comparing `admin_auth0-0.1.5/PKG-INFO` & `admin_auth0-0.2.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: admin_auth0
-Version: 0.1.5
+Version: 0.2.6
 Summary: 
 Author: Serhii Lakodei
 Author-email: serhii.lakodei@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: authlib (>=1.3.0,<2.0.0)
 Requires-Dist: build (>=1.0.3,<2.0.0)
-Requires-Dist: django (==4.2.3)
-Requires-Dist: django-environ (==0.10.0)
+Requires-Dist: django (>=4.2.2,<5.0.0)
+Requires-Dist: django-environ (>=0.10.0,<0.11.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: twine (>=4.0.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 Django Auth0 project for Abex
 
 Require ENV variables:
```

