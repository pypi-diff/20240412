# Comparing `tmp/mypy-boto3-redshift-1.34.57.tar.gz` & `tmp/mypy_boto3_redshift-1.34.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-redshift-1.34.57.tar", last modified: Wed Mar  6 21:33:28 2024, max compression
+gzip compressed data, was "mypy_boto3_redshift-1.34.84.tar", last modified: Fri Apr 12 19:32:38 2024, max compression
```

## Comparing `mypy-boto3-redshift-1.34.57.tar` & `mypy_boto3_redshift-1.34.84.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:28.316246 mypy-boto3-redshift-1.34.57/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-06 21:33:11.000000 mypy-boto3-redshift-1.34.57/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20088 2024-03-06 21:33:28.316246 mypy-boto3-redshift-1.34.57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18529 2024-03-06 21:33:11.000000 mypy-boto3-redshift-1.34.57/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:28.312246 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/
--rw-r--r--   0 runner    (1001) docker     (127)    10719 2024-03-06 21:33:11.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10719 2024-03-06 21:33:11.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-06 21:33:11.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   124644 2024-03-06 21:33:13.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   124641 2024-03-06 21:33:11.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18870 2024-03-06 21:33:13.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    18870 2024-03-06 21:33:13.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    47245 2024-03-06 21:33:13.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    47208 2024-03-06 21:33:13.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:11.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   134416 2024-03-06 21:33:16.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   134416 2024-03-06 21:33:14.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-06 21:33:11.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-03-06 21:33:13.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-03-06 21:33:13.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:28.316246 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20088 2024-03-06 21:33:28.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-06 21:33:28.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 21:33:28.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 21:33:28.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-06 21:33:28.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-06 21:33:28.000000 mypy-boto3-redshift-1.34.57/mypy_boto3_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 21:33:28.316246 mypy-boto3-redshift-1.34.57/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-06 21:33:11.000000 mypy-boto3-redshift-1.34.57/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:38.285303 mypy_boto3_redshift-1.34.84/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 19:32:16.000000 mypy_boto3_redshift-1.34.84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20088 2024-04-12 19:32:38.285303 mypy_boto3_redshift-1.34.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18529 2024-04-12 19:32:16.000000 mypy_boto3_redshift-1.34.84/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:38.281303 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)    10719 2024-04-12 19:32:16.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10719 2024-04-12 19:32:16.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-12 19:32:16.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124644 2024-04-12 19:32:17.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124641 2024-04-12 19:32:17.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18936 2024-04-12 19:32:18.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18936 2024-04-12 19:32:18.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    47245 2024-04-12 19:32:18.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47208 2024-04-12 19:32:18.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:16.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   134457 2024-04-12 19:32:21.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   134457 2024-04-12 19:32:20.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 19:32:16.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-12 19:32:18.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-12 19:32:18.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:38.285303 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20088 2024-04-12 19:32:38.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-12 19:32:38.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:38.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:38.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 19:32:38.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 19:32:38.000000 mypy_boto3_redshift-1.34.84/mypy_boto3_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:32:38.285303 mypy_boto3_redshift-1.34.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-12 19:32:16.000000 mypy_boto3_redshift-1.34.84/setup.py
```

### Comparing `mypy-boto3-redshift-1.34.57/LICENSE` & `mypy_boto3_redshift-1.34.84/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.34.57/PKG-INFO` & `mypy_boto3_redshift-1.34.84/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift
-Version: 1.34.57
-Summary: Type annotations for boto3.Redshift 1.34.57 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.84
+Summary: Type annotations for boto3.Redshift 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift)](https://pepy.tech/project/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.34.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-redshift-1.34.57/README.md` & `mypy_boto3_redshift-1.34.84/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift)](https://pepy.tech/project/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.34.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/__init__.py` & `mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/__init__.pyi` & `mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/__main__.py` & `mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Redshift 1.34.57\n"
-        "Version:         1.34.57\n"
+        "Type annotations for boto3.Redshift 1.34.84\n"
+        "Version:         1.34.84\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.57")
+    print("1.34.84")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/client.py` & `mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/client.pyi` & `mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/literals.py` & `mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,14 +258,15 @@
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
@@ -278,24 +279,26 @@
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
@@ -356,15 +359,14 @@
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
@@ -544,14 +546,15 @@
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

### Comparing `mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/literals.pyi` & `mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -258,14 +258,15 @@
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
@@ -278,24 +279,26 @@
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
@@ -356,15 +359,14 @@
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
@@ -544,14 +546,15 @@
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

### Comparing `mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/paginator.py` & `mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/paginator.pyi` & `mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/type_defs.py` & `mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2354,14 +2354,15 @@
         "EnhancedVpcRouting": NotRequired[bool],
         "MaintenanceTrackName": NotRequired[str],
         "ManualSnapshotRetentionPeriod": NotRequired[int],
         "ManualSnapshotRemainingDays": NotRequired[int],
         "SnapshotRetentionStartTime": NotRequired[datetime],
         "MasterPasswordSecretArn": NotRequired[str],
         "MasterPasswordSecretKmsKeyId": NotRequired[str],
+        "SnapshotArn": NotRequired[str],
     },
 )
 TaggedResourceTypeDef = TypedDict(
     "TaggedResourceTypeDef",
     {
         "Tag": NotRequired[TagTypeDef],
         "ResourceName": NotRequired[str],
```

### Comparing `mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/type_defs.pyi` & `mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2354,14 +2354,15 @@
         "EnhancedVpcRouting": NotRequired[bool],
         "MaintenanceTrackName": NotRequired[str],
         "ManualSnapshotRetentionPeriod": NotRequired[int],
         "ManualSnapshotRemainingDays": NotRequired[int],
         "SnapshotRetentionStartTime": NotRequired[datetime],
         "MasterPasswordSecretArn": NotRequired[str],
         "MasterPasswordSecretKmsKeyId": NotRequired[str],
+        "SnapshotArn": NotRequired[str],
     },
 )
 TaggedResourceTypeDef = TypedDict(
     "TaggedResourceTypeDef",
     {
         "Tag": NotRequired[TagTypeDef],
         "ResourceName": NotRequired[str],
```

### Comparing `mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/waiter.py` & `mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.34.57/mypy_boto3_redshift/waiter.pyi` & `mypy_boto3_redshift-1.34.84/mypy_boto3_redshift/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.34.57/mypy_boto3_redshift.egg-info/PKG-INFO` & `mypy_boto3_redshift-1.34.84/mypy_boto3_redshift.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift
-Version: 1.34.57
-Summary: Type annotations for boto3.Redshift 1.34.57 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.84
+Summary: Type annotations for boto3.Redshift 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift)](https://pepy.tech/project/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.34.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-redshift-1.34.57/mypy_boto3_redshift.egg-info/SOURCES.txt` & `mypy_boto3_redshift-1.34.84/mypy_boto3_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.34.57/setup.py` & `mypy_boto3_redshift-1.34.84/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-redshift",
-    version="1.34.57",
+    version="1.34.84",
     packages=["mypy_boto3_redshift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Redshift 1.34.57 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.Redshift 1.34.84 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

