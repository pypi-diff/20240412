# Comparing `tmp/efootprint-2.0.0.tar.gz` & `tmp/efootprint-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efootprint-2.0.0.tar", max compression
+gzip compressed data, was "efootprint-2.0.1.tar", max compression
```

## Comparing `efootprint-2.0.0.tar` & `efootprint-2.0.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    34522 2023-10-17 09:49:47.557993 efootprint-2.0.0/LICENSE
--rw-r--r--   0        0        0     3456 2024-04-06 12:40:51.663763 efootprint-2.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-06 12:40:52.150404 efootprint-2.0.0/efootprint/__init__.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.648138 efootprint-2.0.0/efootprint/abstract_modeling_classes/__init__.py
--rw-r--r--   0        0        0    11880 2024-04-06 12:40:52.160479 efootprint-2.0.0/efootprint/abstract_modeling_classes/explainable_object_base_class.py
--rw-r--r--   0        0        0     2240 2024-04-06 12:40:52.168353 efootprint-2.0.0/efootprint/abstract_modeling_classes/explainable_object_dict.py
--rw-r--r--   0        0        0    12607 2024-04-06 12:40:52.173001 efootprint-2.0.0/efootprint/abstract_modeling_classes/explainable_objects.py
--rw-r--r--   0        0        0    17405 2024-04-06 12:40:52.176669 efootprint-2.0.0/efootprint/abstract_modeling_classes/modeling_object.py
--rw-r--r--   0        0        0      754 2024-03-04 16:54:55.210288 efootprint-2.0.0/efootprint/abstract_modeling_classes/source_objects.py
--rw-r--r--   0        0        0        0 2024-03-04 16:55:00.126280 efootprint-2.0.0/efootprint/api_utils/__init__.py
--rw-r--r--   0        0        0     5499 2024-04-06 16:25:45.616333 efootprint-2.0.0/efootprint/api_utils/json_to_system.py
--rw-r--r--   0        0        0     1306 2024-04-06 16:25:45.620494 efootprint-2.0.0/efootprint/api_utils/system_to_json.py
--rw-r--r--   0        0        0        0 2024-03-04 16:54:53.623840 efootprint-2.0.0/efootprint/builders/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 16:54:54.164118 efootprint-2.0.0/efootprint/builders/hardware/__init__.py
--rw-r--r--   0        0        0     2076 2024-03-04 16:54:55.218246 efootprint-2.0.0/efootprint/builders/hardware/devices_defaults.py
--rw-r--r--   0        0        0      743 2024-03-04 16:54:55.222924 efootprint-2.0.0/efootprint/builders/hardware/network_defaults.py
--rw-r--r--   0        0        0     8980 2024-04-06 12:40:52.200652 efootprint-2.0.0/efootprint/builders/hardware/servers_boaviztapi.py
--rw-r--r--   0        0        0     2898 2024-03-04 16:54:57.077899 efootprint-2.0.0/efootprint/builders/hardware/servers_defaults.py
--rw-r--r--   0        0        0     1876 2024-03-04 16:54:55.236944 efootprint-2.0.0/efootprint/builders/hardware/storage_defaults.py
--rw-r--r--   0        0        0        0 2024-04-06 16:25:45.621704 efootprint-2.0.0/efootprint/builders/usage/__init__.py
--rw-r--r--   0        0        0       39 2024-04-06 16:25:45.623649 efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/.gitignore
--rw-r--r--   0        0        0        0 2024-04-06 16:25:45.624639 efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/__init__.py
--rw-r--r--   0        0        0     2556 2024-04-06 17:04:29.583138 efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_analysis.py
--rw-r--r--   0        0        0     3888 2024-04-06 17:04:45.906689 efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_for_job_defaults.csv
--rw-r--r--   0        0        0     1827 2024-04-06 16:46:25.107263 efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_job_builder.py
--rw-r--r--   0        0        0    67861 2024-04-06 16:25:45.634291 efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_results__raw.csv
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.656189 efootprint-2.0.0/efootprint/constants/__init__.py
--rw-r--r--   0        0        0     4182 2024-04-06 12:40:52.207602 efootprint-2.0.0/efootprint/constants/countries.py
--rw-r--r--   0        0        0      100 2023-10-26 17:58:06.658280 efootprint-2.0.0/efootprint/constants/custom_units.txt
--rw-r--r--   0        0        0      284 2023-11-13 13:05:11.080734 efootprint-2.0.0/efootprint/constants/files.py
--rw-r--r--   0        0        0     1660 2024-03-04 16:54:55.243478 efootprint-2.0.0/efootprint/constants/sources.py
--rw-r--r--   0        0        0      173 2023-10-26 17:58:06.666143 efootprint-2.0.0/efootprint/constants/units.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.666706 efootprint-2.0.0/efootprint/core/__init__.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.667254 efootprint-2.0.0/efootprint/core/hardware/__init__.py
--rw-r--r--   0        0        0     6034 2024-04-06 12:40:52.212747 efootprint-2.0.0/efootprint/core/hardware/device_population.py
--rw-r--r--   0        0        0     5707 2024-04-06 12:40:52.215226 efootprint-2.0.0/efootprint/core/hardware/hardware_base_classes.py
--rw-r--r--   0        0        0     3367 2024-04-06 12:40:52.219470 efootprint-2.0.0/efootprint/core/hardware/network.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.671292 efootprint-2.0.0/efootprint/core/hardware/servers/__init__.py
--rw-r--r--   0        0        0     3135 2024-03-04 16:54:57.120650 efootprint-2.0.0/efootprint/core/hardware/servers/autoscaling.py
--rw-r--r--   0        0        0     3766 2024-04-06 12:40:52.222595 efootprint-2.0.0/efootprint/core/hardware/servers/on_premise.py
--rw-r--r--   0        0        0     3464 2024-03-04 16:54:59.121266 efootprint-2.0.0/efootprint/core/hardware/servers/server_base_class.py
--rw-r--r--   0        0        0     1972 2024-03-04 16:54:57.211287 efootprint-2.0.0/efootprint/core/hardware/servers/serverless.py
--rw-r--r--   0        0        0     5491 2024-03-04 16:54:59.146307 efootprint-2.0.0/efootprint/core/hardware/storage.py
--rw-r--r--   0        0        0     5312 2024-04-06 16:25:45.643459 efootprint-2.0.0/efootprint/core/service.py
--rw-r--r--   0        0        0    10359 2024-04-06 16:25:45.650082 efootprint-2.0.0/efootprint/core/system.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.688562 efootprint-2.0.0/efootprint/core/usage/__init__.py
--rw-r--r--   0        0        0     3995 2024-04-06 16:25:45.651955 efootprint-2.0.0/efootprint/core/usage/job.py
--rw-r--r--   0        0        0     3890 2024-04-06 12:40:52.233601 efootprint-2.0.0/efootprint/core/usage/usage_pattern.py
--rw-r--r--   0        0        0     2723 2024-04-06 16:25:45.657976 efootprint-2.0.0/efootprint/core/usage/user_journey.py
--rw-r--r--   0        0        0     1510 2024-04-06 16:25:45.660815 efootprint-2.0.0/efootprint/core/usage/user_journey_step.py
--rw-r--r--   0        0        0      805 2023-11-13 13:05:11.082835 efootprint-2.0.0/efootprint/logger.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.698150 efootprint-2.0.0/efootprint/utils/__init__.py
--rw-r--r--   0        0        0     3055 2024-04-06 12:40:52.240288 efootprint-2.0.0/efootprint/utils/calculus_graph.py
--rw-r--r--   0        0        0      146 2023-11-03 15:44:18.031433 efootprint-2.0.0/efootprint/utils/dev_utils/README.md
--rw-r--r--   0        0        0        0 2023-11-03 15:44:18.033655 efootprint-2.0.0/efootprint/utils/dev_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-11-03 15:44:18.035244 efootprint-2.0.0/efootprint/utils/dev_utils/page_weights.py
--rw-r--r--   0        0        0      830 2023-11-03 15:44:18.039040 efootprint-2.0.0/efootprint/utils/dev_utils/selenium_screenshot.py
--rw-r--r--   0        0        0     1407 2024-04-06 12:40:52.242646 efootprint-2.0.0/efootprint/utils/graph_tools.py
--rw-r--r--   0        0        0     2390 2024-04-06 16:50:31.330325 efootprint-2.0.0/efootprint/utils/object_relationships_graphs.py
--rw-r--r--   0        0        0     7612 2024-04-06 16:26:15.688584 efootprint-2.0.0/efootprint/utils/plot_emission_diffs.py
--rw-r--r--   0        0        0     1702 2024-03-04 16:54:53.701197 efootprint-2.0.0/efootprint/utils/tools.py
--rw-r--r--   0        0        0     1258 2024-04-06 17:10:56.033814 efootprint-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     4149 1970-01-01 00:00:00.000000 efootprint-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-10-17 09:49:47.557993 efootprint-2.0.1/LICENSE
+-rw-r--r--   0        0        0     3456 2024-04-06 12:40:51.663763 efootprint-2.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 12:40:52.150404 efootprint-2.0.1/efootprint/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.648138 efootprint-2.0.1/efootprint/abstract_modeling_classes/__init__.py
+-rw-r--r--   0        0        0    11880 2024-04-06 12:40:52.160479 efootprint-2.0.1/efootprint/abstract_modeling_classes/explainable_object_base_class.py
+-rw-r--r--   0        0        0     2240 2024-04-06 12:40:52.168353 efootprint-2.0.1/efootprint/abstract_modeling_classes/explainable_object_dict.py
+-rw-r--r--   0        0        0    12607 2024-04-06 12:40:52.173001 efootprint-2.0.1/efootprint/abstract_modeling_classes/explainable_objects.py
+-rw-r--r--   0        0        0    17481 2024-04-12 11:51:41.746811 efootprint-2.0.1/efootprint/abstract_modeling_classes/modeling_object.py
+-rw-r--r--   0        0        0      754 2024-03-04 16:54:55.210288 efootprint-2.0.1/efootprint/abstract_modeling_classes/source_objects.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:55:00.126280 efootprint-2.0.1/efootprint/api_utils/__init__.py
+-rw-r--r--   0        0        0     5726 2024-04-12 11:51:41.750673 efootprint-2.0.1/efootprint/api_utils/json_to_system.py
+-rw-r--r--   0        0        0     1306 2024-04-06 17:14:03.492802 efootprint-2.0.1/efootprint/api_utils/system_to_json.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:54:53.623840 efootprint-2.0.1/efootprint/builders/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:54:54.164118 efootprint-2.0.1/efootprint/builders/hardware/__init__.py
+-rw-r--r--   0        0        0     2076 2024-03-04 16:54:55.218246 efootprint-2.0.1/efootprint/builders/hardware/devices_defaults.py
+-rw-r--r--   0        0        0      743 2024-03-04 16:54:55.222924 efootprint-2.0.1/efootprint/builders/hardware/network_defaults.py
+-rw-r--r--   0        0        0     8980 2024-04-06 12:40:52.200652 efootprint-2.0.1/efootprint/builders/hardware/servers_boaviztapi.py
+-rw-r--r--   0        0        0     2898 2024-03-04 16:54:57.077899 efootprint-2.0.1/efootprint/builders/hardware/servers_defaults.py
+-rw-r--r--   0        0        0     1876 2024-03-04 16:54:55.236944 efootprint-2.0.1/efootprint/builders/hardware/storage_defaults.py
+-rw-r--r--   0        0        0        0 2024-04-06 17:14:03.495913 efootprint-2.0.1/efootprint/builders/usage/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-06 17:14:03.499539 efootprint-2.0.1/efootprint/builders/usage/job_ecobenchmark/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-06 17:14:03.500532 efootprint-2.0.1/efootprint/builders/usage/job_ecobenchmark/__init__.py
+-rw-r--r--   0        0        0     2556 2024-04-06 17:14:03.502889 efootprint-2.0.1/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_analysis.py
+-rw-r--r--   0        0        0     3888 2024-04-12 11:51:13.287445 efootprint-2.0.1/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_for_job_defaults.csv
+-rw-r--r--   0        0        0     1827 2024-04-06 17:14:03.506424 efootprint-2.0.1/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_job_builder.py
+-rw-r--r--   0        0        0    67861 2024-04-06 17:14:03.511270 efootprint-2.0.1/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_results__raw.csv
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.656189 efootprint-2.0.1/efootprint/constants/__init__.py
+-rw-r--r--   0        0        0     4182 2024-04-06 12:40:52.207602 efootprint-2.0.1/efootprint/constants/countries.py
+-rw-r--r--   0        0        0      100 2023-10-26 17:58:06.658280 efootprint-2.0.1/efootprint/constants/custom_units.txt
+-rw-r--r--   0        0        0      284 2023-11-13 13:05:11.080734 efootprint-2.0.1/efootprint/constants/files.py
+-rw-r--r--   0        0        0     1660 2024-03-04 16:54:55.243478 efootprint-2.0.1/efootprint/constants/sources.py
+-rw-r--r--   0        0        0      173 2023-10-26 17:58:06.666143 efootprint-2.0.1/efootprint/constants/units.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.666706 efootprint-2.0.1/efootprint/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.667254 efootprint-2.0.1/efootprint/core/hardware/__init__.py
+-rw-r--r--   0        0        0     6034 2024-04-06 12:40:52.212747 efootprint-2.0.1/efootprint/core/hardware/device_population.py
+-rw-r--r--   0        0        0     5707 2024-04-06 12:40:52.215226 efootprint-2.0.1/efootprint/core/hardware/hardware_base_classes.py
+-rw-r--r--   0        0        0     3367 2024-04-06 12:40:52.219470 efootprint-2.0.1/efootprint/core/hardware/network.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.671292 efootprint-2.0.1/efootprint/core/hardware/servers/__init__.py
+-rw-r--r--   0        0        0     3135 2024-03-04 16:54:57.120650 efootprint-2.0.1/efootprint/core/hardware/servers/autoscaling.py
+-rw-r--r--   0        0        0     3766 2024-04-06 12:40:52.222595 efootprint-2.0.1/efootprint/core/hardware/servers/on_premise.py
+-rw-r--r--   0        0        0     3464 2024-03-04 16:54:59.121266 efootprint-2.0.1/efootprint/core/hardware/servers/server_base_class.py
+-rw-r--r--   0        0        0     1972 2024-03-04 16:54:57.211287 efootprint-2.0.1/efootprint/core/hardware/servers/serverless.py
+-rw-r--r--   0        0        0     5491 2024-03-04 16:54:59.146307 efootprint-2.0.1/efootprint/core/hardware/storage.py
+-rw-r--r--   0        0        0     5312 2024-04-06 17:14:03.514666 efootprint-2.0.1/efootprint/core/service.py
+-rw-r--r--   0        0        0    10359 2024-04-06 17:14:03.517635 efootprint-2.0.1/efootprint/core/system.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.688562 efootprint-2.0.1/efootprint/core/usage/__init__.py
+-rw-r--r--   0        0        0     3995 2024-04-06 17:14:03.519960 efootprint-2.0.1/efootprint/core/usage/job.py
+-rw-r--r--   0        0        0     3890 2024-04-06 12:40:52.233601 efootprint-2.0.1/efootprint/core/usage/usage_pattern.py
+-rw-r--r--   0        0        0     2723 2024-04-06 17:14:03.529290 efootprint-2.0.1/efootprint/core/usage/user_journey.py
+-rw-r--r--   0        0        0     1510 2024-04-06 17:14:03.531224 efootprint-2.0.1/efootprint/core/usage/user_journey_step.py
+-rw-r--r--   0        0        0      805 2023-11-13 13:05:11.082835 efootprint-2.0.1/efootprint/logger.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.698150 efootprint-2.0.1/efootprint/utils/__init__.py
+-rw-r--r--   0        0        0     3055 2024-04-06 12:40:52.240288 efootprint-2.0.1/efootprint/utils/calculus_graph.py
+-rw-r--r--   0        0        0      146 2023-11-03 15:44:18.031433 efootprint-2.0.1/efootprint/utils/dev_utils/README.md
+-rw-r--r--   0        0        0        0 2023-11-03 15:44:18.033655 efootprint-2.0.1/efootprint/utils/dev_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-03 15:44:18.035244 efootprint-2.0.1/efootprint/utils/dev_utils/page_weights.py
+-rw-r--r--   0        0        0      830 2023-11-03 15:44:18.039040 efootprint-2.0.1/efootprint/utils/dev_utils/selenium_screenshot.py
+-rw-r--r--   0        0        0     1407 2024-04-06 12:40:52.242646 efootprint-2.0.1/efootprint/utils/graph_tools.py
+-rw-r--r--   0        0        0     2390 2024-04-06 17:14:03.536199 efootprint-2.0.1/efootprint/utils/object_relationships_graphs.py
+-rw-r--r--   0        0        0     7612 2024-04-06 17:14:03.543621 efootprint-2.0.1/efootprint/utils/plot_emission_diffs.py
+-rw-r--r--   0        0        0     1702 2024-03-04 16:54:53.701197 efootprint-2.0.1/efootprint/utils/tools.py
+-rw-r--r--   0        0        0     1258 2024-04-12 11:51:41.752879 efootprint-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4149 1970-01-01 00:00:00.000000 efootprint-2.0.1/PKG-INFO
```

### Comparing `efootprint-2.0.0/LICENSE` & `efootprint-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/README.md` & `efootprint-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/abstract_modeling_classes/explainable_object_base_class.py` & `efootprint-2.0.1/efootprint/abstract_modeling_classes/explainable_object_base_class.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/abstract_modeling_classes/explainable_object_dict.py` & `efootprint-2.0.1/efootprint/abstract_modeling_classes/explainable_object_dict.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/abstract_modeling_classes/explainable_objects.py` & `efootprint-2.0.1/efootprint/abstract_modeling_classes/explainable_objects.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/abstract_modeling_classes/modeling_object.py` & `efootprint-2.0.1/efootprint/abstract_modeling_classes/modeling_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 from typing import List, Type
 from copy import copy
 import os
 import json
 from IPython.display import HTML
 
 
