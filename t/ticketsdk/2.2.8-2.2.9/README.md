# Comparing `tmp/ticketsdk-2.2.8.tar.gz` & `tmp/ticketsdk-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ticketsdk-2.2.8.tar", last modified: Thu Apr 11 09:39:25 2024, max compression
+gzip compressed data, was "ticketsdk-2.2.9.tar", last modified: Thu Apr 11 09:48:16 2024, max compression
```

## Comparing `ticketsdk-2.2.8.tar` & `ticketsdk-2.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 09:39:25.348520 ticketsdk-2.2.8/
--rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 09:39:25.348346 ticketsdk-2.2.8/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)     1511 2024-04-11 06:30:52.000000 ticketsdk-2.2.8/README.md
--rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-11 09:39:25.348567 ticketsdk-2.2.8/setup.cfg
--rw-r--r--   0 phamchuong   (501) staff       (20)      851 2024-04-11 09:39:11.000000 ticketsdk-2.2.8/setup.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 09:39:25.347037 ticketsdk-2.2.8/ticketsdk/
--rw-r--r--   0 phamchuong   (501) staff       (20)      516 2024-04-02 03:10:03.000000 ticketsdk-2.2.8/ticketsdk/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-03-27 09:22:59.000000 ticketsdk-2.2.8/ticketsdk/client.py
--rw-r--r--   0 phamchuong   (501) staff       (20)      354 2024-03-27 10:12:08.000000 ticketsdk-2.2.8/ticketsdk/constants.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 09:39:25.347788 ticketsdk-2.2.8/ticketsdk/seller/
--rw-r--r--   0 phamchuong   (501) staff       (20)     3118 2024-04-09 08:03:12.000000 ticketsdk-2.2.8/ticketsdk/seller/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     3089 2024-04-11 07:08:34.000000 ticketsdk-2.2.8/ticketsdk/validators.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 09:39:25.348168 ticketsdk-2.2.8/ticketsdk.egg-info/
--rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 09:39:25.000000 ticketsdk-2.2.8/ticketsdk.egg-info/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)      300 2024-04-11 09:39:25.000000 ticketsdk-2.2.8/ticketsdk.egg-info/SOURCES.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       33 2024-04-11 09:39:25.000000 ticketsdk-2.2.8/ticketsdk.egg-info/dependency_links.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-11 09:39:25.000000 ticketsdk-2.2.8/ticketsdk.egg-info/requires.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       10 2024-04-11 09:39:25.000000 ticketsdk-2.2.8/ticketsdk.egg-info/top_level.txt
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 09:48:16.989842 ticketsdk-2.2.9/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 09:48:16.989658 ticketsdk-2.2.9/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1717 2024-04-11 09:47:21.000000 ticketsdk-2.2.9/README.md
+-rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-11 09:48:16.989887 ticketsdk-2.2.9/setup.cfg
+-rw-r--r--   0 phamchuong   (501) staff       (20)      851 2024-04-11 09:47:33.000000 ticketsdk-2.2.9/setup.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 09:48:16.988406 ticketsdk-2.2.9/ticketsdk/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      516 2024-04-02 03:10:03.000000 ticketsdk-2.2.9/ticketsdk/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-03-27 09:22:59.000000 ticketsdk-2.2.9/ticketsdk/client.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)      354 2024-03-27 10:12:08.000000 ticketsdk-2.2.9/ticketsdk/constants.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 09:48:16.989162 ticketsdk-2.2.9/ticketsdk/seller/
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3118 2024-04-09 08:03:12.000000 ticketsdk-2.2.9/ticketsdk/seller/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3313 2024-04-11 09:47:21.000000 ticketsdk-2.2.9/ticketsdk/validators.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 09:48:16.989461 ticketsdk-2.2.9/ticketsdk.egg-info/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 09:48:16.000000 ticketsdk-2.2.9/ticketsdk.egg-info/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)      300 2024-04-11 09:48:16.000000 ticketsdk-2.2.9/ticketsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       33 2024-04-11 09:48:16.000000 ticketsdk-2.2.9/ticketsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-11 09:48:16.000000 ticketsdk-2.2.9/ticketsdk.egg-info/requires.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       10 2024-04-11 09:48:16.000000 ticketsdk-2.2.9/ticketsdk.egg-info/top_level.txt
```

### Comparing `ticketsdk-2.2.8/README.md` & `ticketsdk-2.2.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -25,15 +25,17 @@
     "ref_code":"test_23_03_2024",
     "ticket_name":"Lấy video đóng gói đơn hàng xxxx",
     "ticket_description" : "Lấy video đóng gói đơn hàng xxxx",
     "issue_code": "OUTBOUND",
     "from_system" : "WMS",
     "requested_email":"tri.nm@nandhlogistics.vn",
     "lambda_type" :"add",
