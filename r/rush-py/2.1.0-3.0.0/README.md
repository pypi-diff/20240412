# Comparing `tmp/rush_py-2.1.0.tar.gz` & `tmp/rush_py-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rush_py-2.1.0.tar", max compression
+gzip compressed data, was "rush_py-3.0.0.tar", max compression
```

## Comparing `rush_py-2.1.0.tar` & `rush_py-3.0.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0     8526 2024-03-25 07:43:11.116074 rush_py-2.1.0/README.md
--rw-r--r--   0        0        0     2603 2024-03-25 07:48:58.360211 rush_py-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      481 2024-03-25 07:43:11.134075 rush_py-2.1.0/rush/__init__.py
--rw-r--r--   0        0        0     1130 2024-03-25 07:43:11.134075 rush_py-2.1.0/rush/async_utils.py
--rw-r--r--   0        0        0       23 2024-01-29 10:45:57.136914 rush_py-2.1.0/rush/data.py
--rw-r--r--   0        0        0     1326 2024-03-25 07:43:11.134075 rush_py-2.1.0/rush/doc.py
--rw-r--r--   0        0        0    12547 2024-02-29 02:25:15.935543 rush_py-2.1.0/rush/graphql_client/__init__.py
--rw-r--r--   0        0        0      240 2024-02-28 07:01:47.469725 rush_py-2.1.0/rush/graphql_client/argument.py
--rw-r--r--   0        0        0      852 2024-02-28 07:01:47.474725 rush_py-2.1.0/rush/graphql_client/arguments.py
--rw-r--r--   0        0        0    12272 2024-02-28 07:02:11.731827 rush_py-2.1.0/rush/graphql_client/async_base_client.py
--rw-r--r--   0        0        0      620 2024-02-28 07:01:47.684735 rush_py-2.1.0/rush/graphql_client/base_model.py
--rw-r--r--   0        0        0      174 2024-02-28 07:01:47.452724 rush_py-2.1.0/rush/graphql_client/cancel_module_instance.py
--rw-r--r--   0        0        0    43228 2024-02-29 02:25:15.935543 rush_py-2.1.0/rush/graphql_client/client.py
--rw-r--r--   0        0        0      253 2024-02-28 07:01:47.459725 rush_py-2.1.0/rush/graphql_client/create_entity.py
--rw-r--r--   0        0        0      277 2024-02-28 07:01:47.461725 rush_py-2.1.0/rush/graphql_client/create_experiment.py
--rw-r--r--   0        0        0      259 2024-02-28 07:01:47.463725 rush_py-2.1.0/rush/graphql_client/create_project.py
--rw-r--r--   0        0        0      259 2024-02-28 07:01:47.467725 rush_py-2.1.0/rush/graphql_client/create_protein.py
--rw-r--r--   0        0        0      314 2024-02-28 07:01:47.465725 rush_py-2.1.0/rush/graphql_client/create_protein_conformer.py
--rw-r--r--   0        0        0      241 2024-02-28 07:01:47.566729 rush_py-2.1.0/rush/graphql_client/create_smol.py
--rw-r--r--   0        0        0      296 2024-02-28 07:01:47.564729 rush_py-2.1.0/rush/graphql_client/create_smol_conformer.py
--rw-r--r--   0        0        0      290 2024-02-28 07:01:47.568729 rush_py-2.1.0/rush/graphql_client/create_smol_tautomer.py
--rw-r--r--   0        0        0      271 2024-02-28 07:01:47.570730 rush_py-2.1.0/rush/graphql_client/create_structure.py
--rw-r--r--   0        0        0      302 2024-02-28 07:01:47.454724 rush_py-2.1.0/rush/graphql_client/delete_module_instance.py
--rw-r--r--   0        0        0      230 2024-02-28 07:01:47.457724 rush_py-2.1.0/rush/graphql_client/deploy.py
--rw-r--r--   0        0        0      510 2024-02-28 07:01:47.506727 rush_py-2.1.0/rush/graphql_client/entity.py
--rw-r--r--   0        0        0     3140 2024-02-29 02:25:15.935543 rush_py-2.1.0/rush/graphql_client/enums.py
--rw-r--r--   0        0        0     2411 2024-02-28 07:01:47.683735 rush_py-2.1.0/rush/graphql_client/exceptions.py
--rw-r--r--   0        0        0      679 2024-02-28 07:01:47.557729 rush_py-2.1.0/rush/graphql_client/experiment.py
--rw-r--r--   0        0        0     5584 2024-02-29 02:25:15.935543 rush_py-2.1.0/rush/graphql_client/fragments.py
--rw-r--r--   0        0        0    12695 2024-02-29 02:25:15.936543 rush_py-2.1.0/rush/graphql_client/input_types.py
--rw-r--r--   0        0        0      702 2024-02-28 07:01:47.478726 rush_py-2.1.0/rush/graphql_client/latest_modules.py
--rw-r--r--   0        0        0     1670 2024-02-28 07:02:11.599821 rush_py-2.1.0/rush/graphql_client/module_instance_details.py
--rw-r--r--   0        0        0     4300 2024-01-29 10:45:57.143915 rush_py-2.1.0/rush/graphql_client/module_instance_full.py
--rw-r--r--   0        0        0      314 2024-02-28 07:01:47.497726 rush_py-2.1.0/rush/graphql_client/module_instance_minimal.py
--rw-r--r--   0        0        0      403 2024-01-29 10:45:57.144914 rush_py-2.1.0/rush/graphql_client/module_instance_status.py
--rw-r--r--   0        0        0     1009 2024-02-28 07:02:11.593821 rush_py-2.1.0/rush/graphql_client/module_instances.py
--rw-r--r--   0        0        0     2804 2024-01-29 10:45:57.145915 rush_py-2.1.0/rush/graphql_client/module_instances_full.py
--rw-r--r--   0        0        0      593 2024-02-28 07:01:47.482726 rush_py-2.1.0/rush/graphql_client/modules.py
--rw-r--r--   0        0        0      160 2024-02-13 05:21:55.039019 rush_py-2.1.0/rush/graphql_client/object.py
--rw-r--r--   0        0        0      266 2024-02-28 07:01:47.502727 rush_py-2.1.0/rush/graphql_client/object_contents.py
--rw-r--r--   0        0        0      241 2024-02-28 07:01:47.499726 rush_py-2.1.0/rush/graphql_client/object_url.py
--rw-r--r--   0        0        0     2121 2024-02-28 07:01:47.518727 rush_py-2.1.0/rush/graphql_client/project.py
--rw-r--r--   0        0        0      604 2024-02-28 07:01:47.523728 rush_py-2.1.0/rush/graphql_client/protein.py
--rw-r--r--   0        0        0      687 2024-02-28 07:01:47.528728 rush_py-2.1.0/rush/graphql_client/protein_conformer.py
--rw-r--r--   0        0        0      210 2024-02-28 07:01:47.559729 rush_py-2.1.0/rush/graphql_client/retry.py
--rw-r--r--   0        0        0      295 2024-02-28 07:01:47.562729 rush_py-2.1.0/rush/graphql_client/run.py
--rw-r--r--   0        0        0      571 2024-02-28 07:01:47.533728 rush_py-2.1.0/rush/graphql_client/smol.py
--rw-r--r--   0        0        0      657 2024-02-28 07:01:47.537728 rush_py-2.1.0/rush/graphql_client/smol_conformer.py
--rw-r--r--   0        0        0      662 2024-02-28 07:01:47.543728 rush_py-2.1.0/rush/graphql_client/smol_tautomer.py
--rw-r--r--   0        0        0     1139 2024-02-28 07:01:47.551729 rush_py-2.1.0/rush/graphql_client/structure.py
--rw-r--r--   0        0        0      161 2024-02-28 07:01:47.572730 rush_py-2.1.0/rush/graphql_client/tag.py
--rw-r--r--   0        0        0      346 2024-02-28 07:01:47.574730 rush_py-2.1.0/rush/graphql_client/track_utilization.py
--rw-r--r--   0        0        0      165 2024-02-28 07:01:47.575730 rush_py-2.1.0/rush/graphql_client/untag.py
--rw-r--r--   0        0        0      375 2024-02-28 07:01:47.578730 rush_py-2.1.0/rush/graphql_client/update_module_instance.py
--rw-r--r--   0        0        0      328 2024-01-29 10:45:57.148915 rush_py-2.1.0/rush/graphql_client/upload.py
--rw-r--r--   0        0        0      293 2024-02-28 07:01:47.580730 rush_py-2.1.0/rush/graphql_client/upload_arg.py
--rw-r--r--   0        0        0     1226 2024-03-25 07:43:11.134075 rush_py-2.1.0/rush/legacy_types.py
--rw-r--r--   0        0        0     7403 2024-02-16 09:06:54.345722 rush_py-2.1.0/rush/local.py
--rw-r--r--   0        0        0     5733 2024-02-16 09:06:54.345722 rush_py-2.1.0/rush/protocols.py
--rw-r--r--   0        0        0    64238 2024-03-25 07:43:11.135075 rush_py-2.1.0/rush/provider.py
--rw-r--r--   0        0        0       98 2024-02-16 09:06:54.345722 rush_py-2.1.0/rush/tests/test_provider.py
--rw-r--r--   0        0        0     1070 2024-02-01 03:43:42.619708 rush_py-2.1.0/rush/tests/test_typedef.py
--rw-r--r--   0        0        0     9688 2024-03-25 07:43:11.135075 rush_py-2.1.0/rush/typedef.py
--rw-r--r--   0        0        0      747 2024-03-25 07:43:11.135075 rush_py-2.1.0/rush/types.py
--rw-r--r--   0        0        0     9320 1970-01-01 00:00:00.000000 rush_py-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     9914 2024-04-12 09:38:51.148131 rush_py-3.0.0/README.md
+-rw-r--r--   0        0        0     2718 2024-04-12 08:49:08.158655 rush_py-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      481 2024-03-25 07:43:11.134075 rush_py-3.0.0/rush/__init__.py
+-rw-r--r--   0        0        0     1569 2024-04-12 08:48:59.531260 rush_py-3.0.0/rush/async_utils.py
+-rw-r--r--   0        0        0       23 2024-01-29 10:45:57.136914 rush_py-3.0.0/rush/data.py
+-rw-r--r--   0        0        0     1326 2024-03-25 07:43:11.134075 rush_py-3.0.0/rush/doc.py
+-rw-r--r--   0        0        0     7663 2024-04-12 08:48:59.531260 rush_py-3.0.0/rush/graphql_client/__init__.py
+-rw-r--r--   0        0        0      267 2024-04-12 08:48:59.531260 rush_py-3.0.0/rush/graphql_client/argument.py
+-rw-r--r--   0        0        0     1036 2024-04-12 08:48:59.532260 rush_py-3.0.0/rush/graphql_client/arguments.py
+-rw-r--r--   0        0        0    12272 2024-04-07 11:13:59.841910 rush_py-3.0.0/rush/graphql_client/async_base_client.py
+-rw-r--r--   0        0        0      620 2024-04-07 11:51:36.271482 rush_py-3.0.0/rush/graphql_client/base_model.py
+-rw-r--r--   0        0        0      174 2024-04-07 11:13:28.065432 rush_py-3.0.0/rush/graphql_client/cancel_module_instance.py
+-rw-r--r--   0        0        0    28860 2024-04-12 08:48:59.532260 rush_py-3.0.0/rush/graphql_client/client.py
+-rw-r--r--   0        0        0      253 2024-02-28 07:01:47.459725 rush_py-3.0.0/rush/graphql_client/create_entity.py
+-rw-r--r--   0        0        0      277 2024-02-28 07:01:47.461725 rush_py-3.0.0/rush/graphql_client/create_experiment.py
+-rw-r--r--   0        0        0      259 2024-02-28 07:01:47.463725 rush_py-3.0.0/rush/graphql_client/create_project.py
+-rw-r--r--   0        0        0      259 2024-02-28 07:01:47.467725 rush_py-3.0.0/rush/graphql_client/create_protein.py
+-rw-r--r--   0        0        0      314 2024-02-28 07:01:47.465725 rush_py-3.0.0/rush/graphql_client/create_protein_conformer.py
+-rw-r--r--   0        0        0      241 2024-02-28 07:01:47.566729 rush_py-3.0.0/rush/graphql_client/create_smol.py
+-rw-r--r--   0        0        0      296 2024-02-28 07:01:47.564729 rush_py-3.0.0/rush/graphql_client/create_smol_conformer.py
+-rw-r--r--   0        0        0      290 2024-02-28 07:01:47.568729 rush_py-3.0.0/rush/graphql_client/create_smol_tautomer.py
+-rw-r--r--   0        0        0      271 2024-02-28 07:01:47.570730 rush_py-3.0.0/rush/graphql_client/create_structure.py
+-rw-r--r--   0        0        0      341 2024-04-12 08:48:59.532260 rush_py-3.0.0/rush/graphql_client/delete_module_instance.py
+-rw-r--r--   0        0        0      255 2024-04-12 08:48:59.533260 rush_py-3.0.0/rush/graphql_client/deploy.py
+-rw-r--r--   0        0        0      510 2024-02-28 07:01:47.506727 rush_py-3.0.0/rush/graphql_client/entity.py
+-rw-r--r--   0        0        0     1491 2024-04-12 08:48:59.533260 rush_py-3.0.0/rush/graphql_client/enums.py
+-rw-r--r--   0        0        0     2411 2024-04-07 11:13:28.519453 rush_py-3.0.0/rush/graphql_client/exceptions.py
+-rw-r--r--   0        0        0      679 2024-02-28 07:01:47.557729 rush_py-3.0.0/rush/graphql_client/experiment.py
+-rw-r--r--   0        0        0     3769 2024-04-12 08:48:59.533260 rush_py-3.0.0/rush/graphql_client/fragments.py
+-rw-r--r--   0        0        0     5332 2024-04-12 08:48:59.533260 rush_py-3.0.0/rush/graphql_client/input_types.py
+-rw-r--r--   0        0        0      825 2024-04-12 08:48:59.534260 rush_py-3.0.0/rush/graphql_client/latest_modules.py
+-rw-r--r--   0        0        0     2004 2024-04-12 08:48:59.534260 rush_py-3.0.0/rush/graphql_client/module_instance_details.py
+-rw-r--r--   0        0        0     4300 2024-01-29 10:45:57.143915 rush_py-3.0.0/rush/graphql_client/module_instance_full.py
+-rw-r--r--   0        0        0      354 2024-04-12 08:48:59.534260 rush_py-3.0.0/rush/graphql_client/module_instance_minimal.py
+-rw-r--r--   0        0        0      403 2024-01-29 10:45:57.144914 rush_py-3.0.0/rush/graphql_client/module_instance_status.py
+-rw-r--r--   0        0        0     3104 2024-04-12 08:48:59.534260 rush_py-3.0.0/rush/graphql_client/module_instances.py
+-rw-r--r--   0        0        0     2804 2024-01-29 10:45:57.145915 rush_py-3.0.0/rush/graphql_client/module_instances_full.py
+-rw-r--r--   0        0        0      686 2024-04-12 08:48:59.534260 rush_py-3.0.0/rush/graphql_client/modules.py
+-rw-r--r--   0        0        0      160 2024-02-13 05:21:55.039019 rush_py-3.0.0/rush/graphql_client/object.py
+-rw-r--r--   0        0        0      292 2024-04-12 08:48:59.535260 rush_py-3.0.0/rush/graphql_client/object_contents.py
+-rw-r--r--   0        0        0      243 2024-04-12 08:48:59.535260 rush_py-3.0.0/rush/graphql_client/object_url.py
+-rw-r--r--   0        0        0     2121 2024-02-28 07:01:47.518727 rush_py-3.0.0/rush/graphql_client/project.py
+-rw-r--r--   0        0        0      604 2024-02-28 07:01:47.523728 rush_py-3.0.0/rush/graphql_client/protein.py
+-rw-r--r--   0        0        0      687 2024-02-28 07:01:47.528728 rush_py-3.0.0/rush/graphql_client/protein_conformer.py
+-rw-r--r--   0        0        0      234 2024-04-12 08:48:59.535260 rush_py-3.0.0/rush/graphql_client/retry.py
+-rw-r--r--   0        0        0      340 2024-04-12 08:48:59.535260 rush_py-3.0.0/rush/graphql_client/run.py
+-rw-r--r--   0        0        0      571 2024-02-28 07:01:47.533728 rush_py-3.0.0/rush/graphql_client/smol.py
+-rw-r--r--   0        0        0      657 2024-02-28 07:01:47.537728 rush_py-3.0.0/rush/graphql_client/smol_conformer.py
+-rw-r--r--   0        0        0      662 2024-02-28 07:01:47.543728 rush_py-3.0.0/rush/graphql_client/smol_tautomer.py
+-rw-r--r--   0        0        0     1139 2024-02-28 07:01:47.551729 rush_py-3.0.0/rush/graphql_client/structure.py
+-rw-r--r--   0        0        0      161 2024-04-07 11:13:28.358446 rush_py-3.0.0/rush/graphql_client/tag.py
+-rw-r--r--   0        0        0      381 2024-04-12 08:48:59.535260 rush_py-3.0.0/rush/graphql_client/track_utilization.py
+-rw-r--r--   0        0        0      165 2024-04-07 11:13:28.369446 rush_py-3.0.0/rush/graphql_client/untag.py
+-rw-r--r--   0        0        0      414 2024-04-12 08:48:59.536260 rush_py-3.0.0/rush/graphql_client/update_module_instance.py
+-rw-r--r--   0        0        0      328 2024-01-29 10:45:57.148915 rush_py-3.0.0/rush/graphql_client/upload.py
+-rw-r--r--   0        0        0      321 2024-04-12 08:48:59.536260 rush_py-3.0.0/rush/graphql_client/upload_arg.py
+-rw-r--r--   0        0        0      506 2024-04-12 08:48:59.536260 rush_py-3.0.0/rush/graphql_client/upload_object.py
+-rw-r--r--   0        0        0     1226 2024-03-25 07:43:11.134075 rush_py-3.0.0/rush/legacy_types.py
+-rw-r--r--   0        0        0     7403 2024-02-16 09:06:54.345722 rush_py-3.0.0/rush/local.py
+-rw-r--r--   0        0        0     5733 2024-02-16 09:06:54.345722 rush_py-3.0.0/rush/protocols.py
+-rw-r--r--   0        0        0    65171 2024-04-12 08:48:59.536260 rush_py-3.0.0/rush/provider.py
+-rw-r--r--   0        0        0       98 2024-02-16 09:06:54.345722 rush_py-3.0.0/rush/tests/test_provider.py
+-rw-r--r--   0        0        0     1070 2024-02-01 03:43:42.619708 rush_py-3.0.0/rush/tests/test_typedef.py
+-rw-r--r--   0        0        0    10193 2024-04-12 08:48:59.536260 rush_py-3.0.0/rush/typedef.py
+-rw-r--r--   0        0        0      747 2024-04-07 11:51:36.271482 rush_py-3.0.0/rush/types.py
+-rw-r--r--   0        0        0    10796 1970-01-01 00:00:00.000000 rush_py-3.0.0/PKG-INFO
```

### Comparing `rush_py-2.1.0/README.md` & `rush_py-3.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -33,25 +33,28 @@
 os.environ["RUSH_TOKEN"] = YOUR_TOKEN
 
 # 1.3 Build your client
 client = rush.build_blocking_provider_with_functions()
 
 # 2.1 Prepare the protein
 prepared_protein_qdxf, prepared_protein_pdb = client.prepare_protein(
-    Path("1B39_A_nohet.pdb"), tags=["example_prep"]
+    Path("1B39_A_nohet.pdb"), None, None, tags=["example_prep"]
 )
 
 # 2.3 Return run values
 print(prepared_protein_qdxf.download(overwrite=True).open().read()[0:50], "...")
 ```
 
-    2024-03-21 14:31:29,560 - rush - INFO - Restoring by default via env
-    2024-03-21 14:31:30,540 - rush - INFO - Trying to restore job with tags: ['example_prep'] and path: github:talo/prepare_protein/947cdbc000031e192153a20a9b4a8fbb12279102#prepare_protein_tengu
-    2024-03-21 14:31:30,586 - rush - INFO - Restoring job from previous run with id ea02e2b4-06b1-4576-a1f9-0ecec22e537b
-    [{"amino_acid_insertion_codes": ["", "", "", "", " ...
+    2024-04-08 17:12:28,141 - rush - INFO - Not restoring by default via default
+    2024-04-08 17:12:29,451 - rush - INFO - Argument 10ef4d21-fac5-4962-973b-cf0f6e26d964 is now ModuleInstanceStatus.RESOLVING
+    2024-04-08 17:12:40,388 - rush - INFO - Argument 10ef4d21-fac5-4962-973b-cf0f6e26d964 is now ModuleInstanceStatus.ADMITTED
+    2024-04-08 17:12:44,734 - rush - INFO - Argument 10ef4d21-fac5-4962-973b-cf0f6e26d964 is now ModuleInstanceStatus.DISPATCHED
+    2024-04-08 17:12:45,825 - rush - INFO - Argument 10ef4d21-fac5-4962-973b-cf0f6e26d964 is now ModuleInstanceStatus.RUNNING
+    2024-04-08 17:12:59,570 - rush - INFO - Argument 10ef4d21-fac5-4962-973b-cf0f6e26d964 is now ModuleInstanceStatus.AWAITING_UPLOAD
+    [{"topology": {"version": "V1", "symbols": ["N", " ...
 
 # 1) Setup
 
 This is where we prepare the rush client, directories, and input data
 we’ll be working with.
 
 ## 1.0) Imports
@@ -112,15 +115,15 @@
 
 ``` python
 # By using the `build_provider_with_functions` method,
 # we will also build helper functions calling each module
 client = rush.build_blocking_provider_with_functions(batch_tags=TAGS)
 ```
 
-    2024-03-21 14:31:32,815 - rush - INFO - Restoring by default via env
+    2024-04-08 17:13:26,467 - rush - INFO - Not restoring by default via default
 
 ## 1.4) Input selection
 
 Fetch a pdb from RCSB, stripping hetatoms and selecting a single chain
 to pass as input to the modules:
 
 ``` python