+PREVIOUS_LIST_VALUE_SET_SUFFIX = "__previous_list_value_set"
+
+
 def get_subclass_attributes(obj, target_class):
     return {attr_name: attr_value for attr_name, attr_value in obj.__dict__.items()
             if issubclass(type(attr_value), target_class)}
 
 
 def check_type_homogeneity_within_list_or_set(input_list_or_set):
     type_set = [type(value) for value in input_list_or_set]
@@ -114,15 +117,15 @@
                         f"{self.name}’s {name} changed from {old_value.name} to {input_value.name}")
                     super().__setattr__(name, input_value)
                     self.handle_object_link_update(input_value, old_value)
 
             elif issubclass(type(input_value), List) and name not in ["modeling_obj_containers"]:
                 if len(input_value) > 0 and type(input_value[0]) == str and self.init_has_passed:
                     raise ValueError(f"There shouldn’t be a str list update after init")
-                old_list_value_attr_name = f"{name}__previous_list_value_set"
+                old_list_value_attr_name = f"{name}{PREVIOUS_LIST_VALUE_SET_SUFFIX}"
                 if not (len(input_value) > 0 and type(input_value[0]) == str):
                     for obj in input_value:
                         obj.add_obj_to_modeling_obj_containers(self)
                     # Necessary to handle syntax obj.list_attr += [new_attr_in_list] because lists are mutable objects
                     # Otherwise if using old_value, it would already be equal to input_value
                     old_list_value = getattr(self, old_list_value_attr_name, None)
                     if self.init_has_passed and old_list_value is not None:
