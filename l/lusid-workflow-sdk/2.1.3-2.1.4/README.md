# Comparing `tmp/lusid_workflow_sdk-2.1.3.tar.gz` & `tmp/lusid_workflow_sdk-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_workflow_sdk-2.1.3.tar", max compression
+gzip compressed data, was "lusid_workflow_sdk-2.1.4.tar", max compression
```

## Comparing `lusid_workflow_sdk-2.1.3.tar` & `lusid_workflow_sdk-2.1.4.tar`

### file list

```diff
@@ -1,88 +1,95 @@
--rw-r--r--   0        0        0    14402 2024-04-11 10:10:07.845642 lusid_workflow_sdk-2.1.3/README.md
--rw-r--r--   0        0        0     7786 2024-04-11 10:10:07.839642 lusid_workflow_sdk-2.1.3/lusid_workflow/__init__.py
--rw-r--r--   0        0        0      297 2024-04-11 10:10:07.839642 lusid_workflow_sdk-2.1.3/lusid_workflow/api/__init__.py
--rw-r--r--   0        0        0    57597 2024-04-11 10:10:07.839642 lusid_workflow_sdk-2.1.3/lusid_workflow/api/task_definitions_api.py
--rw-r--r--   0        0        0    44655 2024-04-11 10:10:07.839642 lusid_workflow_sdk-2.1.3/lusid_workflow/api/tasks_api.py
--rw-r--r--   0        0        0    61860 2024-04-11 10:10:07.839642 lusid_workflow_sdk-2.1.3/lusid_workflow/api/workers_api.py
--rw-r--r--   0        0        0    30785 2024-04-11 10:10:07.840642 lusid_workflow_sdk-2.1.3/lusid_workflow/api_client.py
--rw-r--r--   0        0        0      852 2024-04-11 10:10:07.840642 lusid_workflow_sdk-2.1.3/lusid_workflow/api_response.py
--rw-r--r--   0        0        0    14451 2024-04-11 10:10:07.839642 lusid_workflow_sdk-2.1.3/lusid_workflow/configuration.py
--rw-r--r--   0        0        0     5339 2024-04-11 10:10:07.840642 lusid_workflow_sdk-2.1.3/lusid_workflow/exceptions.py
--rw-r--r--   0        0        0      587 2024-04-11 10:10:07.840642 lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/__init__.py
--rw-r--r--   0        0        0    30652 2024-04-11 10:10:07.840642 lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/api_client.py
--rw-r--r--   0        0        0     9862 2024-04-11 10:10:07.840642 lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8097 2024-04-11 10:10:07.840642 lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/api_configuration.py
--rw-r--r--   0        0        0     6796 2024-04-11 10:10:07.840642 lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-04-11 10:10:07.840642 lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-04-11 10:10:07.840642 lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12707 2024-04-11 10:10:07.840642 lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/rest.py
--rw-r--r--   0        0        0    11573 2024-04-11 10:10:07.840642 lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-04-11 10:10:07.840642 lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3886 2024-04-11 10:10:07.841642 lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     6460 2024-04-11 10:10:07.839642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/__init__.py
--rw-r--r--   0        0        0     3649 2024-04-11 10:10:07.834642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/action_definition.py
--rw-r--r--   0        0        0     3233 2024-04-11 10:10:07.834642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/action_definition_response.py
--rw-r--r--   0        0        0     6172 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/action_details.py
--rw-r--r--   0        0        0     6643 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/action_details_response.py
--rw-r--r--   0        0        0     5406 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/create_child_task_configuration.py
--rw-r--r--   0        0        0     3165 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/create_child_tasks_action.py
--rw-r--r--   0        0        0     3766 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/create_child_tasks_action_response.py
--rw-r--r--   0        0        0     7468 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/create_task_definition_request.py
--rw-r--r--   0        0        0     4145 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/create_task_request.py
--rw-r--r--   0        0        0     3972 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/create_worker_request.py
--rw-r--r--   0        0        0     3459 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/deleted_entity_response.py
--rw-r--r--   0        0        0     2193 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/fail.py
--rw-r--r--   0        0        0     2505 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/fail_response.py
--rw-r--r--   0        0        0     2878 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/field_mapping.py
--rw-r--r--   0        0        0     2607 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/get_worker_result_response.py
--rw-r--r--   0        0        0     2341 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/health_check.py
--rw-r--r--   0        0        0     2814 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/health_check_response.py
--rw-r--r--   0        0        0     2723 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/initial_state.py
--rw-r--r--   0        0        0     2262 2024-04-11 10:10:07.835642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/link.py
--rw-r--r--   0        0        0     2607 2024-04-11 10:10:07.836642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/luminesce_view.py
--rw-r--r--   0        0        0     2811 2024-04-11 10:10:07.836642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/luminesce_view_response.py
--rw-r--r--   0        0        0     3857 2024-04-11 10:10:07.836642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4693 2024-04-11 10:10:07.836642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     4053 2024-04-11 10:10:07.836642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/paged_resource_list_of_task.py
--rw-r--r--   0        0        0     4174 2024-04-11 10:10:07.836642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/paged_resource_list_of_task_definition.py
--rw-r--r--   0        0        0     4077 2024-04-11 10:10:07.836642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/paged_resource_list_of_worker.py
--rw-r--r--   0        0        0     3317 2024-04-11 10:10:07.836642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/parameter.py
--rw-r--r--   0        0        0     2583 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/parameter_value.py
--rw-r--r--   0        0        0     1869 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/resource_id.py
--rw-r--r--   0        0        0     4013 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/resource_list_of_task.py
--rw-r--r--   0        0        0     2793 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/result_field.py
--rw-r--r--   0        0        0     2293 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/result_matching_pattern.py
--rw-r--r--   0        0        0     5713 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/resultant_child_task_configuration.py
--rw-r--r--   0        0        0     5913 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/run_worker_action.py
--rw-r--r--   0        0        0     6227 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/run_worker_action_response.py
--rw-r--r--   0        0        0     2428 2024-04-11 10:10:07.834642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/run_worker_request.py
--rw-r--r--   0        0        0     2360 2024-04-11 10:10:07.834642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/run_worker_response.py
--rw-r--r--   0        0        0     2541 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/scheduler_job.py
--rw-r--r--   0        0        0     2864 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/scheduler_job_response.py
--rw-r--r--   0        0        0     2116 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/sleep.py
--rw-r--r--   0        0        0     2172 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/sleep_response.py
--rw-r--r--   0        0        0     4397 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/stack.py
--rw-r--r--   0        0        0     8353 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/task.py
--rw-r--r--   0        0        0     7864 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/task_definition.py
--rw-r--r--   0        0        0     2090 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/task_definition_version.py
--rw-r--r--   0        0        0     2483 2024-04-11 10:10:07.837642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/task_field_definition.py
--rw-r--r--   0        0        0     2546 2024-04-11 10:10:07.838642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/task_instance_field.py
--rw-r--r--   0        0        0     2279 2024-04-11 10:10:07.838642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/task_state_definition.py
--rw-r--r--   0        0        0     3415 2024-04-11 10:10:07.838642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/task_summary.py
--rw-r--r--   0        0        0     4806 2024-04-11 10:10:07.838642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/task_transition_definition.py
--rw-r--r--   0        0        0     2728 2024-04-11 10:10:07.838642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/transition_trigger_definition.py
--rw-r--r--   0        0        0     2716 2024-04-11 10:10:07.838642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/trigger_parent_task_action.py
--rw-r--r--   0        0        0     2910 2024-04-11 10:10:07.838642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/trigger_parent_task_action_response.py
--rw-r--r--   0        0        0     1951 2024-04-11 10:10:07.838642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/trigger_schema.py
--rw-r--r--   0        0        0     7130 2024-04-11 10:10:07.838642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/update_task_definition_request.py
--rw-r--r--   0        0        0     3588 2024-04-11 10:10:07.838642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/update_task_request.py
--rw-r--r--   0        0        0     3579 2024-04-11 10:10:07.838642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/update_worker_request.py
--rw-r--r--   0        0        0     5124 2024-04-11 10:10:07.838642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/version_info.py
--rw-r--r--   0        0        0     6137 2024-04-11 10:10:07.838642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/worker.py
--rw-r--r--   0        0        0     7051 2024-04-11 10:10:07.839642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/worker_configuration.py
--rw-r--r--   0        0        0     7753 2024-04-11 10:10:07.839642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/worker_configuration_response.py
--rw-r--r--   0        0        0     4204 2024-04-11 10:10:07.839642 lusid_workflow_sdk-2.1.3/lusid_workflow/models/worker_status_triggers.py
--rw-r--r--   0        0        0        0 2024-04-11 10:10:07.839642 lusid_workflow_sdk-2.1.3/lusid_workflow/py.typed
--rw-r--r--   0        0        0    10160 2024-04-11 10:10:07.840642 lusid_workflow_sdk-2.1.3/lusid_workflow/rest.py
--rw-r--r--   0        0        0      855 2024-04-11 10:10:07.845642 lusid_workflow_sdk-2.1.3/pyproject.toml
--rw-r--r--   0        0        0    15447 1970-01-01 00:00:00.000000 lusid_workflow_sdk-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0    12899 2024-04-12 14:47:36.769232 lusid_workflow_sdk-2.1.4/README.md
+-rw-r--r--   0        0        0     8569 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/__init__.py
+-rw-r--r--   0        0        0      406 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/api/__init__.py
+-rw-r--r--   0        0        0     7534 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/api/application_metadata_api.py
+-rw-r--r--   0        0        0    57597 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/api/task_definitions_api.py
+-rw-r--r--   0        0        0    44655 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/api/tasks_api.py
+-rw-r--r--   0        0        0    61860 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/api/workers_api.py
+-rw-r--r--   0        0        0    30785 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/api_response.py
+-rw-r--r--   0        0        0    14451 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/configuration.py
+-rw-r--r--   0        0        0     5339 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/exceptions.py
+-rw-r--r--   0        0        0      587 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/__init__.py
+-rw-r--r--   0        0        0    30652 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/api_client.py
+-rw-r--r--   0        0        0     9862 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8097 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6796 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12707 2024-04-12 14:47:36.764232 lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/rest.py
+-rw-r--r--   0        0        0    11573 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-12 14:47:36.765232 lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3886 2024-04-12 14:47:36.765232 lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     7134 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/__init__.py
+-rw-r--r--   0        0        0     3903 2024-04-12 14:47:36.758232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4846 2024-04-12 14:47:36.758232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     3649 2024-04-12 14:47:36.758232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/action_definition.py
+-rw-r--r--   0        0        0     3233 2024-04-12 14:47:36.758232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/action_definition_response.py
+-rw-r--r--   0        0        0     6172 2024-04-12 14:47:36.758232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/action_details.py
+-rw-r--r--   0        0        0     6643 2024-04-12 14:47:36.758232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/action_details_response.py
+-rw-r--r--   0        0        0     2070 2024-04-12 14:47:36.758232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/action_id.py
+-rw-r--r--   0        0        0     5406 2024-04-12 14:47:36.758232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/create_child_task_configuration.py
+-rw-r--r--   0        0        0     3165 2024-04-12 14:47:36.759232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/create_child_tasks_action.py
+-rw-r--r--   0        0        0     3766 2024-04-12 14:47:36.759232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/create_child_tasks_action_response.py
+-rw-r--r--   0        0        0     7468 2024-04-12 14:47:36.759232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/create_task_definition_request.py
+-rw-r--r--   0        0        0     4145 2024-04-12 14:47:36.759232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/create_task_request.py
+-rw-r--r--   0        0        0     3972 2024-04-12 14:47:36.759232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/create_worker_request.py
+-rw-r--r--   0        0        0     3459 2024-04-12 14:47:36.759232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/deleted_entity_response.py
+-rw-r--r--   0        0        0     2193 2024-04-12 14:47:36.759232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/fail.py
+-rw-r--r--   0        0        0     2505 2024-04-12 14:47:36.759232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/fail_response.py
+-rw-r--r--   0        0        0     2878 2024-04-12 14:47:36.759232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/field_mapping.py
+-rw-r--r--   0        0        0     2607 2024-04-12 14:47:36.759232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/get_worker_result_response.py
+-rw-r--r--   0        0        0     2341 2024-04-12 14:47:36.759232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/health_check.py
+-rw-r--r--   0        0        0     2814 2024-04-12 14:47:36.759232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/health_check_response.py
+-rw-r--r--   0        0        0     3180 2024-04-12 14:47:36.760232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3105 2024-04-12 14:47:36.760232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2723 2024-04-12 14:47:36.760232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/initial_state.py
+-rw-r--r--   0        0        0     2262 2024-04-12 14:47:36.760232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/link.py
+-rw-r--r--   0        0        0     2607 2024-04-12 14:47:36.760232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/luminesce_view.py
+-rw-r--r--   0        0        0     2811 2024-04-12 14:47:36.760232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/luminesce_view_response.py
+-rw-r--r--   0        0        0     3857 2024-04-12 14:47:36.760232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4693 2024-04-12 14:47:36.760232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     4053 2024-04-12 14:47:36.760232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/paged_resource_list_of_task.py
+-rw-r--r--   0        0        0     4174 2024-04-12 14:47:36.760232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/paged_resource_list_of_task_definition.py
+-rw-r--r--   0        0        0     4077 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/paged_resource_list_of_worker.py
+-rw-r--r--   0        0        0     3317 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/parameter.py
+-rw-r--r--   0        0        0     2583 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/parameter_value.py
+-rw-r--r--   0        0        0     1869 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/resource_id.py
+-rw-r--r--   0        0        0     4255 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4013 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/resource_list_of_task.py
+-rw-r--r--   0        0        0     2793 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/result_field.py
+-rw-r--r--   0        0        0     2293 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/result_matching_pattern.py
+-rw-r--r--   0        0        0     5713 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/resultant_child_task_configuration.py
+-rw-r--r--   0        0        0     5913 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/run_worker_action.py
+-rw-r--r--   0        0        0     6227 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/run_worker_action_response.py
+-rw-r--r--   0        0        0     2428 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/run_worker_request.py
+-rw-r--r--   0        0        0     2360 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/run_worker_response.py
+-rw-r--r--   0        0        0     2541 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/scheduler_job.py
+-rw-r--r--   0        0        0     2864 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/scheduler_job_response.py
+-rw-r--r--   0        0        0     2116 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/sleep.py
+-rw-r--r--   0        0        0     2172 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/sleep_response.py
+-rw-r--r--   0        0        0     4397 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/stack.py
+-rw-r--r--   0        0        0     8353 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/task.py
+-rw-r--r--   0        0        0     7864 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/task_definition.py
+-rw-r--r--   0        0        0     2090 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/task_definition_version.py
+-rw-r--r--   0        0        0     2483 2024-04-12 14:47:36.761232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/task_field_definition.py
+-rw-r--r--   0        0        0     2546 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/task_instance_field.py
+-rw-r--r--   0        0        0     2279 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/task_state_definition.py
+-rw-r--r--   0        0        0     3415 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/task_summary.py
+-rw-r--r--   0        0        0     4806 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/task_transition_definition.py
+-rw-r--r--   0        0        0     2728 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/transition_trigger_definition.py
+-rw-r--r--   0        0        0     2716 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/trigger_parent_task_action.py
+-rw-r--r--   0        0        0     2910 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/trigger_parent_task_action_response.py
+-rw-r--r--   0        0        0     1951 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/trigger_schema.py
+-rw-r--r--   0        0        0     7130 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/update_task_definition_request.py
+-rw-r--r--   0        0        0     3588 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/update_task_request.py
+-rw-r--r--   0        0        0     3579 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/update_worker_request.py
+-rw-r--r--   0        0        0     5124 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/version_info.py
+-rw-r--r--   0        0        0     6137 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/worker.py
+-rw-r--r--   0        0        0     7051 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/worker_configuration.py
+-rw-r--r--   0        0        0     7753 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/worker_configuration_response.py
+-rw-r--r--   0        0        0     4204 2024-04-12 14:47:36.762232 lusid_workflow_sdk-2.1.4/lusid_workflow/models/worker_status_triggers.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/py.typed
+-rw-r--r--   0        0        0    10160 2024-04-12 14:47:36.763232 lusid_workflow_sdk-2.1.4/lusid_workflow/rest.py
+-rw-r--r--   0        0        0      855 2024-04-12 14:47:36.769232 lusid_workflow_sdk-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0    13944 1970-01-01 00:00:00.000000 lusid_workflow_sdk-2.1.4/PKG-INFO
```

### Comparing `lusid_workflow_sdk-2.1.3/README.md` & `lusid_workflow_sdk-2.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.884
-- Package version: 2.1.3
+- API version: 0.1.891
+- Package version: 2.1.4
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -130,15 +130,15 @@
 import lusid_workflow
 from lusid_workflow.exceptions import ApiException
 from pprint import pprint
 
 import os
 from lusid_workflow import (
     ApiClientFactory,
-    TaskDefinitionsApi,
+    ApplicationMetadataApi,
     EnvironmentVariablesConfigurationLoader,
     SecretsFileConfigurationLoader,
     ArgsConfigurationLoader
 )
 
 # Use the lusid_workflow ApiClientFactory to build Api instances with a configured api client
 # By default this will read config from environment variables
