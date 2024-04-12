# Comparing `tmp/nats_jwt-0.0.1.tar.gz` & `tmp/nats_jwt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nats_jwt-0.0.1.tar", max compression
+gzip compressed data, was "nats_jwt-0.1.0.tar", max compression
```

## Comparing `nats_jwt-0.0.1.tar` & `nats_jwt-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11345 2024-04-12 10:44:07.909884 nats_jwt-0.0.1/LICENSE
--rw-r--r--   0        0        0     3437 2024-04-12 10:44:07.909884 nats_jwt-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-12 10:44:07.909884 nats_jwt-0.0.1/nats_jwt/__init__.py
--rw-r--r--   0        0        0       22 2024-04-12 10:44:07.909884 nats_jwt-0.0.1/nats_jwt/nkeys_ext/__init__.py
--rw-r--r--   0        0        0     3834 2024-04-12 10:44:07.909884 nats_jwt-0.0.1/nats_jwt/nkeys_ext/nkeys2.py
--rw-r--r--   0        0        0        0 2024-04-12 10:44:07.909884 nats_jwt-0.0.1/nats_jwt/v2/__init__.py
--rw-r--r--   0        0        0    11128 2024-04-12 10:44:07.909884 nats_jwt-0.0.1/nats_jwt/v2/account_claims.py
--rw-r--r--   0        0        0     9897 2024-04-12 10:44:07.909884 nats_jwt-0.0.1/nats_jwt/v2/claims.py
--rw-r--r--   0        0        0       51 2024-04-12 10:44:07.909884 nats_jwt-0.0.1/nats_jwt/v2/common.py
--rw-r--r--   0        0        0     2883 2024-04-12 10:44:07.909884 nats_jwt-0.0.1/nats_jwt/v2/decoder.py
--rw-r--r--   0        0        0     1980 2024-04-12 10:44:07.909884 nats_jwt-0.0.1/nats_jwt/v2/header.py
--rw-r--r--   0        0        0     3582 2024-04-12 10:44:07.909884 nats_jwt-0.0.1/nats_jwt/v2/operator_claims.py
--rw-r--r--   0        0        0     1946 2024-04-12 10:44:07.909884 nats_jwt-0.0.1/nats_jwt/v2/revocation_list.py
--rw-r--r--   0        0        0      118 2024-04-12 10:44:07.913884 nats_jwt-0.0.1/nats_jwt/v2/signing_keys.py
--rw-r--r--   0        0        0    10698 2024-04-12 10:44:07.913884 nats_jwt-0.0.1/nats_jwt/v2/snippets.py
--rw-r--r--   0        0        0     4404 2024-04-12 10:44:07.913884 nats_jwt-0.0.1/nats_jwt/v2/types.py
--rw-r--r--   0        0        0     2942 2024-04-12 10:44:07.913884 nats_jwt-0.0.1/nats_jwt/v2/user_claims.py
--rw-r--r--   0        0        0     1630 2024-04-12 10:44:07.913884 nats_jwt-0.0.1/nats_jwt/v2/validation.py
--rw-r--r--   0        0        0       54 2024-04-12 10:44:07.913884 nats_jwt-0.0.1/nats_jwt/v2/version.py
--rw-r--r--   0        0        0      959 2024-04-12 10:44:07.913884 nats_jwt-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 nats_jwt-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3437 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/nkeys_ext/__init__.py
+-rw-r--r--   0        0        0     3834 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/nkeys_ext/nkeys2.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/v2/__init__.py
+-rw-r--r--   0        0        0    11128 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/v2/account_claims.py
+-rw-r--r--   0        0        0     9897 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/v2/claims.py
+-rw-r--r--   0        0        0       51 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/v2/common.py
+-rw-r--r--   0        0        0     2883 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/v2/decoder.py
+-rw-r--r--   0        0        0     1980 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/v2/header.py
+-rw-r--r--   0        0        0     3582 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/v2/operator_claims.py
+-rw-r--r--   0        0        0     1946 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/v2/revocation_list.py
+-rw-r--r--   0        0        0      118 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/v2/signing_keys.py
+-rw-r--r--   0        0        0    10698 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/v2/snippets.py
+-rw-r--r--   0        0        0     4404 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/v2/types.py
+-rw-r--r--   0        0        0     2942 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/v2/user_claims.py
+-rw-r--r--   0        0        0     1630 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/v2/validation.py
+-rw-r--r--   0        0        0       54 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/nats_jwt/v2/version.py
+-rw-r--r--   0        0        0      960 2024-04-12 10:44:33.953438 nats_jwt-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 nats_jwt-0.1.0/PKG-INFO
```

### Comparing `nats_jwt-0.0.1/LICENSE` & `nats_jwt-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nats_jwt-0.0.1/README.md` & `nats_jwt-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nats_jwt-0.0.1/nats_jwt/nkeys_ext/nkeys2.py` & `nats_jwt-0.1.0/nats_jwt/nkeys_ext/nkeys2.py`

 * *Files identical despite different names*

### Comparing `nats_jwt-0.0.1/nats_jwt/v2/account_claims.py` & `nats_jwt-0.1.0/nats_jwt/v2/account_claims.py`

 * *Files identical despite different names*

### Comparing `nats_jwt-0.0.1/nats_jwt/v2/claims.py` & `nats_jwt-0.1.0/nats_jwt/v2/claims.py`

 * *Files identical despite different names*

### Comparing `nats_jwt-0.0.1/nats_jwt/v2/decoder.py` & `nats_jwt-0.1.0/nats_jwt/v2/decoder.py`

 * *Files identical despite different names*

### Comparing `nats_jwt-0.0.1/nats_jwt/v2/header.py` & `nats_jwt-0.1.0/nats_jwt/v2/header.py`

 * *Files identical despite different names*

### Comparing `nats_jwt-0.0.1/nats_jwt/v2/operator_claims.py` & `nats_jwt-0.1.0/nats_jwt/v2/operator_claims.py`

 * *Files identical despite different names*

### Comparing `nats_jwt-0.0.1/nats_jwt/v2/revocation_list.py` & `nats_jwt-0.1.0/nats_jwt/v2/revocation_list.py`

 * *Files identical despite different names*

### Comparing `nats_jwt-0.0.1/nats_jwt/v2/snippets.py` & `nats_jwt-0.1.0/nats_jwt/v2/snippets.py`

 * *Files identical despite different names*

### Comparing `nats_jwt-0.0.1/nats_jwt/v2/types.py` & `nats_jwt-0.1.0/nats_jwt/v2/types.py`

 * *Files identical despite different names*

### Comparing `nats_jwt-0.0.1/nats_jwt/v2/user_claims.py` & `nats_jwt-0.1.0/nats_jwt/v2/user_claims.py`

 * *Files identical despite different names*

### Comparing `nats_jwt-0.0.1/nats_jwt/v2/validation.py` & `nats_jwt-0.1.0/nats_jwt/v2/validation.py`

 * *Files identical despite different names*

### Comparing `nats_jwt-0.0.1/pyproject.toml` & `nats_jwt-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nats-jwt"
-version = "0.0.1"
+version = "0.1.0"
 description = "JWT tokens signed using NKeys for Ed25519 for the Python3 ecosystem"
 authors = ["Seznam.cz, a.s. <doporucovani-vyvoj@firma.seznam.cz>"]
 license = "Apache-2.0 license"
 readme = "README.md"
 packages = [{include = "nats_jwt"}]
 
 [tool.poetry.dependencies]
@@ -30,11 +30,12 @@
 update_changelog_on_bump = true
 annotated_tag = true
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.3"
 coverage = { version = "^7.3.2", extras = ["toml"] }
 swiftmock = "^0.0.1"
```

### Comparing `nats_jwt-0.0.1/PKG-INFO` & `nats_jwt-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nats-jwt
-Version: 0.0.1
+Version: 0.1.0
 Summary: JWT tokens signed using NKeys for Ed25519 for the Python3 ecosystem
 License: Apache-2.0 license
 Author: Seznam.cz, a.s.
 Author-email: doporucovani-vyvoj@firma.seznam.cz
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