@@ -147,75 +150,88 @@
 ``` python
 # we can check the arguments and outputs for prepare_protein with help()
 help(client.prepare_protein)
 ```
 
     Help on function prepare_protein in module rush.provider:
 
-    prepare_protein(*args: *tuple[RushObject[bytes]], target: 'Target | None' = None, resources: 'Resources | None' = None, tags: 'list[str] | None' = None, restore: 'bool | None' = None) -> tuple[RushObject[list[Record]], RushObject[bytes]]
+    prepare_protein(*args: *tuple[RushObject[bytes], Optional[float], Optional[EnumValue]], target: 'Target | None' = None, resources: 'Resources | None' = None, tags: 'list[str] | None' = None, restore: 'bool | None' = None) -> tuple[RushObject[list[Record]], RushObject[bytes]]
         Prepare a PDB for downstream tasks: protonate, fill missing atoms, etc.
 
         Module version:
-        `github:talo/prepare_protein/947cdbc000031e192153a20a9b4a8fbb12279102#prepare_protein_tengu`
+        `github:talo/prepare_protein/fbeca1ad893cd763b00dc275c43806c0edce03de#prepare_protein_tengu`
 
         QDX Type Description:
 
-            input_pdb: Object[@$Bytes]
+            input_pdb: Object[@$PDB];
+            ph: f32?;
+            naming_scheme: NamingScheme[Amber | Charmm]?
             ->
             output_qdxf: Object[[Conformer]];
-            output_pdb: Object[@$Bytes]
+            output_pdb: Object[@$PDB]
 
 
         :param input_pdb: An input protein as a file; one PDB file
+        :param ph: The ph for determining protonation states; 0-14
+        :param naming_scheme: \
+                        The force field naming scheme to use; \
+                        options are "amber" or "charmm"; \
+                        None produces RCSB/IUPAC standard naming\
+
         :return output_qdxf: An output protein a vec: one qdxf per model in pdb
         :return output_pdb: An output protein as a file: one PDB file
 
 ``` python
 # Here we run the function, it will return a Provider.Arg which you can use to
 # fetch the results
 # We set restore = True so that we can restore a previous run to the same path
 # with the same tags
 prepared_protein_qdxf, prepared_protein_pdb = client.prepare_protein(
-    PROTEIN_PDB_PATH,
+    PROTEIN_PDB_PATH, None, None
 )
 # This initially only has the id of your result; we will show how to fetch the
 # actual value later
 prepared_protein_qdxf
 ```
 
-    2024-03-21 14:31:36,354 - rush - INFO - Trying to restore job with tags: ['qdx', 'rush-py-quickstart', '1B39'] and path: github:talo/prepare_protein/947cdbc000031e192153a20a9b4a8fbb12279102#prepare_protein_tengu
-    2024-03-21 14:31:36,400 - rush - INFO - Restoring job from previous run with id d746634a-8fe8-437d-b468-4bb66f5f4a12
+    2024-04-08 17:13:29,649 - rush - INFO - Trying to restore job with tags: ['qdx', 'rush-py-quickstart', '1B39'] and path: github:talo/prepare_protein/fbeca1ad893cd763b00dc275c43806c0edce03de#prepare_protein_tengu
 
