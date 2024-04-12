# Comparing `tmp/pytest_iam-0.0.8.tar.gz` & `tmp/pytest_iam-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_iam-0.0.8.tar", max compression
+gzip compressed data, was "pytest_iam-0.0.9.tar", max compression
```

## Comparing `pytest_iam-0.0.8.tar` & `pytest_iam-0.0.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1056 2023-08-21 07:44:21.399200 pytest_iam-0.0.8/LICENSE.md
--rw-r--r--   0        0        0     2052 2023-08-28 07:10:34.775338 pytest_iam-0.0.8/README.md
--rw-r--r--   0        0        0     2066 2024-03-14 08:26:03.518734 pytest_iam-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5392 2024-03-12 10:06:06.572687 pytest_iam-0.0.8/pytest_iam/__init__.py
--rw-r--r--   0        0        0     3391 1970-01-01 00:00:00.000000 pytest_iam-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-08-16 13:35:53.181565 pytest_iam-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0     2053 2024-03-15 14:35:37.724461 pytest_iam-0.0.9/README.md
+-rw-r--r--   0        0        0     2066 2024-03-30 10:23:48.546512 pytest_iam-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5873 2024-03-30 10:23:20.689983 pytest_iam-0.0.9/pytest_iam/__init__.py
+-rw-r--r--   0        0        0     3392 1970-01-01 00:00:00.000000 pytest_iam-0.0.9/PKG-INFO
```

### Comparing `pytest_iam-0.0.8/LICENSE.md` & `pytest_iam-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pytest_iam-0.0.8/README.md` & `pytest_iam-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```console
 pip install pytest-iam
 ```
 
 Usage
 -----
 
-pytest-iam provides tools to test your application authentication mechanism agaist a OAuth2/OIDC server:
+pytest-iam provides tools to test your application authentication mechanism against a OAuth2/OIDC server:
 
 - It launches a [Canaille](https://canaille.yaal.coop) instance
 - It provides a ``iam_server`` fixture that comes with several features:
     - the URL of the IAM server to configure your application
     - IAM models (Users, groups, clients, tokens etc.) to prepare your tests and check the side effects.
       More details on [the reference](https://pytest-iam.readthedocs.io/en/latest/reference.html)
     - utilities to log-in users and give their consent to your application
```

### Comparing `pytest_iam-0.0.8/pyproject.toml` & `pytest_iam-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pytest-iam"
-version = "0.0.8"
+version = "0.0.9"
 description = "A fully functional OAUTH2 / OpenID Connect (OIDC) server to be used in your testsuite"
 authors = ["Yaal Coop <contact@yaal.coop>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pytest_iam"}]
 keywords = ["oidc", "oauth", "oauth2", "openid", "identity", "pytest", "unit tests", "iam"]
 classifiers = [
```

### Comparing `pytest_iam-0.0.8/pytest_iam/__init__.py` & `pytest_iam-0.0.9/pytest_iam/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -139,33 +139,46 @@
 def iam_configuration(tmp_path_factory) -> Dict[str, Any]:
     """Fixture for editing the configuration of
     :meth:`~pytest_iam.iam_server`."""
 
     private_key, public_key = generate_keypair()
     return {
         "TESTING": True,
-        "JAVASCRIPT": False,
-        "WTF_CSRF_ENABLED": False,
         "SECRET_KEY": str(uuid.uuid4()),
-        "OIDC": {
+        "WTF_CSRF_ENABLED": False,
+        "CANAILLE": {
+            "JAVASCRIPT": False,
+            "ACL": {
+                "DEFAULT": {
+                    "PERMISSIONS": ["use_oidc", "manage_oidc"],
+                }
+            },
+            "LOGGING": {
+                "version": 1,
+                "formatters": {
+                    "default": {
+                        "format": "[%(asctime)s] %(levelname)s in %(module)s: %(message)s",
+                    }
+                },
+                "handlers": {
+                    "canaille": {
+                        "class": "logging.NullHandler",
+                        "formatter": "default",
+                    }
+                },
+                "root": {"level": "DEBUG", "handlers": ["canaille"]},
+            },
+        },
+        "CANAILLE_OIDC": {
             "DYNAMIC_CLIENT_REGISTRATION_OPEN": True,
             "JWT": {
                 "PUBLIC_KEY": public_key,
                 "PRIVATE_KEY": private_key,
             },
         },
-        "ACL": {
-            "DEFAULT": {
-                "PERMISSIONS": ["use_oidc", "manage_oidc"],
-            }
-        },
-        "LOGGING": {
-            "LEVEL": "DEBUG",
-            "PATH": tmp_path_factory.mktemp("logs") / "canaille.log",
-        },
     }
 
 
 @pytest.fixture(scope="session")
 def iam_server(iam_configuration) -> Server:
     """Fixture that creates a Canaille server listening a random port in a
     thread."""
```

### Comparing `pytest_iam-0.0.8/PKG-INFO` & `pytest_iam-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-iam
-Version: 0.0.8
+Version: 0.0.9
 Summary: A fully functional OAUTH2 / OpenID Connect (OIDC) server to be used in your testsuite
 Home-page: https://gitlab.com/yaal/pytest-iam
 License: MIT
 Keywords: oidc,oauth,oauth2,openid,identity,pytest,unit tests,iam
 Author: Yaal Coop
 Author-email: contact@yaal.coop
 Requires-Python: >=3.8,<4.0
@@ -46,15 +46,15 @@
 ```console
 pip install pytest-iam
 ```
 
 Usage
 -----
 
-pytest-iam provides tools to test your application authentication mechanism agaist a OAuth2/OIDC server:
+pytest-iam provides tools to test your application authentication mechanism against a OAuth2/OIDC server:
 
 - It launches a [Canaille](https://canaille.yaal.coop) instance
 - It provides a ``iam_server`` fixture that comes with several features:
     - the URL of the IAM server to configure your application
     - IAM models (Users, groups, clients, tokens etc.) to prepare your tests and check the side effects.
       More details on [the reference](https://pytest-iam.readthedocs.io/en/latest/reference.html)
     - utilities to log-in users and give their consent to your application
```

