# Comparing `tmp/sysnet-taxonomy-1.0.0.4.tar.gz` & `tmp/sysnet-taxonomy-1.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysnet-taxonomy-1.0.0.4.tar", last modified: Tue Aug 29 16:23:47 2023, max compression
+gzip compressed data, was "sysnet-taxonomy-1.0.1.1.tar", last modified: Fri Apr 12 16:31:29 2024, max compression
```

## Comparing `sysnet-taxonomy-1.0.0.4.tar` & `sysnet-taxonomy-1.0.1.1.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-08-29 16:23:47.522106 sysnet-taxonomy-1.0.0.4/
--rw-rw-rw-   0        0        0     4996 2023-08-29 16:23:47.521106 sysnet-taxonomy-1.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4277 2023-08-29 16:22:14.000000 sysnet-taxonomy-1.0.0.4/README.md
--rw-rw-rw-   0        0        0      654 2023-08-29 16:22:25.000000 sysnet-taxonomy-1.0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-29 16:23:47.522106 sysnet-taxonomy-1.0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      927 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-29 16:23:47.469099 sysnet-taxonomy-1.0.0.4/sysnet_taxonomy.egg-info/
--rw-rw-rw-   0        0        0     4996 2023-08-29 16:23:47.000000 sysnet-taxonomy-1.0.0.4/sysnet_taxonomy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      917 2023-08-29 16:23:47.000000 sysnet-taxonomy-1.0.0.4/sysnet_taxonomy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-29 16:23:47.000000 sysnet-taxonomy-1.0.0.4/sysnet_taxonomy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-08-29 16:23:47.000000 sysnet-taxonomy-1.0.0.4/sysnet_taxonomy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-29 16:23:47.000000 sysnet-taxonomy-1.0.0.4/sysnet_taxonomy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-29 16:23:47.476100 sysnet-taxonomy-1.0.0.4/taxonomy/
--rw-rw-rw-   0        0        0      953 2023-08-28 16:12:35.000000 sysnet-taxonomy-1.0.0.4/taxonomy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-29 16:23:47.485099 sysnet-taxonomy-1.0.0.4/taxonomy/api/
--rw-rw-rw-   0        0        0      233 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.4/taxonomy/api/__init__.py
--rw-rw-rw-   0        0        0    12596 2023-08-29 16:04:40.000000 sysnet-taxonomy-1.0.0.4/taxonomy/api/admins_api.py
--rw-rw-rw-   0        0        0     6885 2023-08-29 16:04:40.000000 sysnet-taxonomy-1.0.0.4/taxonomy/api/developers_api.py
--rw-rw-rw-   0        0        0     8471 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.4/taxonomy/api/public_api.py
--rw-rw-rw-   0        0        0    25013 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.4/taxonomy/api_client.py
--rw-rw-rw-   0        0        0     8218 2023-08-29 16:19:48.000000 sysnet-taxonomy-1.0.0.4/taxonomy/configuration.py
-drwxrwxrwx   0        0        0        0 2023-08-29 16:23:47.499098 sysnet-taxonomy-1.0.0.4/taxonomy/models/
--rw-rw-rw-   0        0        0      667 2023-08-28 16:12:35.000000 sysnet-taxonomy-1.0.0.4/taxonomy/models/__init__.py
--rw-rw-rw-   0        0        0     4207 2023-08-28 16:12:35.000000 sysnet-taxonomy-1.0.0.4/taxonomy/models/additional_type.py
--rw-rw-rw-   0        0        0     3766 2023-08-28 16:12:35.000000 sysnet-taxonomy-1.0.0.4/taxonomy/models/error_model.py
--rw-rw-rw-   0        0        0     4522 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.4/taxonomy/models/hybrid_type.py
--rw-rw-rw-   0        0        0     6778 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.4/taxonomy/models/taxon_entry_list_type.py
--rw-rw-rw-   0        0        0    10821 2023-08-28 16:12:35.000000 sysnet-taxonomy-1.0.0.4/taxonomy/models/taxon_entry_type.py
--rw-rw-rw-   0        0        0    23435 2023-08-29 16:04:40.000000 sysnet-taxonomy-1.0.0.4/taxonomy/models/taxon_type.py
--rw-rw-rw-   0        0        0    12989 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.4/taxonomy/rest.py
-drwxrwxrwx   0        0        0        0 2023-08-29 16:23:47.519134 sysnet-taxonomy-1.0.0.4/test/
--rw-rw-rw-   0        0        0       15 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.4/test/__init__.py
--rw-rw-rw-   0        0        0      876 2023-08-28 16:12:35.000000 sysnet-taxonomy-1.0.0.4/test/test_additional_type.py
--rw-rw-rw-   0        0        0     1066 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.4/test/test_admins_api.py
--rw-rw-rw-   0        0        0      962 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.4/test/test_developers_api.py
--rw-rw-rw-   0        0        0      844 2023-08-28 16:12:35.000000 sysnet-taxonomy-1.0.0.4/test/test_error_model.py
--rw-rw-rw-   0        0        0      844 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.4/test/test_hybrid_type.py
--rw-rw-rw-   0        0        0      951 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.4/test/test_public_api.py
--rw-rw-rw-   0        0        0      912 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.4/test/test_taxon_entry_list_type.py
--rw-rw-rw-   0        0        0      878 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.4/test/test_taxon_entry_type.py
--rw-rw-rw-   0        0        0      836 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.4/test/test_taxon_type.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:31:29.681030 sysnet-taxonomy-1.0.1.1/
+-rw-rw-rw-   0        0        0     4946 2024-04-12 16:31:29.680031 sysnet-taxonomy-1.0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4270 2024-04-12 15:49:47.000000 sysnet-taxonomy-1.0.1.1/README.md
+-rw-rw-rw-   0        0        0      654 2024-04-12 16:00:36.000000 sysnet-taxonomy-1.0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 16:31:29.682031 sysnet-taxonomy-1.0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      927 2024-04-12 14:00:44.000000 sysnet-taxonomy-1.0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:31:29.678029 sysnet-taxonomy-1.0.1.1/sysnet_taxonomy.egg-info/
+-rw-rw-rw-   0        0        0     4946 2024-04-12 16:31:29.000000 sysnet-taxonomy-1.0.1.1/sysnet_taxonomy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      879 2024-04-12 16:31:29.000000 sysnet-taxonomy-1.0.1.1/sysnet_taxonomy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 16:31:29.000000 sysnet-taxonomy-1.0.1.1/sysnet_taxonomy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-12 16:31:29.000000 sysnet-taxonomy-1.0.1.1/sysnet_taxonomy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 16:31:29.626517 sysnet-taxonomy-1.0.1.1/taxonomy/
+-rw-rw-rw-   0        0        0      953 2024-04-12 14:00:43.000000 sysnet-taxonomy-1.0.1.1/taxonomy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:31:29.635564 sysnet-taxonomy-1.0.1.1/taxonomy/api/
+-rw-rw-rw-   0        0        0      233 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.1.1/taxonomy/api/__init__.py
+-rw-rw-rw-   0        0        0    12596 2024-04-12 14:00:43.000000 sysnet-taxonomy-1.0.1.1/taxonomy/api/admins_api.py
+-rw-rw-rw-   0        0        0     6885 2024-04-12 14:00:43.000000 sysnet-taxonomy-1.0.1.1/taxonomy/api/developers_api.py
+-rw-rw-rw-   0        0        0     8762 2024-04-12 14:00:43.000000 sysnet-taxonomy-1.0.1.1/taxonomy/api/public_api.py
+-rw-rw-rw-   0        0        0    25013 2024-04-12 14:00:43.000000 sysnet-taxonomy-1.0.1.1/taxonomy/api_client.py
+-rw-rw-rw-   0        0        0     8314 2024-04-12 15:49:47.000000 sysnet-taxonomy-1.0.1.1/taxonomy/configuration.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:31:29.652032 sysnet-taxonomy-1.0.1.1/taxonomy/models/
+-rw-rw-rw-   0        0        0      667 2024-04-12 14:00:43.000000 sysnet-taxonomy-1.0.1.1/taxonomy/models/__init__.py
+-rw-rw-rw-   0        0        0     4207 2024-04-12 14:00:43.000000 sysnet-taxonomy-1.0.1.1/taxonomy/models/additional_type.py
+-rw-rw-rw-   0        0        0     3766 2024-04-12 14:00:43.000000 sysnet-taxonomy-1.0.1.1/taxonomy/models/error_model.py
+-rw-rw-rw-   0        0        0     4522 2024-04-12 14:00:43.000000 sysnet-taxonomy-1.0.1.1/taxonomy/models/hybrid_type.py
+-rw-rw-rw-   0        0        0     6778 2024-04-12 14:00:43.000000 sysnet-taxonomy-1.0.1.1/taxonomy/models/taxon_entry_list_type.py
+-rw-rw-rw-   0        0        0    10825 2024-04-12 16:00:36.000000 sysnet-taxonomy-1.0.1.1/taxonomy/models/taxon_entry_type.py
+-rw-rw-rw-   0        0        0    23437 2024-04-12 16:00:36.000000 sysnet-taxonomy-1.0.1.1/taxonomy/models/taxon_type.py
+-rw-rw-rw-   0        0        0    12986 2024-04-12 14:00:43.000000 sysnet-taxonomy-1.0.1.1/taxonomy/rest.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:31:29.675035 sysnet-taxonomy-1.0.1.1/test/
+-rw-rw-rw-   0        0        0       15 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.1.1/test/__init__.py
+-rw-rw-rw-   0        0        0     1085 2024-04-12 16:12:15.000000 sysnet-taxonomy-1.0.1.1/test/test_additional_type.py
+-rw-rw-rw-   0        0        0     1066 2024-04-12 14:00:43.000000 sysnet-taxonomy-1.0.1.1/test/test_admins_api.py
+-rw-rw-rw-   0        0        0      962 2024-04-12 14:00:43.000000 sysnet-taxonomy-1.0.1.1/test/test_developers_api.py
+-rw-rw-rw-   0        0        0      911 2024-04-12 16:13:53.000000 sysnet-taxonomy-1.0.1.1/test/test_error_model.py
+-rw-rw-rw-   0        0        0     1085 2024-04-12 16:22:25.000000 sysnet-taxonomy-1.0.1.1/test/test_hybrid_type.py
+-rw-rw-rw-   0        0        0      951 2024-04-12 14:00:43.000000 sysnet-taxonomy-1.0.1.1/test/test_public_api.py
+-rw-rw-rw-   0        0        0      849 2024-04-12 16:23:32.000000 sysnet-taxonomy-1.0.1.1/test/test_taxon_entry_list_type.py
+-rw-rw-rw-   0        0        0      838 2024-04-12 16:26:22.000000 sysnet-taxonomy-1.0.1.1/test/test_taxon_entry_type.py
+-rw-rw-rw-   0        0        0      810 2024-04-12 16:28:33.000000 sysnet-taxonomy-1.0.1.1/test/test_taxon_type.py
```

### Comparing `sysnet-taxonomy-1.0.0.4/PKG-INFO` & `sysnet-taxonomy-1.0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 Metadata-Version: 2.1
 Name: sysnet-taxonomy