-    "attachments" :[]
+    "attachments" :[],
+    "requested_by_employee_email": "test@gmail",
+    "requested_by_employee_name": "requested_by_employee_email"
 }).add_new_ticket()
 
 ```
 
 ### List ticket:
 ```
 Connection(body = {
@@ -58,18 +60,20 @@
 Connection(body={ "lambda_type" :"get_comments", "ticket_id":107 }).list_comment_ticket()
 ```
 
 ### Add new comment ticket
 ```
 Connection(body={ 
     "lambda_type" :"add_comments", 
-    "ticket_id":107, 
+    "ticket_id":283, 
     "content": "This is my text for customer source", 
     "attachments": [],
-     "partner_code": "1" 
+    "partner_code": "BS2X100004",
+    "created_by_employee_email": "test@gmail",
+    "created_by_employee_name": "OK"
 }).create_comment_ticket()
 ```
 ### To upload a Python library to the Python Package Index (PyPI)
 
 1. pip install twine
 2. python setup.py sdist bdist_wheel
 3. twine upload dist/*
```

### Comparing `ticketsdk-2.2.8/setup.py` & `ticketsdk-2.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 PKG = "ticketsdk"
-version = "2.2.8"
+version = "2.2.9"
 long_desc = (
     """This SDK is a programatic inteface into the ticket APIs of NandH Logistics."""
 )
 
 setup(
     name=PKG,
     version=version,
```

### Comparing `ticketsdk-2.2.8/ticketsdk/__init__.py` & `ticketsdk-2.2.9/ticketsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.8/ticketsdk/client.py` & `ticketsdk-2.2.9/ticketsdk/client.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.8/ticketsdk/seller/__init__.py` & `ticketsdk-2.2.9/ticketsdk/seller/__init__.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.8/ticketsdk/validators.py` & `ticketsdk-2.2.9/ticketsdk/validators.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,24 +36,26 @@
     ref_code = fields.Str(required=True)
     partner_code = fields.Str(required=True)
     ticket_name = fields.Str(required=True)
     requested_email = fields.Str(required=True)
     ticket_description = fields.Str(required=True)
     attachments = fields.List(fields.Str(), allow_none=False, allow_empty=True)
     lambda_type = fields.Str(required=True)
+    requested_by_employee_email = fields.Str(required=False)
+    requested_by_employee_name = fields.Str(required=False)
 
     class Meta:
         strict = True
         unknown = RAISE
 
 
 class NewSellerSchema(Schema):
     partner_code = fields.Str(required=True)
     email = fields.Str(required=True)
-    cs_email = fields.Str(required=False, default=None)
+    cs_email = fields.Str(required=False)
     lambda_type = fields.Str(required=True)
     name = fields.Str(required=False)
     company_name = fields.Str(required=False)
 
     class Meta:
         strict = True
         unknown = RAISE
@@ -94,11 +96,13 @@
 
 class CreateCommentTicketSchema(Schema):
     lambda_type = fields.Str(required=True, validate=validate_type_comment)
     ticket_id = fields.Int(required=True)
     content = fields.Str(required=True)
     attachments = fields.List(fields.Str(), allow_none=True, allow_empty=True)
     partner_code = fields.Str(required=True)
+    created_by_employee_email = fields.Str(required=False)
+    created_by_employee_name = fields.Str(required=False)
 
     class Meta:
         strict = True
         unknown = RAISE
```

