# Comparing `tmp/mypy-boto3-mediatailor-1.34.65.tar.gz` & `tmp/mypy_boto3_mediatailor-1.34.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediatailor-1.34.65.tar", last modified: Mon Mar 18 20:47:30 2024, max compression
+gzip compressed data, was "mypy_boto3_mediatailor-1.34.84.tar", last modified: Fri Apr 12 19:32:37 2024, max compression
```

## Comparing `mypy-boto3-mediatailor-1.34.65.tar` & `mypy_boto3_mediatailor-1.34.84.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:30.518612 mypy-boto3-mediatailor-1.34.65/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-18 20:46:58.000000 mypy-boto3-mediatailor-1.34.65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-03-18 20:47:30.518612 mypy-boto3-mediatailor-1.34.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-03-18 20:46:58.000000 mypy-boto3-mediatailor-1.34.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:30.514612 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-03-18 20:46:58.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-03-18 20:46:58.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-18 20:46:58.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34014 2024-03-18 20:46:58.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34011 2024-03-18 20:46:58.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-03-18 20:46:58.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-03-18 20:46:58.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-03-18 20:46:58.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-03-18 20:46:58.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 20:46:58.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    49178 2024-03-18 20:47:00.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    49178 2024-03-18 20:46:59.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-18 20:46:58.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:30.518612 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-03-18 20:47:30.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-18 20:47:30.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 20:47:30.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 20:47:30.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-18 20:47:30.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-18 20:47:30.000000 mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 20:47:30.518612 mypy-boto3-mediatailor-1.34.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-18 20:46:58.000000 mypy-boto3-mediatailor-1.34.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:37.293304 mypy_boto3_mediatailor-1.34.84/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 19:32:09.000000 mypy_boto3_mediatailor-1.34.84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-04-12 19:32:37.293304 mypy_boto3_mediatailor-1.34.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-04-12 19:32:09.000000 mypy_boto3_mediatailor-1.34.84/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:37.293304 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-12 19:32:09.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-12 19:32:09.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-12 19:32:10.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34081 2024-04-12 19:32:10.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34078 2024-04-12 19:32:10.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11006 2024-04-12 19:32:11.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11006 2024-04-12 19:32:11.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-04-12 19:32:10.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-12 19:32:10.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:10.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    49403 2024-04-12 19:32:11.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49403 2024-04-12 19:32:11.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 19:32:09.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:37.293304 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-04-12 19:32:37.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-12 19:32:37.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:37.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:37.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 19:32:37.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 19:32:37.000000 mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:32:37.293304 mypy_boto3_mediatailor-1.34.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-12 19:32:09.000000 mypy_boto3_mediatailor-1.34.84/setup.py
```

### Comparing `mypy-boto3-mediatailor-1.34.65/LICENSE` & `mypy_boto3_mediatailor-1.34.84/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.34.65/PKG-INFO` & `mypy_boto3_mediatailor-1.34.84/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediatailor
-Version: 1.34.65
-Summary: Type annotations for boto3.MediaTailor 1.34.65 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.84
+Summary: Type annotations for boto3.MediaTailor 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediatailor.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediatailor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediatailor)](https://pepy.tech/project/mypy-boto3-mediatailor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaTailor 1.34.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
+[boto3.MediaTailor 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-mediatailor-1.34.65/README.md` & `mypy_boto3_mediatailor-1.34.84/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediatailor.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediatailor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediatailor)](https://pepy.tech/project/mypy-boto3-mediatailor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaTailor 1.34.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
+[boto3.MediaTailor 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/__init__.py` & `mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/__init__.pyi` & `mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/__main__.py` & `mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaTailor 1.34.65\n"
-        "Version:         1.34.65\n"
+        "Type annotations for boto3.MediaTailor 1.34.84\n"
+        "Version:         1.34.84\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.65")
+    print("1.34.84")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/client.py` & `mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import PlaybackModeType, TierType
+from .literals import InsertionModeType, PlaybackModeType, TierType
 from .paginator import (
     GetChannelSchedulePaginator,
     ListAlertsPaginator,
     ListChannelsPaginator,
     ListLiveSourcesPaginator,
     ListPlaybackConfigurationsPaginator,
     ListPrefetchSchedulesPaginator,
@@ -532,14 +532,15 @@
         Name: str,
         AdDecisionServerUrl: str = ...,
         AvailSuppression: AvailSuppressionTypeDef = ...,
         Bumper: BumperTypeDef = ...,
         CdnConfiguration: CdnConfigurationTypeDef = ...,
         ConfigurationAliases: Mapping[str, Mapping[str, str]] = ...,
         DashConfiguration: DashConfigurationForPutTypeDef = ...,
+        InsertionMode: InsertionModeType = ...,
         LivePreRollConfiguration: LivePreRollConfigurationTypeDef = ...,
         ManifestProcessingRules: ManifestProcessingRulesTypeDef = ...,
         PersonalizationThresholdSeconds: int = ...,
         SlateAdUrl: str = ...,
         Tags: Mapping[str, str] = ...,
         TranscodeProfileName: str = ...,
         VideoContentSourceUrl: str = ...,
```

### Comparing `mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/client.pyi` & `mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import PlaybackModeType, TierType
+from .literals import InsertionModeType, PlaybackModeType, TierType
 from .paginator import (
     GetChannelSchedulePaginator,
     ListAlertsPaginator,
     ListChannelsPaginator,
     ListLiveSourcesPaginator,
     ListPlaybackConfigurationsPaginator,
     ListPrefetchSchedulesPaginator,
@@ -529,14 +529,15 @@
         Name: str,
         AdDecisionServerUrl: str = ...,
         AvailSuppression: AvailSuppressionTypeDef = ...,
         Bumper: BumperTypeDef = ...,
         CdnConfiguration: CdnConfigurationTypeDef = ...,
         ConfigurationAliases: Mapping[str, Mapping[str, str]] = ...,
         DashConfiguration: DashConfigurationForPutTypeDef = ...,
+        InsertionMode: InsertionModeType = ...,
         LivePreRollConfiguration: LivePreRollConfigurationTypeDef = ...,
         ManifestProcessingRules: ManifestProcessingRulesTypeDef = ...,
         PersonalizationThresholdSeconds: int = ...,
         SlateAdUrl: str = ...,
         Tags: Mapping[str, str] = ...,
         TranscodeProfileName: str = ...,
         VideoContentSourceUrl: str = ...,
```

### Comparing `mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/literals.py` & `mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 __all__ = (
     "AccessTypeType",
     "AdMarkupTypeType",
     "AlertCategoryType",
     "ChannelStateType",
     "FillPolicyType",
     "GetChannelSchedulePaginatorName",
+    "InsertionModeType",
     "ListAlertsPaginatorName",
     "ListChannelsPaginatorName",
     "ListLiveSourcesPaginatorName",
     "ListPlaybackConfigurationsPaginatorName",
     "ListPrefetchSchedulesPaginatorName",
     "ListSourceLocationsPaginatorName",
     "ListVodSourcesPaginatorName",
@@ -52,14 +53,15 @@
 
 AccessTypeType = Literal["AUTODETECT_SIGV4", "S3_SIGV4", "SECRETS_MANAGER_ACCESS_TOKEN"]
 AdMarkupTypeType = Literal["DATERANGE", "SCTE35_ENHANCED"]
 AlertCategoryType = Literal["INFO", "PLAYBACK_WARNING", "SCHEDULING_ERROR"]
 ChannelStateType = Literal["RUNNING", "STOPPED"]
 FillPolicyType = Literal["FULL_AVAIL_ONLY", "PARTIAL_AVAIL"]
 GetChannelSchedulePaginatorName = Literal["get_channel_schedule"]
+InsertionModeType = Literal["PLAYER_SELECT", "STITCHED_ONLY"]
 ListAlertsPaginatorName = Literal["list_alerts"]
 ListChannelsPaginatorName = Literal["list_channels"]
 ListLiveSourcesPaginatorName = Literal["list_live_sources"]
 ListPlaybackConfigurationsPaginatorName = Literal["list_playback_configurations"]
 ListPrefetchSchedulesPaginatorName = Literal["list_prefetch_schedules"]
 ListSourceLocationsPaginatorName = Literal["list_source_locations"]
 ListVodSourcesPaginatorName = Literal["list_vod_sources"]
@@ -141,14 +143,15 @@
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
@@ -161,24 +164,26 @@
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
@@ -479,20 +484,22 @@
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-3",
+    "me-central-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/literals.pyi` & `mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 __all__ = (
     "AccessTypeType",
     "AdMarkupTypeType",
     "AlertCategoryType",
     "ChannelStateType",
     "FillPolicyType",
     "GetChannelSchedulePaginatorName",
+    "InsertionModeType",
     "ListAlertsPaginatorName",
     "ListChannelsPaginatorName",
     "ListLiveSourcesPaginatorName",
     "ListPlaybackConfigurationsPaginatorName",
     "ListPrefetchSchedulesPaginatorName",
     "ListSourceLocationsPaginatorName",
     "ListVodSourcesPaginatorName",
@@ -52,14 +53,15 @@
 
 AccessTypeType = Literal["AUTODETECT_SIGV4", "S3_SIGV4", "SECRETS_MANAGER_ACCESS_TOKEN"]
 AdMarkupTypeType = Literal["DATERANGE", "SCTE35_ENHANCED"]
 AlertCategoryType = Literal["INFO", "PLAYBACK_WARNING", "SCHEDULING_ERROR"]
 ChannelStateType = Literal["RUNNING", "STOPPED"]
 FillPolicyType = Literal["FULL_AVAIL_ONLY", "PARTIAL_AVAIL"]
 GetChannelSchedulePaginatorName = Literal["get_channel_schedule"]
+InsertionModeType = Literal["PLAYER_SELECT", "STITCHED_ONLY"]
 ListAlertsPaginatorName = Literal["list_alerts"]
 ListChannelsPaginatorName = Literal["list_channels"]
 ListLiveSourcesPaginatorName = Literal["list_live_sources"]
 ListPlaybackConfigurationsPaginatorName = Literal["list_playback_configurations"]
 ListPrefetchSchedulesPaginatorName = Literal["list_prefetch_schedules"]
 ListSourceLocationsPaginatorName = Literal["list_source_locations"]
 ListVodSourcesPaginatorName = Literal["list_vod_sources"]
@@ -141,14 +143,15 @@
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
@@ -161,24 +164,26 @@
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
@@ -479,20 +484,22 @@
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-3",
+    "me-central-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/paginator.py` & `mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/paginator.pyi` & `mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/type_defs.py` & `mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from .literals import (
     AccessTypeType,
     AdMarkupTypeType,
     AlertCategoryType,
     ChannelStateType,
     FillPolicyType,
+    InsertionModeType,
     MessageTypeType,
     ModeType,
     OriginManifestTypeType,
     PlaybackModeType,
     RelativePositionType,
     ScheduleEntryTypeType,
     TierType,
@@ -1097,14 +1098,15 @@
         "AdDecisionServerUrl": str,
         "AvailSuppression": AvailSuppressionTypeDef,
         "Bumper": BumperTypeDef,
         "CdnConfiguration": CdnConfigurationTypeDef,
         "ConfigurationAliases": Dict[str, Dict[str, str]],
         "DashConfiguration": DashConfigurationTypeDef,
         "HlsConfiguration": HlsConfigurationTypeDef,
+        "InsertionMode": InsertionModeType,
         "LivePreRollConfiguration": LivePreRollConfigurationTypeDef,
         "LogConfiguration": LogConfigurationTypeDef,
         "ManifestProcessingRules": ManifestProcessingRulesTypeDef,
         "Name": str,
         "PersonalizationThresholdSeconds": int,
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
@@ -1122,14 +1124,15 @@
         "AdDecisionServerUrl": NotRequired[str],
         "AvailSuppression": NotRequired[AvailSuppressionTypeDef],
         "Bumper": NotRequired[BumperTypeDef],
         "CdnConfiguration": NotRequired[CdnConfigurationTypeDef],
         "ConfigurationAliases": NotRequired[Dict[str, Dict[str, str]]],
         "DashConfiguration": NotRequired[DashConfigurationTypeDef],
         "HlsConfiguration": NotRequired[HlsConfigurationTypeDef],
+        "InsertionMode": NotRequired[InsertionModeType],
         "LivePreRollConfiguration": NotRequired[LivePreRollConfigurationTypeDef],
         "LogConfiguration": NotRequired[LogConfigurationTypeDef],
         "ManifestProcessingRules": NotRequired[ManifestProcessingRulesTypeDef],
         "Name": NotRequired[str],
         "PersonalizationThresholdSeconds": NotRequired[int],
         "PlaybackConfigurationArn": NotRequired[str],
         "PlaybackEndpointPrefix": NotRequired[str],
@@ -1146,14 +1149,15 @@
         "Name": str,
         "AdDecisionServerUrl": NotRequired[str],
         "AvailSuppression": NotRequired[AvailSuppressionTypeDef],
         "Bumper": NotRequired[BumperTypeDef],
         "CdnConfiguration": NotRequired[CdnConfigurationTypeDef],
         "ConfigurationAliases": NotRequired[Mapping[str, Mapping[str, str]]],
         "DashConfiguration": NotRequired[DashConfigurationForPutTypeDef],
+        "InsertionMode": NotRequired[InsertionModeType],
         "LivePreRollConfiguration": NotRequired[LivePreRollConfigurationTypeDef],
         "ManifestProcessingRules": NotRequired[ManifestProcessingRulesTypeDef],
         "PersonalizationThresholdSeconds": NotRequired[int],
         "SlateAdUrl": NotRequired[str],
         "Tags": NotRequired[Mapping[str, str]],
         "TranscodeProfileName": NotRequired[str],
         "VideoContentSourceUrl": NotRequired[str],
@@ -1165,14 +1169,15 @@
         "AdDecisionServerUrl": str,
         "AvailSuppression": AvailSuppressionTypeDef,
         "Bumper": BumperTypeDef,
         "CdnConfiguration": CdnConfigurationTypeDef,
         "ConfigurationAliases": Dict[str, Dict[str, str]],
         "DashConfiguration": DashConfigurationTypeDef,
         "HlsConfiguration": HlsConfigurationTypeDef,
+        "InsertionMode": InsertionModeType,
         "LivePreRollConfiguration": LivePreRollConfigurationTypeDef,
         "LogConfiguration": LogConfigurationTypeDef,
         "ManifestProcessingRules": ManifestProcessingRulesTypeDef,
         "Name": str,
         "PersonalizationThresholdSeconds": int,
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
```

### Comparing `mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor/type_defs.pyi` & `mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from .literals import (
     AccessTypeType,
     AdMarkupTypeType,
     AlertCategoryType,
     ChannelStateType,
     FillPolicyType,
+    InsertionModeType,
     MessageTypeType,
     ModeType,
     OriginManifestTypeType,
     PlaybackModeType,
     RelativePositionType,
     ScheduleEntryTypeType,
     TierType,
@@ -1097,14 +1098,15 @@
         "AdDecisionServerUrl": str,
         "AvailSuppression": AvailSuppressionTypeDef,
         "Bumper": BumperTypeDef,
         "CdnConfiguration": CdnConfigurationTypeDef,
         "ConfigurationAliases": Dict[str, Dict[str, str]],
         "DashConfiguration": DashConfigurationTypeDef,
         "HlsConfiguration": HlsConfigurationTypeDef,
+        "InsertionMode": InsertionModeType,
         "LivePreRollConfiguration": LivePreRollConfigurationTypeDef,
         "LogConfiguration": LogConfigurationTypeDef,
         "ManifestProcessingRules": ManifestProcessingRulesTypeDef,
         "Name": str,
         "PersonalizationThresholdSeconds": int,
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
@@ -1122,14 +1124,15 @@
         "AdDecisionServerUrl": NotRequired[str],
         "AvailSuppression": NotRequired[AvailSuppressionTypeDef],
         "Bumper": NotRequired[BumperTypeDef],
         "CdnConfiguration": NotRequired[CdnConfigurationTypeDef],
         "ConfigurationAliases": NotRequired[Dict[str, Dict[str, str]]],
         "DashConfiguration": NotRequired[DashConfigurationTypeDef],
         "HlsConfiguration": NotRequired[HlsConfigurationTypeDef],
+        "InsertionMode": NotRequired[InsertionModeType],
         "LivePreRollConfiguration": NotRequired[LivePreRollConfigurationTypeDef],
         "LogConfiguration": NotRequired[LogConfigurationTypeDef],
         "ManifestProcessingRules": NotRequired[ManifestProcessingRulesTypeDef],
         "Name": NotRequired[str],
         "PersonalizationThresholdSeconds": NotRequired[int],
         "PlaybackConfigurationArn": NotRequired[str],
         "PlaybackEndpointPrefix": NotRequired[str],
@@ -1146,14 +1149,15 @@
         "Name": str,
         "AdDecisionServerUrl": NotRequired[str],
         "AvailSuppression": NotRequired[AvailSuppressionTypeDef],
         "Bumper": NotRequired[BumperTypeDef],
         "CdnConfiguration": NotRequired[CdnConfigurationTypeDef],
         "ConfigurationAliases": NotRequired[Mapping[str, Mapping[str, str]]],
         "DashConfiguration": NotRequired[DashConfigurationForPutTypeDef],
+        "InsertionMode": NotRequired[InsertionModeType],
         "LivePreRollConfiguration": NotRequired[LivePreRollConfigurationTypeDef],
         "ManifestProcessingRules": NotRequired[ManifestProcessingRulesTypeDef],
         "PersonalizationThresholdSeconds": NotRequired[int],
         "SlateAdUrl": NotRequired[str],
         "Tags": NotRequired[Mapping[str, str]],
         "TranscodeProfileName": NotRequired[str],
         "VideoContentSourceUrl": NotRequired[str],
@@ -1165,14 +1169,15 @@
         "AdDecisionServerUrl": str,
         "AvailSuppression": AvailSuppressionTypeDef,
         "Bumper": BumperTypeDef,
         "CdnConfiguration": CdnConfigurationTypeDef,
         "ConfigurationAliases": Dict[str, Dict[str, str]],
         "DashConfiguration": DashConfigurationTypeDef,
         "HlsConfiguration": HlsConfigurationTypeDef,
+        "InsertionMode": InsertionModeType,
         "LivePreRollConfiguration": LivePreRollConfigurationTypeDef,
         "LogConfiguration": LogConfigurationTypeDef,
         "ManifestProcessingRules": ManifestProcessingRulesTypeDef,
         "Name": str,
         "PersonalizationThresholdSeconds": int,
         "PlaybackConfigurationArn": str,
         "PlaybackEndpointPrefix": str,
```

### Comparing `mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor.egg-info/PKG-INFO` & `mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediatailor
-Version: 1.34.65
-Summary: Type annotations for boto3.MediaTailor 1.34.65 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.84
+Summary: Type annotations for boto3.MediaTailor 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediatailor.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediatailor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediatailor)](https://pepy.tech/project/mypy-boto3-mediatailor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaTailor 1.34.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
+[boto3.MediaTailor 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-mediatailor-1.34.65/mypy_boto3_mediatailor.egg-info/SOURCES.txt` & `mypy_boto3_mediatailor-1.34.84/mypy_boto3_mediatailor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.34.65/setup.py` & `mypy_boto3_mediatailor-1.34.84/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediatailor",
-    version="1.34.65",
+    version="1.34.84",
     packages=["mypy_boto3_mediatailor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.MediaTailor 1.34.65 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.MediaTailor 1.34.84 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