@@ -293,15 +296,15 @@
                     or key.startswith("initial")
                     or key == "modeling_obj_containers"):
                 continue
             if type(value) == str:
                 output_dict[key] = value
             elif type(value) == int:
                 output_dict[key] = value
-            elif type(value) == list and "__previous_list_value_set" not in key:
+            elif type(value) == list and PREVIOUS_LIST_VALUE_SET_SUFFIX not in key:
                 if len(value) == 0:
                     output_dict[key] = value
                 else:
                     if type(value[0]) == str:
                         output_dict[key] = value
                     elif issubclass(type(value[0]), ModelingObject):
                         output_dict[key] = [elt.id for elt in value]
@@ -331,15 +334,15 @@
                 key_value_str = f"{input_key}: {input_value}\n"
             elif type(input_value) == list:
                 if len(input_value) == 0:
                     key_value_str = f"{input_key}: {input_value}\n"
                 else:
                     if type(input_value[0]) == str:
                         key_value_str = f"{input_key}: {input_value}"
-                    elif issubclass(type(input_value[0]), ModelingObject) and "__previous_list_value_set" not in key:
+                    elif issubclass(type(input_value[0]), ModelingObject) and PREVIOUS_LIST_VALUE_SET_SUFFIX not in key:
                         str_value = "[" + ", ".join([elt.id for elt in input_value]) + "]"
                         key_value_str = f"{input_key}: {str_value}\n"
             elif issubclass(type(input_value), ExplainableObject):
                 key_value_str = f"{input_key}: {input_value}\n"
             elif issubclass(type(input_value), ExplainableObjectDict):
                 key_value_str = f"{input_key}: {input_value}\n"
             elif issubclass(type(input_value), ModelingObject):
