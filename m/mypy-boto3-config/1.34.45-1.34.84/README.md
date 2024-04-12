# Comparing `tmp/mypy-boto3-config-1.34.45.tar.gz` & `tmp/mypy_boto3_config-1.34.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-config-1.34.45.tar", last modified: Mon Feb 19 20:21:45 2024, max compression
+gzip compressed data, was "mypy_boto3_config-1.34.84.tar", last modified: Fri Apr 12 19:32:35 2024, max compression
```

## Comparing `mypy-boto3-config-1.34.45.tar` & `mypy_boto3_config-1.34.84.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:21:45.674640 mypy-boto3-config-1.34.45/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-19 20:21:27.000000 mypy-boto3-config-1.34.45/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19081 2024-02-19 20:21:45.674640 mypy-boto3-config-1.34.45/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17523 2024-02-19 20:21:27.000000 mypy-boto3-config-1.34.45/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:21:45.670640 mypy-boto3-config-1.34.45/mypy_boto3_config/
--rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-02-19 20:21:27.000000 mypy-boto3-config-1.34.45/mypy_boto3_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-02-19 20:21:27.000000 mypy-boto3-config-1.34.45/mypy_boto3_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-02-19 20:21:27.000000 mypy-boto3-config-1.34.45/mypy_boto3_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89193 2024-02-19 20:21:28.000000 mypy-boto3-config-1.34.45/mypy_boto3_config/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    89190 2024-02-19 20:21:28.000000 mypy-boto3-config-1.34.45/mypy_boto3_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    34059 2024-02-19 20:21:28.000000 mypy-boto3-config-1.34.45/mypy_boto3_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    34059 2024-02-19 20:21:28.000000 mypy-boto3-config-1.34.45/mypy_boto3_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    42910 2024-02-19 20:21:28.000000 mypy-boto3-config-1.34.45/mypy_boto3_config/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    42878 2024-02-19 20:21:28.000000 mypy-boto3-config-1.34.45/mypy_boto3_config/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 20:21:27.000000 mypy-boto3-config-1.34.45/mypy_boto3_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   104866 2024-02-19 20:21:30.000000 mypy-boto3-config-1.34.45/mypy_boto3_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   104866 2024-02-19 20:21:30.000000 mypy-boto3-config-1.34.45/mypy_boto3_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-19 20:21:27.000000 mypy-boto3-config-1.34.45/mypy_boto3_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:21:45.674640 mypy-boto3-config-1.34.45/mypy_boto3_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19081 2024-02-19 20:21:45.000000 mypy-boto3-config-1.34.45/mypy_boto3_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-19 20:21:45.000000 mypy-boto3-config-1.34.45/mypy_boto3_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 20:21:45.000000 mypy-boto3-config-1.34.45/mypy_boto3_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 20:21:45.000000 mypy-boto3-config-1.34.45/mypy_boto3_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-19 20:21:45.000000 mypy-boto3-config-1.34.45/mypy_boto3_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-19 20:21:45.000000 mypy-boto3-config-1.34.45/mypy_boto3_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 20:21:45.674640 mypy-boto3-config-1.34.45/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-02-19 20:21:27.000000 mypy-boto3-config-1.34.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:35.573306 mypy_boto3_config-1.34.84/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 19:31:51.000000 mypy_boto3_config-1.34.84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19081 2024-04-12 19:32:35.573306 mypy_boto3_config-1.34.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17523 2024-04-12 19:31:51.000000 mypy_boto3_config-1.34.84/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:35.573306 mypy_boto3_config-1.34.84/mypy_boto3_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-04-12 19:31:51.000000 mypy_boto3_config-1.34.84/mypy_boto3_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-04-12 19:31:51.000000 mypy_boto3_config-1.34.84/mypy_boto3_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-12 19:31:51.000000 mypy_boto3_config-1.34.84/mypy_boto3_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89193 2024-04-12 19:31:52.000000 mypy_boto3_config-1.34.84/mypy_boto3_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89190 2024-04-12 19:31:52.000000 mypy_boto3_config-1.34.84/mypy_boto3_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    34125 2024-04-12 19:31:53.000000 mypy_boto3_config-1.34.84/mypy_boto3_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34125 2024-04-12 19:31:53.000000 mypy_boto3_config-1.34.84/mypy_boto3_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    42910 2024-04-12 19:31:53.000000 mypy_boto3_config-1.34.84/mypy_boto3_config/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42878 2024-04-12 19:31:53.000000 mypy_boto3_config-1.34.84/mypy_boto3_config/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:31:51.000000 mypy_boto3_config-1.34.84/mypy_boto3_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   104879 2024-04-12 19:31:54.000000 mypy_boto3_config-1.34.84/mypy_boto3_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104879 2024-04-12 19:31:54.000000 mypy_boto3_config-1.34.84/mypy_boto3_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 19:31:51.000000 mypy_boto3_config-1.34.84/mypy_boto3_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:35.573306 mypy_boto3_config-1.34.84/mypy_boto3_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19081 2024-04-12 19:32:35.000000 mypy_boto3_config-1.34.84/mypy_boto3_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-12 19:32:35.000000 mypy_boto3_config-1.34.84/mypy_boto3_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:35.000000 mypy_boto3_config-1.34.84/mypy_boto3_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:35.000000 mypy_boto3_config-1.34.84/mypy_boto3_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 19:32:35.000000 mypy_boto3_config-1.34.84/mypy_boto3_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 19:32:35.000000 mypy_boto3_config-1.34.84/mypy_boto3_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:32:35.573306 mypy_boto3_config-1.34.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-12 19:31:51.000000 mypy_boto3_config-1.34.84/setup.py
```

### Comparing `mypy-boto3-config-1.34.45/LICENSE` & `mypy_boto3_config-1.34.84/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.34.45/PKG-INFO` & `mypy_boto3_config-1.34.84/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-config
-Version: 1.34.45
-Summary: Type annotations for boto3.ConfigService 1.34.45 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.84
+Summary: Type annotations for boto3.ConfigService 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-config)](https://pepy.tech/project/mypy-boto3-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConfigService 1.34.45](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[boto3.ConfigService 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-config-1.34.45/README.md` & `mypy_boto3_config-1.34.84/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-config)](https://pepy.tech/project/mypy-boto3-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConfigService 1.34.45](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[boto3.ConfigService 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-config-1.34.45/mypy_boto3_config/__init__.py` & `mypy_boto3_config-1.34.84/mypy_boto3_config/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.34.45/mypy_boto3_config/__init__.pyi` & `mypy_boto3_config-1.34.84/mypy_boto3_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.34.45/mypy_boto3_config/__main__.py` & `mypy_boto3_config-1.34.84/mypy_boto3_config/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConfigService 1.34.45\n"
-        "Version:         1.34.45\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.ConfigService 1.34.84\n"
+        "Version:         1.34.84\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.45")
+    print("1.34.84")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-config-1.34.45/mypy_boto3_config/client.py` & `mypy_boto3_config-1.34.84/mypy_boto3_config/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.34.45/mypy_boto3_config/client.pyi` & `mypy_boto3_config-1.34.84/mypy_boto3_config/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.34.45/mypy_boto3_config/literals.py` & `mypy_boto3_config-1.34.84/mypy_boto3_config/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -718,14 +718,15 @@
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
@@ -738,24 +739,26 @@
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
@@ -816,15 +819,14 @@
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
@@ -1004,14 +1006,15 @@
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