-    Arg(id=127ac5f6-1227-49f4-ad2b-45a08e6c64ca, value=None)
+    Arg(id=37deb248-97fe-443d-b243-36ba172ca7be, value=None)
 
 ## 2.1) Run statuses
 
 This will show the status of all of your runs. You can also view run
 statuses on the [Rush UI](https://rush.qdx.co/dashboard/jobs).
 
 ``` python
 client.status()
 ```
 
-    {}
+    {'8e8357a0-3c37-4c23-bf98-567db98d74df': (<ModuleInstanceStatus.RESOLVING: 'RESOLVING'>,
+      'prepare_protein',
+      1)}
 
 ## 2.2) Run Values
 
 This will return the “value” of the output from the function—for files
 you will recieve a url that you can download, otherwise you will recieve
 them as python types:
 
 ``` python
 protein_qdxf_info = prepared_protein_qdxf.get()
 protein_qdxf_info
 ```
 
-    Blocking get
+    2024-04-08 17:13:29,921 - rush - INFO - Argument 37deb248-97fe-443d-b243-36ba172ca7be is now ModuleInstanceStatus.RESOLVING
+    2024-04-08 17:13:36,501 - rush - INFO - Argument 37deb248-97fe-443d-b243-36ba172ca7be is now ModuleInstanceStatus.ADMITTED
+    2024-04-08 17:13:40,894 - rush - INFO - Argument 37deb248-97fe-443d-b243-36ba172ca7be is now ModuleInstanceStatus.DISPATCHED
+    2024-04-08 17:13:43,225 - rush - INFO - Argument 37deb248-97fe-443d-b243-36ba172ca7be is now ModuleInstanceStatus.RUNNING
+    2024-04-08 17:13:55,523 - rush - INFO - Argument 37deb248-97fe-443d-b243-36ba172ca7be is now ModuleInstanceStatus.AWAITING_UPLOAD
 
-    'https://storage.googleapis.com/rush_store_default/af08031b-e871-45e2-a226-e8c7e1fd5719?x-goog-signature=0864503418ee439f8b34e2461b06c15c4e83be22a72b7acd977ed41c02da00915c749bd4f9145b4cec3553fed283ffee660f20b6f418df99ad4bad1c34f8edcdd1e337da2021ef8e0bfae9c8a7bc0b85729c605765e9512a2623f3dacdcaf079bf416a946881873a87f7fc17e3b54fe8651837aa2b47208ac9b9b42d5d8854d2214e2c7002f89d8b82a0ab3317da32aa5030a48590eda2e870bf23388ad4a77ce4a9c1602a1790248439ea8ceac3291824978332266fc39d548822b2f1dc93eb1ddbbcd326c312feac5bb24345cf0d4193657ea1d1e3bec3cb07fc858b924108aaea74415e12c861a355335ea8bc6507834bf42395d9e52c75846986b395ddd3&x-goog-algorithm=GOOG4-RSA-SHA256&x-goog-credential=qdx-store-user%40humming-bird-321603.iam.gserviceaccount.com%2F20240321%2Fasia-southeast1%2Fstorage%2Fgoog4_request&x-goog-date=20240321T063139Z&x-goog-expires=3600&x-goog-signedheaders=host'
+    'https://storage.googleapis.com/qdx-store/4a4271de-5e14-4756-b115-9c034d7ab294?x-goog-signature=202cb9f86a4351fc30780d26713b4478012548544ff30ba6700f349ad1fcc63137dfb1d2db92fc9d39bc51ba9881c44b27e89e0781aec23d034ec61c4efe2c806b8d784d124863a37d16ce0df02880e272aa0d0dc8f6be23f7214f207183337eb80c9dd0d70757e2761d8f366eea997d066761fadd9ed33483aa8ec98e7fb00e62a78501fdbc2e1e3b9eb4f9e2374a68972937bcae562d114a7e705ca645cd7eb80e5df835c9e462aa34601c8e14691ad6bcbfafef751a7562d8ea3640e77e79f2bd2f6f3b2533df462e245fc4991729f44bee6aa7d9de31cb8a14615b37ba7950c40af54f5a9f146a1a1fb91b2a9f6692d1bca60a8fb2cecd98c2b33fdbd558&x-goog-algorithm=GOOG4-RSA-SHA256&x-goog-credential=qdx-store-user%40humming-bird-321603.iam.gserviceaccount.com%2F20240408%2Fasia-southeast1%2Fstorage%2Fgoog4_request&x-goog-date=20240408T091417Z&x-goog-expires=3600&x-goog-signedheaders=host'
 
 ## 2.3) Downloads
 
 We provide a utility to download files into your workspace, you can
 either provide a filename, which will be saved in
 `workspace/objects/[filename]`, or you can provide your own filepath
 which the client will use as-is:
@@ -241,9 +257,9 @@
 
 ``` python
 # we can read our prepared protein pdb like this
 with open(client.workspace / "objects" / "01_prepared_protein.pdb", "r") as f:
     print(f.readline(), "...")
 ```
 
-    REMARK   1 CREATED WITH OPENMM 8.0, 2024-02-29
+    REMARK   1 CREATED WITH OPENMM 8.0, 2024-04-08
      ...
```

### Comparing `rush_py-2.1.0/pyproject.toml` & `rush_py-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rush-py"
-version = "2.1.0"
+version = "3.0.0"
 description = "Python SDK for interacting with the QDX Rush API and modules"
 authors = ["Ryan Swart <ryan.swart@qdx.co>", "Sean Laguna <sean.laguna@qdx.co>"]
 readme = "README.md"
 packages = [{include = "rush"}]
 documentation = "https://talo.github.io/rush-py"
 homepage = "https://rush.qdx.co"
 
@@ -14,17 +14,19 @@
 [tool.poetry.dependencies]
 python = "^3.9,<3.13"
 httpx = "^0.26.0"
 pdb-tools = "^2.5.0"
 pydantic = "^2.6.0"
 typing-extensions = "^4.9.0"
 websockets = "^12"
+aiofiles = "^23.2.1"
+nest-asyncio = "^1.6.0"
 
 [tool.poetry.group.dev.dependencies]
-ariadne-codegen = "0.12.0"
+ariadne-codegen = "0.13.0"
 black = {extras = ["jupyter"], version = "~=23.9.1"}
 flake8 = "~=6.1.0"
 isort = "~=5.12.0"
 jupyter-contrib-nbextensions = "^0.7.0"
 jupyterlab = "^4.0.6"
 nbdev = "^2.3.12"
 notebook = "^7.0.7"
@@ -106,7 +108,10 @@
 type = "uuid.UUID"
 
 [tool.ariadne-codegen.scalars.ModuleId]
 type = "uuid.UUID"
 
 [tool.ariadne-codegen.scalars.ModuleInstanceId]
 type = "uuid.UUID"
+
+[tool.ariadne-codegen.scalars.ObjectDescriptorId]
+type = "uuid.UUID"
```

### Comparing `rush_py-2.1.0/rush/async_utils.py` & `rush_py-3.0.0/rush/async_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,18 +19,30 @@
     Runs the coroutine in an event loop running on a background thread,
     and blocks the current thread until it returns a result.
     This plays well with gevent, since it can yield on the Future result call.
 
     :param coro: A coroutine, typically an async method
     :param timeout: How many seconds we should wait for a result before raising an error
     """
+    try:
+        # FIXME: this is a hack to work around an annoying stall issue in Jupyter notebooks
+        #        for some reason, run_coroutine_threadsafe hangs indefinitely when uploading files
+        #        inside the jupyter notebook. nest_asyncio allows us to just use LOOP.run_until_complete
+        __IPYTHON__  # noqa: F821
+        import nest_asyncio
+
+        nest_asyncio.apply()
+    except Exception:
+        pass
+
     if LOOP.is_running():
         return asyncio.run_coroutine_threadsafe(coro, LOOP).result()
     elif asyncio.get_event_loop().is_running():
-        return asyncio.create_task(coro)
+        r = asyncio.run(coro)
+        return r
     else:
         try:
             return LOOP.run_until_complete(coro)
         except RuntimeError:
             start_background_loop(LOOP)
             return asyncio.run_coroutine_threadsafe(coro, LOOP).result()
         except Exception as e:
```

### Comparing `rush_py-2.1.0/rush/doc.py` & `rush_py-3.0.0/rush/doc.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/graphql_client/async_base_client.py` & `rush_py-3.0.0/rush/graphql_client/async_base_client.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/graphql_client/base_model.py` & `rush_py-3.0.0/rush/graphql_client/base_model.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/graphql_client/client.py` & `rush_py-3.0.0/rush/graphql_client/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,53 +5,24 @@
 from uuid import UUID
 
 from .argument import Argument, ArgumentArgument
 from .arguments import Arguments, ArgumentsMe
 from .async_base_client import AsyncBaseClient
 from .base_model import UNSET, UnsetType, Upload
 from .cancel_module_instance import CancelModuleInstance
-from .create_entity import CreateEntity, CreateEntityCreateEntity
-from .create_experiment import CreateExperiment, CreateExperimentCreateExperiment
-from .create_project import CreateProject, CreateProjectCreateProject
-from .create_protein import CreateProtein, CreateProteinCreateProtein
-from .create_protein_conformer import (
-    CreateProteinConformer,
-    CreateProteinConformerCreateProteinConformer,
-)
-from .create_smol import CreateSmol, CreateSmolCreateSmol
-from .create_smol_conformer import (
-    CreateSmolConformer,
-    CreateSmolConformerCreateSmolConformer,
-)
-from .create_smol_tautomer import (
-    CreateSmolTautomer,
-    CreateSmolTautomerCreateSmolTautomer,
-)
-from .create_structure import CreateStructure, CreateStructureCreateStructure
 from .delete_module_instance import (
     DeleteModuleInstance,
     DeleteModuleInstanceDeleteModuleInstance,
 )
 from .deploy import Deploy, DeployDeploy
-from .entity import Entity, EntityEntity
-from .enums import ModuleInstanceStatus, ModuleInstanceTarget, OrderBy
-from .experiment import Experiment, ExperimentExperiment
+from .enums import ModuleInstanceStatus, ModuleInstanceTarget, ObjectFormat, OrderBy
 from .input_types import (
-    CreateExperimentInput,
-    CreateProjectInput,
-    CreateProteinConformerInput,
-    CreateProteinInput,
-    CreateSmolConformerInput,
-    CreateSmolInput,
-    CreateSmolTautomerInput,
-    CreateStructureInput,
     ModuleInput,
     ModuleInstanceInput,
     ModuleInstanceResourcesInput,
-    RawEntityInput,
     ResourceUtilizationInput,
     TypeQuery,
     UpdateModuleInstanceInput,
 )
 from .latest_modules import LatestModules, LatestModulesLatestModules
 from .module_instance_details import (
     ModuleInstanceDetails,
@@ -59,36 +30,30 @@
 )
 from .module_instance_minimal import (
     ModuleInstanceMinimal,
     ModuleInstanceMinimalModuleInstance,
 )
 from .module_instances import ModuleInstances, ModuleInstancesMe
 from .modules import Modules, ModulesModules
-from .object_contents import ObjectContents, ObjectContentsObject
-from .object_url import ObjectUrl, ObjectUrlObject
-from .project import Project, ProjectProject
-from .protein import Protein, ProteinProtein
-from .protein_conformer import ProteinConformer, ProteinConformerProteinConformer
+from .object_contents import ObjectContents, ObjectContentsObjectPath
+from .object_url import ObjectUrl, ObjectUrlObjectPath
 from .retry import Retry, RetryRetry
 from .run import Run, RunRun
-from .smol import Smol, SmolSmol
-from .smol_conformer import SmolConformer, SmolConformerSmolConformer
-from .smol_tautomer import SmolTautomer, SmolTautomerSmolTautomer
-from .structure import Structure, StructureStructure
 from .tag import Tag
 from .track_utilization import (
     TrackUtilization,
     TrackUtilizationTrackModuleInstanceResourceUtilization,
 )
 from .untag import Untag
 from .update_module_instance import (
     UpdateModuleInstance,
     UpdateModuleInstanceUpdateModuleInstance,
 )
 from .upload_arg import UploadArg, UploadArgUploadArg
+from .upload_object import UploadObject, UploadObjectUploadObject
 
 
 def gql(q: str) -> str:
     return q
 
 
 class Client(AsyncBaseClient):
@@ -138,102 +103,124 @@
             """
         )
         variables: Dict[str, object] = {"module": module}
         response = await self.execute(query=query, operation_name="deploy", variables=variables, **kwargs)
         data = self.get_data(response)
         return Deploy.model_validate(data).deploy
 