```

### Comparing `efootprint-2.0.0/efootprint/abstract_modeling_classes/source_objects.py` & `efootprint-2.0.1/efootprint/abstract_modeling_classes/source_objects.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/api_utils/json_to_system.py` & `efootprint-2.0.1/efootprint/api_utils/json_to_system.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from efootprint.abstract_modeling_classes.explainable_objects import ExplainableQuantity, ExplainableHourlyUsage
+from efootprint.abstract_modeling_classes.modeling_object import PREVIOUS_LIST_VALUE_SET_SUFFIX
 from efootprint.abstract_modeling_classes.source_objects import SourceObject
 from efootprint.abstract_modeling_classes.explainable_object_base_class import ExplainableObject, Source
 from efootprint.abstract_modeling_classes.explainable_object_dict import ExplainableObjectDict
 from efootprint.constants.units import u
 from efootprint.core.service import Service
 from efootprint.core.system import System
 from efootprint.core.hardware.storage import Storage
@@ -16,14 +17,15 @@
 from efootprint.core.usage.user_journey_step import UserJourneyStep
 from efootprint.core.hardware.network import Network
 from efootprint.core.hardware.device_population import DevicePopulation
 from efootprint.constants.countries import Country
 
 import pytz
 import json
+from copy import copy
 
 
 def json_to_explainable_quantity(input_dict):
     output = None
     source = None
     if "source" in input_dict.keys():
         source = Source(input_dict["source"]["name"], input_dict["source"]["link"])
