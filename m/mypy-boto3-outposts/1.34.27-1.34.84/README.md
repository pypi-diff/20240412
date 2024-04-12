# Comparing `tmp/mypy-boto3-outposts-1.34.27.tar.gz` & `tmp/mypy_boto3_outposts-1.34.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-outposts-1.34.27.tar", last modified: Wed Jan 24 20:33:19 2024, max compression
+gzip compressed data, was "mypy_boto3_outposts-1.34.84.tar", last modified: Fri Apr 12 19:32:37 2024, max compression
```

## Comparing `mypy-boto3-outposts-1.34.27.tar` & `mypy_boto3_outposts-1.34.84.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:19.206200 mypy-boto3-outposts-1.34.27/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-24 20:32:52.000000 mypy-boto3-outposts-1.34.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-01-24 20:33:19.206200 mypy-boto3-outposts-1.34.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-01-24 20:32:52.000000 mypy-boto3-outposts-1.34.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:19.206200 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-01-24 20:32:52.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-01-24 20:32:52.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-01-24 20:32:52.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-01-24 20:32:52.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21429 2024-01-24 20:32:52.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-01-24 20:32:52.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-01-24 20:32:52.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-01-24 20:32:52.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-01-24 20:32:52.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 20:32:52.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    22915 2024-01-24 20:32:52.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22915 2024-01-24 20:32:52.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-24 20:32:52.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:19.206200 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-01-24 20:33:19.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-24 20:33:19.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 20:33:19.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 20:33:19.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-24 20:33:19.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-24 20:33:19.000000 mypy-boto3-outposts-1.34.27/mypy_boto3_outposts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-24 20:33:19.206200 mypy-boto3-outposts-1.34.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-01-24 20:32:51.000000 mypy-boto3-outposts-1.34.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:37.957303 mypy_boto3_outposts-1.34.84/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-04-12 19:32:37.957303 mypy_boto3_outposts-1.34.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:37.957303 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21432 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21429 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    22928 2024-04-12 19:32:14.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22928 2024-04-12 19:32:14.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:37.957303 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-04-12 19:32:37.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-12 19:32:37.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:37.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:37.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 19:32:37.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 19:32:37.000000 mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:32:37.957303 mypy_boto3_outposts-1.34.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-12 19:32:13.000000 mypy_boto3_outposts-1.34.84/setup.py
```

### Comparing `mypy-boto3-outposts-1.34.27/LICENSE` & `mypy_boto3_outposts-1.34.84/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.34.27/PKG-INFO` & `mypy_boto3_outposts-1.34.84/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-outposts
-Version: 1.34.27
-Summary: Type annotations for boto3.Outposts 1.34.27 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.84
+Summary: Type annotations for boto3.Outposts 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-outposts)](https://pepy.tech/project/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.34.27](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
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
 [mypy-boto3-outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-outposts-1.34.27/README.md` & `mypy_boto3_outposts-1.34.84/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-outposts)](https://pepy.tech/project/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.34.27](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
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
 [mypy-boto3-outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/__init__.py` & `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/__init__.pyi` & `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/__main__.py` & `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Outposts 1.34.27\nVersion:         1.34.27\nBuilder version:"
-        " 7.23.1\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.Outposts 1.34.84\n"
+        "Version:         1.34.84\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.27")
+    print("1.34.84")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/client.py` & `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/client.pyi` & `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/literals.py` & `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 OrderTypeType = Literal["OUTPOST", "REPLACEMENT"]
 PaymentOptionType = Literal["ALL_UPFRONT", "NO_UPFRONT", "PARTIAL_UPFRONT"]
 PaymentTermType = Literal["ONE_YEAR", "THREE_YEARS"]
 PowerConnectorType = Literal["AH530P7W", "AH532P6W", "IEC309", "L6_30P"]
 PowerDrawKvaType = Literal["POWER_10_KVA", "POWER_15_KVA", "POWER_30_KVA", "POWER_5_KVA"]
 PowerFeedDropType = Literal["ABOVE_RACK", "BELOW_RACK"]
 PowerPhaseType = Literal["SINGLE_PHASE", "THREE_PHASE"]
-ShipmentCarrierType = Literal["DBS", "DHL", "FEDEX", "UPS"]
+ShipmentCarrierType = Literal["DBS", "DHL", "EXPEDITORS", "FEDEX", "UPS"]
 SupportedHardwareTypeType = Literal["RACK", "SERVER"]
 SupportedStorageEnumType = Literal["EBS", "S3"]
 UplinkCountType = Literal[
     "UPLINK_COUNT_1",
     "UPLINK_COUNT_12",
     "UPLINK_COUNT_16",
     "UPLINK_COUNT_2",
@@ -156,14 +156,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -174,14 +175,15 @@
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
@@ -199,14 +201,15 @@
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
@@ -219,24 +222,26 @@
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
@@ -297,15 +302,14 @@
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
@@ -485,14 +489,15 @@
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

### Comparing `mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/literals.pyi` & `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 OrderTypeType = Literal["OUTPOST", "REPLACEMENT"]
 PaymentOptionType = Literal["ALL_UPFRONT", "NO_UPFRONT", "PARTIAL_UPFRONT"]
 PaymentTermType = Literal["ONE_YEAR", "THREE_YEARS"]
 PowerConnectorType = Literal["AH530P7W", "AH532P6W", "IEC309", "L6_30P"]
 PowerDrawKvaType = Literal["POWER_10_KVA", "POWER_15_KVA", "POWER_30_KVA", "POWER_5_KVA"]
 PowerFeedDropType = Literal["ABOVE_RACK", "BELOW_RACK"]
 PowerPhaseType = Literal["SINGLE_PHASE", "THREE_PHASE"]
-ShipmentCarrierType = Literal["DBS", "DHL", "FEDEX", "UPS"]
+ShipmentCarrierType = Literal["DBS", "DHL", "EXPEDITORS", "FEDEX", "UPS"]
 SupportedHardwareTypeType = Literal["RACK", "SERVER"]
 SupportedStorageEnumType = Literal["EBS", "S3"]
 UplinkCountType = Literal[
     "UPLINK_COUNT_1",
     "UPLINK_COUNT_12",
     "UPLINK_COUNT_16",
     "UPLINK_COUNT_2",
@@ -156,14 +156,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -174,14 +175,15 @@
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
@@ -199,14 +201,15 @@
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
@@ -219,24 +222,26 @@
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
@@ -297,15 +302,14 @@
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
@@ -485,14 +489,15 @@
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

### Comparing `mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/paginator.py` & `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/paginator.pyi` & `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/type_defs.py` & `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,18 +191,18 @@
         "Quantity": NotRequired[int],
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
 CreateOutpostInputRequestTypeDef = TypedDict(
     "CreateOutpostInputRequestTypeDef",
     {
         "Name": str,
         "SiteId": str,
```

### Comparing `mypy-boto3-outposts-1.34.27/mypy_boto3_outposts/type_defs.pyi` & `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -191,18 +191,18 @@
         "Quantity": NotRequired[int],
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
 CreateOutpostInputRequestTypeDef = TypedDict(
     "CreateOutpostInputRequestTypeDef",
     {
         "Name": str,
         "SiteId": str,
```

### Comparing `mypy-boto3-outposts-1.34.27/mypy_boto3_outposts.egg-info/PKG-INFO` & `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-outposts
-Version: 1.34.27
-Summary: Type annotations for boto3.Outposts 1.34.27 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.84
+Summary: Type annotations for boto3.Outposts 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-outposts)](https://pepy.tech/project/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.34.27](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
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
 [mypy-boto3-outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-outposts-1.34.27/mypy_boto3_outposts.egg-info/SOURCES.txt` & `mypy_boto3_outposts-1.34.84/mypy_boto3_outposts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.34.27/setup.py` & `mypy_boto3_outposts-1.34.84/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-outposts",
-    version="1.34.27",
+    version="1.34.84",
     packages=["mypy_boto3_outposts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.Outposts 1.34.27 service generated with mypy-boto3-builder"
-        " 7.23.1"
-    ),
+    description="Type annotations for boto3.Outposts 1.34.84 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

