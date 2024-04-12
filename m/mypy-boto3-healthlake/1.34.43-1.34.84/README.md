# Comparing `tmp/mypy-boto3-healthlake-1.34.43.tar.gz` & `tmp/mypy_boto3_healthlake-1.34.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-healthlake-1.34.43.tar", last modified: Thu Feb 15 20:47:29 2024, max compression
+gzip compressed data, was "mypy_boto3_healthlake-1.34.84.tar", last modified: Fri Apr 12 19:32:36 2024, max compression
```

## Comparing `mypy-boto3-healthlake-1.34.43.tar` & `mypy_boto3_healthlake-1.34.84.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 20:47:29.445507 mypy-boto3-healthlake-1.34.43/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-15 20:46:53.000000 mypy-boto3-healthlake-1.34.43/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12259 2024-02-15 20:47:29.445507 mypy-boto3-healthlake-1.34.43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-02-15 20:46:53.000000 mypy-boto3-healthlake-1.34.43/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 20:47:29.441506 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-15 20:46:53.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-15 20:46:53.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-15 20:46:53.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-02-15 20:46:53.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-02-15 20:46:53.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-02-15 20:46:53.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-02-15 20:46:53.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 20:46:53.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12418 2024-02-15 20:46:54.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12418 2024-02-15 20:46:54.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-15 20:46:53.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 20:47:29.445507 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12259 2024-02-15 20:47:29.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-15 20:47:29.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 20:47:29.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 20:47:29.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-15 20:47:29.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-15 20:47:29.000000 mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 20:47:29.445507 mypy-boto3-healthlake-1.34.43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-02-15 20:46:53.000000 mypy-boto3-healthlake-1.34.43/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:36.317305 mypy_boto3_healthlake-1.34.84/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 19:32:06.000000 mypy_boto3_healthlake-1.34.84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12259 2024-04-12 19:32:36.317305 mypy_boto3_healthlake-1.34.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-12 19:32:06.000000 mypy_boto3_healthlake-1.34.84/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:36.313305 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 19:32:06.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 19:32:06.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-12 19:32:06.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-04-12 19:32:06.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-04-12 19:32:06.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-04-12 19:32:06.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-04-12 19:32:06.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:06.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-04-12 19:32:06.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-04-12 19:32:06.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 19:32:06.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:36.317305 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12259 2024-04-12 19:32:36.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-12 19:32:36.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:36.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:36.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 19:32:36.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 19:32:36.000000 mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:32:36.317305 mypy_boto3_healthlake-1.34.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-12 19:32:06.000000 mypy_boto3_healthlake-1.34.84/setup.py
```

### Comparing `mypy-boto3-healthlake-1.34.43/LICENSE` & `mypy_boto3_healthlake-1.34.84/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.34.43/PKG-INFO` & `mypy_boto3_healthlake-1.34.84/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-healthlake
-Version: 1.34.43
-Summary: Type annotations for boto3.HealthLake 1.34.43 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.84
+Summary: Type annotations for boto3.HealthLake 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-healthlake)](https://pepy.tech/project/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.34.43](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-healthlake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-healthlake-1.34.43/README.md` & `mypy_boto3_healthlake-1.34.84/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-healthlake)](https://pepy.tech/project/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.34.43](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-healthlake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/__main__.py` & `mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.HealthLake 1.34.43\n"
-        "Version:         1.34.43\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.HealthLake 1.34.84\n"
+        "Version:         1.34.84\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.43")
+    print("1.34.84")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/client.py` & `mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/client.pyi` & `mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/literals.py` & `mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,26 +19,28 @@
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AuthorizationStrategyType",
     "CmkTypeType",
     "DatastoreStatusType",
+    "ErrorCategoryType",
     "FHIRVersionType",
     "JobStatusType",
     "PreloadDataTypeType",
     "HealthLakeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 AuthorizationStrategyType = Literal["AWS_AUTH", "SMART_ON_FHIR_V1"]
 CmkTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KMS_KEY"]
