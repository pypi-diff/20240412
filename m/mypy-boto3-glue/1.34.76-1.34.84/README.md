# Comparing `tmp/mypy-boto3-glue-1.34.76.tar.gz` & `tmp/mypy_boto3_glue-1.34.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-glue-1.34.76.tar", last modified: Tue Apr  2 19:32:31 2024, max compression
+gzip compressed data, was "mypy_boto3_glue-1.34.84.tar", last modified: Fri Apr 12 19:32:35 2024, max compression
```

## Comparing `mypy-boto3-glue-1.34.76.tar` & `mypy_boto3_glue-1.34.84.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:31.483228 mypy-boto3-glue-1.34.76/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-04-02 19:32:31.483228 mypy-boto3-glue-1.34.76/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:31.479228 mypy-boto3-glue-1.34.76/mypy_boto3_glue/
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   145115 2024-04-02 19:31:57.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   145112 2024-04-02 19:31:56.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22643 2024-04-02 19:31:57.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    22643 2024-04-02 19:31:57.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21346 2024-04-02 19:31:57.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21326 2024-04-02 19:31:57.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   238231 2024-04-02 19:32:02.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   238231 2024-04-02 19:32:00.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:31.483228 mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-04-02 19:32:31.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-02 19:32:31.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:32:31.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:32:31.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:32:31.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 19:32:31.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:32:31.483228 mypy-boto3-glue-1.34.76/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:35.941305 mypy_boto3_glue-1.34.84/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-04-12 19:32:35.937305 mypy_boto3_glue-1.34.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:35.937305 mypy_boto3_glue-1.34.84/mypy_boto3_glue/
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145215 2024-04-12 19:32:01.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145212 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22665 2024-04-12 19:32:01.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22665 2024-04-12 19:32:01.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21346 2024-04-12 19:32:01.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21326 2024-04-12 19:32:01.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   238323 2024-04-12 19:32:06.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   238323 2024-04-12 19:32:04.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:35.937305 mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-04-12 19:32:35.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 19:32:35.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:35.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:35.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 19:32:35.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 19:32:35.000000 mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:32:35.941305 mypy_boto3_glue-1.34.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-12 19:31:59.000000 mypy_boto3_glue-1.34.84/setup.py
```

### Comparing `mypy-boto3-glue-1.34.76/LICENSE` & `mypy_boto3_glue-1.34.84/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.34.76/PKG-INFO` & `mypy_boto3_glue-1.34.84/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glue
-Version: 1.34.76
-Summary: Type annotations for boto3.Glue 1.34.76 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.84
+Summary: Type annotations for boto3.Glue 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glue)](https://pepy.tech/project/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-glue-1.34.76/README.md` & `mypy_boto3_glue-1.34.84/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glue)](https://pepy.tech/project/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-glue-1.34.76/mypy_boto3_glue/__init__.py` & `mypy_boto3_glue-1.34.84/mypy_boto3_glue/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.34.76/mypy_boto3_glue/__init__.pyi` & `mypy_boto3_glue-1.34.84/mypy_boto3_glue/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.34.76/mypy_boto3_glue/__main__.py` & `mypy_boto3_glue-1.34.84/mypy_boto3_glue/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Glue 1.34.76\n"
-        "Version:         1.34.76\n"
+        "Type annotations for boto3.Glue 1.34.84\n"
+        "Version:         1.34.84\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.76")
+    print("1.34.84")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-glue-1.34.76/mypy_boto3_glue/client.py` & `mypy_boto3_glue-1.34.84/mypy_boto3_glue/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1962,21 +1962,24 @@
         *,
         CatalogId: str,
         DatabaseName: str,
         Name: str,
         SupportedPermissionTypes: Sequence[PermissionTypeType],
         Region: str = ...,
         AuditContext: AuditContextTypeDef = ...,
