# Comparing `tmp/sandesh.py-0.0.1.tar.gz` & `tmp/sandesh.py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sandesh.py-0.0.1.tar", last modified: Fri Apr 12 15:00:22 2024, max compression
+gzip compressed data, was "sandesh.py-0.0.2.tar", last modified: Fri Apr 12 16:40:53 2024, max compression
```

## Comparing `sandesh.py-0.0.1.tar` & `sandesh.py-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sandesh   (1000) sandesh   (1000)        0 2024-04-12 15:00:22.283492 sandesh.py-0.0.1/
--rw-r--r--   0 sandesh   (1000) sandesh   (1000)     1070 2024-02-09 05:49:03.000000 sandesh.py-0.0.1/LICENSE
--rw-r--r--   0 sandesh   (1000) sandesh   (1000)     1667 2024-04-12 15:00:22.283492 sandesh.py-0.0.1/PKG-INFO
--rw-r--r--   0 sandesh   (1000) sandesh   (1000)     1051 2024-04-11 15:33:41.000000 sandesh.py-0.0.1/README.md
--rw-r--r--   0 sandesh   (1000) sandesh   (1000)      662 2024-02-12 09:57:27.000000 sandesh.py-0.0.1/pyproject.toml
-drwxr-xr-x   0 sandesh   (1000) sandesh   (1000)        0 2024-04-12 15:00:22.283492 sandesh.py-0.0.1/sandesh.py.egg-info/
--rw-r--r--   0 sandesh   (1000) sandesh   (1000)     1667 2024-04-12 15:00:22.000000 sandesh.py-0.0.1/sandesh.py.egg-info/PKG-INFO
--rw-r--r--   0 sandesh   (1000) sandesh   (1000)      286 2024-04-12 15:00:22.000000 sandesh.py-0.0.1/sandesh.py.egg-info/SOURCES.txt
--rw-r--r--   0 sandesh   (1000) sandesh   (1000)        1 2024-04-12 15:00:22.000000 sandesh.py-0.0.1/sandesh.py.egg-info/dependency_links.txt
--rw-r--r--   0 sandesh   (1000) sandesh   (1000)       11 2024-04-12 15:00:22.000000 sandesh.py-0.0.1/sandesh.py.egg-info/top_level.txt
-drwxr-xr-x   0 sandesh   (1000) sandesh   (1000)        0 2024-04-12 15:00:22.283492 sandesh.py-0.0.1/sandesh_py/
--rw-r--r--   0 sandesh   (1000) sandesh   (1000)       35 2024-02-12 09:45:16.000000 sandesh.py-0.0.1/sandesh_py/__init__.py
--rw-r--r--   0 sandesh   (1000) sandesh   (1000)     2170 2024-04-11 15:25:38.000000 sandesh.py-0.0.1/sandesh_py/attachments.py
--rw-r--r--   0 sandesh   (1000) sandesh   (1000)     1669 2024-04-11 15:36:44.000000 sandesh.py-0.0.1/sandesh_py/mailer.py
--rw-r--r--   0 sandesh   (1000) sandesh   (1000)     3323 2024-04-11 15:37:18.000000 sandesh.py-0.0.1/sandesh_py/smtp.py
--rw-r--r--   0 sandesh   (1000) sandesh   (1000)      436 2024-02-18 17:15:35.000000 sandesh.py-0.0.1/sandesh_py/types.py
--rw-r--r--   0 sandesh   (1000) sandesh   (1000)       38 2024-04-12 15:00:22.283492 sandesh.py-0.0.1/setup.cfg
--rw-r--r--   0 sandesh   (1000) sandesh   (1000)      330 2024-04-12 14:53:38.000000 sandesh.py-0.0.1/setup.py
+drwxr-xr-x   0 sandesh   (1000) sandesh   (1000)        0 2024-04-12 16:40:53.116470 sandesh.py-0.0.2/
+-rw-r--r--   0 sandesh   (1000) sandesh   (1000)     1070 2024-02-09 05:49:03.000000 sandesh.py-0.0.2/LICENSE
+-rw-r--r--   0 sandesh   (1000) sandesh   (1000)     1651 2024-04-12 16:40:53.116470 sandesh.py-0.0.2/PKG-INFO
+-rw-r--r--   0 sandesh   (1000) sandesh   (1000)     1035 2024-04-12 16:07:01.000000 sandesh.py-0.0.2/README.md
+-rw-r--r--   0 sandesh   (1000) sandesh   (1000)      662 2024-04-12 16:40:44.000000 sandesh.py-0.0.2/pyproject.toml
+drwxr-xr-x   0 sandesh   (1000) sandesh   (1000)        0 2024-04-12 16:40:53.116470 sandesh.py-0.0.2/sandesh.py.egg-info/
+-rw-r--r--   0 sandesh   (1000) sandesh   (1000)     1651 2024-04-12 16:40:53.000000 sandesh.py-0.0.2/sandesh.py.egg-info/PKG-INFO
+-rw-r--r--   0 sandesh   (1000) sandesh   (1000)      286 2024-04-12 16:40:53.000000 sandesh.py-0.0.2/sandesh.py.egg-info/SOURCES.txt
+-rw-r--r--   0 sandesh   (1000) sandesh   (1000)        1 2024-04-12 16:40:53.000000 sandesh.py-0.0.2/sandesh.py.egg-info/dependency_links.txt
+-rw-r--r--   0 sandesh   (1000) sandesh   (1000)       11 2024-04-12 16:40:53.000000 sandesh.py-0.0.2/sandesh.py.egg-info/top_level.txt
+drwxr-xr-x   0 sandesh   (1000) sandesh   (1000)        0 2024-04-12 16:40:53.116470 sandesh.py-0.0.2/sandesh_py/
+-rw-r--r--   0 sandesh   (1000) sandesh   (1000)       35 2024-02-12 09:45:16.000000 sandesh.py-0.0.2/sandesh_py/__init__.py
+-rw-r--r--   0 sandesh   (1000) sandesh   (1000)     2170 2024-04-11 15:25:38.000000 sandesh.py-0.0.2/sandesh_py/attachments.py
+-rw-r--r--   0 sandesh   (1000) sandesh   (1000)     1669 2024-04-11 15:36:44.000000 sandesh.py-0.0.2/sandesh_py/mailer.py
+-rw-r--r--   0 sandesh   (1000) sandesh   (1000)     3323 2024-04-11 15:37:18.000000 sandesh.py-0.0.2/sandesh_py/smtp.py
+-rw-r--r--   0 sandesh   (1000) sandesh   (1000)      436 2024-02-18 17:15:35.000000 sandesh.py-0.0.2/sandesh_py/types.py
+-rw-r--r--   0 sandesh   (1000) sandesh   (1000)       38 2024-04-12 16:40:53.116470 sandesh.py-0.0.2/setup.cfg
+-rw-r--r--   0 sandesh   (1000) sandesh   (1000)      330 2024-04-12 14:53:38.000000 sandesh.py-0.0.2/setup.py
```

### Comparing `sandesh.py-0.0.1/LICENSE` & `sandesh.py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sandesh.py-0.0.1/PKG-INFO` & `sandesh.py-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sandesh.py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Basic implementaion of SMTP client using TCP communication with the SMTP server using the `socket` module.
 Author: Sandesh Khadaka
 Author-email: Sandesh Khadka <mail@khadkasandesh.com.np>
 Project-URL: Homepage, https://github.com/sandeshkhadka/sandesh
 Project-URL: Issues, https://github.com/sandeshkhadka/sandesh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,48 +13,48 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sandesh - Send Mail 🕊️
 
 Basic implementaion of SMTP client using TCP communication with the SMTP server using the `socket` module.
 