@@ -68,25 +70,26 @@
             current_class_dict[class_instance_key] = new_obj
             flat_obj_dict[class_instance_key] = new_obj
 
         class_obj_dict[class_key] = current_class_dict
 
     for class_key in class_obj_dict.keys():
         for mod_obj_key, mod_obj in class_obj_dict[class_key].items():
-            for attr_key, attr_value in mod_obj.__dict__.items():
+            for attr_key, attr_value in list(mod_obj.__dict__.items()):
                 if type(attr_value) == str and attr_key != "id" and attr_value in flat_obj_dict.keys():
                     mod_obj.__dict__[attr_key] = flat_obj_dict[attr_value]
                     flat_obj_dict[attr_value].add_obj_to_modeling_obj_containers(mod_obj)
                 elif type(attr_value) == list and attr_key != "modeling_obj_containers":
                     output_val = []
                     for elt in attr_value:
                         if type(elt) == str and elt in flat_obj_dict.keys():
                             output_val.append(flat_obj_dict[elt])
                             flat_obj_dict[elt].add_obj_to_modeling_obj_containers(mod_obj)
                     mod_obj.__dict__[attr_key] = output_val
+                    mod_obj.__dict__[f"{attr_key}{PREVIOUS_LIST_VALUE_SET_SUFFIX}"] = copy(output_val)
             mod_obj.__dict__["dont_handle_input_updates"] = False
             mod_obj.__dict__["init_has_passed"] = True
 
     for mod_obj_key, mod_obj in class_obj_dict["DevicePopulation"].items():
         mod_obj.user_journey_freq_per_up = ExplainableObjectDict()
         mod_obj.nb_user_journeys_in_parallel_during_usage_per_up = ExplainableObjectDict()
         mod_obj.utc_time_intervals_per_up = ExplainableObjectDict()