### Comparing `mypy-boto3-config-1.34.45/mypy_boto3_config/literals.pyi` & `mypy_boto3_config-1.34.84/mypy_boto3_config/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -718,14 +718,15 @@
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
@@ -738,24 +739,26 @@
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
@@ -816,15 +819,14 @@
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
@@ -1004,14 +1006,15 @@
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

### Comparing `mypy-boto3-config-1.34.45/mypy_boto3_config/paginator.py` & `mypy_boto3_config-1.34.84/mypy_boto3_config/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.34.45/mypy_boto3_config/paginator.pyi` & `mypy_boto3_config-1.34.84/mypy_boto3_config/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.34.45/mypy_boto3_config/type_defs.py` & `mypy_boto3_config-1.34.84/mypy_boto3_config/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,18 +457,18 @@
         "configurationItemDeliveryTime": NotRequired[datetime],
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
 ResourceKeyTypeDef = TypedDict(
     "ResourceKeyTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
```

### Comparing `mypy-boto3-config-1.34.45/mypy_boto3_config/type_defs.pyi` & `mypy_boto3_config-1.34.84/mypy_boto3_config/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -457,18 +457,18 @@
         "configurationItemDeliveryTime": NotRequired[datetime],
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
 ResourceKeyTypeDef = TypedDict(
     "ResourceKeyTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
```

### Comparing `mypy-boto3-config-1.34.45/mypy_boto3_config.egg-info/PKG-INFO` & `mypy_boto3_config-1.34.84/mypy_boto3_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-config
-Version: 1.34.45
-Summary: Type annotations for boto3.ConfigService 1.34.45 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.84
+Summary: Type annotations for boto3.ConfigService 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-config)](https://pepy.tech/project/mypy-boto3-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConfigService 1.34.45](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[boto3.ConfigService 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-config-1.34.45/mypy_boto3_config.egg-info/SOURCES.txt` & `mypy_boto3_config-1.34.84/mypy_boto3_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.34.45/setup.py` & `mypy_boto3_config-1.34.84/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-config",
-    version="1.34.45",
+    version="1.34.84",
     packages=["mypy_boto3_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.ConfigService 1.34.45 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.ConfigService 1.34.84 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