@@ -166,33 +166,33 @@
 # in accordance with the API server security policy.
 
 
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
-    api_instance = api_client_factory.build(TaskDefinitionsApi)
-    create_task_definition_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example TaskDefinition","description":"Test","states":[{"name":"Submitted"},{"name":"InProgress"},{"name":"SendingSurvey"},{"name":"Done"},{"name":"SurveyNotSent"},{"name":"NotDone"}],"fieldSchema":[{"name":"clientId","type":"String"},{"name":"assignee","type":"String"},{"name":"resolutionDetail","type":"String"}],"initialState":{"name":"Submitted","requiredFields":["clientId"]},"triggers":[{"name":"start","trigger":{"type":"External"}},{"name":"cancel","trigger":{"type":"External"}},{"name":"resolve","trigger":{"type":"External"}},{"name":"timeout","trigger":{"type":"External"}},{"name":"success","trigger":{"type":"External"}},{"name":"failure","trigger":{"type":"External"}}],"transitions":[{"fromState":"Submitted","toState":"InProgress","trigger":"start","guard":"fields['assignee'] exists AND fields['assignee'] NOT eq ''"},{"fromState":"InProgress","toState":"SendingSurvey","trigger":"resolve","guard":"fields['resolutionDetail'] exists AND fields['resolutionDetail'] NOT eq ''","action":"health-check"},{"fromState":"SendingSurvey","toState":"Done","trigger":"success"},{"fromState":"SendingSurvey","toState":"SurveyNotSent","trigger":"failure"},{"fromState":"SendingSurvey","toState":"NotDone","trigger":"timeout"},{"fromState":"InProgress","toState":"NotDone","trigger":"cancel","guard":"fields['cancellationDetail'] exists AND fields['cancellationDetail'] NOT eq ''"}],"actions":[{"name":"health-check","runAsUserId":"user-id","actionDetails":{"type":"RunWorker","workerId":{"scope":"Health","code":"HealthCheckWorker"},"workerAsAt":"2022-01-01T01:02:03.0000000+00:00","workerParameters":{},"workerStatusTriggers":{"started":null,"completedWithResults":null,"completedNoResults":null,"failedToStart":null,"failedToComplete":null},"childTaskConfigurations":[{"taskDefinitionId":{"scope":"AAA","code":"BBB"},"mapStackingKeyFrom":null,"childTaskFields":{"assignee":{"mapFrom":"foo","setTo":"bar"}},"resultMatchingPattern":null,"taskDefinitionAsAt":null,"initialTrigger":"test-trigger"}]}}]} # CreateTaskDefinitionRequest | The data to create a Task Definition
+    api_instance = api_client_factory.build(ApplicationMetadataApi)
 
     try:
-        # [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition
-        api_response = await api_instance.create_task_definition(create_task_definition_request)
-        print("The response of TaskDefinitionsApi->create_task_definition:\n")
+        # [EXPERIMENTAL] ListAccessControlledResources: Get resources available for access control
+        api_response = await api_instance.list_access_controlled_resources()
+        print("The response of ApplicationMetadataApi->list_access_controlled_resources:\n")
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling TaskDefinitionsApi->create_task_definition: %s\n" % e)
+        print("Exception when calling ApplicationMetadataApi->list_access_controlled_resources: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://fbn-prd.lusid.com/workflow*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EXPERIMENTAL] ListAccessControlledResources: Get resources available for access control
 *TaskDefinitionsApi* | [**create_task_definition**](docs/TaskDefinitionsApi.md#create_task_definition) | **POST** /api/taskdefinitions | [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition
 *TaskDefinitionsApi* | [**delete_task_definition**](docs/TaskDefinitionsApi.md#delete_task_definition) | **DELETE** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] DeleteTaskDefinition: Delete a Task Definition
 *TaskDefinitionsApi* | [**get_task_definition**](docs/TaskDefinitionsApi.md#get_task_definition) | **GET** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] GetTaskDefinition: Get a Task Definition
 *TaskDefinitionsApi* | [**list_task_definitions**](docs/TaskDefinitionsApi.md#list_task_definitions) | **GET** /api/taskdefinitions | [EXPERIMENTAL] ListTaskDefinitions: List Task Definitions
 *TaskDefinitionsApi* | [**list_tasks_for_task_definition**](docs/TaskDefinitionsApi.md#list_tasks_for_task_definition) | **GET** /api/taskdefinitions/{scope}/{code}/tasks | [EXPERIMENTAL] ListTasksForTaskDefinition: List Tasks for a Task Definition
 *TaskDefinitionsApi* | [**update_task_definition**](docs/TaskDefinitionsApi.md#update_task_definition) | **PUT** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] UpdateTaskDefinition: Update an existing Task Definition
 *TasksApi* | [**create_task**](docs/TasksApi.md#create_task) | **POST** /api/tasks | [EXPERIMENTAL] CreateTask: Create a new Task
@@ -207,43 +207,49 @@
 *WorkersApi* | [**list_workers**](docs/WorkersApi.md#list_workers) | **GET** /api/workers | [EXPERIMENTAL] ListWorkers: List Workers
 *WorkersApi* | [**run_worker**](docs/WorkersApi.md#run_worker) | **POST** /api/workers/{scope}/{code}/$run | [EXPERIMENTAL] RunWorker: Run a Worker
 *WorkersApi* | [**update_worker**](docs/WorkersApi.md#update_worker) | **PUT** /api/workers/{scope}/{code} | [EXPERIMENTAL] UpdateWorker: Update a Worker
 
 
 ## Documentation For Models
 
+ - [AccessControlledAction](docs/AccessControlledAction.md)
+ - [AccessControlledResource](docs/AccessControlledResource.md)
  - [ActionDefinition](docs/ActionDefinition.md)
  - [ActionDefinitionResponse](docs/ActionDefinitionResponse.md)
  - [ActionDetails](docs/ActionDetails.md)
  - [ActionDetailsResponse](docs/ActionDetailsResponse.md)
+ - [ActionId](docs/ActionId.md)
  - [CreateChildTaskConfiguration](docs/CreateChildTaskConfiguration.md)
  - [CreateChildTasksAction](docs/CreateChildTasksAction.md)
  - [CreateChildTasksActionResponse](docs/CreateChildTasksActionResponse.md)
  - [CreateTaskDefinitionRequest](docs/CreateTaskDefinitionRequest.md)
  - [CreateTaskRequest](docs/CreateTaskRequest.md)
  - [CreateWorkerRequest](docs/CreateWorkerRequest.md)
  - [DeletedEntityResponse](docs/DeletedEntityResponse.md)
  - [Fail](docs/Fail.md)
  - [FailResponse](docs/FailResponse.md)
  - [FieldMapping](docs/FieldMapping.md)
  - [GetWorkerResultResponse](docs/GetWorkerResultResponse.md)
  - [HealthCheck](docs/HealthCheck.md)
  - [HealthCheckResponse](docs/HealthCheckResponse.md)
+ - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
+ - [IdentifierPartSchema](docs/IdentifierPartSchema.md)
  - [InitialState](docs/InitialState.md)
  - [Link](docs/Link.md)
  - [LuminesceView](docs/LuminesceView.md)
  - [LuminesceViewResponse](docs/LuminesceViewResponse.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
  - [PagedResourceListOfTask](docs/PagedResourceListOfTask.md)
  - [PagedResourceListOfTaskDefinition](docs/PagedResourceListOfTaskDefinition.md)
  - [PagedResourceListOfWorker](docs/PagedResourceListOfWorker.md)
  - [Parameter](docs/Parameter.md)
  - [ParameterValue](docs/ParameterValue.md)
  - [ResourceId](docs/ResourceId.md)
+ - [ResourceListOfAccessControlledResource](docs/ResourceListOfAccessControlledResource.md)
  - [ResourceListOfTask](docs/ResourceListOfTask.md)
  - [ResultField](docs/ResultField.md)
  - [ResultMatchingPattern](docs/ResultMatchingPattern.md)
  - [ResultantChildTaskConfiguration](docs/ResultantChildTaskConfiguration.md)
  - [RunWorkerAction](docs/RunWorkerAction.md)
  - [RunWorkerActionResponse](docs/RunWorkerActionResponse.md)
  - [RunWorkerRequest](docs/RunWorkerRequest.md)
```

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/__init__.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,56 +13,63 @@
     Do not edit the class manually.
 """
 
 
 from __future__ import absolute_import
 
 # import apis into sdk package
+from lusid_workflow.api.application_metadata_api import ApplicationMetadataApi
 from lusid_workflow.api.task_definitions_api import TaskDefinitionsApi
 from lusid_workflow.api.tasks_api import TasksApi
 from lusid_workflow.api.workers_api import WorkersApi
 
 # import ApiClient
 from lusid_workflow.api_client import ApiClient
 from lusid_workflow.configuration import Configuration
 from lusid_workflow.exceptions import OpenApiException
 from lusid_workflow.exceptions import ApiTypeError
 from lusid_workflow.exceptions import ApiValueError
 from lusid_workflow.exceptions import ApiKeyError
 from lusid_workflow.exceptions import ApiException
 # import models into sdk package
+from lusid_workflow.models.access_controlled_action import AccessControlledAction
+from lusid_workflow.models.access_controlled_resource import AccessControlledResource
 from lusid_workflow.models.action_definition import ActionDefinition
 from lusid_workflow.models.action_definition_response import ActionDefinitionResponse
 from lusid_workflow.models.action_details import ActionDetails
 from lusid_workflow.models.action_details_response import ActionDetailsResponse
+from lusid_workflow.models.action_id import ActionId
 from lusid_workflow.models.create_child_task_configuration import CreateChildTaskConfiguration
 from lusid_workflow.models.create_child_tasks_action import CreateChildTasksAction
 from lusid_workflow.models.create_child_tasks_action_response import CreateChildTasksActionResponse
 from lusid_workflow.models.create_task_definition_request import CreateTaskDefinitionRequest
 from lusid_workflow.models.create_task_request import CreateTaskRequest
 from lusid_workflow.models.create_worker_request import CreateWorkerRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
 from lusid_workflow.models.fail import Fail
 from lusid_workflow.models.fail_response import FailResponse
 from lusid_workflow.models.field_mapping import FieldMapping
 from lusid_workflow.models.get_worker_result_response import GetWorkerResultResponse
 from lusid_workflow.models.health_check import HealthCheck
 from lusid_workflow.models.health_check_response import HealthCheckResponse
+from lusid_workflow.models.id_selector_definition import IdSelectorDefinition
+from lusid_workflow.models.identifier_part_schema import IdentifierPartSchema
 from lusid_workflow.models.initial_state import InitialState
 from lusid_workflow.models.link import Link
 from lusid_workflow.models.luminesce_view import LuminesceView
 from lusid_workflow.models.luminesce_view_response import LuminesceViewResponse
 from lusid_workflow.models.lusid_problem_details import LusidProblemDetails
 from lusid_workflow.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from lusid_workflow.models.paged_resource_list_of_task import PagedResourceListOfTask
 from lusid_workflow.models.paged_resource_list_of_task_definition import PagedResourceListOfTaskDefinition
 from lusid_workflow.models.paged_resource_list_of_worker import PagedResourceListOfWorker
 from lusid_workflow.models.parameter import Parameter
 from lusid_workflow.models.parameter_value import ParameterValue
 from lusid_workflow.models.resource_id import ResourceId
+from lusid_workflow.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 from lusid_workflow.models.resource_list_of_task import ResourceListOfTask
 from lusid_workflow.models.result_field import ResultField
 from lusid_workflow.models.result_matching_pattern import ResultMatchingPattern
 from lusid_workflow.models.resultant_child_task_configuration import ResultantChildTaskConfiguration
 from lusid_workflow.models.run_worker_action import RunWorkerAction
 from lusid_workflow.models.run_worker_action_response import RunWorkerActionResponse
 from lusid_workflow.models.run_worker_request import RunWorkerRequest
@@ -102,46 +109,53 @@
     EnvironmentVariablesConfigurationLoader,
     ArgsConfigurationLoader,
     SyncApiClient
 )
 
 
 __all__ = [
+    "ApplicationMetadataApi",
     "TaskDefinitionsApi",
     "TasksApi",
     "WorkersApi",
+    "AccessControlledAction",
+    "AccessControlledResource",
     "ActionDefinition",
     "ActionDefinitionResponse",
     "ActionDetails",
     "ActionDetailsResponse",
+    "ActionId",
     "CreateChildTaskConfiguration",
     "CreateChildTasksAction",
     "CreateChildTasksActionResponse",
     "CreateTaskDefinitionRequest",
     "CreateTaskRequest",
     "CreateWorkerRequest",
     "DeletedEntityResponse",
     "Fail",
     "FailResponse",
     "FieldMapping",
     "GetWorkerResultResponse",
     "HealthCheck",
     "HealthCheckResponse",
+    "IdSelectorDefinition",
+    "IdentifierPartSchema",
     "InitialState",
     "Link",
     "LuminesceView",
     "LuminesceViewResponse",
     "LusidProblemDetails",
     "LusidValidationProblemDetails",
     "PagedResourceListOfTask",
     "PagedResourceListOfTaskDefinition",
     "PagedResourceListOfWorker",
     "Parameter",
     "ParameterValue",
     "ResourceId",
+    "ResourceListOfAccessControlledResource",
     "ResourceListOfTask",
     "ResultField",
     "ResultMatchingPattern",
     "ResultantChildTaskConfiguration",
     "RunWorkerAction",
     "RunWorkerActionResponse",
     "RunWorkerRequest",
```

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/api/task_definitions_api.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/api/task_definitions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/api/tasks_api.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/api/workers_api.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/api/workers_api.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/api_client.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/api_response.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/api_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/configuration.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid_workflow-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.884\n"\
+               "Version of the API: 0.1.891\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/exceptions.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/__init__.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/api_client.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/api_client_factory.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/api_configuration.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/configuration_loaders.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/proxy_config.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/refreshing_token.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/rest.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/retry.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/socket_keep_alive.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/extensions/tcp_keep_alive_connector.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/__init__.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,43 +10,49 @@
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 # import models into model package
+from lusid_workflow.models.access_controlled_action import AccessControlledAction
+from lusid_workflow.models.access_controlled_resource import AccessControlledResource
 from lusid_workflow.models.action_definition import ActionDefinition
 from lusid_workflow.models.action_definition_response import ActionDefinitionResponse
 from lusid_workflow.models.action_details import ActionDetails
 from lusid_workflow.models.action_details_response import ActionDetailsResponse
+from lusid_workflow.models.action_id import ActionId
 from lusid_workflow.models.create_child_task_configuration import CreateChildTaskConfiguration
 from lusid_workflow.models.create_child_tasks_action import CreateChildTasksAction
 from lusid_workflow.models.create_child_tasks_action_response import CreateChildTasksActionResponse
 from lusid_workflow.models.create_task_definition_request import CreateTaskDefinitionRequest
 from lusid_workflow.models.create_task_request import CreateTaskRequest
 from lusid_workflow.models.create_worker_request import CreateWorkerRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
 from lusid_workflow.models.fail import Fail
 from lusid_workflow.models.fail_response import FailResponse
 from lusid_workflow.models.field_mapping import FieldMapping
 from lusid_workflow.models.get_worker_result_response import GetWorkerResultResponse
 from lusid_workflow.models.health_check import HealthCheck
 from lusid_workflow.models.health_check_response import HealthCheckResponse
+from lusid_workflow.models.id_selector_definition import IdSelectorDefinition
+from lusid_workflow.models.identifier_part_schema import IdentifierPartSchema
 from lusid_workflow.models.initial_state import InitialState
 from lusid_workflow.models.link import Link
 from lusid_workflow.models.luminesce_view import LuminesceView
 from lusid_workflow.models.luminesce_view_response import LuminesceViewResponse
 from lusid_workflow.models.lusid_problem_details import LusidProblemDetails
 from lusid_workflow.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from lusid_workflow.models.paged_resource_list_of_task import PagedResourceListOfTask
 from lusid_workflow.models.paged_resource_list_of_task_definition import PagedResourceListOfTaskDefinition
 from lusid_workflow.models.paged_resource_list_of_worker import PagedResourceListOfWorker
 from lusid_workflow.models.parameter import Parameter
 from lusid_workflow.models.parameter_value import ParameterValue
 from lusid_workflow.models.resource_id import ResourceId
+from lusid_workflow.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 from lusid_workflow.models.resource_list_of_task import ResourceListOfTask
 from lusid_workflow.models.result_field import ResultField
 from lusid_workflow.models.result_matching_pattern import ResultMatchingPattern
 from lusid_workflow.models.resultant_child_task_configuration import ResultantChildTaskConfiguration
 from lusid_workflow.models.run_worker_action import RunWorkerAction
 from lusid_workflow.models.run_worker_action_response import RunWorkerActionResponse
 from lusid_workflow.models.run_worker_request import RunWorkerRequest
@@ -75,43 +81,49 @@
 from lusid_workflow.models.worker import Worker
 from lusid_workflow.models.worker_configuration import WorkerConfiguration
 from lusid_workflow.models.worker_configuration_response import WorkerConfigurationResponse
 from lusid_workflow.models.worker_status_triggers import WorkerStatusTriggers
 
 
 __all__ = [
+    "AccessControlledAction",
+    "AccessControlledResource",
     "ActionDefinition",
     "ActionDefinitionResponse",
     "ActionDetails",
     "ActionDetailsResponse",
+    "ActionId",
     "CreateChildTaskConfiguration",
     "CreateChildTasksAction",
     "CreateChildTasksActionResponse",
     "CreateTaskDefinitionRequest",
     "CreateTaskRequest",
     "CreateWorkerRequest",
     "DeletedEntityResponse",
     "Fail",
     "FailResponse",
     "FieldMapping",
     "GetWorkerResultResponse",
     "HealthCheck",
     "HealthCheckResponse",
+    "IdSelectorDefinition",
+    "IdentifierPartSchema",
     "InitialState",
     "Link",
     "LuminesceView",
     "LuminesceViewResponse",
     "LusidProblemDetails",
     "LusidValidationProblemDetails",
     "PagedResourceListOfTask",
     "PagedResourceListOfTaskDefinition",
     "PagedResourceListOfWorker",
     "Parameter",
     "ParameterValue",
     "ResourceId",
+    "ResourceListOfAccessControlledResource",
     "ResourceListOfTask",
     "ResultField",
     "ResultMatchingPattern",
     "ResultantChildTaskConfiguration",
     "RunWorkerAction",
     "RunWorkerActionResponse",
     "RunWorkerRequest",
```

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/action_definition.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/action_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/action_definition_response.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/action_definition_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/action_details.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/action_details.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/action_details_response.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/action_details_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/create_child_task_configuration.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/create_child_task_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/create_child_tasks_action.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/create_child_tasks_action.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/create_child_tasks_action_response.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/create_child_tasks_action_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/create_task_definition_request.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/create_task_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/create_task_request.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/create_task_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/create_worker_request.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/create_worker_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/deleted_entity_response.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/deleted_entity_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/fail.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/fail.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/fail_response.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/fail_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/field_mapping.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/field_mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/get_worker_result_response.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/get_worker_result_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/health_check.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/health_check.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/health_check_response.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/health_check_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/initial_state.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/initial_state.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/link.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/link.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/luminesce_view.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/luminesce_view.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/luminesce_view_response.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/luminesce_view_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/lusid_problem_details.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/lusid_validation_problem_details.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/paged_resource_list_of_task.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/paged_resource_list_of_task.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/paged_resource_list_of_task_definition.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/paged_resource_list_of_task_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/paged_resource_list_of_worker.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/paged_resource_list_of_worker.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/parameter.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/parameter_value.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/parameter_value.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/resource_id.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/resource_list_of_task.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/resource_list_of_task.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/result_field.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/result_field.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/result_matching_pattern.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/result_matching_pattern.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/resultant_child_task_configuration.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/resultant_child_task_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/run_worker_action.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/run_worker_action.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/run_worker_action_response.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/run_worker_action_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/run_worker_request.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/run_worker_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/run_worker_response.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/run_worker_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/scheduler_job.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/scheduler_job.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/scheduler_job_response.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/scheduler_job_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/sleep.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/sleep.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/sleep_response.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/sleep_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/stack.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/stack.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/task.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/task.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/task_definition.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/task_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/task_definition_version.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/task_definition_version.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/task_field_definition.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/task_field_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/task_instance_field.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/task_instance_field.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/task_state_definition.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/task_state_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/task_summary.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/task_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/task_transition_definition.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/task_transition_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/transition_trigger_definition.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/transition_trigger_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/trigger_parent_task_action.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/trigger_parent_task_action.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/trigger_parent_task_action_response.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/trigger_parent_task_action_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/trigger_schema.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/trigger_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/update_task_definition_request.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/update_task_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/update_task_request.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/update_task_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/update_worker_request.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/update_worker_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/version_info.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/version_info.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/worker.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/worker.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/worker_configuration.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/worker_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/worker_configuration_response.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/worker_configuration_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/models/worker_status_triggers.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/models/worker_status_triggers.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/lusid_workflow/rest.py` & `lusid_workflow_sdk-2.1.4/lusid_workflow/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.3/pyproject.toml` & `lusid_workflow_sdk-2.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-workflow-sdk"
-version = "2.1.3"
+version = "2.1.4"
 description = "FINBOURNE Workflow API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/workflow-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Workflow API", "lusid-workflow-sdk"]
 packages = [
```

### Comparing `lusid_workflow_sdk-2.1.3/PKG-INFO` & `lusid_workflow_sdk-2.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-workflow-sdk
-Version: 2.1.3
+Version: 2.1.4
 Summary: FINBOURNE Workflow API
 Home-page: https://github.com/finbourne/workflow-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Workflow API,lusid-workflow-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.884
-- Package version: 2.1.3
+- API version: 0.1.891
+- Package version: 2.1.4
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -156,15 +156,15 @@
 import lusid_workflow
 from lusid_workflow.exceptions import ApiException
 from pprint import pprint
 
 import os
 from lusid_workflow import (
     ApiClientFactory,
-    TaskDefinitionsApi,
+    ApplicationMetadataApi,
     EnvironmentVariablesConfigurationLoader,
     SecretsFileConfigurationLoader,
     ArgsConfigurationLoader
 )
 
 # Use the lusid_workflow ApiClientFactory to build Api instances with a configured api client
 # By default this will read config from environment variables
@@ -192,33 +192,33 @@
 # in accordance with the API server security policy.
 
 
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
-    api_instance = api_client_factory.build(TaskDefinitionsApi)
-    create_task_definition_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example TaskDefinition","description":"Test","states":[{"name":"Submitted"},{"name":"InProgress"},{"name":"SendingSurvey"},{"name":"Done"},{"name":"SurveyNotSent"},{"name":"NotDone"}],"fieldSchema":[{"name":"clientId","type":"String"},{"name":"assignee","type":"String"},{"name":"resolutionDetail","type":"String"}],"initialState":{"name":"Submitted","requiredFields":["clientId"]},"triggers":[{"name":"start","trigger":{"type":"External"}},{"name":"cancel","trigger":{"type":"External"}},{"name":"resolve","trigger":{"type":"External"}},{"name":"timeout","trigger":{"type":"External"}},{"name":"success","trigger":{"type":"External"}},{"name":"failure","trigger":{"type":"External"}}],"transitions":[{"fromState":"Submitted","toState":"InProgress","trigger":"start","guard":"fields['assignee'] exists AND fields['assignee'] NOT eq ''"},{"fromState":"InProgress","toState":"SendingSurvey","trigger":"resolve","guard":"fields['resolutionDetail'] exists AND fields['resolutionDetail'] NOT eq ''","action":"health-check"},{"fromState":"SendingSurvey","toState":"Done","trigger":"success"},{"fromState":"SendingSurvey","toState":"SurveyNotSent","trigger":"failure"},{"fromState":"SendingSurvey","toState":"NotDone","trigger":"timeout"},{"fromState":"InProgress","toState":"NotDone","trigger":"cancel","guard":"fields['cancellationDetail'] exists AND fields['cancellationDetail'] NOT eq ''"}],"actions":[{"name":"health-check","runAsUserId":"user-id","actionDetails":{"type":"RunWorker","workerId":{"scope":"Health","code":"HealthCheckWorker"},"workerAsAt":"2022-01-01T01:02:03.0000000+00:00","workerParameters":{},"workerStatusTriggers":{"started":null,"completedWithResults":null,"completedNoResults":null,"failedToStart":null,"failedToComplete":null},"childTaskConfigurations":[{"taskDefinitionId":{"scope":"AAA","code":"BBB"},"mapStackingKeyFrom":null,"childTaskFields":{"assignee":{"mapFrom":"foo","setTo":"bar"}},"resultMatchingPattern":null,"taskDefinitionAsAt":null,"initialTrigger":"test-trigger"}]}}]} # CreateTaskDefinitionRequest | The data to create a Task Definition
+    api_instance = api_client_factory.build(ApplicationMetadataApi)
 
     try:
-        # [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition
-        api_response = await api_instance.create_task_definition(create_task_definition_request)
-        print("The response of TaskDefinitionsApi->create_task_definition:\n")
+        # [EXPERIMENTAL] ListAccessControlledResources: Get resources available for access control
+        api_response = await api_instance.list_access_controlled_resources()
+        print("The response of ApplicationMetadataApi->list_access_controlled_resources:\n")
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling TaskDefinitionsApi->create_task_definition: %s\n" % e)
+        print("Exception when calling ApplicationMetadataApi->list_access_controlled_resources: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://fbn-prd.lusid.com/workflow*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EXPERIMENTAL] ListAccessControlledResources: Get resources available for access control
 *TaskDefinitionsApi* | [**create_task_definition**](docs/TaskDefinitionsApi.md#create_task_definition) | **POST** /api/taskdefinitions | [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition
 *TaskDefinitionsApi* | [**delete_task_definition**](docs/TaskDefinitionsApi.md#delete_task_definition) | **DELETE** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] DeleteTaskDefinition: Delete a Task Definition
 *TaskDefinitionsApi* | [**get_task_definition**](docs/TaskDefinitionsApi.md#get_task_definition) | **GET** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] GetTaskDefinition: Get a Task Definition
 *TaskDefinitionsApi* | [**list_task_definitions**](docs/TaskDefinitionsApi.md#list_task_definitions) | **GET** /api/taskdefinitions | [EXPERIMENTAL] ListTaskDefinitions: List Task Definitions
 *TaskDefinitionsApi* | [**list_tasks_for_task_definition**](docs/TaskDefinitionsApi.md#list_tasks_for_task_definition) | **GET** /api/taskdefinitions/{scope}/{code}/tasks | [EXPERIMENTAL] ListTasksForTaskDefinition: List Tasks for a Task Definition
 *TaskDefinitionsApi* | [**update_task_definition**](docs/TaskDefinitionsApi.md#update_task_definition) | **PUT** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] UpdateTaskDefinition: Update an existing Task Definition
 *TasksApi* | [**create_task**](docs/TasksApi.md#create_task) | **POST** /api/tasks | [EXPERIMENTAL] CreateTask: Create a new Task
@@ -233,43 +233,49 @@
 *WorkersApi* | [**list_workers**](docs/WorkersApi.md#list_workers) | **GET** /api/workers | [EXPERIMENTAL] ListWorkers: List Workers
 *WorkersApi* | [**run_worker**](docs/WorkersApi.md#run_worker) | **POST** /api/workers/{scope}/{code}/$run | [EXPERIMENTAL] RunWorker: Run a Worker
 *WorkersApi* | [**update_worker**](docs/WorkersApi.md#update_worker) | **PUT** /api/workers/{scope}/{code} | [EXPERIMENTAL] UpdateWorker: Update a Worker
 
 
 ## Documentation For Models
 
+ - [AccessControlledAction](docs/AccessControlledAction.md)
+ - [AccessControlledResource](docs/AccessControlledResource.md)
  - [ActionDefinition](docs/ActionDefinition.md)
  - [ActionDefinitionResponse](docs/ActionDefinitionResponse.md)
  - [ActionDetails](docs/ActionDetails.md)
  - [ActionDetailsResponse](docs/ActionDetailsResponse.md)
+ - [ActionId](docs/ActionId.md)
  - [CreateChildTaskConfiguration](docs/CreateChildTaskConfiguration.md)
  - [CreateChildTasksAction](docs/CreateChildTasksAction.md)
  - [CreateChildTasksActionResponse](docs/CreateChildTasksActionResponse.md)
  - [CreateTaskDefinitionRequest](docs/CreateTaskDefinitionRequest.md)
  - [CreateTaskRequest](docs/CreateTaskRequest.md)
  - [CreateWorkerRequest](docs/CreateWorkerRequest.md)
  - [DeletedEntityResponse](docs/DeletedEntityResponse.md)
  - [Fail](docs/Fail.md)
  - [FailResponse](docs/FailResponse.md)
  - [FieldMapping](docs/FieldMapping.md)
  - [GetWorkerResultResponse](docs/GetWorkerResultResponse.md)
  - [HealthCheck](docs/HealthCheck.md)
  - [HealthCheckResponse](docs/HealthCheckResponse.md)
+ - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
+ - [IdentifierPartSchema](docs/IdentifierPartSchema.md)
  - [InitialState](docs/InitialState.md)
  - [Link](docs/Link.md)
  - [LuminesceView](docs/LuminesceView.md)
  - [LuminesceViewResponse](docs/LuminesceViewResponse.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
  - [PagedResourceListOfTask](docs/PagedResourceListOfTask.md)
  - [PagedResourceListOfTaskDefinition](docs/PagedResourceListOfTaskDefinition.md)
  - [PagedResourceListOfWorker](docs/PagedResourceListOfWorker.md)
  - [Parameter](docs/Parameter.md)
  - [ParameterValue](docs/ParameterValue.md)
  - [ResourceId](docs/ResourceId.md)
+ - [ResourceListOfAccessControlledResource](docs/ResourceListOfAccessControlledResource.md)
  - [ResourceListOfTask](docs/ResourceListOfTask.md)
  - [ResultField](docs/ResultField.md)
  - [ResultMatchingPattern](docs/ResultMatchingPattern.md)
  - [ResultantChildTaskConfiguration](docs/ResultantChildTaskConfiguration.md)
  - [RunWorkerAction](docs/RunWorkerAction.md)
  - [RunWorkerActionResponse](docs/RunWorkerActionResponse.md)
  - [RunWorkerRequest](docs/RunWorkerRequest.md)
```

