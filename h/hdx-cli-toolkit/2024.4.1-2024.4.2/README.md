# Comparing `tmp/hdx_cli_toolkit-2024.4.1.tar.gz` & `tmp/hdx_cli_toolkit-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx_cli_toolkit-2024.4.1.tar", last modified: Sat Apr  6 13:26:23 2024, max compression
+gzip compressed data, was "hdx_cli_toolkit-2024.4.2.tar", last modified: Fri Apr 12 09:53:20 2024, max compression
```

## Comparing `hdx_cli_toolkit-2024.4.1.tar` & `hdx_cli_toolkit-2024.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:26:23.985731 hdx_cli_toolkit-2024.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-06 13:26:23.985731 hdx_cli_toolkit-2024.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 13:26:23.985731 hdx_cli_toolkit-2024.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:26:23.981731 hdx_cli_toolkit-2024.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:26:23.985731 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    14701 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/hdx_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:26:23.985731 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-06 13:26:23.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-06 13:26:23.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 13:26:23.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-06 13:26:23.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-06 13:26:23.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 13:26:23.000000 hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:26:23.985731 hdx_cli_toolkit-2024.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/tests/test_cli_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/tests/test_hdx_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/tests/test_hdx_utilities_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-06 13:26:08.000000 hdx_cli_toolkit-2024.4.1/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:53:20.715656 hdx_cli_toolkit-2024.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-12 09:53:20.715656 hdx_cli_toolkit-2024.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:53:20.715656 hdx_cli_toolkit-2024.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:53:20.711656 hdx_cli_toolkit-2024.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:53:20.715656 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14911 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/hdx_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:53:20.715656 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-12 09:53:20.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-12 09:53:20.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:53:20.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-12 09:53:20.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-12 09:53:20.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 09:53:20.000000 hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:53:20.715656 hdx_cli_toolkit-2024.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/tests/test_cli_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/tests/test_hdx_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/tests/test_hdx_utilities_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-12 09:53:06.000000 hdx_cli_toolkit-2024.4.2/tests/test_utilities.py
```

### Comparing `hdx_cli_toolkit-2024.4.1/LICENSE` & `hdx_cli_toolkit-2024.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.1/PKG-INFO` & `hdx_cli_toolkit-2024.4.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx_cli_toolkit
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: HDX CLI tool kit for commandline interaction with HDX
 Author: Ian Hopkinson
 Author-email: ian.hopkinson@un.org
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Ian Hopkinson
         