-Version: 1.0.0.4
+Version: 1.0.1.1
 Summary: SYSNET CITES Taxonomy REST API client
 Home-page: 
 Author-email: Radim Jaeger <rjaeger@sysnet.cz>
 Project-URL: Homepage, https://github.com/SYSNET-CZ/swagger/tree/main/clients/taxonomy
-Keywords: Swagger,API pro taxonomii CITES
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # sysnet-taxonomy
 Toto je API pro taxonomii CITES
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.0.0
-- Package version: 1.0.0.004
+- API version: 1.0.1
+- Package version: 1.0.1.001
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.9+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on Github, you can install directly from Github
 
 ```sh
-pip install sysnet-taxonomy
+pip install taxonomy
 ```
 
 Then import the package:
 ```python
 import taxonomy 
 ```
 
@@ -100,15 +99,15 @@
     api_instance.put_taxon(body, identifier)
 except ApiException as e:
     print("Exception when calling AdminsApi->put_taxon: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://service.sysnet.cz/taxonomy/1.0.0*
+All URIs are relative to *https://service.sysnet.cz/taxonomy/1.0.1*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AdminsApi* | [**add_taxon**](docs/AdminsApi.md#add_taxon) | **POST** /taxon | přidá nový taxon
 *AdminsApi* | [**delete_taxon**](docs/AdminsApi.md#delete_taxon) | **DELETE** /taxon/{identifier} | odstraní existující taxon
 *AdminsApi* | [**put_taxon**](docs/AdminsApi.md#put_taxon) | **PUT** /taxon/{identifier} | upraví existující taxon
 *DevelopersApi* | [**info_api**](docs/DevelopersApi.md#info_api) | **GET** /info | vrací servisní informace
```

### Comparing `sysnet-taxonomy-1.0.0.4/README.md` & `sysnet-taxonomy-1.0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # sysnet-taxonomy
 Toto je API pro taxonomii CITES
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.0.0
-- Package version: 1.0.0.004
+- API version: 1.0.1
+- Package version: 1.0.1.001
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.9+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on Github, you can install directly from Github
 
 ```sh
-pip install sysnet-taxonomy
+pip install taxonomy
 ```
 
 Then import the package:
 ```python
 import taxonomy 
 ```
 
@@ -85,15 +85,15 @@
     api_instance.put_taxon(body, identifier)
 except ApiException as e:
     print("Exception when calling AdminsApi->put_taxon: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://service.sysnet.cz/taxonomy/1.0.0*
+All URIs are relative to *https://service.sysnet.cz/taxonomy/1.0.1*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AdminsApi* | [**add_taxon**](docs/AdminsApi.md#add_taxon) | **POST** /taxon | přidá nový taxon
 *AdminsApi* | [**delete_taxon**](docs/AdminsApi.md#delete_taxon) | **DELETE** /taxon/{identifier} | odstraní existující taxon
 *AdminsApi* | [**put_taxon**](docs/AdminsApi.md#put_taxon) | **PUT** /taxon/{identifier} | upraví existující taxon
 *DevelopersApi* | [**info_api**](docs/DevelopersApi.md#info_api) | **GET** /info | vrací servisní informace
```

### Comparing `sysnet-taxonomy-1.0.0.4/pyproject.toml` & `sysnet-taxonomy-1.0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sysnet-taxonomy"
-version = "1.0.0.004"
+version = "1.0.1.001"
 authors = [
   { name="Radim Jaeger", email="rjaeger@sysnet.cz" },
 ]
 description = "SYSNET CITES Taxonomy REST API client"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `sysnet-taxonomy-1.0.0.4/setup.py` & `sysnet-taxonomy-1.0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "sysnet-taxonomy"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `sysnet-taxonomy-1.0.0.4/sysnet_taxonomy.egg-info/PKG-INFO` & `sysnet-taxonomy-1.0.1.1/sysnet_taxonomy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 Metadata-Version: 2.1
 Name: sysnet-taxonomy
-Version: 1.0.0.4
+Version: 1.0.1.1
 Summary: SYSNET CITES Taxonomy REST API client
 Home-page: 
 Author-email: Radim Jaeger <rjaeger@sysnet.cz>
 Project-URL: Homepage, https://github.com/SYSNET-CZ/swagger/tree/main/clients/taxonomy
-Keywords: Swagger,API pro taxonomii CITES
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # sysnet-taxonomy
 Toto je API pro taxonomii CITES
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.0.0
-- Package version: 1.0.0.004
+- API version: 1.0.1
+- Package version: 1.0.1.001
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.9+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on Github, you can install directly from Github
 
 ```sh
-pip install sysnet-taxonomy
+pip install taxonomy
 ```
 
 Then import the package:
 ```python
 import taxonomy 
 ```
 
@@ -100,15 +99,15 @@
     api_instance.put_taxon(body, identifier)
 except ApiException as e:
     print("Exception when calling AdminsApi->put_taxon: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://service.sysnet.cz/taxonomy/1.0.0*
+All URIs are relative to *https://service.sysnet.cz/taxonomy/1.0.1*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AdminsApi* | [**add_taxon**](docs/AdminsApi.md#add_taxon) | **POST** /taxon | přidá nový taxon
 *AdminsApi* | [**delete_taxon**](docs/AdminsApi.md#delete_taxon) | **DELETE** /taxon/{identifier} | odstraní existující taxon
 *AdminsApi* | [**put_taxon**](docs/AdminsApi.md#put_taxon) | **PUT** /taxon/{identifier} | upraví existující taxon
 *DevelopersApi* | [**info_api**](docs/DevelopersApi.md#info_api) | **GET** /info | vrací servisní informace
```

### Comparing `sysnet-taxonomy-1.0.0.4/sysnet_taxonomy.egg-info/SOURCES.txt` & `sysnet-taxonomy-1.0.1.1/sysnet_taxonomy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 README.md
 pyproject.toml
 setup.py
 sysnet_taxonomy.egg-info/PKG-INFO
 sysnet_taxonomy.egg-info/SOURCES.txt
 sysnet_taxonomy.egg-info/dependency_links.txt
-sysnet_taxonomy.egg-info/requires.txt
 sysnet_taxonomy.egg-info/top_level.txt
 taxonomy/__init__.py
 taxonomy/api_client.py
 taxonomy/configuration.py
 taxonomy/rest.py
 taxonomy/api/__init__.py
 taxonomy/api/admins_api.py
```

### Comparing `sysnet-taxonomy-1.0.0.4/taxonomy/__init__.py` & `sysnet-taxonomy-1.0.1.1/taxonomy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
```

### Comparing `sysnet-taxonomy-1.0.0.4/taxonomy/api/admins_api.py` & `sysnet-taxonomy-1.0.1.1/taxonomy/api/admins_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sysnet-taxonomy-1.0.0.4/taxonomy/api/developers_api.py` & `sysnet-taxonomy-1.0.1.1/taxonomy/api/developers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sysnet-taxonomy-1.0.0.4/taxonomy/api/public_api.py` & `sysnet-taxonomy-1.0.1.1/taxonomy/api/public_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -132,14 +132,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.search_taxons(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str key: předává volitelný text pro vyhledání taxonů
+        :param str published: předává volitelný text pro vyhledání taxonů
         :param int start: První dokument na stránce
         :param int page_size: Velikost stránky při stránkovaném výstupu
         :param int page: Číslo stránky výstupu
         :return: TaxonEntryListType
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -157,23 +158,24 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.search_taxons_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str key: předává volitelný text pro vyhledání taxonů
+        :param str published: předává volitelný text pro vyhledání taxonů
         :param int start: První dokument na stránce
         :param int page_size: Velikost stránky při stránkovaném výstupu
         :param int page: Číslo stránky výstupu
         :return: TaxonEntryListType
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['key', 'start', 'page_size', 'page']  # noqa: E501
+        all_params = ['key', 'published', 'start', 'page_size', 'page']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -188,14 +190,16 @@
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'key' in params:
             query_params.append(('key', params['key']))  # noqa: E501
+        if 'published' in params:
+            query_params.append(('published', params['published']))  # noqa: E501
         if 'start' in params:
             query_params.append(('start', params['start']))  # noqa: E501
         if 'page_size' in params:
             query_params.append(('page_size', params['page_size']))  # noqa: E501
         if 'page' in params:
             query_params.append(('page', params['page']))  # noqa: E501
```

### Comparing `sysnet-taxonomy-1.0.0.4/taxonomy/api_client.py` & `sysnet-taxonomy-1.0.1.1/taxonomy/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 from __future__ import absolute_import
 
 import datetime
 import json
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/1.0.0/python'
+        self.user_agent = 'Swagger-Codegen/1.0.1/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `sysnet-taxonomy-1.0.0.4/taxonomy/configuration.py` & `sysnet-taxonomy-1.0.1.1/taxonomy/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import copy
@@ -42,15 +42,15 @@
     Ref: https://github.com/swagger-api/swagger-codegen
     Do not edit the class manually.
     """
 
     def __init__(self):
         """Constructor"""
         # Default Base url
-        self.host = "https://service.sysnet.cz/taxonomy/1.0.0"
+        self.host = "https://service.sysnet.cz/taxonomy/1.0.1"
         # Temp file folder for downloading files
         self.temp_folder_path = None
 
         # Authentication Settings
         # dict to store API key(s)
         self.api_key = {}
         # dict to store API prefix (e.g. Bearer)
@@ -215,17 +215,20 @@
                 return key
 
     def get_basic_auth_token(self):
         """Gets HTTP basic authentication header (string).
 
         :return: The token for basic HTTP authentication.
         """
-        return urllib3.util.make_headers(
-            basic_auth=self.username + ':' + self.password
-        ).get('authorization')
+        token = ""
+        if self.username or self.password:
+            token = urllib3.util.make_headers(
+                basic_auth=self.username + ':' + self.password
+            ).get('authorization')
+        return token
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         return {
@@ -242,10 +245,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.0.0".\
+               "Version of the API: 1.0.1\n"\
+               "SDK Package Version: 1.0.1".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `sysnet-taxonomy-1.0.0.4/taxonomy/models/__init__.py` & `sysnet-taxonomy-1.0.1.1/taxonomy/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import models into model package
```

### Comparing `sysnet-taxonomy-1.0.0.4/taxonomy/models/additional_type.py` & `sysnet-taxonomy-1.0.1.1/taxonomy/models/additional_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-taxonomy-1.0.0.4/taxonomy/models/error_model.py` & `sysnet-taxonomy-1.0.1.1/taxonomy/models/error_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-taxonomy-1.0.0.4/taxonomy/models/hybrid_type.py` & `sysnet-taxonomy-1.0.1.1/taxonomy/models/hybrid_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-taxonomy-1.0.0.4/taxonomy/models/taxon_entry_list_type.py` & `sysnet-taxonomy-1.0.1.1/taxonomy/models/taxon_entry_list_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-taxonomy-1.0.0.4/taxonomy/models/taxon_entry_type.py` & `sysnet-taxonomy-1.0.1.1/taxonomy/models/taxon_entry_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -260,15 +260,15 @@
         """Sets the regulation_cites of this TaxonEntryType.
 
         Exemplář sledovaný podle CITES  # noqa: E501
 
         :param regulation_cites: The regulation_cites of this TaxonEntryType.  # noqa: E501
         :type: str
         """
-        allowed_values = ["I", "I/II", "II", "II/III", "III", "NC", "Not CITES. Protected by the Act 114/1992.", "Not CITES", "", ""]  # noqa: E501
+        allowed_values = ["I", "I/II", "II", "II/III", "III", "NC", "Not CITES. Protected by the Act 114/1992.", "Not CITES", "", None]  # noqa: E501
         if regulation_cites not in allowed_values:
             raise ValueError(
                 "Invalid value for `regulation_cites` ({0}), must be one of {1}"  # noqa: E501
                 .format(regulation_cites, allowed_values)
             )
 
         self._regulation_cites = regulation_cites
@@ -289,15 +289,15 @@
         """Sets the regulation_eu of this TaxonEntryType.
 
         Exemplář sledovaný podle EU  # noqa: E501
 
         :param regulation_eu: The regulation_eu of this TaxonEntryType.  # noqa: E501
         :type: str
         """
-        allowed_values = ["A", "A/B", "B", "B/D", "C", "D", "", ""]  # noqa: E501
+        allowed_values = ["A", "A/B", "B", "B/D", "C", "D", "", None]  # noqa: E501
         if regulation_eu not in allowed_values:
             raise ValueError(
                 "Invalid value for `regulation_eu` ({0}), must be one of {1}"  # noqa: E501
                 .format(regulation_eu, allowed_values)
             )
 
         self._regulation_eu = regulation_eu
```

### Comparing `sysnet-taxonomy-1.0.0.4/taxonomy/models/taxon_type.py` & `sysnet-taxonomy-1.0.1.1/taxonomy/models/taxon_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -575,15 +575,15 @@
         """Sets the regulation_449 of this TaxonType.
 
         Exemplář sledovaný podle zákona 449 (myslivost)  # noqa: E501
 
         :param regulation_449: The regulation_449 of this TaxonType.  # noqa: E501
         :type: str
         """
-        allowed_values = ["A", "B", "", ""]  # noqa: E501
+        allowed_values = ["A", "B", "", None]  # noqa: E501
         if regulation_449 not in allowed_values:
             raise ValueError(
                 "Invalid value for `regulation_449` ({0}), must be one of {1}"  # noqa: E501
                 .format(regulation_449, allowed_values)
             )
 
         self._regulation_449 = regulation_449
```

### Comparing `sysnet-taxonomy-1.0.0.4/taxonomy/rest.py` & `sysnet-taxonomy-1.0.1.1/taxonomy/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import io
@@ -38,19 +38,19 @@
         self.urllib3_response = resp
         self.status = resp.status
         self.reason = resp.reason
         self.data = resp.data
 
     def getheaders(self):
         """Returns a dictionary of the response headers."""
-        return self.urllib3_response.getheaders()
+        return self.urllib3_response.headers
 
     def getheader(self, name, default=None):
         """Returns a given response header."""
-        return self.urllib3_response.getheader(name, default)
+        return self.urllib3_response.headers.get(name, default)
 
 
 class RESTClientObject(object):
 
     def __init__(self, configuration, pools_size=4, maxsize=None):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
```

### Comparing `sysnet-taxonomy-1.0.0.4/test/test_additional_type.py` & `sysnet-taxonomy-1.0.1.1/test/test_taxon_entry_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import taxonomy
-from taxonomy.models.additional_type import AdditionalType  # noqa: E501
+from taxonomy.models.taxon_entry_type import TaxonEntryType  # noqa: E501
 from taxonomy.rest import ApiException
 
 
-class TestAdditionalType(unittest.TestCase):
-    """AdditionalType unit test stubs"""
+class TestTaxonEntryType(unittest.TestCase):
+    """TaxonEntryType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAdditionalType(self):
-        """Test AdditionalType"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = taxonomy.models.additional_type.AdditionalType()  # noqa: E501
-        pass
+    def testTaxonEntryType(self):
+        """Test TaxonEntryType"""
+        model = taxonomy.models.taxon_entry_type.TaxonEntryType(name_scientific='Nepenthes veitchii')
+        assert model is not None
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sysnet-taxonomy-1.0.0.4/test/test_admins_api.py` & `sysnet-taxonomy-1.0.1.1/test/test_admins_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-taxonomy-1.0.0.4/test/test_developers_api.py` & `sysnet-taxonomy-1.0.1.1/test/test_developers_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-taxonomy-1.0.0.4/test/test_error_model.py` & `sysnet-taxonomy-1.0.1.1/test/test_taxon_type.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import taxonomy
-from taxonomy.models.error_model import ErrorModel  # noqa: E501
+from taxonomy.models.taxon_type import TaxonType  # noqa: E501
 from taxonomy.rest import ApiException
 
 
-class TestErrorModel(unittest.TestCase):
-    """ErrorModel unit test stubs"""
+class TestTaxonType(unittest.TestCase):
+    """TaxonType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testErrorModel(self):
-        """Test ErrorModel"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = taxonomy.models.error_model.ErrorModel()  # noqa: E501
-        pass
+    def testTaxonType(self):
+        """Test TaxonType"""
+        model = taxonomy.models.taxon_type.TaxonType(name_scientific='Nepenthes veitchii')  # noqa: E501
+        assert model is not None
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sysnet-taxonomy-1.0.0.4/test/test_hybrid_type.py` & `sysnet-taxonomy-1.0.1.1/test/test_additional_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import taxonomy
-from taxonomy.models.hybrid_type import HybridType  # noqa: E501
+from taxonomy.models.additional_type import AdditionalType  # noqa: E501
 from taxonomy.rest import ApiException
 
 
-class TestHybridType(unittest.TestCase):
-    """HybridType unit test stubs"""
+class TestAdditionalType(unittest.TestCase):
+    """AdditionalType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testHybridType(self):
-        """Test HybridType"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = taxonomy.models.hybrid_type.HybridType()  # noqa: E501
-        pass
+    def testAdditionalType(self):
+        """Test AdditionalType"""
+        model = taxonomy.models.additional_type.AdditionalType(
+            special_conditions='Nějaký <strong>HTML</strong> text pro AOPK',
+            fertility=25
+        )  # noqa: E501
+        assert 'HTML' in model.special_conditions, '{}.special_conditions musí obsahovat \'HTML\''
+        assert 25 == model.fertility, '{}.facility musí být 25'.format('AdditionalType')
 
 
 if __name__ == '__main__':
     unittest.main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sysnet-taxonomy-1.0.0.4/test/test_public_api.py` & `sysnet-taxonomy-1.0.1.1/test/test_public_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-taxonomy-1.0.0.4/test/test_taxon_entry_list_type.py` & `sysnet-taxonomy-1.0.1.1/test/test_taxon_entry_list_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     API pro taxonomii CITES
 
     Toto je API pro taxonomii CITES  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: rjaeger@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
@@ -26,14 +26,14 @@
         pass
 
     def tearDown(self):
         pass
 
     def testTaxonEntryListType(self):
         """Test TaxonEntryListType"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = taxonomy.models.taxon_entry_list_type.TaxonEntryListType()  # noqa: E501
+        model = taxonomy.models.taxon_entry_list_type.TaxonEntryListType()
+        assert model is not None
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