```

### Comparing `efootprint-2.0.0/efootprint/api_utils/system_to_json.py` & `efootprint-2.0.1/efootprint/api_utils/system_to_json.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/builders/hardware/devices_defaults.py` & `efootprint-2.0.1/efootprint/builders/hardware/devices_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/builders/hardware/network_defaults.py` & `efootprint-2.0.1/efootprint/builders/hardware/network_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/builders/hardware/servers_boaviztapi.py` & `efootprint-2.0.1/efootprint/builders/hardware/servers_boaviztapi.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/builders/hardware/servers_defaults.py` & `efootprint-2.0.1/efootprint/builders/hardware/servers_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/builders/hardware/storage_defaults.py` & `efootprint-2.0.1/efootprint/builders/hardware/storage_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_analysis.py` & `efootprint-2.0.1/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_analysis.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_for_job_defaults.csv` & `efootprint-2.0.1/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_for_job_defaults.csv`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_job_builder.py` & `efootprint-2.0.1/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_job_builder.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_results__raw.csv` & `efootprint-2.0.1/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_results__raw.csv`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/constants/countries.py` & `efootprint-2.0.1/efootprint/constants/countries.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/constants/sources.py` & `efootprint-2.0.1/efootprint/constants/sources.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/core/hardware/device_population.py` & `efootprint-2.0.1/efootprint/core/hardware/device_population.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/core/hardware/hardware_base_classes.py` & `efootprint-2.0.1/efootprint/core/hardware/hardware_base_classes.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/core/hardware/network.py` & `efootprint-2.0.1/efootprint/core/hardware/network.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/core/hardware/servers/autoscaling.py` & `efootprint-2.0.1/efootprint/core/hardware/servers/autoscaling.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/core/hardware/servers/on_premise.py` & `efootprint-2.0.1/efootprint/core/hardware/servers/on_premise.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/core/hardware/servers/server_base_class.py` & `efootprint-2.0.1/efootprint/core/hardware/servers/server_base_class.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/core/hardware/servers/serverless.py` & `efootprint-2.0.1/efootprint/core/hardware/servers/serverless.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/core/hardware/storage.py` & `efootprint-2.0.1/efootprint/core/hardware/storage.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/core/service.py` & `efootprint-2.0.1/efootprint/core/service.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/core/system.py` & `efootprint-2.0.1/efootprint/core/system.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/core/usage/job.py` & `efootprint-2.0.1/efootprint/core/usage/job.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/core/usage/usage_pattern.py` & `efootprint-2.0.1/efootprint/core/usage/usage_pattern.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/core/usage/user_journey.py` & `efootprint-2.0.1/efootprint/core/usage/user_journey.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/core/usage/user_journey_step.py` & `efootprint-2.0.1/efootprint/core/usage/user_journey_step.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/logger.py` & `efootprint-2.0.1/efootprint/logger.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/utils/calculus_graph.py` & `efootprint-2.0.1/efootprint/utils/calculus_graph.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/utils/dev_utils/selenium_screenshot.py` & `efootprint-2.0.1/efootprint/utils/dev_utils/selenium_screenshot.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/utils/graph_tools.py` & `efootprint-2.0.1/efootprint/utils/graph_tools.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/utils/object_relationships_graphs.py` & `efootprint-2.0.1/efootprint/utils/object_relationships_graphs.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/utils/plot_emission_diffs.py` & `efootprint-2.0.1/efootprint/utils/plot_emission_diffs.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/efootprint/utils/tools.py` & `efootprint-2.0.1/efootprint/utils/tools.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.0/pyproject.toml` & `efootprint-2.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.poetry]
 name = "efootprint"
-version = "2.0.0"
+version = "2.0.1"
 description = "Digital service environmental footprint model"
 authors = ["Vincent Villet for Publicis Sapient"]
 readme = "README.md"
 include = ["efootprint/constants/custom_units.txt"]
 
 [tool.black]
 line-length = 120
```

### Comparing `efootprint-2.0.0/PKG-INFO` & `efootprint-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efootprint
-Version: 2.0.0
+Version: 2.0.1
 Summary: Digital service environmental footprint model
 Author: Vincent Villet for Publicis Sapient
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

