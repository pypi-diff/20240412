# Comparing `tmp/pybankid-1.0.0.tar.gz` & `tmp/pybankid-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybankid-1.0.0.tar", last modified: Thu Mar 28 21:24:02 2024, max compression
+gzip compressed data, was "pybankid-1.0.1.tar", last modified: Fri Apr 12 21:51:33 2024, max compression
```

## Comparing `pybankid-1.0.0.tar` & `pybankid-1.0.1.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:24:02.337893 pybankid-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-28 21:23:58.000000 pybankid-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-28 21:23:58.000000 pybankid-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-03-28 21:24:02.337893 pybankid-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-03-28 21:23:58.000000 pybankid-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:24:02.329893 pybankid-1.0.0/bankid/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14872 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/asyncclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/baseclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:24:02.333893 pybankid-1.0.0/bankid/certs/
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/certs/FPTestcert4_20220818.p12
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/certs/FPTestcert4_20220818_cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/certs/FPTestcert4_20220818_key.pem
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/certs/FPTestcert4_20230629.p12
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/certs/FPTestcert4_20230629_cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/certs/FPTestcert4_20230629_key.pem
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/certs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/certs/appapi.bankid.com.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/certs/appapi.test.bankid.com.pem
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/certs/appapi2.bankid.com.pem
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/certs/appapi2.test.bankid.com.pem
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/certutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:24:02.333893 pybankid-1.0.0/bankid/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/experimental/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/experimental/verify.py
--rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-03-28 21:23:58.000000 pybankid-1.0.0/bankid/syncclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:24:02.329893 pybankid-1.0.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:24:02.333893 pybankid-1.0.0/examples/qrdemo/
--rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-03-28 21:23:58.000000 pybankid-1.0.0/examples/qrdemo/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-28 21:23:58.000000 pybankid-1.0.0/examples/qrdemo/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:24:02.333893 pybankid-1.0.0/examples/qrdemo/qrdemo/
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-03-28 21:23:58.000000 pybankid-1.0.0/examples/qrdemo/qrdemo/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:24:02.333893 pybankid-1.0.0/examples/qrdemo/qrdemo/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-28 21:23:58.000000 pybankid-1.0.0/examples/qrdemo/qrdemo/templates/auth_complete.html
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-28 21:23:58.000000 pybankid-1.0.0/examples/qrdemo/qrdemo/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-03-28 21:23:58.000000 pybankid-1.0.0/examples/qrdemo/qrdemo/templates/qr.html
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-28 21:23:58.000000 pybankid-1.0.0/examples/qrdemo/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:24:02.337893 pybankid-1.0.0/pybankid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-03-28 21:24:02.000000 pybankid-1.0.0/pybankid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-28 21:24:02.000000 pybankid-1.0.0/pybankid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 21:24:02.000000 pybankid-1.0.0/pybankid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-28 21:24:02.000000 pybankid-1.0.0/pybankid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-28 21:24:02.000000 pybankid-1.0.0/pybankid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-28 21:23:58.000000 pybankid-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-28 21:24:02.337893 pybankid-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-03-28 21:23:58.000000 pybankid-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 21:24:02.337893 pybankid-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 21:23:58.000000 pybankid-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-28 21:23:58.000000 pybankid-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-03-28 21:23:58.000000 pybankid-1.0.0/tests/test_asyncclient.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-28 21:23:58.000000 pybankid-1.0.0/tests/test_certutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-28 21:23:58.000000 pybankid-1.0.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-03-28 21:23:58.000000 pybankid-1.0.0/tests/test_syncclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.917935 pybankid-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-12 21:51:29.000000 pybankid-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-12 21:51:29.000000 pybankid-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-12 21:51:33.917935 pybankid-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-04-12 21:51:29.000000 pybankid-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.909934 pybankid-1.0.1/bankid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14872 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/asyncclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/baseclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.909934 pybankid-1.0.1/bankid/certs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/FPTestcert4_20220818.p12
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/FPTestcert4_20220818_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/FPTestcert4_20220818_key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/FPTestcert4_20230629.p12
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/FPTestcert4_20230629_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/FPTestcert4_20230629_key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/appapi.bankid.com.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/appapi.test.bankid.com.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/appapi2.bankid.com.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certs/appapi2.test.bankid.com.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/certutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.913935 pybankid-1.0.1/bankid/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/experimental/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/experimental/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/qr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-04-12 21:51:29.000000 pybankid-1.0.1/bankid/syncclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.905934 pybankid-1.0.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.913935 pybankid-1.0.1/examples/qrdemo/
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-12 21:51:29.000000 pybankid-1.0.1/examples/qrdemo/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-12 21:51:29.000000 pybankid-1.0.1/examples/qrdemo/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.913935 pybankid-1.0.1/examples/qrdemo/qrdemo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-12 21:51:29.000000 pybankid-1.0.1/examples/qrdemo/qrdemo/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.913935 pybankid-1.0.1/examples/qrdemo/qrdemo/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-12 21:51:29.000000 pybankid-1.0.1/examples/qrdemo/qrdemo/templates/auth_complete.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-12 21:51:29.000000 pybankid-1.0.1/examples/qrdemo/qrdemo/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-12 21:51:29.000000 pybankid-1.0.1/examples/qrdemo/qrdemo/templates/qr.html
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-12 21:51:29.000000 pybankid-1.0.1/examples/qrdemo/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.913935 pybankid-1.0.1/pybankid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-12 21:51:33.000000 pybankid-1.0.1/pybankid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-12 21:51:33.000000 pybankid-1.0.1/pybankid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:51:33.000000 pybankid-1.0.1/pybankid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 21:51:33.000000 pybankid-1.0.1/pybankid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 21:51:33.000000 pybankid-1.0.1/pybankid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 21:51:29.000000 pybankid-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 21:51:33.917935 pybankid-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-12 21:51:29.000000 pybankid-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:33.913935 pybankid-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:51:29.000000 pybankid-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-12 21:51:29.000000 pybankid-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-12 21:51:29.000000 pybankid-1.0.1/tests/test_asyncclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-12 21:51:29.000000 pybankid-1.0.1/tests/test_certutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-12 21:51:29.000000 pybankid-1.0.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-12 21:51:29.000000 pybankid-1.0.1/tests/test_syncclient.py
```

### Comparing `pybankid-1.0.0/LICENSE` & `pybankid-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/PKG-INFO` & `pybankid-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybankid
-Version: 1.0.0
+Version: 1.0.1
 Summary: BankID Relying Party client for Python
 Home-page: https://github.com/hbldh/pybankid
 Author: Henrik Blidh
 Author-email: henrik.blidh@nedomkull.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -12,246 +12,206 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: importlib-resources>=5.12.0
 Provides-Extra: signature-verification
