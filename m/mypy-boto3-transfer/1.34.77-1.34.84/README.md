# Comparing `tmp/mypy-boto3-transfer-1.34.77.tar.gz` & `tmp/mypy_boto3_transfer-1.34.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-transfer-1.34.77.tar", last modified: Wed Apr  3 19:32:40 2024, max compression
+gzip compressed data, was "mypy_boto3_transfer-1.34.84.tar", last modified: Fri Apr 12 19:32:38 2024, max compression
```

## Comparing `mypy-boto3-transfer-1.34.77.tar` & `mypy_boto3_transfer-1.34.84.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.880159 mypy-boto3-transfer-1.34.77/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-04-03 19:32:40.880159 mypy-boto3-transfer-1.34.77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.880159 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47413 2024-04-03 19:32:26.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    47410 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-04-03 19:32:26.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-04-03 19:32:26.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-03 19:32:26.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-04-03 19:32:26.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    51669 2024-04-03 19:32:27.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    51669 2024-04-03 19:32:27.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-03 19:32:26.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-03 19:32:26.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.880159 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-04-03 19:32:40.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-03 19:32:40.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:40.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:40.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 19:32:40.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 19:32:40.000000 mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:32:40.880159 mypy-boto3-transfer-1.34.77/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-03 19:32:25.000000 mypy-boto3-transfer-1.34.77/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:38.645303 mypy_boto3_transfer-1.34.84/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-04-12 19:32:38.645303 mypy_boto3_transfer-1.34.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:38.645303 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47413 2024-04-12 19:32:22.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47410 2024-04-12 19:32:22.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13303 2024-04-12 19:32:23.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13303 2024-04-12 19:32:23.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-12 19:32:22.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-04-12 19:32:22.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    51669 2024-04-12 19:32:24.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51669 2024-04-12 19:32:23.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-12 19:32:22.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-12 19:32:22.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:38.645303 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-04-12 19:32:38.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-12 19:32:38.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:38.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:38.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 19:32:38.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 19:32:38.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:32:38.645303 mypy_boto3_transfer-1.34.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/setup.py
```

### Comparing `mypy-boto3-transfer-1.34.77/LICENSE` & `mypy_boto3_transfer-1.34.84/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.77/PKG-INFO` & `mypy_boto3_transfer-1.34.84/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.34.77
-Summary: Type annotations for boto3.Transfer 1.34.77 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.84
+Summary: Type annotations for boto3.Transfer 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-transfer-1.34.77/README.md` & `mypy_boto3_transfer-1.34.84/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/__init__.py` & `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/__init__.pyi` & `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/__main__.py` & `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Transfer 1.34.77\n"
-        "Version:         1.34.77\n"
+        "Type annotations for boto3.Transfer 1.34.84\n"
+        "Version:         1.34.84\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.77")
+    print("1.34.84")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/client.py` & `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/client.pyi` & `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/literals.py` & `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     "RegionName",
 )
 
 AgreementStatusTypeType = Literal["ACTIVE", "INACTIVE"]
 As2TransportType = Literal["HTTP"]
 CertificateStatusTypeType = Literal["ACTIVE", "INACTIVE", "PENDING_ROTATION"]
 CertificateTypeType = Literal["CERTIFICATE", "CERTIFICATE_WITH_PRIVATE_KEY"]
-CertificateUsageTypeType = Literal["ENCRYPTION", "SIGNING"]
+CertificateUsageTypeType = Literal["ENCRYPTION", "SIGNING", "TLS"]
 CompressionEnumType = Literal["DISABLED", "ZLIB"]
 CustomStepStatusType = Literal["FAILURE", "SUCCESS"]
 DirectoryListingOptimizationType = Literal["DISABLED", "ENABLED"]
 DomainType = Literal["EFS", "S3"]
 EncryptionAlgType = Literal["AES128_CBC", "AES192_CBC", "AES256_CBC", "DES_EDE3_CBC", "NONE"]
 EncryptionTypeType = Literal["PGP"]
 EndpointTypeType = Literal["PUBLIC", "VPC", "VPC_ENDPOINT"]
@@ -216,14 +216,15 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
```

### Comparing `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/literals.pyi` & `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     "RegionName",
 )
 
 AgreementStatusTypeType = Literal["ACTIVE", "INACTIVE"]
 As2TransportType = Literal["HTTP"]
 CertificateStatusTypeType = Literal["ACTIVE", "INACTIVE", "PENDING_ROTATION"]
 CertificateTypeType = Literal["CERTIFICATE", "CERTIFICATE_WITH_PRIVATE_KEY"]
-CertificateUsageTypeType = Literal["ENCRYPTION", "SIGNING"]
+CertificateUsageTypeType = Literal["ENCRYPTION", "SIGNING", "TLS"]
 CompressionEnumType = Literal["DISABLED", "ZLIB"]
 CustomStepStatusType = Literal["FAILURE", "SUCCESS"]
 DirectoryListingOptimizationType = Literal["DISABLED", "ENABLED"]
 DomainType = Literal["EFS", "S3"]
 EncryptionAlgType = Literal["AES128_CBC", "AES192_CBC", "AES256_CBC", "DES_EDE3_CBC", "NONE"]
 EncryptionTypeType = Literal["PGP"]
 EndpointTypeType = Literal["PUBLIC", "VPC", "VPC_ENDPOINT"]
@@ -216,14 +216,15 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
```

### Comparing `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/paginator.py` & `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/paginator.pyi` & `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/type_defs.py` & `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/type_defs.pyi` & `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/waiter.py` & `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer/waiter.pyi` & `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/PKG-INFO` & `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.34.77
-Summary: Type annotations for boto3.Transfer 1.34.77 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.84
+Summary: Type annotations for boto3.Transfer 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-transfer-1.34.77/mypy_boto3_transfer.egg-info/SOURCES.txt` & `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.34.77/setup.py` & `mypy_boto3_transfer-1.34.84/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-transfer",
-    version="1.34.77",
+    version="1.34.84",
     packages=["mypy_boto3_transfer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Transfer 1.34.77 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.Transfer 1.34.84 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

