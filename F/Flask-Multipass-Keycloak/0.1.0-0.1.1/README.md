# Comparing `tmp/flask_multipass_keycloak-0.1.0-py3-none-any.whl.zip` & `tmp/flask_multipass_keycloak-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 6398 bytes, number of entries: 6
+Zip file size: 6403 bytes, number of entries: 6
 -rw-r--r--  2.0 unx     9279 b- defN 80-Jan-01 00:00 flask_multipass_keycloak.py
--rw-r--r--  2.0 unx     1101 b- defN 80-Jan-01 00:00 flask_multipass_keycloak-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4249 b- defN 80-Jan-01 00:00 flask_multipass_keycloak-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 flask_multipass_keycloak-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      186 b- defN 80-Jan-01 00:00 flask_multipass_keycloak-0.1.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      559 b- defN 16-Jan-01 00:00 flask_multipass_keycloak-0.1.0.dist-info/RECORD
-6 files, 15462 bytes uncompressed, 5372 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx     1101 b- defN 80-Jan-01 00:00 flask_multipass_keycloak-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4291 b- defN 80-Jan-01 00:00 flask_multipass_keycloak-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 flask_multipass_keycloak-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      186 b- defN 80-Jan-01 00:00 flask_multipass_keycloak-0.1.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      559 b- defN 16-Jan-01 00:00 flask_multipass_keycloak-0.1.1.dist-info/RECORD
+6 files, 15504 bytes uncompressed, 5377 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: flask_multipass_keycloak.py
 Comment: 
 
-Filename: flask_multipass_keycloak-0.1.0.dist-info/LICENSE
+Filename: flask_multipass_keycloak-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: flask_multipass_keycloak-0.1.0.dist-info/METADATA
+Filename: flask_multipass_keycloak-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: flask_multipass_keycloak-0.1.0.dist-info/WHEEL
+Filename: flask_multipass_keycloak-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: flask_multipass_keycloak-0.1.0.dist-info/entry_points.txt
+Filename: flask_multipass_keycloak-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: flask_multipass_keycloak-0.1.0.dist-info/RECORD
+Filename: flask_multipass_keycloak-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `flask_multipass_keycloak-0.1.0.dist-info/LICENSE` & `flask_multipass_keycloak-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `flask_multipass_keycloak-0.1.0.dist-info/METADATA` & `flask_multipass_keycloak-0.1.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Flask-Multipass-Keycloak
-Version: 0.1.0
+Version: 0.1.1
 Summary: Flask-Multipass provider for Keycloak
-Home-page: https://github.com/indico/flask-multipass-keycloak
+Home-page: https://github.com/unconventionaldotdev/flask-multipass-keycloak
 License: MIT
 Author: Alejandro Avilés
 Author-email: ome@unconventional.dev
 Maintainer: Adrian Moennich
 Maintainer-email: adrian.moennich@cern.ch
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -15,15 +15,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: flask-multipass[authlib] (>=0.4.3)
-Project-URL: Repository, https://github.com/indico/flask-multipass-keycloak
+Project-URL: Repository, https://github.com/unconventionaldotdev/flask-multipass-keycloak
 Description-Content-Type: text/markdown
 
 # Flask-Multipass-Keycloak
 
 This package provides the `keycloak` authentication and identity providers for [Flask-Multipass][multipass].
 
 `KeycloakAuthProvider`
@@ -82,15 +82,15 @@
 - [`make`](https://www.gnu.org/software/make/) (available in most systems)
 - [`poetry`](https://python-poetry.org/) ([installation guide](https://python-poetry.org/docs/#installation))
 - [`pyenv`](https://github.com/pyenv/pyenv) ([installation guide](https://github.com/pyenv/pyenv#installation))
 
 First, clone the repository locally with:
 
 ```shell
-git clone https://github.com/indico/flask-multipass-keycloak
+git clone https://github.com/unconventionaldotdev/flask-multipass-keycloak
 cd flask-multipass-keycloak
 ```
 
 Before creating the virtualenv, make sure to be using the same version of Python that the development of the project is targeting. This is the first version specified in the `.python-version` file and you can install it with `pyenv`:
 
 ```sh
 pyenv install
```

## Comparing `flask_multipass_keycloak-0.1.0.dist-info/RECORD` & `flask_multipass_keycloak-0.1.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 flask_multipass_keycloak.py,sha256=HNxeYtHIh48hIsyJgKrZVC2I8L34SqyIvBg7r8pabBI,9279
-flask_multipass_keycloak-0.1.0.dist-info/LICENSE,sha256=yPtRmLQVOw1jZIJ9HeJ6Su2-NA_RAXG53XdfeQ7Vyvk,1101
-flask_multipass_keycloak-0.1.0.dist-info/METADATA,sha256=951it41Ih54c1uhg-hJNVawxGUsJbdgFoBabpdSXW2U,4249
-flask_multipass_keycloak-0.1.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-flask_multipass_keycloak-0.1.0.dist-info/entry_points.txt,sha256=ILfaOe7bZ9xxrIOG7j21RgKMrlMwJYJbsOeslcvWz5I,186
-flask_multipass_keycloak-0.1.0.dist-info/RECORD,,
+flask_multipass_keycloak-0.1.1.dist-info/LICENSE,sha256=yPtRmLQVOw1jZIJ9HeJ6Su2-NA_RAXG53XdfeQ7Vyvk,1101
+flask_multipass_keycloak-0.1.1.dist-info/METADATA,sha256=4aAapGIfZqWZh0o1EB_1U4l0-2fTJsDW2r2WsZj7cgQ,4291
+flask_multipass_keycloak-0.1.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+flask_multipass_keycloak-0.1.1.dist-info/entry_points.txt,sha256=ILfaOe7bZ9xxrIOG7j21RgKMrlMwJYJbsOeslcvWz5I,186
+flask_multipass_keycloak-0.1.1.dist-info/RECORD,,
```