+        ParentResourceArn: str = ...,
+        RootResourceArn: str = ...,
         SupportedDialect: SupportedDialectTypeDef = ...,
         Permissions: Sequence[PermissionType] = ...,
         QuerySessionContext: QuerySessionContextTypeDef = ...,
     ) -> GetUnfilteredTableMetadataResponseTypeDef:
         """
-        Retrieves table metadata from the Data Catalog that contains unfiltered
-        metadata.
+        Allows a third-party analytical engine to retrieve unfiltered table metadata
+        from the Data
+        Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_table_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_unfiltered_table_metadata)
         """
 
     def get_user_defined_function(
         self, *, DatabaseName: str, FunctionName: str, CatalogId: str = ...
```

### Comparing `mypy-boto3-glue-1.34.76/mypy_boto3_glue/client.pyi` & `mypy_boto3_glue-1.34.84/mypy_boto3_glue/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1959,21 +1959,24 @@
         *,
         CatalogId: str,
         DatabaseName: str,
         Name: str,
         SupportedPermissionTypes: Sequence[PermissionTypeType],
         Region: str = ...,
         AuditContext: AuditContextTypeDef = ...,
+        ParentResourceArn: str = ...,
+        RootResourceArn: str = ...,
         SupportedDialect: SupportedDialectTypeDef = ...,
         Permissions: Sequence[PermissionType] = ...,
         QuerySessionContext: QuerySessionContextTypeDef = ...,
     ) -> GetUnfilteredTableMetadataResponseTypeDef:
         """
-        Retrieves table metadata from the Data Catalog that contains unfiltered
-        metadata.
+        Allows a third-party analytical engine to retrieve unfiltered table metadata
+        from the Data
+        Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_table_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_unfiltered_table_metadata)
         """
 
     def get_user_defined_function(
         self, *, DatabaseName: str, FunctionName: str, CatalogId: str = ...
```

### Comparing `mypy-boto3-glue-1.34.76/mypy_boto3_glue/literals.py` & `mypy_boto3_glue-1.34.84/mypy_boto3_glue/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,14 +486,15 @@
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

### Comparing `mypy-boto3-glue-1.34.76/mypy_boto3_glue/literals.pyi` & `mypy_boto3_glue-1.34.84/mypy_boto3_glue/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -486,14 +486,15 @@
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

### Comparing `mypy-boto3-glue-1.34.76/mypy_boto3_glue/paginator.py` & `mypy_boto3_glue-1.34.84/mypy_boto3_glue/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.34.76/mypy_boto3_glue/paginator.pyi` & `mypy_boto3_glue-1.34.84/mypy_boto3_glue/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.34.76/mypy_boto3_glue/type_defs.py` & `mypy_boto3_glue-1.34.84/mypy_boto3_glue/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -6054,14 +6054,16 @@
     {
         "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
         "SupportedPermissionTypes": Sequence[PermissionTypeType],
         "Region": NotRequired[str],
         "AuditContext": NotRequired[AuditContextTypeDef],
+        "ParentResourceArn": NotRequired[str],
+        "RootResourceArn": NotRequired[str],
         "SupportedDialect": NotRequired[SupportedDialectTypeDef],
         "Permissions": NotRequired[Sequence[PermissionType]],
         "QuerySessionContext": NotRequired[QuerySessionContextTypeDef],
     },
 )
 GetMLTaskRunsRequestRequestTypeDef = TypedDict(
     "GetMLTaskRunsRequestRequestTypeDef",
```

### Comparing `mypy-boto3-glue-1.34.76/mypy_boto3_glue/type_defs.pyi` & `mypy_boto3_glue-1.34.84/mypy_boto3_glue/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -6054,14 +6054,16 @@
     {
         "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
         "SupportedPermissionTypes": Sequence[PermissionTypeType],
         "Region": NotRequired[str],
         "AuditContext": NotRequired[AuditContextTypeDef],
+        "ParentResourceArn": NotRequired[str],
+        "RootResourceArn": NotRequired[str],
         "SupportedDialect": NotRequired[SupportedDialectTypeDef],
         "Permissions": NotRequired[Sequence[PermissionType]],
         "QuerySessionContext": NotRequired[QuerySessionContextTypeDef],
     },
 )
 GetMLTaskRunsRequestRequestTypeDef = TypedDict(
     "GetMLTaskRunsRequestRequestTypeDef",
```

### Comparing `mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/PKG-INFO` & `mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glue
-Version: 1.34.76
-Summary: Type annotations for boto3.Glue 1.34.76 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.84
+Summary: Type annotations for boto3.Glue 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glue)](https://pepy.tech/project/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/SOURCES.txt` & `mypy_boto3_glue-1.34.84/mypy_boto3_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.34.76/setup.py` & `mypy_boto3_glue-1.34.84/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-glue",
-    version="1.34.76",
+    version="1.34.84",
     packages=["mypy_boto3_glue"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Glue 1.34.76 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.Glue 1.34.84 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