-DatastoreStatusType = Literal["ACTIVE", "CREATING", "DELETED", "DELETING"]
+DatastoreStatusType = Literal["ACTIVE", "CREATE_FAILED", "CREATING", "DELETED", "DELETING"]
+ErrorCategoryType = Literal["NON_RETRYABLE_ERROR", "RETRYABLE_ERROR"]
 FHIRVersionType = Literal["R4"]
 JobStatusType = Literal[
     "CANCEL_COMPLETED",
     "CANCEL_FAILED",
     "CANCEL_IN_PROGRESS",
     "CANCEL_SUBMITTED",
     "COMPLETED",
@@ -90,14 +92,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -115,14 +118,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -135,24 +139,26 @@
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
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -213,15 +219,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -401,14 +406,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/literals.pyi` & `mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -19,26 +19,28 @@
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AuthorizationStrategyType",
     "CmkTypeType",
     "DatastoreStatusType",
+    "ErrorCategoryType",
     "FHIRVersionType",
     "JobStatusType",
     "PreloadDataTypeType",
     "HealthLakeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 AuthorizationStrategyType = Literal["AWS_AUTH", "SMART_ON_FHIR_V1"]
 CmkTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KMS_KEY"]
-DatastoreStatusType = Literal["ACTIVE", "CREATING", "DELETED", "DELETING"]
+DatastoreStatusType = Literal["ACTIVE", "CREATE_FAILED", "CREATING", "DELETED", "DELETING"]
+ErrorCategoryType = Literal["NON_RETRYABLE_ERROR", "RETRYABLE_ERROR"]
 FHIRVersionType = Literal["R4"]
 JobStatusType = Literal[
     "CANCEL_COMPLETED",
     "CANCEL_FAILED",
     "CANCEL_IN_PROGRESS",
     "CANCEL_SUBMITTED",
     "COMPLETED",
@@ -90,14 +92,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -115,14 +118,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -135,24 +139,26 @@
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
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -213,15 +219,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -401,14 +406,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/type_defs.py` & `mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,21 @@
     ```
 """
 
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
-from .literals import AuthorizationStrategyType, CmkTypeType, DatastoreStatusType, JobStatusType
+from .literals import (
+    AuthorizationStrategyType,
+    CmkTypeType,
+    DatastoreStatusType,
+    ErrorCategoryType,
+    JobStatusType,
+)
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
     from typing import NotRequired
@@ -33,14 +39,15 @@
 
 __all__ = (
     "IdentityProviderConfigurationTypeDef",
     "PreloadDataConfigTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "TimestampTypeDef",
+    "ErrorCauseTypeDef",
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRExportJobRequestRequestTypeDef",
     "DescribeFHIRImportJobRequestRequestTypeDef",
     "InputDataConfigTypeDef",
     "JobProgressReportTypeDef",
     "KmsEncryptionConfigTypeDef",
@@ -95,21 +102,28 @@
         "Value": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 TimestampTypeDef = Union[datetime, str]
+ErrorCauseTypeDef = TypedDict(
+    "ErrorCauseTypeDef",
+    {
+        "ErrorMessage": NotRequired[str],
+        "ErrorCategory": NotRequired[ErrorCategoryType],
+    },
+)
 DeleteFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 DescribeFHIRDatastoreRequestRequestTypeDef = TypedDict(
@@ -304,14 +318,15 @@
         "DatastoreTypeVersion": Literal["R4"],
         "DatastoreEndpoint": str,
         "DatastoreName": NotRequired[str],
         "CreatedAt": NotRequired[datetime],
         "SseConfiguration": NotRequired[SseConfigurationTypeDef],
         "PreloadDataConfig": NotRequired[PreloadDataConfigTypeDef],
         "IdentityProviderConfiguration": NotRequired[IdentityProviderConfigurationTypeDef],
+        "ErrorCause": NotRequired[ErrorCauseTypeDef],
     },
 )
 ExportJobPropertiesTypeDef = TypedDict(
     "ExportJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
```

### Comparing `mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake/type_defs.pyi` & `mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,21 @@
     ```
 """
 
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
-from .literals import AuthorizationStrategyType, CmkTypeType, DatastoreStatusType, JobStatusType
+from .literals import (
+    AuthorizationStrategyType,
+    CmkTypeType,
+    DatastoreStatusType,
+    ErrorCategoryType,
+    JobStatusType,
+)
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
     from typing import NotRequired
@@ -33,14 +39,15 @@
 
 __all__ = (
     "IdentityProviderConfigurationTypeDef",
     "PreloadDataConfigTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "TimestampTypeDef",
+    "ErrorCauseTypeDef",
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRExportJobRequestRequestTypeDef",
     "DescribeFHIRImportJobRequestRequestTypeDef",
     "InputDataConfigTypeDef",
     "JobProgressReportTypeDef",
     "KmsEncryptionConfigTypeDef",
@@ -95,21 +102,28 @@
         "Value": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 TimestampTypeDef = Union[datetime, str]
+ErrorCauseTypeDef = TypedDict(
+    "ErrorCauseTypeDef",
+    {
+        "ErrorMessage": NotRequired[str],
+        "ErrorCategory": NotRequired[ErrorCategoryType],
+    },
+)
 DeleteFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 DescribeFHIRDatastoreRequestRequestTypeDef = TypedDict(
@@ -304,14 +318,15 @@
         "DatastoreTypeVersion": Literal["R4"],
         "DatastoreEndpoint": str,
         "DatastoreName": NotRequired[str],
         "CreatedAt": NotRequired[datetime],
         "SseConfiguration": NotRequired[SseConfigurationTypeDef],
         "PreloadDataConfig": NotRequired[PreloadDataConfigTypeDef],
         "IdentityProviderConfiguration": NotRequired[IdentityProviderConfigurationTypeDef],
+        "ErrorCause": NotRequired[ErrorCauseTypeDef],
     },
 )
 ExportJobPropertiesTypeDef = TypedDict(
     "ExportJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
```

### Comparing `mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake.egg-info/PKG-INFO` & `mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-healthlake
-Version: 1.34.43
-Summary: Type annotations for boto3.HealthLake 1.34.43 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.84
+Summary: Type annotations for boto3.HealthLake 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-healthlake)](https://pepy.tech/project/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.34.43](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-healthlake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-healthlake-1.34.43/mypy_boto3_healthlake.egg-info/SOURCES.txt` & `mypy_boto3_healthlake-1.34.84/mypy_boto3_healthlake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.34.43/setup.py` & `mypy_boto3_healthlake-1.34.84/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-healthlake",
-    version="1.34.43",
+    version="1.34.84",
     packages=["mypy_boto3_healthlake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.HealthLake 1.34.43 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.HealthLake 1.34.84 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