+Requires-Dist: pyOpenSSL; extra == "signature-verification"
 Requires-Dist: pytz; extra == "signature-verification"
 Requires-Dist: asn1crypto; extra == "signature-verification"
-Requires-Dist: pyOpenSSL; extra == "signature-verification"
 
 
-PyBankID
-========
+# PyBankID
 
-.. image:: https://github.com/hbldh/pybankid/workflows/Build%20and%20Test/badge.svg
-    :target: https://github.com/hbldh/pybankid/actions?query=workflow%3A%22Build+and+Test%22
-.. image:: https://readthedocs.org/projects/pybankid/badge/?version=latest
-    :target: http://pybankid.readthedocs.org/en/latest/?badge=latest
-    :alt: Documentation Status
-.. image:: http://img.shields.io/pypi/v/pybankid.svg
-    :target: https://pypi.python.org/pypi/pybankid/
-.. image:: http://img.shields.io/pypi/l/pybankid.svg
-    :target: https://pypi.python.org/pypi/pybankid/
-.. image:: https://coveralls.io/repos/github/hbldh/pybankid/badge.svg?branch=master
-    :target: https://coveralls.io/github/hbldh/pybankid?branch=master
-
-PyBankID is a client for providing BankID services as a Relying Party, i.e.
-providing authentication and signing functionality to end users. This package
-provides a simplifying interface for initiating authentication
-and signing orders and then collecting the results from the BankID servers.
-
-The only supported BankID API version supported by PyBankID from version 1.0.0
-is v6.0, which means that the Secure Start solution is the only supported way
-of providing BankID services. PyBankID versions prior to 1.0.0 will not
-work after 1st of May 2024.
-
-If you intend to use PyBankID in your project, you are advised to read
-the `BankID Integration Guide
-<https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide>`_ before
-doing anything else. There, one can find information
-about how the BankID methods are defined and how to use them.
-
-Installation
-------------
-
-PyBankID can be installed though pip:
-
-.. code-block:: bash
-
-    pip install pybankid
-
-Usage
------
-
-PyBankID provides both a synchronous and an asynchronous client for
-communication with BankID services. Example below will use the asynchronous
-client, but the synchronous client is used in the same way by merely omitting
-the ``await`` keyword.
-
-Synchronous client
-~~~~~~~~~~~~~~~~~~
-
-.. code-block:: python
-
-    >>> from bankid import BankIDClient
-    >>> client = BankIDClient(certificates=(
-       'path/to/certificate.pem',
-       'path/to/key.pem',
-    ))
-
-Connection to production server is the default in the client. If test
-server is desired, send in the ``test_server=True`` keyword in the init
-of the client.
-
-When using the JSON client, authentication and signing calls requires
-the end user's ip address to be included in all calls. An authentication order
-is initiated as such:
-
-.. code-block:: python
-
-    >>> client.authenticate(end_user_ip='194.168.2.25')
-    {
-        'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
-        'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
-        'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
-        'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
-    }
+![Build and Test](https://github.com/hbldh/pybankid/workflows/Build%20and%20Test/badge.svg)
+![Documentation Status](https://readthedocs.org/projects/pybankid/badge/?version=latest)
+![PyPI Version](http://img.shields.io/pypi/v/pybankid.svg)
+![PyPI License](http://img.shields.io/pypi/l/pybankid.svg)
+![Coverage](https://coveralls.io/repos/github/hbldh/pybankid/badge.svg?branch=master)
 
-and a sign order is initiated in a similar fashion:
+PyBankID is a client for providing BankID services as a Relying Party, i.e., providing authentication and signing functionality to end users. This package provides a simplifying interface for initiating authentication and signing orders and then collecting the results from the BankID servers.
+
+The only supported BankID API version supported by PyBankID from version 1.0.0 is v6.0, which means that the Secure Start solution is the only supported way of providing BankID services. PyBankID versions prior to 1.0.0 will not work after 1st of May 2024.
+
+If you intend to use PyBankID in your project, you are advised to read the [BankID Integration Guide](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide) before doing anything else. There, one can find information about how the BankID methods are defined and how to use them.
+
+## Installation
+
+PyBankID can be installed through pip:
+
+```bash
+pip install pybankid
+```
+
+## Usage
 
-.. code-block:: python
+PyBankID provides both a synchronous and an asynchronous client for communication with BankID services. The example below will use the asynchronous client, but the synchronous client is used in the same way by merely omitting the `await` keyword.
 
-    >>> client.sign(
-       end_user_ip='194.168.2.25',
-       user_visible_data="The information to sign."
-    )
-    {
-        'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
-        'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
-        'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
-        'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
-    }
-
-If you want to ascertain that only one individual can authenticate or sign, you can
-specify this using the ``requirement`` keyword:
-
-.. code-block:: python
-
-    >>> client.sign(
-       end_user_ip='194.168.2.25',
-       user_visible_data="The information to sign."
-       requirement={"personalNumber": "YYYYMMDDXXXX"}
-    )
-    {
-        'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
-        'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
-        'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
-        'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
-    }
-
-If someone else than the one you specified tries to authenticate or sign, the
-BankID app will state that the request is not intended for the user.
-
-The status of an order can then be studied by polling
-with the ``collect`` method using the received ``orderRef``:
-
-.. code-block:: python
-
-    >>> client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
-    {
-        'hintCode': 'outstandingTransaction',
-        'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
-        'status': 'pending'
-    }
-    >>> client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
-    {
-        'hintCode': 'userSign',
-        'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
-        'status': 'pending'
-    }
-    >>> client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
-    {
-        'completionData': {
-            'cert': {
-                'notAfter': '1581289199000',
-                'notBefore': '1518130800000'
-            },
-            'device': {
-                'ipAddress': '0.0.0.0'
-            },
-            'ocspResponse': 'MIIHegoBAKCCB[...]',
-            'signature': 'PD94bWwgdmVyc2lv[...]',
-            'user': {
-                'givenName': 'Namn',
-                'name': 'Namn Namnsson',
-                'personalNumber': 'YYYYMMDDXXXX',
-                'surname': 'Namnsson'
-            }
+### Synchronous client
+
+```python
+from bankid import BankIDClient
+client = BankIDClient(certificates=(
+    'path/to/certificate.pem', 
+    'path/to/key.pem', 
+))
+```
+
+Connection to the production server is the default in the client. If a test server is desired, send in the `test_server=True` keyword in the init of the client.
+
+When using the JSON client, authentication and signing calls require the end user's IP address to be included in all calls. An authentication order is initiated as such:
+
+```python
+client.authenticate(end_user_ip='194.168.2.25')
+{
+    'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
+    'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
+    'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
+    'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
+}
+```
+
+and a sign order is initiated in a similar fashion:
+
+```python
+client.sign(
+    end_user_ip='194.168.2.25',
+    user_visible_data="The information to sign."
+)
+{
+    'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
+    'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
+    'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
+    'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
+}
+```
+
+If you want to ascertain that only one individual can authenticate or sign, you can specify this using the `requirement` keyword:
+
+```python
+client.sign(
+   end_user_ip='194.168.2.25',
+   user_visible_data="The information to sign."
+   requirement={"personalNumber": "YYYYMMDDXXXX"}
+)
+{
+    'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
+    'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
+    'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
+    'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
+}
+```
+
+If someone else than the one you specified tries to authenticate or sign, the BankID app will state that the request is not intended for the user.
+
+The status of an order can then be studied by polling with the `collect` method using the received `orderRef`:
+
+```python
+client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
+{
+    'hintCode': 'outstandingTransaction',
+    'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
+    'status': 'pending'
+}
+```
+
+```python
+client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
+{
+    'hintCode': 'userSign',
+    'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
+    'status': 'pending'
+}
+```
+
+```python
+client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
+{
+    'completionData': {
+        'cert': {
+            'notAfter': '1581289199000',
+            'notBefore': '1518130800000'
+        },
+        'device': {
+            'ipAddress': '0.0.0.0'
         },
-        'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
-        'status': 'complete'
-    }
-
-Please note that the ``collect`` method should be used sparingly: in the
-`BankID Integration Guide <https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide>`_
-it is specified that *"collect should be called every two seconds and must not be
-called more frequent than once per second"*.
-
-Asynchronous client
-~~~~~~~~~~~~~~~~~~~
-
-The asynchronous client is used in the same way as the asynchronous client, but the
-methods are blocking.
-
-The synchronous guide above can be used as a reference for the asynchronous client
-as well, by simply adding the ``await`` keyword:
-
-.. code-block:: python
-
-    >>> from bankid import BankIDAsyncClient
-    >>> client = BankIDAsyncClient(certificates=(
-        'path/to/certificate.pem',
-        'path/to/key.pem',
-    ))
-    >>> await client.authenticate(end_user_ip='194.168.2.25')
-    {
-        'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
-        'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
-        'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
-        'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
-    }
-
-PyBankID and QR codes
-~~~~~~~~~~~~~~~~~~~~~
-
-PyBankID can generate QR codes for you, and there is an example application in the
-`examples folder of the repo <https://github.com/hbldh/pybankid/tree/master/examples>`_ where a
-Flask application called ``qrdemo`` shows one way to do authentication with animated QR codes.
-
-Certificates
-------------
-
-Production certificates
-~~~~~~~~~~~~~~~~~~~~~~~
-
-If you want to use BankID in a production environment, then you will have to
-purchase this service from one of the
-`selling banks <https://www.bankid.com/foretag/anslut-foeretag>`_.
-They will then provide you with a certificate that can be used to authenticate
-your company/application with the BankID servers.
-
-This certificate has to be processed somewhat to be able to use with PyBankID,
-and how to do this depends on what the selling bank provides you with.
-
-Test certificate
-~~~~~~~~~~~~~~~~
-
-The certificate to use when developing against the BankID test servers can
-be obtained through PyBankID:
-
-.. code-block:: python
-
-    >>> import os
-    >>> import bankid
-    >>> dir_to_save_cert_and_key_in = os.path.expanduser('~')
-    >>> cert_and_key = bankid.create_bankid_test_server_cert_and_key(
-        dir_to_save_cert_and_key_in)
-    >>> print(cert_and_key)
-    ['/home/hbldh/certificate.pem', '/home/hbldh/key.pem']
-    >>> client = bankid.BankIDClient(
-        certificates=cert_and_key, test_server=True)
+        'ocspResponse': 'MIIHegoBAKCCB[...]',
+        'signature': 'PD94bWwgdmVyc2lv[...]',
+        'user': {
+            'givenName': 'Namn',
+            'name': 'Namn Namnsson',
+            'personalNumber': 'YYYYMMDDXXXX',
+            'surname': 'Namnsson'
+        }
+    },
+    'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
+    'status': 'complete'
+}
+```
+
+
+Please note that the `collect` method should be used sparingly: in the [BankID Integration Guide](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide) it is specified that *"collect should be called every two seconds and must not be called more frequent than once per second"*.
+
+### Asynchronous client
+
+The asynchronous client is used in the same way as the synchronous client, but the methods are blocking.
+
+The synchronous guide above can be used as a reference for the asynchronous client as well, by simply adding the `await` keyword:
+
+```python
+from bankid import BankIDClientAsync
+client = BankIDClientAsync(certificates=(
+    'path/to/certificate.pem', 
+    'path/to/key.pem', 
+))
+
+await client.authenticate(end_user_ip='194.168.2.25')
+{
+    'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
+    'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
+    'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
+    'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
+}
+```
+
+
+## PyBankID and QR codes
+
+PyBankID can generate QR codes for you, and there is an example application in the [examples folder of the repo](https://github.com/hbldh/pybankid/tree/master/examples) where a Flask application called `qrdemo` shows one way to do authentication with animated QR codes.
+
+## Certificates
+
+### Production certificates
+
+If you want to use BankID in a production environment, then you will have to purchase this service from one of the [selling banks](https://www.bankid.com/foretag/anslut-foeretag). They will then provide you with a certificate that can be used to authenticate your company/application with the BankID servers.
+
+This certificate has to be processed somewhat to be able to use with PyBankID, and how to do this depends on what the selling bank provides you with.
+
+### Test certificate
+
+The certificate to use when developing against the BankID test servers can be obtained through PyBankID:
 
-Testing
--------
+```python
+import os
+import bankid
+dir_to_save_cert_and_key_in = os.path.expanduser('~')
+cert_and_key = bankid.create_bankid_test_server_cert_and_key(
+    dir_to_save_cert_and_key_in)
+print(cert_and_key)
+['/home/hbldh/certificate.pem', '/home/hbldh/key.pem']
+client = bankid.BankIDClient(
+    certificates=cert_and_key, test_server=True)
+```
 
-The PyBankID solution can be tested with `pytest <https://pytest.org/>`_:
+## Testing
 
-.. code-block:: bash
+The PyBankID solution can be tested with [pytest](https://pytest.org/):
 
-    py.test tests/
+```bash
+pytest tests/
+```
```

### Comparing `pybankid-1.0.0/README.rst` & `pybankid-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,229 +1,189 @@
-PyBankID
-========
+# PyBankID
 
-.. image:: https://github.com/hbldh/pybankid/workflows/Build%20and%20Test/badge.svg
-    :target: https://github.com/hbldh/pybankid/actions?query=workflow%3A%22Build+and+Test%22
-.. image:: https://readthedocs.org/projects/pybankid/badge/?version=latest
-    :target: http://pybankid.readthedocs.org/en/latest/?badge=latest
-    :alt: Documentation Status
-.. image:: http://img.shields.io/pypi/v/pybankid.svg
-    :target: https://pypi.python.org/pypi/pybankid/
-.. image:: http://img.shields.io/pypi/l/pybankid.svg
-    :target: https://pypi.python.org/pypi/pybankid/
-.. image:: https://coveralls.io/repos/github/hbldh/pybankid/badge.svg?branch=master
-    :target: https://coveralls.io/github/hbldh/pybankid?branch=master
-
-PyBankID is a client for providing BankID services as a Relying Party, i.e.
-providing authentication and signing functionality to end users. This package
-provides a simplifying interface for initiating authentication
-and signing orders and then collecting the results from the BankID servers.
-
-The only supported BankID API version supported by PyBankID from version 1.0.0
-is v6.0, which means that the Secure Start solution is the only supported way
-of providing BankID services. PyBankID versions prior to 1.0.0 will not
-work after 1st of May 2024.
-
-If you intend to use PyBankID in your project, you are advised to read
-the `BankID Integration Guide
-<https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide>`_ before
-doing anything else. There, one can find information
-about how the BankID methods are defined and how to use them.
-
-Installation
-------------
-
-PyBankID can be installed though pip:
-
-.. code-block:: bash
-
-    pip install pybankid
-
-Usage
------
-
-PyBankID provides both a synchronous and an asynchronous client for
-communication with BankID services. Example below will use the asynchronous
-client, but the synchronous client is used in the same way by merely omitting
-the ``await`` keyword.
-
-Synchronous client
-~~~~~~~~~~~~~~~~~~
-
-.. code-block:: python
-
-    >>> from bankid import BankIDClient
-    >>> client = BankIDClient(certificates=(
-       'path/to/certificate.pem',
-       'path/to/key.pem',
-    ))
-
-Connection to production server is the default in the client. If test
-server is desired, send in the ``test_server=True`` keyword in the init
-of the client.
-
-When using the JSON client, authentication and signing calls requires
-the end user's ip address to be included in all calls. An authentication order
-is initiated as such:
-
-.. code-block:: python
-
-    >>> client.authenticate(end_user_ip='194.168.2.25')
-    {
-        'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
-        'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
-        'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
-        'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
-    }
+![Build and Test](https://github.com/hbldh/pybankid/workflows/Build%20and%20Test/badge.svg)
+![Documentation Status](https://readthedocs.org/projects/pybankid/badge/?version=latest)
+![PyPI Version](http://img.shields.io/pypi/v/pybankid.svg)
+![PyPI License](http://img.shields.io/pypi/l/pybankid.svg)
+![Coverage](https://coveralls.io/repos/github/hbldh/pybankid/badge.svg?branch=master)
 
-and a sign order is initiated in a similar fashion:
+PyBankID is a client for providing BankID services as a Relying Party, i.e., providing authentication and signing functionality to end users. This package provides a simplifying interface for initiating authentication and signing orders and then collecting the results from the BankID servers.
+
+The only supported BankID API version supported by PyBankID from version 1.0.0 is v6.0, which means that the Secure Start solution is the only supported way of providing BankID services. PyBankID versions prior to 1.0.0 will not work after 1st of May 2024.
+
+If you intend to use PyBankID in your project, you are advised to read the [BankID Integration Guide](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide) before doing anything else. There, one can find information about how the BankID methods are defined and how to use them.
+
+## Installation
+
+PyBankID can be installed through pip:
+
+```bash
+pip install pybankid
+```
+
+## Usage
+
+PyBankID provides both a synchronous and an asynchronous client for communication with BankID services. The example below will use the asynchronous client, but the synchronous client is used in the same way by merely omitting the `await` keyword.
 
-.. code-block:: python
+### Synchronous client
 
-    >>> client.sign(
-       end_user_ip='194.168.2.25',
-       user_visible_data="The information to sign."
-    )
-    {
-        'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
-        'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
-        'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
-        'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
-    }
-
-If you want to ascertain that only one individual can authenticate or sign, you can
-specify this using the ``requirement`` keyword:
-
-.. code-block:: python
-
-    >>> client.sign(
-       end_user_ip='194.168.2.25',
-       user_visible_data="The information to sign."
-       requirement={"personalNumber": "YYYYMMDDXXXX"}
-    )
-    {
-        'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
-        'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
-        'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
-        'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
-    }
-
-If someone else than the one you specified tries to authenticate or sign, the
-BankID app will state that the request is not intended for the user.
-
-The status of an order can then be studied by polling
-with the ``collect`` method using the received ``orderRef``:
-
-.. code-block:: python
-
-    >>> client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
-    {
-        'hintCode': 'outstandingTransaction',
-        'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
-        'status': 'pending'
-    }
-    >>> client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
-    {
-        'hintCode': 'userSign',
-        'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
-        'status': 'pending'
-    }
-    >>> client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
-    {
-        'completionData': {
-            'cert': {
-                'notAfter': '1581289199000',
-                'notBefore': '1518130800000'
-            },
-            'device': {
-                'ipAddress': '0.0.0.0'
-            },
-            'ocspResponse': 'MIIHegoBAKCCB[...]',
-            'signature': 'PD94bWwgdmVyc2lv[...]',
-            'user': {
-                'givenName': 'Namn',
-                'name': 'Namn Namnsson',
-                'personalNumber': 'YYYYMMDDXXXX',
-                'surname': 'Namnsson'
-            }
+```python
+from bankid import BankIDClient
+client = BankIDClient(certificates=(
+    'path/to/certificate.pem', 
+    'path/to/key.pem', 
+))
+```
+
+Connection to the production server is the default in the client. If a test server is desired, send in the `test_server=True` keyword in the init of the client.
+
+When using the JSON client, authentication and signing calls require the end user's IP address to be included in all calls. An authentication order is initiated as such:
+
+```python
+client.authenticate(end_user_ip='194.168.2.25')
+{
+    'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
+    'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
+    'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
+    'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
+}
+```
+
+and a sign order is initiated in a similar fashion:
+
+```python
+client.sign(
+    end_user_ip='194.168.2.25',
+    user_visible_data="The information to sign."
+)
+{
+    'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
+    'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
+    'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
+    'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
+}
+```
+
+If you want to ascertain that only one individual can authenticate or sign, you can specify this using the `requirement` keyword:
+
+```python
+client.sign(
+   end_user_ip='194.168.2.25',
+   user_visible_data="The information to sign."
+   requirement={"personalNumber": "YYYYMMDDXXXX"}
+)
+{
+    'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
+    'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
+    'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
+    'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
+}
+```
+
+If someone else than the one you specified tries to authenticate or sign, the BankID app will state that the request is not intended for the user.
+
+The status of an order can then be studied by polling with the `collect` method using the received `orderRef`:
+
+```python
+client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
+{
+    'hintCode': 'outstandingTransaction',
+    'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
+    'status': 'pending'
+}
+```
+
+```python
+client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
+{
+    'hintCode': 'userSign',
+    'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
+    'status': 'pending'
+}
+```
+
+```python
+client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
+{
+    'completionData': {
+        'cert': {
+            'notAfter': '1581289199000',
+            'notBefore': '1518130800000'
         },
-        'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
-        'status': 'complete'
-    }
-
-Please note that the ``collect`` method should be used sparingly: in the
-`BankID Integration Guide <https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide>`_
-it is specified that *"collect should be called every two seconds and must not be
-called more frequent than once per second"*.
-
-Asynchronous client
-~~~~~~~~~~~~~~~~~~~
-
-The asynchronous client is used in the same way as the asynchronous client, but the
-methods are blocking.
-
-The synchronous guide above can be used as a reference for the asynchronous client
-as well, by simply adding the ``await`` keyword:
-
-.. code-block:: python
-
-    >>> from bankid import BankIDAsyncClient
-    >>> client = BankIDAsyncClient(certificates=(
-        'path/to/certificate.pem',
-        'path/to/key.pem',
-    ))
-    >>> await client.authenticate(end_user_ip='194.168.2.25')
-    {
-        'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
-        'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
-        'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
-        'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
-    }
-
-PyBankID and QR codes
-~~~~~~~~~~~~~~~~~~~~~
-
-PyBankID can generate QR codes for you, and there is an example application in the
-`examples folder of the repo <https://github.com/hbldh/pybankid/tree/master/examples>`_ where a
-Flask application called ``qrdemo`` shows one way to do authentication with animated QR codes.
-
-Certificates
-------------
-
-Production certificates
-~~~~~~~~~~~~~~~~~~~~~~~
-
-If you want to use BankID in a production environment, then you will have to
-purchase this service from one of the
-`selling banks <https://www.bankid.com/foretag/anslut-foeretag>`_.
-They will then provide you with a certificate that can be used to authenticate
-your company/application with the BankID servers.
-
-This certificate has to be processed somewhat to be able to use with PyBankID,
-and how to do this depends on what the selling bank provides you with.
-
-Test certificate
-~~~~~~~~~~~~~~~~
-
-The certificate to use when developing against the BankID test servers can
-be obtained through PyBankID:
-
-.. code-block:: python
-
-    >>> import os
-    >>> import bankid
-    >>> dir_to_save_cert_and_key_in = os.path.expanduser('~')
-    >>> cert_and_key = bankid.create_bankid_test_server_cert_and_key(
-        dir_to_save_cert_and_key_in)
-    >>> print(cert_and_key)
-    ['/home/hbldh/certificate.pem', '/home/hbldh/key.pem']
-    >>> client = bankid.BankIDClient(
-        certificates=cert_and_key, test_server=True)
+        'device': {
+            'ipAddress': '0.0.0.0'
+        },
+        'ocspResponse': 'MIIHegoBAKCCB[...]',
+        'signature': 'PD94bWwgdmVyc2lv[...]',
+        'user': {
+            'givenName': 'Namn',
+            'name': 'Namn Namnsson',
+            'personalNumber': 'YYYYMMDDXXXX',
+            'surname': 'Namnsson'
+        }
+    },
+    'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
+    'status': 'complete'
+}
+```
+
+
+Please note that the `collect` method should be used sparingly: in the [BankID Integration Guide](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide) it is specified that *"collect should be called every two seconds and must not be called more frequent than once per second"*.
+
+### Asynchronous client
+
+The asynchronous client is used in the same way as the synchronous client, but the methods are blocking.
+
+The synchronous guide above can be used as a reference for the asynchronous client as well, by simply adding the `await` keyword:
+
+```python
+from bankid import BankIDClientAsync
+client = BankIDClientAsync(certificates=(
+    'path/to/certificate.pem', 
+    'path/to/key.pem', 
+))
+
+await client.authenticate(end_user_ip='194.168.2.25')
+{
+    'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
+    'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
+    'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
+    'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
+}
+```
+
+
+## PyBankID and QR codes
+
+PyBankID can generate QR codes for you, and there is an example application in the [examples folder of the repo](https://github.com/hbldh/pybankid/tree/master/examples) where a Flask application called `qrdemo` shows one way to do authentication with animated QR codes.
+
+## Certificates
+
+### Production certificates
+
+If you want to use BankID in a production environment, then you will have to purchase this service from one of the [selling banks](https://www.bankid.com/foretag/anslut-foeretag). They will then provide you with a certificate that can be used to authenticate your company/application with the BankID servers.
+
+This certificate has to be processed somewhat to be able to use with PyBankID, and how to do this depends on what the selling bank provides you with.
+
+### Test certificate
+
+The certificate to use when developing against the BankID test servers can be obtained through PyBankID:
 
-Testing
--------
+```python
+import os
+import bankid
+dir_to_save_cert_and_key_in = os.path.expanduser('~')
+cert_and_key = bankid.create_bankid_test_server_cert_and_key(
+    dir_to_save_cert_and_key_in)
+print(cert_and_key)
+['/home/hbldh/certificate.pem', '/home/hbldh/key.pem']
+client = bankid.BankIDClient(
+    certificates=cert_and_key, test_server=True)
+```
 
-The PyBankID solution can be tested with `pytest <https://pytest.org/>`_:
+## Testing
 
-.. code-block:: bash
+The PyBankID solution can be tested with [pytest](https://pytest.org/):
 
-    py.test tests/
+```bash
+pytest tests/
+```
```

### Comparing `pybankid-1.0.0/bankid/__init__.py` & `pybankid-1.0.1/bankid/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,18 @@
 """
 
 from bankid import exceptions
 from bankid.__version__ import __version__, version
 from bankid.certutils import create_bankid_test_server_cert_and_key
 from bankid.syncclient import BankIDClient
 from bankid.asyncclient import BankIDAsyncClient
+from bankid.qr import generate_qr_code_content
 
 __all__ = [
     "BankIDClient",
     "BankIDAsyncClient",
     "exceptions",
     "create_bankid_test_server_cert_and_key",
+    "generate_qr_code_content",
     "__version__",
     "version",
 ]
```

### Comparing `pybankid-1.0.0/bankid/asyncclient.py` & `pybankid-1.0.1/bankid/asyncclient.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/bankid/baseclient.py` & `pybankid-1.0.1/bankid/baseclient.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import base64
 from datetime import datetime
-import hashlib
-import hmac
-from math import floor
-import time
 from typing import Tuple, Optional, Dict, Any
 from urllib.parse import urljoin
 
+from bankid.qr import generate_qr_code_content
 from bankid.certutils import resolve_cert_path
 
 
 class BankIDClientBaseclass:
     """Baseclass for BankID clients.
 
     Both the synchronous and asynchronous clients inherit from this base class and has the methods implemented here.
@@ -38,27 +35,16 @@
         self._phone_sign_endpoint = urljoin(self.api_url, "phone/sign")
         self._collect_endpoint = urljoin(self.api_url, "collect")
         self._cancel_endpoint = urljoin(self.api_url, "cancel")
 
         self.client = None
 
     @staticmethod
-    def generate_qr_code_content(qr_start_token: str, start_t: [float, datetime], qr_start_secret: str):
-        """Given QR start token, time.time() or UTC datetime when initiated authentication call was made and the
-        QR start secret, calculate the current QR code content to display.
-        """
-        if isinstance(start_t, datetime):
-            start_t = start_t.timestamp()
-        elapsed_seconds_since_call = int(floor(time.time() - start_t))
-        qr_auth_code = hmac.new(
-            qr_start_secret.encode(),
-            msg=str(elapsed_seconds_since_call).encode(),
-            digestmod=hashlib.sha256,
-        ).hexdigest()
-        return f"bankid.{qr_start_token}.{elapsed_seconds_since_call}.{qr_auth_code}"
+    def generate_qr_code_content(qr_start_token: str, start_t: [float, datetime], qr_start_secret: str) -> str:
+        return generate_qr_code_content(qr_start_token, start_t, qr_start_secret)
 
     @staticmethod
     def _encode_user_data(user_data):
         if isinstance(user_data, str):
             return base64.b64encode(user_data.encode("utf-8")).decode("ascii")
         else:
             return base64.b64encode(user_data).decode("ascii")
```

### Comparing `pybankid-1.0.0/bankid/certs/FPTestcert4_20220818.p12` & `pybankid-1.0.1/bankid/certs/FPTestcert4_20220818.p12`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/bankid/certs/FPTestcert4_20220818_cert.pem` & `pybankid-1.0.1/bankid/certs/FPTestcert4_20220818_cert.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/bankid/certs/FPTestcert4_20220818_key.pem` & `pybankid-1.0.1/bankid/certs/FPTestcert4_20220818_key.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/bankid/certs/FPTestcert4_20230629.p12` & `pybankid-1.0.1/bankid/certs/FPTestcert4_20230629.p12`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/bankid/certs/FPTestcert4_20230629_cert.pem` & `pybankid-1.0.1/bankid/certs/FPTestcert4_20230629_cert.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/bankid/certs/FPTestcert4_20230629_key.pem` & `pybankid-1.0.1/bankid/certs/FPTestcert4_20230629_key.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/bankid/certs/appapi.bankid.com.pem` & `pybankid-1.0.1/bankid/certs/appapi.bankid.com.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/bankid/certs/appapi.test.bankid.com.pem` & `pybankid-1.0.1/bankid/certs/appapi.test.bankid.com.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/bankid/certs/appapi2.bankid.com.pem` & `pybankid-1.0.1/bankid/certs/appapi2.bankid.com.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/bankid/certs/appapi2.test.bankid.com.pem` & `pybankid-1.0.1/bankid/certs/appapi2.test.bankid.com.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/bankid/certutils.py` & `pybankid-1.0.1/bankid/certutils.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/bankid/exceptions.py` & `pybankid-1.0.1/bankid/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/bankid/experimental/helper.py` & `pybankid-1.0.1/bankid/experimental/helper.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/bankid/experimental/verify.py` & `pybankid-1.0.1/bankid/experimental/verify.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/bankid/syncclient.py` & `pybankid-1.0.1/bankid/syncclient.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/examples/qrdemo/.gitignore` & `pybankid-1.0.1/examples/qrdemo/.gitignore`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/examples/qrdemo/README.md` & `pybankid-1.0.1/examples/qrdemo/README.md`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/examples/qrdemo/qrdemo/app.py` & `pybankid-1.0.1/examples/qrdemo/qrdemo/app.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/examples/qrdemo/qrdemo/templates/auth_complete.html` & `pybankid-1.0.1/examples/qrdemo/qrdemo/templates/auth_complete.html`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/examples/qrdemo/qrdemo/templates/index.html` & `pybankid-1.0.1/examples/qrdemo/qrdemo/templates/index.html`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/examples/qrdemo/qrdemo/templates/qr.html` & `pybankid-1.0.1/examples/qrdemo/qrdemo/templates/qr.html`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/pybankid.egg-info/PKG-INFO` & `pybankid-1.0.1/pybankid.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybankid
-Version: 1.0.0
+Version: 1.0.1
 Summary: BankID Relying Party client for Python
 Home-page: https://github.com/hbldh/pybankid
 Author: Henrik Blidh
 Author-email: henrik.blidh@nedomkull.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -12,246 +12,206 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: importlib-resources>=5.12.0
 Provides-Extra: signature-verification
+Requires-Dist: pyOpenSSL; extra == "signature-verification"
 Requires-Dist: pytz; extra == "signature-verification"
 Requires-Dist: asn1crypto; extra == "signature-verification"
-Requires-Dist: pyOpenSSL; extra == "signature-verification"
 
 
-PyBankID
-========
+# PyBankID
 
-.. image:: https://github.com/hbldh/pybankid/workflows/Build%20and%20Test/badge.svg
-    :target: https://github.com/hbldh/pybankid/actions?query=workflow%3A%22Build+and+Test%22
-.. image:: https://readthedocs.org/projects/pybankid/badge/?version=latest
-    :target: http://pybankid.readthedocs.org/en/latest/?badge=latest
-    :alt: Documentation Status
-.. image:: http://img.shields.io/pypi/v/pybankid.svg
-    :target: https://pypi.python.org/pypi/pybankid/
-.. image:: http://img.shields.io/pypi/l/pybankid.svg
-    :target: https://pypi.python.org/pypi/pybankid/
-.. image:: https://coveralls.io/repos/github/hbldh/pybankid/badge.svg?branch=master
-    :target: https://coveralls.io/github/hbldh/pybankid?branch=master
-
-PyBankID is a client for providing BankID services as a Relying Party, i.e.
-providing authentication and signing functionality to end users. This package
-provides a simplifying interface for initiating authentication
-and signing orders and then collecting the results from the BankID servers.
-
-The only supported BankID API version supported by PyBankID from version 1.0.0
-is v6.0, which means that the Secure Start solution is the only supported way
-of providing BankID services. PyBankID versions prior to 1.0.0 will not
-work after 1st of May 2024.
-
-If you intend to use PyBankID in your project, you are advised to read
-the `BankID Integration Guide
-<https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide>`_ before
-doing anything else. There, one can find information
-about how the BankID methods are defined and how to use them.
-
-Installation
-------------
-
-PyBankID can be installed though pip:
-
-.. code-block:: bash
-
-    pip install pybankid
-
-Usage
------
-
-PyBankID provides both a synchronous and an asynchronous client for
-communication with BankID services. Example below will use the asynchronous
-client, but the synchronous client is used in the same way by merely omitting
-the ``await`` keyword.
-
-Synchronous client
-~~~~~~~~~~~~~~~~~~
-
-.. code-block:: python
-
-    >>> from bankid import BankIDClient
-    >>> client = BankIDClient(certificates=(
-       'path/to/certificate.pem',
-       'path/to/key.pem',
-    ))
-
-Connection to production server is the default in the client. If test
-server is desired, send in the ``test_server=True`` keyword in the init
-of the client.
-
-When using the JSON client, authentication and signing calls requires
-the end user's ip address to be included in all calls. An authentication order
-is initiated as such:
-
-.. code-block:: python
-
-    >>> client.authenticate(end_user_ip='194.168.2.25')
-    {
-        'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
-        'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
-        'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
-        'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
-    }
+![Build and Test](https://github.com/hbldh/pybankid/workflows/Build%20and%20Test/badge.svg)
+![Documentation Status](https://readthedocs.org/projects/pybankid/badge/?version=latest)
+![PyPI Version](http://img.shields.io/pypi/v/pybankid.svg)
+![PyPI License](http://img.shields.io/pypi/l/pybankid.svg)
+![Coverage](https://coveralls.io/repos/github/hbldh/pybankid/badge.svg?branch=master)
 
-and a sign order is initiated in a similar fashion:
+PyBankID is a client for providing BankID services as a Relying Party, i.e., providing authentication and signing functionality to end users. This package provides a simplifying interface for initiating authentication and signing orders and then collecting the results from the BankID servers.
+
+The only supported BankID API version supported by PyBankID from version 1.0.0 is v6.0, which means that the Secure Start solution is the only supported way of providing BankID services. PyBankID versions prior to 1.0.0 will not work after 1st of May 2024.
+
+If you intend to use PyBankID in your project, you are advised to read the [BankID Integration Guide](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide) before doing anything else. There, one can find information about how the BankID methods are defined and how to use them.
+
+## Installation
+
+PyBankID can be installed through pip:
+
+```bash
+pip install pybankid
+```
+
+## Usage
 
-.. code-block:: python
+PyBankID provides both a synchronous and an asynchronous client for communication with BankID services. The example below will use the asynchronous client, but the synchronous client is used in the same way by merely omitting the `await` keyword.
 
-    >>> client.sign(
-       end_user_ip='194.168.2.25',
-       user_visible_data="The information to sign."
-    )
-    {
-        'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
-        'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
-        'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
-        'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
-    }
-
-If you want to ascertain that only one individual can authenticate or sign, you can
-specify this using the ``requirement`` keyword:
-
-.. code-block:: python
-
-    >>> client.sign(
-       end_user_ip='194.168.2.25',
-       user_visible_data="The information to sign."
-       requirement={"personalNumber": "YYYYMMDDXXXX"}
-    )
-    {
-        'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
-        'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
-        'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
-        'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
-    }
-
-If someone else than the one you specified tries to authenticate or sign, the
-BankID app will state that the request is not intended for the user.
-
-The status of an order can then be studied by polling
-with the ``collect`` method using the received ``orderRef``:
-
-.. code-block:: python
-
-    >>> client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
-    {
-        'hintCode': 'outstandingTransaction',
-        'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
-        'status': 'pending'
-    }
-    >>> client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
-    {
-        'hintCode': 'userSign',
-        'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
-        'status': 'pending'
-    }
-    >>> client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
-    {
-        'completionData': {
-            'cert': {
-                'notAfter': '1581289199000',
-                'notBefore': '1518130800000'
-            },
-            'device': {
-                'ipAddress': '0.0.0.0'
-            },
-            'ocspResponse': 'MIIHegoBAKCCB[...]',
-            'signature': 'PD94bWwgdmVyc2lv[...]',
-            'user': {
-                'givenName': 'Namn',
-                'name': 'Namn Namnsson',
-                'personalNumber': 'YYYYMMDDXXXX',
-                'surname': 'Namnsson'
-            }
+### Synchronous client
+
+```python
+from bankid import BankIDClient
+client = BankIDClient(certificates=(
+    'path/to/certificate.pem', 
+    'path/to/key.pem', 
+))
+```
+
+Connection to the production server is the default in the client. If a test server is desired, send in the `test_server=True` keyword in the init of the client.
+
+When using the JSON client, authentication and signing calls require the end user's IP address to be included in all calls. An authentication order is initiated as such:
+
+```python
+client.authenticate(end_user_ip='194.168.2.25')
+{
+    'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
+    'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
+    'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
+    'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
+}
+```
+
+and a sign order is initiated in a similar fashion:
+
+```python
+client.sign(
+    end_user_ip='194.168.2.25',
+    user_visible_data="The information to sign."
+)
+{
+    'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
+    'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
+    'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
+    'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
+}
+```
+
+If you want to ascertain that only one individual can authenticate or sign, you can specify this using the `requirement` keyword:
+
+```python
+client.sign(
+   end_user_ip='194.168.2.25',
+   user_visible_data="The information to sign."
+   requirement={"personalNumber": "YYYYMMDDXXXX"}
+)
+{
+    'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
+    'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
+    'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
+    'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
+}
+```
+
+If someone else than the one you specified tries to authenticate or sign, the BankID app will state that the request is not intended for the user.
+
+The status of an order can then be studied by polling with the `collect` method using the received `orderRef`:
+
+```python
+client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
+{
+    'hintCode': 'outstandingTransaction',
+    'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
+    'status': 'pending'
+}
+```
+
+```python
+client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
+{
+    'hintCode': 'userSign',
+    'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
+    'status': 'pending'
+}
+```
+
+```python
+client.collect(order_ref="a9b791c3-459f-492b-bf61-23027876140b")
+{
+    'completionData': {
+        'cert': {
+            'notAfter': '1581289199000',
+            'notBefore': '1518130800000'
+        },
+        'device': {
+            'ipAddress': '0.0.0.0'
         },
-        'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
-        'status': 'complete'
-    }
-
-Please note that the ``collect`` method should be used sparingly: in the
-`BankID Integration Guide <https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide>`_
-it is specified that *"collect should be called every two seconds and must not be
-called more frequent than once per second"*.
-
-Asynchronous client
-~~~~~~~~~~~~~~~~~~~
-
-The asynchronous client is used in the same way as the asynchronous client, but the
-methods are blocking.
-
-The synchronous guide above can be used as a reference for the asynchronous client
-as well, by simply adding the ``await`` keyword:
-
-.. code-block:: python
-
-    >>> from bankid import BankIDAsyncClient
-    >>> client = BankIDAsyncClient(certificates=(
-        'path/to/certificate.pem',
-        'path/to/key.pem',
-    ))
-    >>> await client.authenticate(end_user_ip='194.168.2.25')
-    {
-        'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
-        'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
-        'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
-        'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
-    }
-
-PyBankID and QR codes
-~~~~~~~~~~~~~~~~~~~~~
-
-PyBankID can generate QR codes for you, and there is an example application in the
-`examples folder of the repo <https://github.com/hbldh/pybankid/tree/master/examples>`_ where a
-Flask application called ``qrdemo`` shows one way to do authentication with animated QR codes.
-
-Certificates
-------------
-
-Production certificates
-~~~~~~~~~~~~~~~~~~~~~~~
-
-If you want to use BankID in a production environment, then you will have to
-purchase this service from one of the
-`selling banks <https://www.bankid.com/foretag/anslut-foeretag>`_.
-They will then provide you with a certificate that can be used to authenticate
-your company/application with the BankID servers.
-
-This certificate has to be processed somewhat to be able to use with PyBankID,
-and how to do this depends on what the selling bank provides you with.
-
-Test certificate
-~~~~~~~~~~~~~~~~
-
-The certificate to use when developing against the BankID test servers can
-be obtained through PyBankID:
-
-.. code-block:: python
-
-    >>> import os
-    >>> import bankid
-    >>> dir_to_save_cert_and_key_in = os.path.expanduser('~')
-    >>> cert_and_key = bankid.create_bankid_test_server_cert_and_key(
-        dir_to_save_cert_and_key_in)
-    >>> print(cert_and_key)
-    ['/home/hbldh/certificate.pem', '/home/hbldh/key.pem']
-    >>> client = bankid.BankIDClient(
-        certificates=cert_and_key, test_server=True)
+        'ocspResponse': 'MIIHegoBAKCCB[...]',
+        'signature': 'PD94bWwgdmVyc2lv[...]',
+        'user': {
+            'givenName': 'Namn',
+            'name': 'Namn Namnsson',
+            'personalNumber': 'YYYYMMDDXXXX',
+            'surname': 'Namnsson'
+        }
+    },
+    'orderRef': 'a9b791c3-459f-492b-bf61-23027876140b',
+    'status': 'complete'
+}
+```
+
+
+Please note that the `collect` method should be used sparingly: in the [BankID Integration Guide](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide) it is specified that *"collect should be called every two seconds and must not be called more frequent than once per second"*.
+
+### Asynchronous client
+
+The asynchronous client is used in the same way as the synchronous client, but the methods are blocking.
+
+The synchronous guide above can be used as a reference for the asynchronous client as well, by simply adding the `await` keyword:
+
+```python
+from bankid import BankIDClientAsync
+client = BankIDClientAsync(certificates=(
+    'path/to/certificate.pem', 
+    'path/to/key.pem', 
+))
+
+await client.authenticate(end_user_ip='194.168.2.25')
+{
+    'orderRef': 'ee3421ea-2096-4000-8130-82648efe0927',
+    'autoStartToken': 'e8df5c3c-c67b-4a01-bfe5-fefeab760beb',
+    'qrStartToken': '01f94e28-857f-4d8a-bf8e-6c5a24466658',
+    'qrStartSecret': 'b4214886-3b5b-46ab-bc08-6862fddc0e06'
+}
+```
+
+
+## PyBankID and QR codes
+
+PyBankID can generate QR codes for you, and there is an example application in the [examples folder of the repo](https://github.com/hbldh/pybankid/tree/master/examples) where a Flask application called `qrdemo` shows one way to do authentication with animated QR codes.
+
+## Certificates
+
+### Production certificates
+
+If you want to use BankID in a production environment, then you will have to purchase this service from one of the [selling banks](https://www.bankid.com/foretag/anslut-foeretag). They will then provide you with a certificate that can be used to authenticate your company/application with the BankID servers.
+
+This certificate has to be processed somewhat to be able to use with PyBankID, and how to do this depends on what the selling bank provides you with.
+
+### Test certificate
+
+The certificate to use when developing against the BankID test servers can be obtained through PyBankID:
 
-Testing
--------
+```python
+import os
+import bankid
+dir_to_save_cert_and_key_in = os.path.expanduser('~')
+cert_and_key = bankid.create_bankid_test_server_cert_and_key(
+    dir_to_save_cert_and_key_in)
+print(cert_and_key)
+['/home/hbldh/certificate.pem', '/home/hbldh/key.pem']
+client = bankid.BankIDClient(
+    certificates=cert_and_key, test_server=True)
+```
 
-The PyBankID solution can be tested with `pytest <https://pytest.org/>`_:
+## Testing
 
-.. code-block:: bash
+The PyBankID solution can be tested with [pytest](https://pytest.org/):
 
-    py.test tests/
+```bash
+pytest tests/
+```
```

### Comparing `pybankid-1.0.0/pybankid.egg-info/SOURCES.txt` & `pybankid-1.0.1/pybankid.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 requirements.txt
 setup.cfg
 setup.py
 bankid/__init__.py
 bankid/__version__.py
 bankid/asyncclient.py
 bankid/baseclient.py
 bankid/certutils.py
 bankid/exceptions.py
+bankid/qr.py
 bankid/syncclient.py
 bankid/certs/FPTestcert4_20220818.p12
 bankid/certs/FPTestcert4_20220818_cert.pem
 bankid/certs/FPTestcert4_20220818_key.pem
 bankid/certs/FPTestcert4_20230629.p12
 bankid/certs/FPTestcert4_20230629_cert.pem
 bankid/certs/FPTestcert4_20230629_key.pem
```

### Comparing `pybankid-1.0.0/setup.py` & `pybankid-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 # What packages are required for this module to be executed?
 REQUIRED = open("requirements.txt").read().splitlines()
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.rst' is present in your MANIFEST.in file!
-with io.open(os.path.join(here, "README.rst"), encoding="utf-8") as f:
+with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
 # Load the package's __version__.py module as a dictionary.
 about = {}
 with open(os.path.join(here, "bankid", "__version__.py")) as f:
     exec(f.read(), about)
 
@@ -83,15 +83,15 @@
 
 # Where the magic happens:
 setup(
     name=NAME,
     version=about["__version__"],
     description=DESCRIPTION,
     long_description=long_description,
-    long_description_content_type="text/x-rst",
+    long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     packages=find_packages(exclude=("tests",)),
     install_requires=REQUIRED,
     include_package_data=True,
     package_data={"": ["*.pem", "*.p12"]},
```

### Comparing `pybankid-1.0.0/tests/conftest.py` & `pybankid-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/tests/test_asyncclient.py` & `pybankid-1.0.1/tests/test_asyncclient.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/tests/test_exceptions.py` & `pybankid-1.0.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.0.0/tests/test_syncclient.py` & `pybankid-1.0.1/tests/test_syncclient.py`

 * *Files identical despite different names*