-    async def create_entity(self, entity: RawEntityInput, **kwargs: Any) -> CreateEntityCreateEntity:
-        query = gql(
-            """
-            mutation create_entity($entity: RawEntityInput!) {
-              create_entity(entity: $entity) {
-                id
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"entity": entity}
-        response = await self.execute(
-            query=query, operation_name="create_entity", variables=variables, **kwargs
-        )
-        data = self.get_data(response)
-        return CreateEntity.model_validate(data).create_entity
-
-    async def create_experiment(
-        self, experiment: CreateExperimentInput, **kwargs: Any
-    ) -> CreateExperimentCreateExperiment:
-        query = gql(
-            """
-            mutation create_experiment($experiment: CreateExperimentInput!) {
-              create_experiment(input: $experiment) {
-                id
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"experiment": experiment}
-        response = await self.execute(
-            query=query, operation_name="create_experiment", variables=variables, **kwargs
-        )
-        data = self.get_data(response)
-        return CreateExperiment.model_validate(data).create_experiment
-
-    async def create_project(self, project: CreateProjectInput, **kwargs: Any) -> CreateProjectCreateProject:
-        query = gql(
-            """
-            mutation create_project($project: CreateProjectInput!) {
-              create_project(input: $project) {
-                id
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"project": project}
-        response = await self.execute(
-            query=query, operation_name="create_project", variables=variables, **kwargs
-        )
-        data = self.get_data(response)
-        return CreateProject.model_validate(data).create_project
-
-    async def create_protein_conformer(
-        self, protein_conformer: CreateProteinConformerInput, **kwargs: Any
-    ) -> CreateProteinConformerCreateProteinConformer:
-        query = gql(
-            """
-            mutation create_protein_conformer($protein_conformer: CreateProteinConformerInput!) {
-              create_protein_conformer(input: $protein_conformer) {
-                id
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"protein_conformer": protein_conformer}
-        response = await self.execute(
-            query=query, operation_name="create_protein_conformer", variables=variables, **kwargs
-        )
-        data = self.get_data(response)
-        return CreateProteinConformer.model_validate(data).create_protein_conformer
-
-    async def create_protein(self, protein: CreateProteinInput, **kwargs: Any) -> CreateProteinCreateProtein:
+    async def module_instances(
+        self,
+        after: Union[Optional[str], UnsetType] = UNSET,
+        before: Union[Optional[str], UnsetType] = UNSET,
+        first: Union[Optional[int], UnsetType] = UNSET,
+        last: Union[Optional[int], UnsetType] = UNSET,
+        path: Union[Optional[str], UnsetType] = UNSET,
+        name: Union[Optional[str], UnsetType] = UNSET,
+        status: Union[Optional[ModuleInstanceStatus], UnsetType] = UNSET,
+        tags: Union[Optional[List[str]], UnsetType] = UNSET,
+        ids: Union[Optional[List[UUID]], UnsetType] = UNSET,
+        in_argument_ids: Union[Optional[List[UUID]], UnsetType] = UNSET,
+        **kwargs: Any
+    ) -> ModuleInstancesMe:
         query = gql(
             """
-            mutation create_protein($protein: CreateProteinInput!) {
-              create_protein(input: $protein) {
-                id
+            query module_instances($after: String, $before: String, $first: Int, $last: Int, $path: String, $name: String, $status: ModuleInstanceStatus, $tags: [String!], $ids: [ModuleInstanceId!], $in_argument_ids: [ArgumentId!]) {
+              me {
+                account {
+                  module_instances(
+                    first: $first
+                    last: $last
+                    after: $after
+                    before: $before
+                    path: $path
+                    status: $status
+                    name: $name
+                    tags: $tags
+                    ids: $ids
+                    in_arguments: $in_argument_ids
+                  ) {
+                    edges {
+                      cursor
+                      node {
+                        id
+                        account_id
+                        created_at
+                        deleted_at
+                        queued_at
+                        admitted_at
+                        dispatched_at
+                        completed_at
+                        path
+                        status
+                        target
+                        tags
+                        ins {
+                          id
+                          created_at
+                          deleted_at
+                          rejected_at
+                          account_id
+                          typeinfo
+                          value
+                          tags
+                        }
+                        outs {
+                          id
+                          created_at
+                          deleted_at
+                          rejected_at
+                          account_id
+                          typeinfo
+                          value
+                          tags
+                        }
+                        resources {
+                          gpus
+                          nodes
+                          mem
+                          storage
+                          walltime
+                        }
+                        progress {
+                          n
+                          n_expected
+                          n_max
+                          done
+                        }
+                      }
+                    }
+                    pageInfo {
+                      hasPreviousPage
+                      hasNextPage
+                      startCursor
+                      endCursor
+                    }
+                  }
+                }
               }
             }
             """
         )
-        variables: Dict[str, object] = {"protein": protein}
+        variables: Dict[str, object] = {
+            "after": after,
+            "before": before,
+            "first": first,
+            "last": last,
+            "path": path,
+            "name": name,
+            "status": status,
+            "tags": tags,
+            "ids": ids,
+            "in_argument_ids": in_argument_ids,
+        }
         response = await self.execute(
-            query=query, operation_name="create_protein", variables=variables, **kwargs
+            query=query, operation_name="module_instances", variables=variables, **kwargs
         )
         data = self.get_data(response)
-        return CreateProtein.model_validate(data).create_protein
+        return ModuleInstances.model_validate(data).me
 
     async def argument(self, id: UUID, **kwargs: Any) -> ArgumentArgument:
         query = gql(
             """
             query argument($id: ArgumentId!) {
               argument(id: $id) {
                 ...ArgumentFull
@@ -637,143 +624,14 @@
         }
         response = await self.execute(
             query=query, operation_name="module_instance_details", variables=variables, **kwargs
         )
         data = self.get_data(response)
         return ModuleInstanceDetails.model_validate(data).module_instance
 
-    async def module_instances(
-        self,
-        after: Union[Optional[str], UnsetType] = UNSET,
-        before: Union[Optional[str], UnsetType] = UNSET,
-        first: Union[Optional[int], UnsetType] = UNSET,
-        last: Union[Optional[int], UnsetType] = UNSET,
-        path: Union[Optional[str], UnsetType] = UNSET,
-        name: Union[Optional[str], UnsetType] = UNSET,
-        status: Union[Optional[ModuleInstanceStatus], UnsetType] = UNSET,
-        tags: Union[Optional[List[str]], UnsetType] = UNSET,
-        ids: Union[Optional[List[UUID]], UnsetType] = UNSET,
-        in_argument_ids: Union[Optional[List[UUID]], UnsetType] = UNSET,
-        **kwargs: Any
-    ) -> ModuleInstancesMe:
-        query = gql(
-            """
-            query module_instances($after: String, $before: String, $first: Int, $last: Int, $path: String, $name: String, $status: ModuleInstanceStatus, $tags: [String!], $ids: [ModuleInstanceId!], $in_argument_ids: [ArgumentId!]) {
-              me {
-                account {
-                  module_instances(
-                    first: $first
-                    last: $last
-                    after: $after
-                    before: $before
-                    path: $path
-                    status: $status
-                    name: $name
-                    tags: $tags
-                    ids: $ids
-                    in_arguments: $in_argument_ids
-                  ) {
-                    edges {
-                      cursor
-                      node {
-                        ...SimpleModuleInstanceFull
-                      }
-                    }
-                    pageInfo {
-                      ...PageInfoFull
-                    }
-                  }
-                }
-              }
-            }
-
-            fragment PageInfoFull on PageInfo {
-              hasPreviousPage
-              hasNextPage
-              startCursor
-              endCursor
-            }
-
-            fragment SimpleModuleInstanceCommon on SimpleModuleInstance {
-              id
-              account_id
-              created_at
-              deleted_at
-              queued_at
-              admitted_at
-              dispatched_at
-              completed_at
-              path
-              status
-              target
-              tags
-              failure_reason
-              failure_context {
-                stdout
-                stderr
-                syserr
-              }
-            }
-
-            fragment SimpleModuleInstanceFull on SimpleModuleInstance {
-              ...SimpleModuleInstanceCommon
-              ins {
-                id
-                created_at
-                deleted_at
-                rejected_at
-                account_id
-                typeinfo
-                value
-                tags
-              }
-              outs {
-                id
-                created_at
-                deleted_at
-                rejected_at
-                account_id
-                typeinfo
-                value
-                tags
-              }
-              resources {
-                gpus
-                nodes
-                mem
-                storage
-                walltime
-              }
-              progress {
-                n
-                n_expected
-                n_max
-                done
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {
-            "after": after,
-            "before": before,
-            "first": first,
-            "last": last,
-            "path": path,
-            "name": name,
-            "status": status,
-            "tags": tags,
-            "ids": ids,
-            "in_argument_ids": in_argument_ids,
-        }
-        response = await self.execute(
-            query=query, operation_name="module_instances", variables=variables, **kwargs
-        )
-        data = self.get_data(response)
-        return ModuleInstances.model_validate(data).me
-
     async def module_instance_minimal(self, id: UUID, **kwargs: Any) -> ModuleInstanceMinimalModuleInstance:
         query = gql(
             """
             query module_instance_minimal($id: ModuleInstanceId!) {
               module_instance(id: $id) {
                 ...ModuleInstanceCommon
               }
@@ -805,301 +663,45 @@
         variables: Dict[str, object] = {"id": id}
         response = await self.execute(
             query=query, operation_name="module_instance_minimal", variables=variables, **kwargs
         )
         data = self.get_data(response)
         return ModuleInstanceMinimal.model_validate(data).module_instance
 
-    async def object_url(self, id: UUID, **kwargs: Any) -> Optional[ObjectUrlObject]:
+    async def object_url(self, path: Any, **kwargs: Any) -> ObjectUrlObjectPath:
         query = gql(
             """
-            query object_url($id: ArgumentId!) {
-              object(id: $id) {
+            query object_url($path: UUID!) {
+              object_path(path: $path) {
                 url
               }
             }
             """
         )
-        variables: Dict[str, object] = {"id": id}
+        variables: Dict[str, object] = {"path": path}
         response = await self.execute(query=query, operation_name="object_url", variables=variables, **kwargs)
         data = self.get_data(response)
-        return ObjectUrl.model_validate(data).object
+        return ObjectUrl.model_validate(data).object_path
 
-    async def object_contents(self, id: UUID, **kwargs: Any) -> Optional[ObjectContentsObject]:
+    async def object_contents(self, path: Any, **kwargs: Any) -> ObjectContentsObjectPath:
         query = gql(
             """
-            query object_contents($id: ArgumentId!) {
-              object(id: $id) {
+            query object_contents($path: UUID!) {
+              object_path(path: $path) {
                 contents
               }
             }
             """
         )
-        variables: Dict[str, object] = {"id": id}
+        variables: Dict[str, object] = {"path": path}
         response = await self.execute(
             query=query, operation_name="object_contents", variables=variables, **kwargs
         )
         data = self.get_data(response)
-        return ObjectContents.model_validate(data).object
-
-    async def entity(self, id: Any, **kwargs: Any) -> Optional[EntityEntity]:
-        query = gql(
-            """
-            query entity($id: UUID!) {
-              entity(id: $id) {
-                id
-                createdAt
-                updatedAt
-                deletedAt
-                data
-                tags
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"id": id}
-        response = await self.execute(query=query, operation_name="entity", variables=variables, **kwargs)
-        data = self.get_data(response)
-        return Entity.model_validate(data).entity
-
-    async def project(self, id: Any, **kwargs: Any) -> Optional[ProjectProject]:
-        query = gql(
-            """
-            query project($id: UUID!) {
-              project(id: $id) {
-                createdAt
-                updatedAt
-                deletedAt
-                data {
-                  name
-                }
-                tags
-                proteins {
-                  edges {
-                    node {
-                      id
-                    }
-                  }
-                }
-                protein_conformers {
-                  edges {
-                    node {
-                      id
-                    }
-                  }
-                }
-                smols {
-                  edges {
-                    node {
-                      id
-                    }
-                  }
-                }
-                smol_conformers {
-                  edges {
-                    node {
-                      id
-                    }
-                  }
-                }
-                smol_tautomers {
-                  edges {
-                    node {
-                      id
-                    }
-                  }
-                }
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"id": id}
-        response = await self.execute(query=query, operation_name="project", variables=variables, **kwargs)
-        data = self.get_data(response)
-        return Project.model_validate(data).project
-
-    async def protein(self, id: Any, **kwargs: Any) -> Optional[ProteinProtein]:
-        query = gql(
-            """
-            query protein($id: UUID!) {
-              protein(id: $id) {
-                id
-                createdAt
-                updatedAt
-                deletedAt
-                data {
-                  name
-                  sequence
-                }
-                tags
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"id": id}
-        response = await self.execute(query=query, operation_name="protein", variables=variables, **kwargs)
-        data = self.get_data(response)
-        return Protein.model_validate(data).protein
-
-    async def protein_conformer(self, id: Any, **kwargs: Any) -> Optional[ProteinConformerProteinConformer]:
-        query = gql(
-            """
-            query protein_conformer($id: UUID!) {
-              protein_conformer(id: $id) {
-                id
-                createdAt
-                updatedAt
-                deletedAt
-                data {
-                  name
-                }
-                tags
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"id": id}
-        response = await self.execute(
-            query=query, operation_name="protein_conformer", variables=variables, **kwargs
-        )
-        data = self.get_data(response)
-        return ProteinConformer.model_validate(data).protein_conformer
-
-    async def smol(self, id: Any, **kwargs: Any) -> Optional[SmolSmol]:
-        query = gql(
-            """
-            query smol($id: UUID!) {
-              smol(id: $id) {
-                id
-                createdAt
-                updatedAt
-                deletedAt
-                data {
-                  name
-                  inchi
-                }
-                tags
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"id": id}
-        response = await self.execute(query=query, operation_name="smol", variables=variables, **kwargs)
-        data = self.get_data(response)
-        return Smol.model_validate(data).smol
-
-    async def smol_conformer(self, id: Any, **kwargs: Any) -> Optional[SmolConformerSmolConformer]:
-        query = gql(
-            """
-            query smol_conformer($id: UUID!) {
-              smol_conformer(id: $id) {
-                id
-                createdAt
-                updatedAt
-                deletedAt
-                data {
-                  name
-                }
-                tags
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"id": id}
-        response = await self.execute(
-            query=query, operation_name="smol_conformer", variables=variables, **kwargs
-        )
-        data = self.get_data(response)
-        return SmolConformer.model_validate(data).smol_conformer
-
-    async def smol_tautomer(self, id: Any, **kwargs: Any) -> Optional[SmolTautomerSmolTautomer]:
-        query = gql(
-            """
-            query smol_tautomer($id: UUID!) {
-              smol_tautomer(id: $id) {
-                id
-                createdAt
-                updatedAt
-                deletedAt
-                data {
-                  name
-                  inchi
-                }
-                tags
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"id": id}
-        response = await self.execute(
-            query=query, operation_name="smol_tautomer", variables=variables, **kwargs
-        )
-        data = self.get_data(response)
-        return SmolTautomer.model_validate(data).smol_tautomer
-
-    async def structure(self, id: Any, **kwargs: Any) -> Optional[StructureStructure]:
-        query = gql(
-            """
-            query structure($id: UUID!) {
-              structure(id: $id) {
-                id
-                createdAt
-                updatedAt
-                deletedAt
-                data {
-                  name
-                }
-                topology {
-                  symbols
-                  geometry
-                  connectivity
-                  formal_charges
-                  labels
-                  partial_charges
-                  fragments
-                  fragment_formal_charges
-                  fragment_partial_charges
-                  velocities
-                  alts
-                }
-                tags
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"id": id}
-        response = await self.execute(query=query, operation_name="structure", variables=variables, **kwargs)
-        data = self.get_data(response)
-        return Structure.model_validate(data).structure
-
-    async def experiment(self, id: Any, **kwargs: Any) -> Optional[ExperimentExperiment]:
-        query = gql(
-            """
-            query experiment($id: UUID!) {
-              experiment(id: $id) {
-                id
-                createdAt
-                updatedAt
-                deletedAt
-                data {
-                  name
-                  unit
-                  measure
-                  value
-                  assay
-                }
-                tags
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"id": id}
-        response = await self.execute(query=query, operation_name="experiment", variables=variables, **kwargs)
-        data = self.get_data(response)
-        return Experiment.model_validate(data).experiment
+        return ObjectContents.model_validate(data).object_path
 
     async def retry(
         self,
         instance: UUID,
         target: ModuleInstanceTarget,
         resources: Union[Optional[ModuleInstanceResourcesInput], UnsetType] = UNSET,
         **kwargs: Any
@@ -1136,88 +738,14 @@
             """
         )
         variables: Dict[str, object] = {"instance": instance}
         response = await self.execute(query=query, operation_name="run", variables=variables, **kwargs)
         data = self.get_data(response)
         return Run.model_validate(data).run
 
-    async def create_smol_conformer(
-        self, smol_conformer: CreateSmolConformerInput, **kwargs: Any
-    ) -> CreateSmolConformerCreateSmolConformer:
-        query = gql(
-            """
-            mutation create_smol_conformer($smol_conformer: CreateSmolConformerInput!) {
-              create_smol_conformer(input: $smol_conformer) {
-                id
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"smol_conformer": smol_conformer}
-        response = await self.execute(
-            query=query, operation_name="create_smol_conformer", variables=variables, **kwargs
-        )
-        data = self.get_data(response)
-        return CreateSmolConformer.model_validate(data).create_smol_conformer
-
-    async def create_smol(self, smol: CreateSmolInput, **kwargs: Any) -> CreateSmolCreateSmol:
-        query = gql(
-            """
-            mutation create_smol($smol: CreateSmolInput!) {
-              create_smol(input: $smol) {
-                id
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"smol": smol}
-        response = await self.execute(
-            query=query, operation_name="create_smol", variables=variables, **kwargs
-        )
-        data = self.get_data(response)
-        return CreateSmol.model_validate(data).create_smol
-
-    async def create_smol_tautomer(
-        self, smol_tautomer: CreateSmolTautomerInput, **kwargs: Any
-    ) -> CreateSmolTautomerCreateSmolTautomer:
-        query = gql(
-            """
-            mutation create_smol_tautomer($smol_tautomer: CreateSmolTautomerInput!) {
-              create_smol_tautomer(input: $smol_tautomer) {
-                id
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"smol_tautomer": smol_tautomer}
-        response = await self.execute(
-            query=query, operation_name="create_smol_tautomer", variables=variables, **kwargs
-        )
-        data = self.get_data(response)
-        return CreateSmolTautomer.model_validate(data).create_smol_tautomer
-
-    async def create_structure(
-        self, structure: CreateStructureInput, **kwargs: Any
-    ) -> CreateStructureCreateStructure:
-        query = gql(
-            """
-            mutation create_structure($structure: CreateStructureInput!) {
-              create_structure(input: $structure) {
-                id
-              }
-            }
-            """
-        )
-        variables: Dict[str, object] = {"structure": structure}
-        response = await self.execute(
-            query=query, operation_name="create_structure", variables=variables, **kwargs
-        )
-        data = self.get_data(response)
-        return CreateStructure.model_validate(data).create_structure
-
     async def tag(
         self,
         tags: List[str],
         module_instance_id: Union[Optional[UUID], UnsetType] = UNSET,
         argument_id: Union[Optional[UUID], UnsetType] = UNSET,
         module_id: Union[Optional[UUID], UnsetType] = UNSET,
         **kwargs: Any
@@ -1324,7 +852,35 @@
             }
             """
         )
         variables: Dict[str, object] = {"typeinfo": typeinfo, "file": file}
         response = await self.execute(query=query, operation_name="upload_arg", variables=variables, **kwargs)
         data = self.get_data(response)
         return UploadArg.model_validate(data).upload_arg
+
+    async def upload_object(
+        self, file: Upload, typeinfo: Any, format: ObjectFormat, **kwargs: Any
+    ) -> UploadObjectUploadObject:
+        query = gql(
+            """
+            mutation upload_object($file: Upload!, $typeinfo: JSON!, $format: ObjectFormat!) {
+              upload_object(file: $file, typeinfo: $typeinfo, format: $format) {
+                id
+                object {
+                  path
+                  size
+                  format
+                }
+              }
+            }
+            """
+        )
+        variables: Dict[str, object] = {
+            "file": file,
+            "typeinfo": typeinfo,
+            "format": format,
+        }
+        response = await self.execute(
+            query=query, operation_name="upload_object", variables=variables, **kwargs
+        )
+        data = self.get_data(response)
+        return UploadObject.model_validate(data).upload_object
```

### Comparing `rush_py-2.1.0/rush/graphql_client/exceptions.py` & `rush_py-3.0.0/rush/graphql_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/graphql_client/experiment.py` & `rush_py-3.0.0/rush/graphql_client/experiment.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/graphql_client/fragments.py` & `rush_py-3.0.0/rush/graphql_client/input_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,221 +1,192 @@
 # Generated by ariadne-codegen
-# Source: combined.graphql
+# Source: schema.graphql
 
 from datetime import datetime
 from typing import Any, List, Optional
 from uuid import UUID
 
 from pydantic import Field
 
 from .base_model import BaseModel
-from .enums import ModuleFailureReason, ModuleInstanceStatus, ModuleInstanceTarget
+from .enums import MemUnits, ModuleInstanceStatus, ModuleInstanceTarget, Order
 
 
-class ArgumentFull(BaseModel):
-    id: UUID
-    name: Optional[str]
-    typeinfo: Any
-    value: Optional[Any]
-    created_at: datetime
-    rejected_at: Optional[datetime]
-    source: Optional[UUID]
-    tags: Optional[List[str]]
+class AccountBucketConfigInput(BaseModel):
+    data_bucket: str
+    log_bucket: str
+    bucket_region: str
 
 
-class ModuleFull(BaseModel):
-    id: UUID
-    name: str
-    created_at: datetime
-    deleted_at: Optional[datetime]
-    path: str
-    usage: Optional[str]
-    ins: List[Any]
-    ins_usage: Optional[List[str]]
-    outs: List[Any]
-    outs_usage: Optional[List[str]]
-    description: Optional[str]
-    typedesc: str
-    tags: Optional[List[str]]
-    targets: Optional[List[ModuleInstanceTarget]]
-    resource_bounds: Optional["ModuleFullResourceBounds"]
-
-
-class ModuleFullResourceBounds(BaseModel):
-    gpu_min: int
-    gpu_max: int
-    gpu_hint: int
-    gpu_mem_min: Optional[int]
-    gpu_mem_max: Optional[int]
-    gpu_mem_hint: Optional[int]
-    cpu_min: Optional[int]
-    cpu_max: Optional[int]
-    cpu_hint: Optional[int]
-    node_min: int
-    node_max: int
-    node_hint: int
-    mem_min: int
-    mem_max: int
-    storage_min: int
-    storage_max: int
+class AccountConfigInput(BaseModel):
+    config_account: Optional[UUID] = None
+    bucket_config: Optional["AccountBucketConfigInput"] = None
 
 
-class ModuleInstanceCommon(BaseModel):
-    id: UUID
+class ArgumentInput(BaseModel):
+    id: Optional[UUID] = None
+    name: Optional[str] = None
+    tags: Optional[List[str]] = None
+    value: Optional[Any] = None
+
+
+class CreateProject(BaseModel):
     account_id: UUID
-    name: Optional[str]
-    created_at: datetime
-    deleted_at: Optional[datetime]
-    queued_at: Optional[datetime]
-    admitted_at: Optional[datetime]
-    dispatched_at: Optional[datetime]
-    completed_at: Optional[datetime]
-    path: str
-    status: ModuleInstanceStatus
-    target: ModuleInstanceTarget
-    tags: Optional[List[str]]
-    failure_reason: Optional[ModuleFailureReason]
-    failure_context: Optional["ModuleInstanceCommonFailureContext"]
+    name: Optional[str] = None
+    description: Optional[str] = None
+    tags: Optional[List[str]] = None
 
 
-class ModuleInstanceCommonFailureContext(BaseModel):
-    stdout: Optional[str]
-    stderr: Optional[str]
-    syserr: Optional[str]
+class CreateProtein(BaseModel):
+    sequence: str
+    project_id: Any
+    name: Optional[str] = None
+    description: Optional[str] = None
+    tags: Optional[List[str]] = None
 
 
-class ModuleInstanceFull(ModuleInstanceCommon):
-    ins: List["ModuleInstanceFullIns"]
-    outs: List["ModuleInstanceFullOuts"]
-    resources: Optional["ModuleInstanceFullResources"]
-    progress: Optional["ModuleInstanceFullProgress"]
-    resource_utilization: Optional["ModuleInstanceFullResourceUtilization"]
+class DateTimeFilter(BaseModel):
+    eq: Optional[datetime] = None
+    ne: Optional[datetime] = None
+    gt: Optional[datetime] = None
+    ge: Optional[datetime] = None
+    lt: Optional[datetime] = None
+    le: Optional[datetime] = None
 
 
-class ModuleInstanceFullIns(BaseModel):
-    id: UUID
-    created_at: datetime
-    deleted_at: Optional[datetime]
-    rejected_at: Optional[datetime]
-    account_id: UUID
-    typeinfo: Any
-    value: Optional[Any]
-    tags: Optional[List[str]]
+class Jsonfilter(BaseModel):
+    eq: Optional["JsonobjectFilter"] = None
+    ne: Optional["JsonobjectFilter"] = None
 
 
-class ModuleInstanceFullOuts(BaseModel):
-    id: UUID
-    created_at: datetime
-    deleted_at: Optional[datetime]
-    rejected_at: Optional[datetime]
-    account_id: UUID
-    typeinfo: Any
-    value: Optional[Any]
-    tags: Optional[List[str]]
+class JsonobjectFilter(BaseModel):
+    key: str
+    value: str
 
 
-class ModuleInstanceFullResources(BaseModel):
-    gpus: Optional[int]
-    nodes: Optional[int]
-    mem: Optional[int]
-    storage: Optional[int]
-    walltime: Optional[int]
+class MetadataSortBy(BaseModel):
+    created_at: Optional[Order] = None
+    updated_at: Optional[Order] = None
+    deleted_at: Optional[Order] = None
+    name: Optional[Order] = None
+    description: Optional[Order] = None
 
 
-class ModuleInstanceFullProgress(BaseModel):
-    n: int
-    n_expected: int
-    n_max: int
-    done: bool
+class ModuleInput(BaseModel):
+    path: str
+    tags: Optional[List[str]] = None
+    tests: List["TestCase"]
 
 
-class ModuleInstanceFullResourceUtilization(BaseModel):
-    gpu: Optional[float]
-    mem: Optional[float]
+class ModuleInstanceInput(BaseModel):
+    path: str
+    args: List["ArgumentInput"]
+    name: Optional[str] = None
+    target: Optional[ModuleInstanceTarget] = None
+    resources: Optional["ModuleInstanceResourcesInput"] = None
+    tags: Optional[List[str]] = None
+    out_tags: Optional[List[Optional[List[str]]]] = None
+    out_names: Optional[List[Optional[str]]] = None
+    end: Optional[bool] = None
+
+
+class ModuleInstanceResourcesInput(BaseModel):
+    gpus: Optional[int] = None
+    gpu_mem: Optional[int] = None
+    gpu_mem_units: Optional[MemUnits] = None
+    cpus: Optional[int] = None
+    nodes: Optional[int] = None
+    mem: Optional[int] = None
+    mem_units: Optional[MemUnits] = None
+    storage: Optional[int] = None
+    storage_units: Optional[MemUnits] = None
+    walltime: Optional[int] = None
+    storage_mounts: Optional[List[str]] = None
+
+
+class ObjectDescriptorFilter(BaseModel):
+    all: Optional[List["ObjectDescriptorFilter"]] = None
+    any: Optional[List["ObjectDescriptorFilter"]] = None
+    id: Optional["UuidFilter"] = None
+    object: Optional["Jsonfilter"] = None
+    base_url: Optional["StringFilter"] = None
+    created_at: Optional["DateTimeFilter"] = None
+    updated_at: Optional["DateTimeFilter"] = None
+    deleted_at: Optional["DateTimeFilter"] = None
+    name: Optional["StringFilter"] = None
+    description: Optional["StringFilter"] = None
+
+
+class ObjectDescriptorSortBy(BaseModel):
+    id: Optional[Order] = None
+    base_url: Optional[Order] = None
+    account_id: Optional[Order] = None
+    metadata: Optional["MetadataSortBy"] = None
+
+
+class ResourceUtilizationInput(BaseModel):
+    module_instance_id: UUID = Field(alias="moduleInstanceId")
+    gpu: Optional[float] = None
+    mem: Optional[float] = None
     storage: float
     walltime: float
     cputime: float
     inodes: float
-    sus: Optional[int]
+    sus: Optional[int] = None
 
 
-class PageInfoFull(BaseModel):
-    has_previous_page: bool = Field(alias="hasPreviousPage")
-    has_next_page: bool = Field(alias="hasNextPage")
-    start_cursor: Optional[str] = Field(alias="startCursor")
-    end_cursor: Optional[str] = Field(alias="endCursor")
+class StringFilter(BaseModel):
+    eq: Optional[str] = None
+    ne: Optional[str] = None
+    gt: Optional[str] = None
+    ge: Optional[str] = None
+    lt: Optional[str] = None
+    le: Optional[str] = None
+    like: Optional[str] = None
+    in_: Optional[List[str]] = Field(alias="in", default=None)
+    not_in: Optional[List[str]] = None
 
 
-class SimpleModuleInstanceCommon(BaseModel):
-    id: UUID
-    account_id: UUID
-    created_at: datetime
-    deleted_at: Optional[datetime]
-    queued_at: Optional[datetime]
-    admitted_at: Optional[datetime]
-    dispatched_at: Optional[datetime]
-    completed_at: Optional[datetime]
-    path: str
-    status: ModuleInstanceStatus
+class TestCase(BaseModel):
+    args: List["ArgumentInput"]
     target: ModuleInstanceTarget
-    tags: Optional[List[str]]
-    failure_reason: Optional[ModuleFailureReason]
-    failure_context: Optional["SimpleModuleInstanceCommonFailureContext"]
+    resources: Optional["ModuleInstanceResourcesInput"] = None
+    tags: Optional[List[str]] = None
 
 
-class SimpleModuleInstanceCommonFailureContext(BaseModel):
-    stdout: Optional[str]
-    stderr: Optional[str]
-    syserr: Optional[str]
+class TokenFilter(BaseModel):
+    all: Optional[List["TokenFilter"]] = None
+    any: Optional[List["TokenFilter"]] = None
+    id: Optional["UuidFilter"] = None
+    created_at: Optional["DateTimeFilter"] = None
+    updated_at: Optional["DateTimeFilter"] = None
+    deleted_at: Optional["DateTimeFilter"] = None
 
 
-class SimpleModuleInstanceFull(SimpleModuleInstanceCommon):
-    ins: List["SimpleModuleInstanceFullIns"]
-    outs: List["SimpleModuleInstanceFullOuts"]
-    resources: Optional["SimpleModuleInstanceFullResources"]
-    progress: Optional["SimpleModuleInstanceFullProgress"]
+class TokenSortBy(BaseModel):
+    id: Optional[Order] = None
+    created_at: Optional[Order] = None
+    updated_at: Optional[Order] = None
+    deleted_at: Optional[Order] = None
+    user_id: Optional[Order] = None
 
 
-class SimpleModuleInstanceFullIns(BaseModel):
-    id: UUID
-    created_at: datetime
-    deleted_at: Optional[datetime]
-    rejected_at: Optional[datetime]
-    account_id: UUID
-    typeinfo: Any
-    value: Optional[Any]
-    tags: Optional[List[str]]
+class TypeQuery(BaseModel):
+    path: List[str]
+    query: Any
 
 
-class SimpleModuleInstanceFullOuts(BaseModel):
+class UpdateModuleInstanceInput(BaseModel):
     id: UUID
-    created_at: datetime
-    deleted_at: Optional[datetime]
-    rejected_at: Optional[datetime]
-    account_id: UUID
-    typeinfo: Any
-    value: Optional[Any]
-    tags: Optional[List[str]]
-
-
-class SimpleModuleInstanceFullResources(BaseModel):
-    gpus: Optional[int]
-    nodes: Optional[int]
-    mem: Optional[int]
-    storage: Optional[int]
-    walltime: Optional[int]
-
-
-class SimpleModuleInstanceFullProgress(BaseModel):
-    n: int
-    n_expected: int
-    n_max: int
-    done: bool
-
-
-ArgumentFull.model_rebuild()
-ModuleFull.model_rebuild()
-ModuleInstanceCommon.model_rebuild()
-ModuleInstanceFull.model_rebuild()
-PageInfoFull.model_rebuild()
-SimpleModuleInstanceCommon.model_rebuild()
-SimpleModuleInstanceFull.model_rebuild()
+    path: Optional[str] = None
+    ins: Optional[List["ArgumentInput"]] = None
+    outs: Optional[List["ArgumentInput"]] = None
+    target: Optional[ModuleInstanceTarget] = None
+    status: Optional[ModuleInstanceStatus] = None
+    resources: Optional["ModuleInstanceResourcesInput"] = None
+    tags: Optional[List[str]] = None
+
+
+class UuidFilter(BaseModel):
+    eq: Optional[Any] = None
+    ne: Optional[Any] = None
+    in_: Optional[List[Any]] = Field(alias="in", default=None)
```

### Comparing `rush_py-2.1.0/rush/graphql_client/latest_modules.py` & `rush_py-3.0.0/rush/graphql_client/latest_modules.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,7 +25,12 @@
 class LatestModulesLatestModulesEdges(BaseModel):
     cursor: str
     node: "LatestModulesLatestModulesEdgesNode"
 
 
 class LatestModulesLatestModulesEdgesNode(ModuleFull):
     pass
+
+
+LatestModules.model_rebuild()
+LatestModulesLatestModules.model_rebuild()
+LatestModulesLatestModulesEdges.model_rebuild()
```

### Comparing `rush_py-2.1.0/rush/graphql_client/module_instance_details.py` & `rush_py-3.0.0/rush/graphql_client/module_instance_details.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,7 +53,15 @@
     node: "ModuleInstanceDetailsModuleInstanceStderrEdgesNode"
 
 
 class ModuleInstanceDetailsModuleInstanceStderrEdgesNode(BaseModel):
     id: str
     created_at: datetime
     content: List[str]
+
+
+ModuleInstanceDetails.model_rebuild()
+ModuleInstanceDetailsModuleInstance.model_rebuild()
+ModuleInstanceDetailsModuleInstanceStdout.model_rebuild()
+ModuleInstanceDetailsModuleInstanceStdoutEdges.model_rebuild()
+ModuleInstanceDetailsModuleInstanceStderr.model_rebuild()
+ModuleInstanceDetailsModuleInstanceStderrEdges.model_rebuild()
```

### Comparing `rush_py-2.1.0/rush/graphql_client/module_instance_full.py` & `rush_py-3.0.0/rush/graphql_client/module_instance_full.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/graphql_client/module_instances_full.py` & `rush_py-3.0.0/rush/graphql_client/module_instances_full.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/graphql_client/project.py` & `rush_py-3.0.0/rush/graphql_client/project.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/graphql_client/protein.py` & `rush_py-3.0.0/rush/graphql_client/protein.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/graphql_client/protein_conformer.py` & `rush_py-3.0.0/rush/graphql_client/protein_conformer.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/graphql_client/smol.py` & `rush_py-3.0.0/rush/graphql_client/smol.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/graphql_client/smol_conformer.py` & `rush_py-3.0.0/rush/graphql_client/smol_conformer.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/graphql_client/smol_tautomer.py` & `rush_py-3.0.0/rush/graphql_client/smol_tautomer.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/graphql_client/structure.py` & `rush_py-3.0.0/rush/graphql_client/structure.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/legacy_types.py` & `rush_py-3.0.0/rush/legacy_types.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/local.py` & `rush_py-3.0.0/rush/local.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/protocols.py` & `rush_py-3.0.0/rush/protocols.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/provider.py` & `rush_py-3.0.0/rush/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import asyncio
 import base64
 from collections.abc import AsyncGenerator
 import json
 import logging
 import math
+import mimetypes
 import os
 import random
 import re
 import sys
 import time
 import threading
 from collections import Counter
@@ -43,36 +44,42 @@
 from .graphql_client.arguments import (
     ArgumentsMeAccountArguments,
     ArgumentsMeAccountArgumentsEdgesNode,
     ArgumentsMeAccountArgumentsPageInfo,
 )
 from .graphql_client.base_model import UNSET, UnsetType, Upload
 from .graphql_client.client import Client
-from .graphql_client.enums import MemUnits, ModuleInstanceStatus, ModuleInstanceTarget
+from .graphql_client.enums import MemUnits, ModuleInstanceStatus, ModuleInstanceTarget, ObjectFormat
 from .graphql_client.fragments import ModuleFull, ModuleInstanceFullProgress, PageInfoFull
 from .graphql_client.input_types import ArgumentInput, ModuleInstanceInput, ModuleInstanceResourcesInput
 from .graphql_client.latest_modules import LatestModulesLatestModulesPageInfo
 from .graphql_client.module_instance_details import ModuleInstanceDetailsModuleInstance
 from .graphql_client.module_instance_full import ModuleInstanceFullModuleInstance
 from .graphql_client.module_instances import (
     ModuleInstancesMeAccountModuleInstancesEdgesNode,
     ModuleInstancesMeAccountModuleInstancesPageInfo,
 )
 from .graphql_client.modules import ModulesModulesPageInfo
-from .graphql_client.object_contents import ObjectContentsObject
+from .graphql_client.object_contents import ObjectContentsObjectPath
 from .graphql_client.retry import RetryRetry
 from .graphql_client.run import RunRun
-from .typedef import SCALARS, build_typechecker, type_from_typedef
+from .typedef import SCALARS, RushType, build_typechecker, type_from_typedef
 
 if sys.version_info >= (3, 12):
     from .types import ArgId, ModuleInstanceId, Resources, Target
 else:
     from .legacy_types import ArgId, ModuleInstanceId, Resources, Target
 
 
+class VirtualObject:
+    path: str
+    size: int
+    format: ObjectFormat
+
+
 @dataclass
 class ModuleInstanceHistory:
     path: str
     id: ModuleInstanceId
     status: ModuleInstanceStatus
     tags: list[str]
 
@@ -237,14 +244,16 @@
         self.restore_by_default = restore_by_default
         self.history = None
         self.client = client
         self.client.http_client.timeout = httpx.Timeout(60)
         self.module_paths: dict[str, str] = {}
         self.logger = logger
 
+        self.__is_blocking__ = False
+
         if workspace:
             self.workspace: Path | None = Path(workspace)
             if not self.workspace.exists():
                 raise Exception("Workspace directory does not exist")
             if (self.workspace / "rush.lock").exists():
                 self.config_dir: Path | None = self.workspace
             else:
@@ -446,67 +455,68 @@
             return_paged,  # type: ignore
             PageVars(after=after, before=before, first=first, last=last),
             {
                 "tags": tags,
             },
         )
 
-    async def object(self, id: ArgId):
+    async def object(self, path: UUID):
         """
         Retrieve an object from the database.
 
         :param id: The ID of the object.
         :return: The object.
         """
         # retry the download if it fails
         retries = 3
         while retries > 0:
             try:
-                return await self.client.object_url(id)
+                return await self.client.object_url(path)
             except Exception as e:
                 retries -= 1
                 if retries == 0:
                     raise e
                 else:
                     await asyncio.sleep(1)
 
     async def download_object(
         self,
-        id: ArgId,
+        path: UUID,
         filename: str | None = None,
         filepath: Path | None = None,
         overwrite: bool = False,
         signed: bool = True,
+        decode: bool = False,
     ):
         """
         Retrieve an object from the store: a wrapper for object with simpler behavior.
 
         :param id: The ID of the object.
         :param filepath: Where to download the object.
         :param filename: Download to the workspace with this name under "objects".
         """
-        obj = (await self.object(id)) if signed else (await self.client.object_contents(id))
+        obj = (await self.object(path)) if signed else (await self.client.object_contents(path))
         if not obj:
             return None
 
         if filepath is None:
             if filename is None:
-                filename = str(id)
+                filename = str(path)
             if filename and self.workspace:
                 if not (self.workspace / "objects").exists():
                     (self.workspace / "objects").mkdir()
                 filepath = self.workspace / "objects" / filename
 
                 if filepath.exists() and not overwrite:
                     raise FileExistsError(f"File {filename} already exists in workspace")
 
         if filepath:
             if filepath.exists() and not overwrite:
                 raise FileExistsError(f"File {filename} already exists in workspace")
-            if obj and isinstance(obj, ObjectContentsObject):
+            if obj and isinstance(obj, ObjectContentsObjectPath):
                 json.dump(obj.contents, open(filepath, "w"))
             elif obj:
                 with httpx.stream(method="get", url=obj.url) as r:
                     r.raise_for_status()
 
                     buf = ""
                     with open(filepath, "wb") as f:
@@ -515,15 +525,15 @@
                         for chunk in r.iter_text():
                             if not first_chunk and not is_encoded:
                                 f.write(chunk.encode("utf-8"))
                                 continue
 
                             # handle json
                             if first_chunk:
-                                if len(chunk) > 0 and (chunk[0] == "[" or chunk[0] == "{"):
+                                if len(chunk) > 0 and (chunk[0] == "[" or chunk[0] == "{") or not decode:
                                     f.write(chunk.encode("utf-8"))
                                     first_chunk = False
                                     continue
                                 else:
                                     first_chunk = False
                                     is_encoded = True
 
@@ -639,37 +649,24 @@
                 return res[0]
 
         # always request a bit of space because the run will always create files
         storage_requirements = {"storage": 10 * 1024 * 1024}
 
         # TODO: less insane version of this
         def gen_arg_dict(
-            input: BaseProvider.Arg[Any] | BaseProvider.BlockingArg[Any] | ArgId | UUID | Path | IOBase | Any,
+            input: BaseProvider.Arg[Any] | BaseProvider.BlockingArg[Any] | ArgId | UUID | VirtualObject | Any,
         ) -> ArgumentInput:
             arg = ArgumentInput()
             if isinstance(input, BaseProvider.Arg) or isinstance(input, BaseProvider.BlockingArg):
                 if input.id is None:
                     arg.value = input.value
                 else:
                     arg.id = input.id
             elif isinstance(input, ArgId):
                 arg.id = input
-            elif isinstance(input, Path):
-                storage_requirements["storage"] += input.stat().st_size
-                if input.name.endswith(".json"):
-                    with open(input, "r") as f:
-                        arg = ArgumentInput(value=json.load(f))
-                else:
-                    arg = ArgumentInput(value=base64.b64encode(input.read_bytes()).decode("utf-8"))
-            elif isinstance(input, IOBase):
-                data = input.read()
-                # The only other case is bytes-like, i.e. isinstance(data, (bytes, bytearray))
-                if isinstance(data, str):
-                    data = data.encode("utf-8")
-                arg = ArgumentInput(value=base64.b64encode(data).decode("utf-8"))
             else:
                 arg = ArgumentInput(value=input)
             return arg
 
         arg_dicts = [gen_arg_dict(input) for input in args]
 
         if not resources:
@@ -940,19 +937,16 @@
                 if names and name not in names and tags:
                     continue
                 modules += [(name, module)]
 
         for name, module in sorted(modules):
             path = module.path
 
-            in_types = tuple(type_from_typedef(i) for i in module.ins)
             out_types = tuple(type_from_typedef(i) for i in module.outs)
 
-            typechecker = build_typechecker(*in_types)
-
             def random_target():
                 allowed_default_targets = ["NIX_SSH", "NIX_SSH_2"]
                 if "NIX_SSH_3" in str(module.targets) or "NIX_SSH_3_GPU" in str(module.targets):
                     allowed_default_targets.append("NIX_SSH_3")
                 return random.choice(allowed_default_targets)
 
             default_resources = None
@@ -962,32 +956,36 @@
                     "storage_units": "MB",
                     "gpus": module.resource_bounds.gpu_hint,
                 }
 
             def closure(
                 name: str,
                 path: str,
-                typechecker: Any,
+                module_ins: list[Any],
                 default_resources: Resources | None,
             ):
+                in_types = tuple(type_from_typedef(i) for i in module_ins)
+                typechecker = build_typechecker(*in_types)
+
                 async def runner(
                     *args: Any,
                     target: Target | None = None,
                     resources: Resources | None = default_resources,
                     tags: list[str] | None = None,
                     restore: bool | None = None,
                 ):
+                    args = await self.upload_args(args, module_ins)
                     if target is None:
                         target = random_target()
                     typechecker(*args)
                     run = await self.run(
                         path, list(args), target, resources, tags, out_tags=None, restore=restore
                     )
                     return tuple(
-                        (BaseProvider.BlockingArg if LOOP.is_running() else BaseProvider.Arg)(
+                        (BaseProvider.BlockingArg if self.__is_blocking__ else BaseProvider.Arg)(
                             self, out.id, source=run.id
                         )
                         for out in run.outs
                     )
 
                 runner.__name__ = name
 
@@ -1047,19 +1045,42 @@
                     runner.__annotations__["args"] = Unpack[
                         tuple[tuple(t.to_python_type() for t in in_types)]
                     ]
                     runner.__annotations__["return"] = tuple[tuple(t.to_python_type() for t in out_types)]
 
                 return runner
 
-            runner = closure(name, path, typechecker, default_resources)
+            runner = closure(name, path, module.ins, default_resources)
             self.__setattr__(name, runner)
             ret[name] = runner
         return ret
 
+    async def upload_args(
+        self,
+        args: tuple[Any, ...],
+        in_types: list[Any],
+    ) -> tuple[Any, ...]:
+        """
+        Walk through input types and for any that are files, upload them.
+        Replace the file with the uploaded object in the arg list and return the list.
+
+        :param args: The arguments to be uploaded.
+        :param in_types: The types of the arguments.
+
+        :return: Arguments with files replaced with virtual objects.
+        """
+        newargs = []
+        for i, arg in enumerate(args):
+            if isinstance(arg, Path):
+                obj = await self.upload(arg, in_types[i])
+                newargs.append(obj.object)
+            else:
+                newargs.append(arg)
+        return tuple(newargs)
+
     async def retry(
         self,
         id: ModuleInstanceId,
         target: Target,
         resources: Resources | None = None,
     ) -> RetryRetry:
         """
@@ -1069,26 +1090,31 @@
         :return: The ID of the new module instance.
         """
         return await self.client.retry(instance=id, resources=resources, target=target)  # type: ignore
 
     async def upload(
         self,
         file: Path | str,
-        typeinfo: dict[str, Any],
+        typeinfo: dict[str, Any] | RushType[Any],
     ):
         """
         Upload an Object with typeinfo and store as an Argument.
 
         :param file: The file to be uploaded.
         :param typeinfo: The typeinfo of the file.
         """
+        if isinstance(file, str):
+            file = Path(file)
         with open(file, "rb") as f:
-            return await self.client.upload_arg(
+            format = ObjectFormat.JSON if file.suffix == ".json" else ObjectFormat.BIN
+            mimetype = mimetypes.guess_type(file)[0]
+            return await self.client.upload_object(
                 typeinfo=typeinfo,
-                file=Upload(filename=f.name, content=f, content_type="application/octet-stream"),
+                format=format,
+                file=Upload(filename=f.name, content=f, content_type=mimetype or "text/plain"),
             )
 
     async def module_instance(self, id: ModuleInstanceId) -> ModuleInstanceDetailsModuleInstance:
         """
         Retrieve a module instance by its ID.
 
         :param id: The ID of the module instance to be retrieved.
@@ -1264,15 +1290,18 @@
                                 module_instance = await self.provider.module_instance(self.source)
                                 if module_instance.status != self.status:
                                     self.provider.logger.info(
                                         f"Argument {self.id} is now {module_instance.status}"
                                     )
                                     self.status = module_instance.status
                                 if module_instance.status == ModuleInstanceStatus.RUNNING:
-                                    if module_instance.progress != self.progress:
+                                    if (
+                                        module_instance.progress
+                                        and module_instance.progress.n != self.progress.n
+                                    ):
                                         print(f"Progress: {module_instance.progress}", end="\r")
                             await asyncio.sleep(5)
                         else:
                             raise e
                     else:
                         self.provider.logger.error(e.errors)
                         raise e
@@ -1309,15 +1338,18 @@
                     (self.typeinfo["k"] == "record" and self.typeinfo["n"] == "Object")
                     or (
                         self.typeinfo["k"] == "optional"
                         and (self.typeinfo["t"]["k"] == "record" and self.typeinfo["t"]["n"] == "Object")
                     )
                 ):
                     signed = "$" in json.dumps(self.typeinfo)
-                    return await self.provider.download_object(self.id, filename, filepath, overwrite, signed)
+                    decode = not (self.value and dict.get(self.value, "format") == "Bin")
+                    return await self.provider.download_object(
+                        self.value["path"], filename, filepath, overwrite, signed, decode
+                    )
                 else:
                     raise Exception("Cannot download non-object argument")
             else:
                 raise Exception("Cannot download argument without typeinfo")
 
         async def get(self) -> T:
             return await self._get()
@@ -1370,15 +1402,15 @@
 
             # if typeinfo is a dict, check if it is an object, and if so, download it
             if self.typeinfo and self.provider and self.id and isinstance(self.typeinfo, dict):
                 if (self.typeinfo["k"] == "record" and self.typeinfo["n"] == "Object") or (
                     self.typeinfo["k"] == "optional"
                     and (self.typeinfo["t"]["k"] == "record" and self.typeinfo["t"]["n"] == "Object")
                 ):
-                    return (await self.provider.object(self.id)).url
+                    return (await self.provider.object(self.value["path"])).url
             return self.value
 
     class BlockingArg(Arg[T]):
         def __init__(
             self,
             provider: "BaseProvider | None",
             id: UUID | None = None,
@@ -1454,15 +1486,14 @@
             logger.info("Restoring by default via env")
             restore_by_default = True
         elif os.getenv("RUSH_RESTORE_BY_DEFAULT") == "False" and restore_by_default is None:
             logger.info("Not restoring by default via env")
             restore_by_default = False
 
         elif restore_by_default is None:
-            logger.info("Not restoring by default via default")
             restore_by_default = False
 
         if access_token is None or url is None:
             # try to check the environment variables
 
             if access_token is None:
                 access_token = os.environ.get("RUSH_TOKEN")
@@ -1536,85 +1567,85 @@
     :param workspace: The workspace directory to use.
     :param batch_tags: The tags that will be placed on all runs by default.
     :return: The built RushProvider.
     """
     provider = Provider(
         access_token, url, workspace, batch_tags, logger, restore_by_default=restore_by_default
     )
-    if not LOOP.is_running():
+    if not LOOP.is_running() and not asyncio.get_event_loop().is_running():
         _LOOP_THREAD = threading.Thread(target=start_background_loop, args=(LOOP,), daemon=True)
         _LOOP_THREAD.start()
 
     # functions that don't get called internally can be overridden with blocking versions
-    blockable_functions = ("nuke", "status", "logs", "upload", "retry", "tag")
+    blockable_functions = ("nuke", "status", "logs", "retry", "tag")
     built_fns = asyncio_run(provider.get_module_functions(names=module_names, tags=module_tags))
     # for each async function in the provider, create a blocking version
     blocking_versions: dict[str, Callable[..., Any]] = {}
     for name, func in provider.__dict__.items():
         if (
             asyncio.iscoroutinefunction(func)
             or inspect.iscoroutine(func)
             or inspect.iscoroutinefunction(func)
         ):
 
-            def closure(func):
+            def closure(func, n):
                 def blocking_func(
                     *args,
                     target: Target | None = None,
                     resources: Resources | None = None,
                     tags: list[str] | None = None,
                     restore: bool | None = None,
                 ):
                     return asyncio_run(
                         func(*args, target=target, resources=resources, tags=tags, restore=restore)
                     )
 
                 return blocking_func
 
             name = name if name in built_fns else f"{name}_blocking"
-            blocking_func = closure(func)
+            blocking_func = closure(func, name)
             blocking_func.__name__ = f"{name}"
             blocking_func.__doc__ = func.__doc__
             blocking_func.__annotations__ = func.__annotations__
 
             blocking_versions[name] = blocking_func
 
     for name, func in BaseProvider.__dict__.items():
         if (
             asyncio.iscoroutinefunction(func)
             or inspect.iscoroutine(func)
             or inspect.iscoroutinefunction(func)
         ):
 
-            def closure(func: Callable[..., Awaitable[T]]):
+            def closure(func: Callable[..., Awaitable[T]], n):
                 def blocking_func(*args: Any, **kwargs: Any) -> Any:
                     r = asyncio_run(func(provider, *args, **kwargs))
                     if isinstance(r, AsyncGenerator):
                         res = []
                         while True:
                             try:
                                 res += [asyncio_run(anext(r))]
                             except StopAsyncIteration:
                                 return res
                     return r
 
                 return blocking_func
 
             name = name if name in blockable_functions else f"{name}_blocking"
-            blocking_func = closure(func)
+            blocking_func = closure(func, name)
             blocking_func.__name__ = f"{name}"
             blocking_func.__doc__ = func.__doc__
             blocking_func.__annotations__ = func.__annotations__
 
             blocking_versions[name] = blocking_func
 
     for name, func in BaseProvider.__dict__.items():
         if inspect.isasyncgenfunction(func) or inspect.isasyncgen(func):
 
-            def closure(func: Callable[..., Awaitable[T]]):
+            def closure(func: Callable[..., Awaitable[T]], n):
                 def blocking_func(*args: Any, **kwargs: Any) -> Any:
                     r = func(provider, *args, **kwargs)
                     if isinstance(r, AsyncGenerator):
                         try:
                             hn = asyncio_run(anext(r))
                         except StopAsyncIteration:
                             return
@@ -1625,16 +1656,17 @@
                             except StopAsyncIteration:
                                 return
                     return r
 
                 return blocking_func
 
             name = name if name in blockable_functions else f"{name}_blocking"
-            blocking_func = closure(func)
+            blocking_func = closure(func, name)
             blocking_func.__name__ = f"{name}"
             blocking_func.__doc__ = func.__doc__
             blocking_func.__annotations__ = func.__annotations__
 
             blocking_versions[name] = blocking_func
 
     provider.__dict__.update(blocking_versions)
+    provider.__is_blocking__ = True
     return provider
```

### Comparing `rush_py-2.1.0/rush/tests/test_typedef.py` & `rush_py-3.0.0/rush/tests/test_typedef.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/rush/typedef.py` & `rush_py-3.0.0/rush/typedef.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from dataclasses import dataclass
 from io import BytesIO, StringIO
 from numbers import Number
 from pathlib import Path
 from typing import Any, Generic, Literal, TypeVar
 from uuid import UUID
 
+from rush.graphql_client.upload_object import UploadObjectUploadObjectObject
+
 try:
     from typing import Unpack
 except ImportError:
     from typing_extensions import Unpack
 
 
 T = TypeVar("T")
@@ -30,15 +32,37 @@
 
 
 class _RushObject(Generic[U]):
     object: U | None = None
 
 
 SCALARS = Literal[
-    "bool", "u8", "u16", "u32", "u64", "i8", "i16", "i32", "i64", "f32", "f64", "string", "bytes"
+    "bool",
+    "u8",
+    "u16",
+    "u32",
+    "u64",
+    "i8",
+    "i16",
+    "i32",
+    "i64",
+    "f32",
+    "f64",
+    "string",
+    "bytes",
+    "a3m",
+    "gro",
+    "mdp",
+    "mol2",
+    "pdb",
+    "pdbqt",
+    "sdf",
+    "smi",
+    "trr",
+    "xtc",
 ]
 
 SCALAR_STRS: list[SCALARS] = [
     "bool",
     "u8",
     "u16",
     "u32",
@@ -47,34 +71,52 @@
     "i16",
     "i32",
     "i64",
     "f32",
     "f64",
     "string",
     "bytes",
+    "a3m",
+    "gro",
+    "mdp",
+    "mol2",
+    "pdb",
+    "pdbqt",
+    "sdf",
+    "smi",
+    "trr",
+    "xtc",
 ]
 
-
 scalar_types_mapping: dict[str, type[Any]] = {
     "bool": bool,
     "u8": int,
     "u16": int,
     "u32": int,
     "u64": int,
     "i8": int,
     "i16": int,
     "i32": int,
     "i64": int,
     "f32": float,
     "f64": float,
     "string": str,
     "bytes": bytes,
+    "a3m": bytes,
+    "gro": bytes,
+    "mdp": bytes,
+    "mol2": bytes,
+    "pdb": bytes,
+    "pdbqt": bytes,
+    "sdf": bytes,
+    "smi": bytes,
+    "trr": bytes,
+    "xtc": bytes,
 }
 
-
 KINDS = Literal["array", "optional", "enum", "record", "tuple", "@"]
 
 
 @dataclass
 class SimpleType:
     k: KINDS | None
     t: SCALARS | "SimpleType"
@@ -155,15 +197,15 @@
         self.k = "array"
         self.t = array
 
     def to_python_type(self) -> type[list[Any]]:
         return list[self.t.to_python_type()]
 
     def matches(self, other: list[T] | Any) -> tuple[bool, str | None]:
-        if not (isinstance(other, list) or isinstance(other, tuple)):
+        if not isinstance(other, (list, tuple)):
             return (False, f"Expected list or tuple, got {type(other)}")
         for x in other:
             ok, reason = self.t.matches(x)
             if not ok:
                 return (False, reason)
         return (True, None)
 
@@ -212,15 +254,15 @@
         self.t = object
         self.n = "Object"
 
     def to_python_type(self) -> type[RushObject[Any]]:
         return RushObject[self.t.to_python_type()]
 
     def matches(self, other: Path | StringIO | BytesIO | Any) -> tuple[bool, str | None]:
-        if isinstance(other, _RushObject) or isinstance(other, Path) or isinstance(other, StringIO):
+        if isinstance(other, (_RushObject, Path, StringIO, UploadObjectUploadObjectObject)):
             return (True, None)
         else:
             return (False, f"Expected Path, got {type(other)}")
 
 
 class ScalarType(Generic[T], RushType[T]):
     def __init__(self, scalar: SCALARS | str):
@@ -238,15 +280,15 @@
         if self.literal:
             if other == self.literal:
                 return (True, None)
             else:
                 return (False, f"Expected {self.literal}, got {other}")
         elif not self.py_type:
             return (True, None)
-        elif isinstance(other, self.py_type) or (isinstance(other, Number) and self.py_type == float):
+        elif isinstance(other, self.py_type) or (isinstance(other, Number) and self.py_type is float):
             return (True, None)
         else:
             return (False, f"Expected {self.py_type}, got {other}")
 
 
 def type_from_typedef(res: Any) -> RushType[Any]:
     if isinstance(res, dict):
```

### Comparing `rush_py-2.1.0/rush/types.py` & `rush_py-3.0.0/rush/types.py`

 * *Files identical despite different names*

### Comparing `rush_py-2.1.0/PKG-INFO` & `rush_py-3.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: rush-py
-Version: 2.1.0
+Version: 3.0.0
 Summary: Python SDK for interacting with the QDX Rush API and modules
 Home-page: https://rush.qdx.co
 Author: Ryan Swart
 Author-email: ryan.swart@qdx.co
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
+Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0)
 Requires-Dist: pdb-tools (>=2.5.0,<3.0.0)
 Requires-Dist: pydantic (>=2.6.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Requires-Dist: websockets (>=12,<13)
 Project-URL: Documentation, https://talo.github.io/rush-py
 Description-Content-Type: text/markdown
 
@@ -54,25 +56,28 @@
 os.environ["RUSH_TOKEN"] = YOUR_TOKEN
 
 # 1.3 Build your client
 client = rush.build_blocking_provider_with_functions()
 
 # 2.1 Prepare the protein
 prepared_protein_qdxf, prepared_protein_pdb = client.prepare_protein(
-    Path("1B39_A_nohet.pdb"), tags=["example_prep"]
+    Path("1B39_A_nohet.pdb"), None, None, tags=["example_prep"]
 )
 
 # 2.3 Return run values
 print(prepared_protein_qdxf.download(overwrite=True).open().read()[0:50], "...")
 ```
 
-    2024-03-21 14:31:29,560 - rush - INFO - Restoring by default via env
-    2024-03-21 14:31:30,540 - rush - INFO - Trying to restore job with tags: ['example_prep'] and path: github:talo/prepare_protein/947cdbc000031e192153a20a9b4a8fbb12279102#prepare_protein_tengu
-    2024-03-21 14:31:30,586 - rush - INFO - Restoring job from previous run with id ea02e2b4-06b1-4576-a1f9-0ecec22e537b
-    [{"amino_acid_insertion_codes": ["", "", "", "", " ...
+    2024-04-08 17:12:28,141 - rush - INFO - Not restoring by default via default
+    2024-04-08 17:12:29,451 - rush - INFO - Argument 10ef4d21-fac5-4962-973b-cf0f6e26d964 is now ModuleInstanceStatus.RESOLVING
+    2024-04-08 17:12:40,388 - rush - INFO - Argument 10ef4d21-fac5-4962-973b-cf0f6e26d964 is now ModuleInstanceStatus.ADMITTED
+    2024-04-08 17:12:44,734 - rush - INFO - Argument 10ef4d21-fac5-4962-973b-cf0f6e26d964 is now ModuleInstanceStatus.DISPATCHED
+    2024-04-08 17:12:45,825 - rush - INFO - Argument 10ef4d21-fac5-4962-973b-cf0f6e26d964 is now ModuleInstanceStatus.RUNNING
+    2024-04-08 17:12:59,570 - rush - INFO - Argument 10ef4d21-fac5-4962-973b-cf0f6e26d964 is now ModuleInstanceStatus.AWAITING_UPLOAD
+    [{"topology": {"version": "V1", "symbols": ["N", " ...
 
 # 1) Setup
 
 This is where we prepare the rush client, directories, and input data
 we’ll be working with.
 
 ## 1.0) Imports
@@ -133,15 +138,15 @@
 
 ``` python
 # By using the `build_provider_with_functions` method,
 # we will also build helper functions calling each module
 client = rush.build_blocking_provider_with_functions(batch_tags=TAGS)
 ```
 
-    2024-03-21 14:31:32,815 - rush - INFO - Restoring by default via env
+    2024-04-08 17:13:26,467 - rush - INFO - Not restoring by default via default
 
 ## 1.4) Input selection
 
 Fetch a pdb from RCSB, stripping hetatoms and selecting a single chain
 to pass as input to the modules:
 
 ``` python
@@ -168,75 +173,88 @@
 ``` python
 # we can check the arguments and outputs for prepare_protein with help()
 help(client.prepare_protein)
 ```
 
     Help on function prepare_protein in module rush.provider:
 
-    prepare_protein(*args: *tuple[RushObject[bytes]], target: 'Target | None' = None, resources: 'Resources | None' = None, tags: 'list[str] | None' = None, restore: 'bool | None' = None) -> tuple[RushObject[list[Record]], RushObject[bytes]]
+    prepare_protein(*args: *tuple[RushObject[bytes], Optional[float], Optional[EnumValue]], target: 'Target | None' = None, resources: 'Resources | None' = None, tags: 'list[str] | None' = None, restore: 'bool | None' = None) -> tuple[RushObject[list[Record]], RushObject[bytes]]
         Prepare a PDB for downstream tasks: protonate, fill missing atoms, etc.
 
         Module version:
-        `github:talo/prepare_protein/947cdbc000031e192153a20a9b4a8fbb12279102#prepare_protein_tengu`
+        `github:talo/prepare_protein/fbeca1ad893cd763b00dc275c43806c0edce03de#prepare_protein_tengu`
 
         QDX Type Description:
 
-            input_pdb: Object[@$Bytes]
+            input_pdb: Object[@$PDB];
+            ph: f32?;
+            naming_scheme: NamingScheme[Amber | Charmm]?
             ->
             output_qdxf: Object[[Conformer]];
-            output_pdb: Object[@$Bytes]
+            output_pdb: Object[@$PDB]
 
 
         :param input_pdb: An input protein as a file; one PDB file
+        :param ph: The ph for determining protonation states; 0-14
+        :param naming_scheme: \
+                        The force field naming scheme to use; \
+                        options are "amber" or "charmm"; \
+                        None produces RCSB/IUPAC standard naming\
+
         :return output_qdxf: An output protein a vec: one qdxf per model in pdb
         :return output_pdb: An output protein as a file: one PDB file
 
 ``` python
 # Here we run the function, it will return a Provider.Arg which you can use to
 # fetch the results
 # We set restore = True so that we can restore a previous run to the same path
 # with the same tags
 prepared_protein_qdxf, prepared_protein_pdb = client.prepare_protein(
-    PROTEIN_PDB_PATH,
+    PROTEIN_PDB_PATH, None, None
 )
 # This initially only has the id of your result; we will show how to fetch the
 # actual value later
 prepared_protein_qdxf
 ```
 
-    2024-03-21 14:31:36,354 - rush - INFO - Trying to restore job with tags: ['qdx', 'rush-py-quickstart', '1B39'] and path: github:talo/prepare_protein/947cdbc000031e192153a20a9b4a8fbb12279102#prepare_protein_tengu
-    2024-03-21 14:31:36,400 - rush - INFO - Restoring job from previous run with id d746634a-8fe8-437d-b468-4bb66f5f4a12
+    2024-04-08 17:13:29,649 - rush - INFO - Trying to restore job with tags: ['qdx', 'rush-py-quickstart', '1B39'] and path: github:talo/prepare_protein/fbeca1ad893cd763b00dc275c43806c0edce03de#prepare_protein_tengu
 
-    Arg(id=127ac5f6-1227-49f4-ad2b-45a08e6c64ca, value=None)
+    Arg(id=37deb248-97fe-443d-b243-36ba172ca7be, value=None)
 
 ## 2.1) Run statuses
 
 This will show the status of all of your runs. You can also view run
 statuses on the [Rush UI](https://rush.qdx.co/dashboard/jobs).
 
 ``` python
 client.status()
 ```
 
-    {}
+    {'8e8357a0-3c37-4c23-bf98-567db98d74df': (<ModuleInstanceStatus.RESOLVING: 'RESOLVING'>,
+      'prepare_protein',
+      1)}
 
 ## 2.2) Run Values
 
 This will return the “value” of the output from the function—for files
 you will recieve a url that you can download, otherwise you will recieve
 them as python types:
 
 ``` python
 protein_qdxf_info = prepared_protein_qdxf.get()
 protein_qdxf_info
 ```
 
-    Blocking get
+    2024-04-08 17:13:29,921 - rush - INFO - Argument 37deb248-97fe-443d-b243-36ba172ca7be is now ModuleInstanceStatus.RESOLVING
+    2024-04-08 17:13:36,501 - rush - INFO - Argument 37deb248-97fe-443d-b243-36ba172ca7be is now ModuleInstanceStatus.ADMITTED
+    2024-04-08 17:13:40,894 - rush - INFO - Argument 37deb248-97fe-443d-b243-36ba172ca7be is now ModuleInstanceStatus.DISPATCHED
+    2024-04-08 17:13:43,225 - rush - INFO - Argument 37deb248-97fe-443d-b243-36ba172ca7be is now ModuleInstanceStatus.RUNNING
+    2024-04-08 17:13:55,523 - rush - INFO - Argument 37deb248-97fe-443d-b243-36ba172ca7be is now ModuleInstanceStatus.AWAITING_UPLOAD
 
-    'https://storage.googleapis.com/rush_store_default/af08031b-e871-45e2-a226-e8c7e1fd5719?x-goog-signature=0864503418ee439f8b34e2461b06c15c4e83be22a72b7acd977ed41c02da00915c749bd4f9145b4cec3553fed283ffee660f20b6f418df99ad4bad1c34f8edcdd1e337da2021ef8e0bfae9c8a7bc0b85729c605765e9512a2623f3dacdcaf079bf416a946881873a87f7fc17e3b54fe8651837aa2b47208ac9b9b42d5d8854d2214e2c7002f89d8b82a0ab3317da32aa5030a48590eda2e870bf23388ad4a77ce4a9c1602a1790248439ea8ceac3291824978332266fc39d548822b2f1dc93eb1ddbbcd326c312feac5bb24345cf0d4193657ea1d1e3bec3cb07fc858b924108aaea74415e12c861a355335ea8bc6507834bf42395d9e52c75846986b395ddd3&x-goog-algorithm=GOOG4-RSA-SHA256&x-goog-credential=qdx-store-user%40humming-bird-321603.iam.gserviceaccount.com%2F20240321%2Fasia-southeast1%2Fstorage%2Fgoog4_request&x-goog-date=20240321T063139Z&x-goog-expires=3600&x-goog-signedheaders=host'
+    'https://storage.googleapis.com/qdx-store/4a4271de-5e14-4756-b115-9c034d7ab294?x-goog-signature=202cb9f86a4351fc30780d26713b4478012548544ff30ba6700f349ad1fcc63137dfb1d2db92fc9d39bc51ba9881c44b27e89e0781aec23d034ec61c4efe2c806b8d784d124863a37d16ce0df02880e272aa0d0dc8f6be23f7214f207183337eb80c9dd0d70757e2761d8f366eea997d066761fadd9ed33483aa8ec98e7fb00e62a78501fdbc2e1e3b9eb4f9e2374a68972937bcae562d114a7e705ca645cd7eb80e5df835c9e462aa34601c8e14691ad6bcbfafef751a7562d8ea3640e77e79f2bd2f6f3b2533df462e245fc4991729f44bee6aa7d9de31cb8a14615b37ba7950c40af54f5a9f146a1a1fb91b2a9f6692d1bca60a8fb2cecd98c2b33fdbd558&x-goog-algorithm=GOOG4-RSA-SHA256&x-goog-credential=qdx-store-user%40humming-bird-321603.iam.gserviceaccount.com%2F20240408%2Fasia-southeast1%2Fstorage%2Fgoog4_request&x-goog-date=20240408T091417Z&x-goog-expires=3600&x-goog-signedheaders=host'
 
 ## 2.3) Downloads
 
 We provide a utility to download files into your workspace, you can
 either provide a filename, which will be saved in
 `workspace/objects/[filename]`, or you can provide your own filepath
 which the client will use as-is:
@@ -262,10 +280,10 @@
 
 ``` python
 # we can read our prepared protein pdb like this
 with open(client.workspace / "objects" / "01_prepared_protein.pdb", "r") as f:
     print(f.readline(), "...")
 ```
 
-    REMARK   1 CREATED WITH OPENMM 8.0, 2024-02-29
+    REMARK   1 CREATED WITH OPENMM 8.0, 2024-04-08
      ...
```