+## Installation
+
+```shell
+pip install sandesh.py
+```
+
 ## Usage
 
 ```python
+from sandesh_py import smtp
 
-import sandesh_py as sandesh
-auth = {"username": SMTP_USERNAME, "password": SMTP_PASSWORD},
-options = {"notls": False}
-client = sandesh.SMTPClient(
-    SMTP_HOST,
-    SMTP_PORT,
-    auth,
-    options
-t
+auth: smtp.SMTPAuth = {
+    "username": YOUR_SMTP_USERNAME,
+    "password": YOUR_SMTP_PASSWORD,
+}
+options: smtp.SMTPOptions = {"notls": False}
+client = smtp.SMTPClient(SMTP_SERVER_HOST, SMTP_PORT, auth, options)
 
 client.connect()
 mail = smtp.Mail(
     {
-        "mailTo": "recipient@example.com",
-        "mailFrom": "sender@example.com",
-        "subject": "Email Subject",
-        "body": "Email Body",
-        "attachments": [
-        # attachment files MUST be under 20 MB
-        "path/to/attachment",
-        "path/to/attachment"
-        ]
+        "mailTo": "receiver@email.com",
+        "mailFrom": "sender@email.com",
+        "subject": "Mail subject",
+        "body": "This is demonstartaion of use of sandesh_py package",
+        "attachment": [
+            "/path/to/attachment/1",
+            "/path/to/attachment/2",
+        ],
     }
 )
-client.sendMail(mail)
+print(client.sendMail(mail))
 client.close()
 
-
 ```
 
 ## ToDo List
 
-- [x] Support authentication using username and password
-- [x] Implement SSL/TLS encryption for secure communication
 - [x] Add support for MIME to handle attachments and alternative content types
 - [ ] Support Oath and API authentication
 - [ ] Connection Pooling and Asynchronous Delivery
```

### Comparing `sandesh.py-0.0.1/README.md` & `sandesh.py-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # Sandesh - Send Mail 🕊️
 
 Basic implementaion of SMTP client using TCP communication with the SMTP server using the `socket` module.
 