@@ -45,14 +45,15 @@
 
 ## Overview
 
 This toolkit provides a commandline interface to the [Humanitarian Data Exchange](https://data.humdata.org/) (HDX) to allow for bulk modification operations and other administrative activities such as getting `id` values for users and organization. It is useful for those managing HDX and developers building data pipelines for HDX. The currently supported commands are as follows:
 
 ```
   configuration              Print configuration information to terminal
+  download                   Download dataset resources from HDX
   get_organization_metadata  Get an organization id and other metadata
   get_user_metadata          Get user id and other metadata
   list                       List datasets in HDX
   print                      Print datasets in HDX to the terminal
   quickcharts                Upload QuickChart JSON description to HDX
   showcase                   Upload showcase to HDX
   update                     Update datasets in HDX
@@ -149,13 +150,8 @@
 
 Most tests use mocking in place of HDX, although the `test_integration.py` suite runs against the `stage` server.
 
 New features should be developed against a GitHub issue on a separate branch with a name starting `GH[issue number]_`. `PULL_REQUEST_TEMPLATE.md` should be used in preparing pull requests. Versioning is updated manually in `pyproject.toml` and is described in the template, in brief it is CalVer `YYYY.MM.Micro`.
 
 ## Publication
 
-Publication to PyPI is done using `hatch` which requires the following environment variables:
-
-```
-HATCH_INDEX_USER - set to `__token__`
-HATCH_INDEX_AUTH - API key provided by PyPI
-```
+Publication to PyPI is done automatically when a release is created.
```

### Comparing `hdx_cli_toolkit-2024.4.1/README.md` & `hdx_cli_toolkit-2024.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 ## Overview
 
 This toolkit provides a commandline interface to the [Humanitarian Data Exchange](https://data.humdata.org/) (HDX) to allow for bulk modification operations and other administrative activities such as getting `id` values for users and organization. It is useful for those managing HDX and developers building data pipelines for HDX. The currently supported commands are as follows:
 
 ```
   configuration              Print configuration information to terminal
+  download                   Download dataset resources from HDX
   get_organization_metadata  Get an organization id and other metadata
   get_user_metadata          Get user id and other metadata
   list                       List datasets in HDX
   print                      Print datasets in HDX to the terminal
   quickcharts                Upload QuickChart JSON description to HDX
   showcase                   Upload showcase to HDX
   update                     Update datasets in HDX
@@ -106,13 +107,8 @@
 
 Most tests use mocking in place of HDX, although the `test_integration.py` suite runs against the `stage` server.
 
 New features should be developed against a GitHub issue on a separate branch with a name starting `GH[issue number]_`. `PULL_REQUEST_TEMPLATE.md` should be used in preparing pull requests. Versioning is updated manually in `pyproject.toml` and is described in the template, in brief it is CalVer `YYYY.MM.Micro`.
 
 ## Publication
 
-Publication to PyPI is done using `hatch` which requires the following environment variables:
-
-```
-HATCH_INDEX_USER - set to `__token__`
-HATCH_INDEX_AUTH - API key provided by PyPI
-```
+Publication to PyPI is done automatically when a release is created.
```

### Comparing `hdx_cli_toolkit-2024.4.1/pyproject.toml` & `hdx_cli_toolkit-2024.4.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hdx_cli_toolkit"
-version = "2024.4.1"
+version = "2024.4.2"
 description = "HDX CLI tool kit for commandline interaction with HDX"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 requires-python = ">=3.11"
 authors = [
   {email = "ian.hopkinson@un.org"},
   {name = "Ian Hopkinson"}
```

### Comparing `hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/cli.py` & `hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,16 +418,17 @@
     attributes_file_path: str = "",
 ):
     """Upload showcase to HDX"""
     print_banner("showcase")
     print(f"Adding showcase defined at '{attributes_file_path}'")
     t0 = time.time()
     statuses = add_showcase(showcase_name, hdx_site, attributes_file_path)
-    for status in statuses:
-        print(status, flush=True)
+    if statuses:
+        for status in statuses:
+            print(status, flush=True)
 
     print(f"Showcase update took {time.time() - t0:.2f} seconds")
 
 
 @hdx_toolkit.command(name="update_resource")
 @click.option(
     "--dataset_name",
@@ -479,18 +480,19 @@
         f"Updating/adding '{resource_name}' in '{dataset_name}' "
         f"with file at '{resource_file_path}'"
     )
     t0 = time.time()
     statuses = update_resource_in_hdx(
         dataset_name, resource_name, hdx_site, resource_file_path, live, description=description
     )
-    for status in statuses:
-        print(status, flush=True)
+    if statuses:
+        for status in statuses:
+            print(status, flush=True)
 
-    print(f"Resource update took {time.time() - t0:.2f} seconds")
+        print(f"Resource update took {time.time() - t0:.2f} seconds")
 
 
 @hdx_toolkit.command(name="download")
 @click.option(
     "--dataset",
     is_flag=False,
     default="all",
```

### Comparing `hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/hdx_utilities.py` & `hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/hdx_utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,54 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
 
 import fnmatch
+import functools
 import json
 import os
 import time
 import traceback
 
 from pathlib import Path
 
+import click
 import yaml
 
 from hdx.api.configuration import Configuration, ConfigurationError
 from hdx.data.organization import Organization
 from hdx.data.resource_view import ResourceView
 from hdx.data.hdxobject import HDXError
 from hdx.data.dataset import Dataset
 from hdx.data.showcase import Showcase
 from hdx.data.resource import Resource
 from hdx.data.user import User
 
 from hdx_cli_toolkit.utilities import read_attributes
 
 
+def hdx_error_handler(f):
+    @functools.wraps(f)
+    def inner(*args, **kwargs):
+        try:
+            return f(*args, **kwargs)
+        except HDXError:
+            if "Authorization Error" in traceback.format_exc():
+                click.secho(
+                    "Could not perform operation on HDX because of an authorization error",
+                    fg="red",
+                    color=True,
+                )
+            else:
+                print(traceback.format_exc)
+
+    return inner
+
+
+@hdx_error_handler
 def get_filtered_datasets(
     organization: str = "",
     dataset_filter: str = "*",
     query: str = None,
     hdx_site: str = "stage",
     verbose: bool = True,
 ) -> list[Dataset]:
@@ -78,14 +99,15 @@
             f"({organization['name']})' matching filter conditions:",
             flush=True,
         )
 
     return filtered_datasets
 
 
+@hdx_error_handler
 def update_values_in_hdx(
     filtered_datasets: list[Dataset], key, value, conversion_func, hdx_site: str = "stage"
 ):
     n_changed = 0
     n_failures = 0
     for dataset in filtered_datasets:
         t0 = time.time()
@@ -111,53 +133,49 @@
             )
             print(
                 f"{dataset['name']:<70.70}{old_value:<20.20}{str(dataset[key]):<20.20}"
                 f"{time.time()-t0:0.2f}",
                 flush=True,
             )
         except (HDXError, KeyError):
-            if "Authorization Error" in traceback.format_exc():
-                print(
-                    f"Could not update {dataset['name']} on '{hdx_site}' "
-                    "because of an Authorization Error",
-                    flush=True,
-                )
-            else:
-                print(f"Could not update {dataset['name']} on '{hdx_site}'", flush=True)
+            print(f"Could not update {dataset['name']} on '{hdx_site}'", flush=True)
             n_failures += 1
 
             print(
                 f"{dataset['name']:<70.70}{old_value:<20.20}{old_value:<20.20}"
                 f"{time.time()-t0:0.2f}",
                 flush=True,
             )
 
     return n_changed, n_failures
 
 
+@hdx_error_handler
 def get_organizations_from_hdx(organization: str, hdx_site: str = "stage"):
     configure_hdx_connection(hdx_site)
     filtered_organizations = []
     all_organizations = Organization.get_all_organization_names(include_extras=True)
     for an_organization in all_organizations:
         if fnmatch.fnmatch(an_organization, f"*{organization}*"):
             organization_metadata = Organization.read_from_hdx(an_organization)
             filtered_organizations.append(organization_metadata)
 
     return filtered_organizations
 
 
+@hdx_error_handler
 def get_users_from_hdx(user: str, hdx_site: str = "stage"):
     configure_hdx_connection(hdx_site=hdx_site)
 
     user_list = User.get_all_users(q=user)
 
     return user_list
 
 
+@hdx_error_handler
 def decorate_dataset_with_extras(
     dataset: Dataset, hdx_site: str = "stage", verbose: bool = False
 ) -> dict:
     """A function to add resource, quickcharts (resource_view) and showcases keys to a dataset
     dictionary representation for the print command. fs_check_info and hxl_preview_config are
     converted from JSON objects serialised as single strings to dictionaries to make printed output
     more readable. This decoration means that the dataset dictionary cannot be uploaded to HDX.
@@ -190,14 +208,15 @@
 
     showcases = dataset.get_showcases()
     output_dict["showcases"] = [x.data for x in showcases]
 
     return output_dict
 
 
+@hdx_error_handler
 def add_showcase(showcase_name: str, hdx_site: str, attributes_file_path: str) -> list[str]:
     configure_hdx_connection(hdx_site)
     statuses = []
     showcase_attributes = read_attributes(showcase_name, attributes_filepath=attributes_file_path)
     showcase = Showcase(
         {
             "name": showcase_attributes["name"],
@@ -216,14 +235,15 @@
     dataset = Dataset.read_from_hdx(showcase_attributes["parent_dataset"])
     showcase.add_dataset(dataset)
     statuses.append(f"Added dataset '{dataset['name']}' to showcase '{showcase_name}'")
 
     return statuses
 
 
+@hdx_error_handler
 def update_resource_in_hdx(
     dataset_name: str,
     resource_name: str,
     hdx_site: str,
     resource_file_path: str,
     live: bool,
     description: str = "new resource",
@@ -308,14 +328,15 @@
             statuses.append("Update to HDX successful")
             return statuses
 
     statuses.append("No '--live' flag supplied so no update to HDX made, otherwise successful")
     return statuses
 
 
+@hdx_error_handler
 def add_quickcharts(dataset_name, hdx_site, resource_name, hdx_hxl_preview_file_path):
     configure_hdx_connection(hdx_site=hdx_site)
     status = "Successful"
 
     # read the json file
     with open(hdx_hxl_preview_file_path, "r", encoding="utf-8") as json_file:
         recipe = json.load(json_file)
@@ -344,14 +365,15 @@
     # delete the temp file
     if os.path.exists(temp_yaml_path):
         os.remove(temp_yaml_path)
 
     return status
 
 
+@hdx_error_handler
 def download_hdx_datasets(
     dataset_filter: str,
     resource_filter: str = "*",
     hdx_site: str = "stage",
     download_directory: str = None,
 ):
     configure_hdx_connection(hdx_site=hdx_site)
@@ -377,14 +399,15 @@
                 resource_url, resource_file = resource.download(folder=download_directory)
                 print(f"...from {resource_url}")
                 download_paths.append(resource_file)
 
     return download_paths
 
 
+@hdx_error_handler
 def configure_hdx_connection(hdx_site: str, verbose: bool = True):
     try:
         Configuration.create(
             user_agent_config_yaml=os.path.join(os.path.expanduser("~"), ".useragents.yaml"),
             user_agent_lookup="hdx-cli-toolkit",
             hdx_site=hdx_site,
             hdx_read_only=False,
```

### Comparing `hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit/utilities.py` & `hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit/utilities.py`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/PKG-INFO` & `hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx_cli_toolkit
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: HDX CLI tool kit for commandline interaction with HDX
 Author: Ian Hopkinson
 Author-email: ian.hopkinson@un.org
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Ian Hopkinson
         
@@ -45,14 +45,15 @@
 
 ## Overview
 
 This toolkit provides a commandline interface to the [Humanitarian Data Exchange](https://data.humdata.org/) (HDX) to allow for bulk modification operations and other administrative activities such as getting `id` values for users and organization. It is useful for those managing HDX and developers building data pipelines for HDX. The currently supported commands are as follows:
 
 ```
   configuration              Print configuration information to terminal
+  download                   Download dataset resources from HDX
   get_organization_metadata  Get an organization id and other metadata
   get_user_metadata          Get user id and other metadata
   list                       List datasets in HDX
   print                      Print datasets in HDX to the terminal
   quickcharts                Upload QuickChart JSON description to HDX
   showcase                   Upload showcase to HDX
   update                     Update datasets in HDX
@@ -149,13 +150,8 @@
 
 Most tests use mocking in place of HDX, although the `test_integration.py` suite runs against the `stage` server.
 
 New features should be developed against a GitHub issue on a separate branch with a name starting `GH[issue number]_`. `PULL_REQUEST_TEMPLATE.md` should be used in preparing pull requests. Versioning is updated manually in `pyproject.toml` and is described in the template, in brief it is CalVer `YYYY.MM.Micro`.
 
 ## Publication
 
-Publication to PyPI is done using `hatch` which requires the following environment variables:
-
-```
-HATCH_INDEX_USER - set to `__token__`
-HATCH_INDEX_AUTH - API key provided by PyPI
-```
+Publication to PyPI is done automatically when a release is created.
```

### Comparing `hdx_cli_toolkit-2024.4.1/src/hdx_cli_toolkit.egg-info/SOURCES.txt` & `hdx_cli_toolkit-2024.4.2/src/hdx_cli_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.1/tests/test_cli.py` & `hdx_cli_toolkit-2024.4.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.1/tests/test_hdx_utilities.py` & `hdx_cli_toolkit-2024.4.2/tests/test_hdx_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import os
 from unittest import mock
 from unittest.mock import patch
 
 from hdx_cli_toolkit.hdx_utilities import add_showcase, get_filtered_datasets
 
 
-# @patch("hdx.data.showcase.Showcase")
 @patch("hdx_cli_toolkit.hdx_utilities.Showcase")
 @patch("hdx.data.dataset.Dataset.read_from_hdx")
 def test_add_showcase(mock_hdx, mock_showcase):
     attributes_file_path = os.path.join(os.path.dirname(__file__), "fixtures", "attributes.csv")
     showcase_name = "climada-litpop-showcase"
     mock_showcase().add_tags.return_value = (mock.MagicMock(), mock.MagicMock())
     mock_hdx.return_value = {"name": "mock name"}
```

### Comparing `hdx_cli_toolkit-2024.4.1/tests/test_hdx_utilities_integration.py` & `hdx_cli_toolkit-2024.4.2/tests/test_hdx_utilities_integration.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,26 +6,36 @@
 import json
 import os
 
 import pytest
 
 from hdx.data.dataset import Dataset
 from hdx.data.resource import Resource
+from hdx.data.resource_view import ResourceView
 
-from hdx_cli_toolkit.hdx_utilities import update_resource_in_hdx, configure_hdx_connection
+from hdx_cli_toolkit.hdx_utilities import (
+    update_resource_in_hdx,
+    configure_hdx_connection,
+    update_values_in_hdx,
+    add_showcase,
+    add_quickcharts,
+)
+
+from hdx_cli_toolkit.utilities import make_conversion_func
 
 
 DATASET_NAME = "hdx_cli_toolkit_test"
 TEST_RESOURCE_NAME = "test_resource_1"
+HDX_SITE = "stage"
 
 
-@pytest.fixture(autouse=True)
+@pytest.fixture(scope="module", autouse=True)
 def setup_and_teardown_dataset_in_hdx():
     # This is pytest setup
-    configure_hdx_connection(hdx_site="stage")
+    configure_hdx_connection(hdx_site=HDX_SITE)
     dataset = Dataset.read_from_hdx(DATASET_NAME)
     if dataset:
         dataset.delete_from_hdx()
     title = "HDX CLI toolkit test"
     dataset = Dataset({"name": DATASET_NAME, "title": title})
     dataset.update_from_yaml(
         os.path.join(os.path.dirname(__file__), "fixtures", "hdx_dataset_static.yaml")
@@ -49,35 +59,43 @@
 
     dataset.create_in_hdx(hxl_update=False, updated_by_script="hdx_cli_toolkit_ignore")
 
     assert Dataset.read_from_hdx(DATASET_NAME) is not None
     # This is pytest teardown
     yield
     dataset = Dataset.read_from_hdx(DATASET_NAME)
+
+    showcases = dataset.get_showcases()
+    for showcase in showcases:
+        showcase.delete_from_hdx()
+
     if dataset:
         dataset.delete_from_hdx()
 
 
 def test_update_resource():
     dataset = Dataset.read_from_hdx(DATASET_NAME)
     original_resources = dataset.get_resources()
 
     new_resource_file_path = os.path.join(os.path.dirname(__file__), "fixtures", "test-2.csv")
     statuses = update_resource_in_hdx(
-        DATASET_NAME, TEST_RESOURCE_NAME, "stage", new_resource_file_path, live=True
+        DATASET_NAME, TEST_RESOURCE_NAME, HDX_SITE, new_resource_file_path, live=True
     )
 
     for status in statuses:
         print(status, flush=True)
 
     assert len(statuses) == 5
 
     revised_dataset = Dataset.read_from_hdx(DATASET_NAME)
     revised_resources = revised_dataset.get_resources()
 
+    for revised_ in revised_resources:
+        print(revised_["name"], revised_["url"], flush=True)
+
     assert len(original_resources) == len(revised_resources)
     assert original_resources[0].data["name"] == "test_resource_1"
     assert revised_resources[0].data["name"] == "test_resource_1"
 
     assert original_resources[0].data["url"].endswith("test.csv")
     assert revised_resources[0].data["url"].endswith("test-2.csv")
 
@@ -85,32 +103,100 @@
 
 
 def test_add_resource():
     dataset = Dataset.read_from_hdx(DATASET_NAME)
     original_resources = dataset.get_resources()
     new_resource_name = "inserted_resource"
 
-    new_resource_file_path = os.path.join(os.path.dirname(__file__), "fixtures", "test-2.csv")
+    new_resource_file_path = os.path.join(os.path.dirname(__file__), "fixtures", "test-3.csv")
     statuses = update_resource_in_hdx(
-        DATASET_NAME, new_resource_name, "stage", new_resource_file_path, live=True
+        DATASET_NAME, new_resource_name, HDX_SITE, new_resource_file_path, live=True
     )
 
     for status in statuses:
         print(status, flush=True)
 
     assert len(statuses) == 5
 
     revised_dataset = Dataset.read_from_hdx(DATASET_NAME)
     revised_resources = revised_dataset.get_resources()
     for revised_ in revised_resources:
-        print(revised_["name"], flush=True)
+        print(revised_["name"], revised_["url"], flush=True)
 
     assert len(original_resources) == 1
     assert len(revised_resources) == 2
 
     assert revised_resources[0].data["name"] == "inserted_resource"
     assert revised_resources[1].data["name"] == "test_resource_1"
 
-    assert revised_resources[0].data["url"].endswith("test-2.csv")
-    assert revised_resources[1].data["url"].endswith("test.csv")
+    assert revised_resources[0].data["url"].endswith("test-3.csv")
 
-    assert revised_resources[0].data["size"] > original_resources[0].data["size"]
+
+def test_update_key():
+    dataset = Dataset.read_from_hdx(DATASET_NAME)
+    key = "notes"
+    value = "new notes"
+    conversion_func, _ = make_conversion_func(value)
+    n_changed, n_failures = update_values_in_hdx(
+        [dataset], key, value, conversion_func, hdx_site=HDX_SITE
+    )
+
+    assert n_changed == 1
+    assert n_failures == 0
+    dataset = Dataset.read_from_hdx(DATASET_NAME)
+
+    assert dataset["notes"] == "new notes"
+
+
+def test_add_showcase():
+    attributes_file_path = os.path.join(os.path.dirname(__file__), "fixtures", "attributes.csv")
+    showcase_name = "climada-litpop-showcase"
+
+    statuses = add_showcase(showcase_name, HDX_SITE, attributes_file_path)
+
+    assert statuses == [
+        "3 of 3 showcase tags added",
+        "Added dataset 'hdx_cli_toolkit_test' to showcase 'climada-litpop-showcase'",
+    ]
+
+    dataset = Dataset.read_from_hdx(DATASET_NAME)
+    showcases = dataset.get_showcases()
+
+    assert len(showcases) == 1
+    assert showcases[0]["title"] == "CLIMADA LitPop Methodology Documentation"
+
+
+def test_add_quickcharts():
+    resource_name = "admin1-summaries-flood.csv"
+    new_resource_file_path = os.path.join(os.path.dirname(__file__), "fixtures", resource_name)
+    _ = update_resource_in_hdx(
+        DATASET_NAME, resource_name, HDX_SITE, new_resource_file_path, live=True
+    )
+
+    hdx_hxl_preview_file_path = os.path.join(
+        os.path.dirname(__file__), "fixtures", "quickchart-flood.json"
+    )
+
+    status = add_quickcharts(DATASET_NAME, HDX_SITE, resource_name, hdx_hxl_preview_file_path)
+
+    assert status == "Successful"
+
+    dataset = Dataset.read_from_hdx(DATASET_NAME)
+    resources = dataset.get_resources()
+
+    quickchart_dicts = []
+    for resource in resources:
+        resource_dict = resource.data
+        if resource_dict["name"] != resource_name:
+            continue
+        dataset_quickcharts = ResourceView.get_all_for_resource(resource_dict["id"])
+        if dataset_quickcharts is not None:
+            for quickchart in dataset_quickcharts:
+                quickchart_dict = quickchart.data
+                if "hxl_preview_config" in quickchart_dict:
+                    quickchart_dict["hxl_preview_config"] = json.loads(
+                        quickchart_dict["hxl_preview_config"]
+                    )
+                quickchart_dicts.append(quickchart_dict)
+
+    assert len(quickchart_dicts) == 2
+    assert quickchart_dicts[1]["title"] == "Quick Charts"
```

