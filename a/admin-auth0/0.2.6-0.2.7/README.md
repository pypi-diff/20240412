# Comparing `tmp/admin_auth0-0.2.6.tar.gz` & `tmp/admin_auth0-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admin_auth0-0.2.6.tar", max compression
+gzip compressed data, was "admin_auth0-0.2.7.tar", max compression
```

## Comparing `admin_auth0-0.2.6.tar` & `admin_auth0-0.2.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      258 2024-04-12 15:04:26.711020 admin_auth0-0.2.6/README.md
--rw-r--r--   0        0        0        0 2024-04-12 15:04:26.711020 admin_auth0-0.2.6/admin_auth0/__init__.py
--rw-r--r--   0        0        0      632 2024-04-12 15:04:26.711020 admin_auth0-0.2.6/admin_auth0/auth0.py
--rw-r--r--   0        0        0     2127 2024-04-12 15:04:26.711020 admin_auth0-0.2.6/admin_auth0/authentication.py
--rw-r--r--   0        0        0      236 2024-04-12 15:04:26.711020 admin_auth0-0.2.6/admin_auth0/urls.py
--rw-r--r--   0        0        0     1344 2024-04-12 15:04:26.711020 admin_auth0-0.2.6/admin_auth0/views.py
--rw-r--r--   0        0        0      393 2024-04-12 15:04:26.711020 admin_auth0-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 admin_auth0-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      258 2024-04-12 15:21:04.150226 admin_auth0-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 15:21:04.150226 admin_auth0-0.2.7/admin_auth0/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-12 15:21:04.150226 admin_auth0-0.2.7/admin_auth0/auth0.py
+-rw-r--r--   0        0        0     2127 2024-04-12 15:21:04.150226 admin_auth0-0.2.7/admin_auth0/authentication.py
+-rw-r--r--   0        0        0      236 2024-04-12 15:21:04.150226 admin_auth0-0.2.7/admin_auth0/urls.py
+-rw-r--r--   0        0        0     1344 2024-04-12 15:21:04.150226 admin_auth0-0.2.7/admin_auth0/views.py
+-rw-r--r--   0        0        0      394 2024-04-12 15:21:04.150226 admin_auth0-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 admin_auth0-0.2.7/PKG-INFO
```

### Comparing `admin_auth0-0.2.6/admin_auth0/auth0.py` & `admin_auth0-0.2.7/admin_auth0/auth0.py`

 * *Files identical despite different names*

### Comparing `admin_auth0-0.2.6/admin_auth0/authentication.py` & `admin_auth0-0.2.7/admin_auth0/authentication.py`

 * *Files identical despite different names*

### Comparing `admin_auth0-0.2.6/admin_auth0/views.py` & `admin_auth0-0.2.7/admin_auth0/views.py`

 * *Files identical despite different names*

### Comparing `admin_auth0-0.2.6/PKG-INFO` & `admin_auth0-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: admin_auth0
-Version: 0.2.6
+Version: 0.2.7
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
-Requires-Dist: django (>=4.2.2,<5.0.0)
+Requires-Dist: django (>=4.2.2)
 Requires-Dist: django-environ (>=0.10.0,<0.11.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: twine (>=4.0.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 Django Auth0 project for Abex
```