+## Installation
+
+```shell
+pip install sandesh.py
+```
+
 ## Usage
 
 ```python
+from sandesh_py import smtp
 
-import sandesh_py as sandesh
-auth = {"username": SMTP_USERNAME, "password": SMTP_PASSWORD},
-options = {"notls": False}
-client = sandesh.SMTPClient(
-    SMTP_HOST,
-    SMTP_PORT,
-    auth,
-    options
-t
+auth: smtp.SMTPAuth = {
+    "username": YOUR_SMTP_USERNAME,
+    "password": YOUR_SMTP_PASSWORD,
+}
+options: smtp.SMTPOptions = {"notls": False}
+client = smtp.SMTPClient(SMTP_SERVER_HOST, SMTP_PORT, auth, options)
 
 client.connect()
 mail = smtp.Mail(
     {
-        "mailTo": "recipient@example.com",
-        "mailFrom": "sender@example.com",
-        "subject": "Email Subject",
-        "body": "Email Body",
-        "attachments": [
-        # attachment files MUST be under 20 MB
-        "path/to/attachment",
-        "path/to/attachment"
-        ]
+        "mailTo": "receiver@email.com",
+        "mailFrom": "sender@email.com",
+        "subject": "Mail subject",
+        "body": "This is demonstartaion of use of sandesh_py package",
+        "attachment": [
+            "/path/to/attachment/1",
+            "/path/to/attachment/2",
+        ],
     }
 )
-client.sendMail(mail)
+print(client.sendMail(mail))
 client.close()
 
-
 ```
 
 ## ToDo List
 
-- [x] Support authentication using username and password
-- [x] Implement SSL/TLS encryption for secure communication
 - [x] Add support for MIME to handle attachments and alternative content types
 - [ ] Support Oath and API authentication
 - [ ] Connection Pooling and Asynchronous Delivery
```

### Comparing `sandesh.py-0.0.1/pyproject.toml` & `sandesh.py-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sandesh.py"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Sandesh Khadka", email="mail@khadkasandesh.com.np" },
 ]
 description = "Basic implementaion of SMTP client using TCP communication with the SMTP server using the `socket` module."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `sandesh.py-0.0.1/sandesh.py.egg-info/PKG-INFO` & `sandesh.py-0.0.2/sandesh.py.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sandesh.py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Basic implementaion of SMTP client using TCP communication with the SMTP server using the `socket` module.
 Author: Sandesh Khadaka
 Author-email: Sandesh Khadka <mail@khadkasandesh.com.np>
 Project-URL: Homepage, https://github.com/sandeshkhadka/sandesh
 Project-URL: Issues, https://github.com/sandeshkhadka/sandesh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,48 +13,48 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sandesh - Send Mail 🕊️
 
 Basic implementaion of SMTP client using TCP communication with the SMTP server using the `socket` module.
 
+## Installation
+
+```shell
+pip install sandesh.py
+```
+
 ## Usage
 
 ```python
+from sandesh_py import smtp
 
-import sandesh_py as sandesh
-auth = {"username": SMTP_USERNAME, "password": SMTP_PASSWORD},
-options = {"notls": False}
-client = sandesh.SMTPClient(
-    SMTP_HOST,
-    SMTP_PORT,
-    auth,
-    options
-t
+auth: smtp.SMTPAuth = {
+    "username": YOUR_SMTP_USERNAME,
+    "password": YOUR_SMTP_PASSWORD,
+}
+options: smtp.SMTPOptions = {"notls": False}
+client = smtp.SMTPClient(SMTP_SERVER_HOST, SMTP_PORT, auth, options)
 
 client.connect()
 mail = smtp.Mail(
     {
-        "mailTo": "recipient@example.com",
-        "mailFrom": "sender@example.com",
-        "subject": "Email Subject",
-        "body": "Email Body",
-        "attachments": [
-        # attachment files MUST be under 20 MB
-        "path/to/attachment",
-        "path/to/attachment"
-        ]
+        "mailTo": "receiver@email.com",
+        "mailFrom": "sender@email.com",
+        "subject": "Mail subject",
+        "body": "This is demonstartaion of use of sandesh_py package",
+        "attachment": [
+            "/path/to/attachment/1",
+            "/path/to/attachment/2",
+        ],
     }
 )
-client.sendMail(mail)
+print(client.sendMail(mail))
 client.close()
 
-
 ```
 
 ## ToDo List
 
-- [x] Support authentication using username and password
-- [x] Implement SSL/TLS encryption for secure communication
 - [x] Add support for MIME to handle attachments and alternative content types
 - [ ] Support Oath and API authentication
 - [ ] Connection Pooling and Asynchronous Delivery
```

### Comparing `sandesh.py-0.0.1/sandesh_py/attachments.py` & `sandesh.py-0.0.2/sandesh_py/attachments.py`

 * *Files identical despite different names*

### Comparing `sandesh.py-0.0.1/sandesh_py/mailer.py` & `sandesh.py-0.0.2/sandesh_py/mailer.py`

 * *Files identical despite different names*

### Comparing `sandesh.py-0.0.1/sandesh_py/smtp.py` & `sandesh.py-0.0.2/sandesh_py/smtp.py`

 * *Files identical despite different names*

