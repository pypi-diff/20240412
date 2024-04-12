# Comparing `tmp/dcicutils-8.8.2.1b7.tar.gz` & `tmp/dcicutils-8.8.2.1b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-8.8.2.1b7.tar", max compression
+gzip compressed data, was "dcicutils-8.8.2.1b8.tar", max compression
```

## Comparing `dcicutils-8.8.2.1b7.tar` & `dcicutils-8.8.2.1b8.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1102 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/LICENSE.txt
--rw-r--r--   0        0        0     1166 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/README.rst
--rw-r--r--   0        0        0        0 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    34669 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/bundle_utils.py
--rw-r--r--   0        0        0     2522 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/captured_output.py
--rw-r--r--   0        0        0    13786 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3955 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    25653 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     7414 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/data_readers.py
--rw-r--r--   0        0        0     3098 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/data_utils.py
--rw-r--r--   0        0        0     4666 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/datetime_utils.py
--rw-r--r--   0        0        0    68891 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    72972 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     2663 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/file_utils.py
--rw-r--r--   0        0        0    10026 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    34149 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2024-04-10 16:51:10.066199 dcicutils-8.8.2.1b7/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    28151 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/lang_utils.py
--rw-r--r--   0        0        0      278 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/license_policies/c4-infrastructure.jsonc
--rw-r--r--   0        0        0      296 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/license_policies/c4-python-infrastructure.jsonc
--rw-r--r--   0        0        0     5790 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/license_policies/park-lab-common-server.jsonc
--rw-r--r--   0        0        0    18864 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/license_policies/park-lab-common.jsonc
--rw-r--r--   0        0        0     3260 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
--rw-r--r--   0        0        0      283 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/license_policies/park-lab-pipeline.jsonc
--rw-r--r--   0        0        0    46978 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/log_utils.py
--rw-r--r--   0        0        0   102210 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    15422 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/portal_object_utils.py
--rw-r--r--   0        0        0    30480 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/portal_utils.py
--rw-r--r--   0        0        0    13555 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/progress_bar.py
--rw-r--r--   0        0        0    31250 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20534 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   160208 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     7055 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28868 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    10095 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/schema_utils.py
--rw-r--r--   0        0        0    13889 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0     4184 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/scripts/run_license_checker.py
--rw-r--r--   0        0        0    26262 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/scripts/view_portal_object.py
--rw-r--r--   0        0        0    19745 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    33629 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/sheet_utils.py
--rw-r--r--   0        0        0    22961 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0    58188 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/structured_data.py
--rw-r--r--   0        0        0     2895 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/submitr/progress_constants.py
--rw-r--r--   0        0        0     3467 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/submitr/ref_lookup_strategy.py
--rw-r--r--   0        0        0     8082 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1403 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/tmpfile_utils.py
--rw-r--r--   0        0        0     1769 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/trace_utils.py
--rw-r--r--   0        0        0    14797 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/validation_utils.py
--rw-r--r--   0        0        0     4343 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/variant_utils.py
--rw-r--r--   0        0        0     2027 2024-04-10 16:51:10.070199 dcicutils-8.8.2.1b7/dcicutils/zip_utils.py
--rw-r--r--   0        0        0     4714 2024-04-10 16:51:10.074199 dcicutils-8.8.2.1b7/pyproject.toml
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.8.2.1b7/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/README.rst
+-rw-r--r--   0        0        0        0 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    34669 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/bundle_utils.py
+-rw-r--r--   0        0        0     2522 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/captured_output.py
+-rw-r--r--   0        0        0    13786 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3955 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    25653 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     7414 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/data_readers.py
+-rw-r--r--   0        0        0     3098 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/data_utils.py
+-rw-r--r--   0        0        0     4666 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/datetime_utils.py
+-rw-r--r--   0        0        0    69506 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    72972 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0     2663 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/file_utils.py
+-rw-r--r--   0        0        0    10026 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    34149 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    28151 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0      278 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/license_policies/c4-infrastructure.jsonc
+-rw-r--r--   0        0        0      296 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/license_policies/c4-python-infrastructure.jsonc
+-rw-r--r--   0        0        0     5790 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/license_policies/park-lab-common-server.jsonc
+-rw-r--r--   0        0        0    18864 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/license_policies/park-lab-common.jsonc
+-rw-r--r--   0        0        0     3260 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
+-rw-r--r--   0        0        0      283 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/license_policies/park-lab-pipeline.jsonc
+-rw-r--r--   0        0        0    46978 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2024-04-12 02:28:20.552921 dcicutils-8.8.2.1b8/dcicutils/log_utils.py
+-rw-r--r--   0        0        0   102210 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    15422 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/portal_object_utils.py
+-rw-r--r--   0        0        0    30480 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/portal_utils.py
+-rw-r--r--   0        0        0    13554 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/progress_bar.py
+-rw-r--r--   0        0        0    31250 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20534 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   160208 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     7055 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28868 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    10095 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/schema_utils.py
+-rw-r--r--   0        0        0    13889 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0     4184 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/scripts/run_license_checker.py
+-rw-r--r--   0        0        0    26262 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/scripts/view_portal_object.py
+-rw-r--r--   0        0        0    19745 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    33629 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/sheet_utils.py
+-rw-r--r--   0        0        0    22961 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0    58188 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/structured_data.py
+-rw-r--r--   0        0        0     2895 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/submitr/progress_constants.py
+-rw-r--r--   0        0        0     3467 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/submitr/ref_lookup_strategy.py
+-rw-r--r--   0        0        0     8082 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1403 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/tmpfile_utils.py
+-rw-r--r--   0        0        0     1769 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0    14797 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/validation_utils.py
+-rw-r--r--   0        0        0     4343 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/variant_utils.py
+-rw-r--r--   0        0        0     2027 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/dcicutils/zip_utils.py
+-rw-r--r--   0        0        0     4714 2024-04-12 02:28:20.556921 dcicutils-8.8.2.1b8/pyproject.toml
+-rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.8.2.1b8/PKG-INFO
```

### Comparing `dcicutils-8.8.2.1b7/LICENSE.txt` & `dcicutils-8.8.2.1b8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/README.rst` & `dcicutils-8.8.2.1b8/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/base.py` & `dcicutils-8.8.2.1b8/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/beanstalk_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/bundle_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/captured_output.py` & `dcicutils-8.8.2.1b8/dcicutils/captured_output.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/cloudformation_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/codebuild_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/command_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/common.py` & `dcicutils-8.8.2.1b8/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/contribution_scripts.py` & `dcicutils-8.8.2.1b8/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/contribution_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/creds_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/data_readers.py` & `dcicutils-8.8.2.1b8/dcicutils/data_readers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/data_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/datetime_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/deployment_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/deployment_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,14 +426,15 @@
                                      indexer=None, index_server=None, sentry_dsn=None, tibanna_cwls_bucket=None,
                                      tibanna_output_bucket=None,
                                      application_bucket_prefix=None, foursight_bucket_prefix=None,
                                      auth0_domain=None, auth0_client=None, auth0_secret=None,
                                      auth0_allowed_connections=None,
                                      re_captcha_key=None, re_captcha_secret=None,
                                      redis_server=None,
+                                     google_api_key=None,
                                      file_upload_bucket=None, file_wfout_bucket=None,
                                      blob_bucket=None, system_bucket=None, metadata_bundles_bucket=None):
 
         """
         Builds a .ini file from a given template file.
 
         Args:
@@ -502,14 +503,15 @@
                                                auth0_domain=auth0_domain,
                                                auth0_client=auth0_client,
                                                auth0_secret=auth0_secret,
                                                auth0_allowed_connections=auth0_allowed_connections,
                                                re_captcha_key=re_captcha_key,
                                                re_captcha_secret=re_captcha_secret,
                                                redis_server=redis_server,
+                                               google_api_key=google_api_key,
                                                file_upload_bucket=file_upload_bucket,
                                                file_wfout_bucket=file_wfout_bucket,
                                                blob_bucket=blob_bucket,
                                                system_bucket=system_bucket,
                                                metadata_bundles_bucket=metadata_bundles_bucket,
                                                )
 
@@ -572,14 +574,15 @@
                                        indexer=None, index_server=None, sentry_dsn=None, tibanna_cwls_bucket=None,
                                        tibanna_output_bucket=None,
                                        application_bucket_prefix=None, foursight_bucket_prefix=None,
                                        auth0_domain=None, auth0_client=None, auth0_secret=None,
                                        auth0_allowed_connections=None,
                                        re_captcha_key=None, re_captcha_secret=None,
                                        redis_server=None,
+                                       google_api_key=None,
                                        file_upload_bucket=None,
                                        file_wfout_bucket=None, blob_bucket=None, system_bucket=None,
                                        metadata_bundles_bucket=None):
         """
         Sends output to init_file_stream corresponding to the data noe would want in an ini file
         for the given template_file_name and available environment variables.
 
@@ -628,14 +631,15 @@
         if (os.environ.get("ENCODED_BS_ENV") and os.environ.get("ENCODED_ENV_NAME")
                 and os.environ.get("ENCODED_BS_ENV") != os.environ.get("ENCODED_ENV_NAME")):
             raise ValueError("If both ENCODED_BS_ENV and ENCODED_ENV_NAME are supplied, they must agree.")
 
         higlass_server = higlass_server or os.environ.get('ENCODED_HIGLASS_SERVER', "MISSING_ENCODED_HIGLASS_SERVER")
         es_server = es_server or os.environ.get('ENCODED_ES_SERVER', "MISSING_ENCODED_ES_SERVER")
         redis_server = redis_server or os.environ.get('ENCODED_REDIS_SERVER', '')  # optional
+        google_api_key = google_api_key or os.environ.get('GOOGLE_API_KEY', '')  # optional
         env_bucket = (env_bucket
                       or EnvBase.global_env_bucket_name()
                       or ("MISSING_GLOBAL_ENV_BUCKET"
                           if cls.APP_ORCHESTRATED
                           else (LEGACY_CGAP_GLOBAL_ENV_BUCKET if cls.APP_KIND == 'cgap' else LEGACY_GLOBAL_ENV_BUCKET)))
         env_ecosystem = (env_ecosystem
                          or os.environ.get("ENCODED_ECOSYSTEM")
@@ -769,14 +773,15 @@
             'APP_VERSION': app_version,
             'PROJECT_VERSION': toml.load(cls.PYPROJECT_FILE_NAME)['tool']['poetry']['version'],
             'SNOVAULT_VERSION': pkg_resources.get_distribution("dcicsnovault").version,
             'UTILS_VERSION': pkg_resources.get_distribution("dcicutils").version,
             'HIGLASS_SERVER': higlass_server,
             'ES_SERVER': es_server,
             'REDIS_SERVER': redis_server,
+            'GOOGLE_API_KEY': google_api_key,
             'ENV_BUCKET': env_bucket,
             'ENV_ECOSYSTEM': env_ecosystem,
             'ENV_NAME': env_name,
             'BS_ENV': env_name,  # The ENV_NAME should be preferred. This one is deprecated now. -kmp 20-May-2022
             'BS_MIRROR_ENV': deprecated_bs_mirror_env,  # This info is in the ecosystem. -kmp 20-May-2022
             'S3_BUCKET_ORG': s3_bucket_org,
             'S3_BUCKET_ENV': s3_bucket_env,
@@ -941,14 +946,17 @@
                                 default=None)
             parser.add_argument("--sentry_dsn",
                                 help="a sentry DSN",
                                 default=None)
             parser.add_argument("--redis_server",
                                 help="server URL to a Redis Cluster",
                                 default=None)
+            parser.add_argument("--google_api_key",
+                                help="Google API key to get smaht-submitr metadata template version",
+                                default=None)
             parser.add_argument("--tibanna_cwls_bucket",
                                 help="the name of a Tibanna CWLs bucket to use",
                                 default=None)
             parser.add_argument("--tibanna_output_bucket",
                                 help="the name of a Tibanna logs bucket to use",
                                 default=None)
             parser.add_argument("--application_bucket_prefix",
@@ -1020,14 +1028,15 @@
                                              foursight_bucket_prefix=args.foursight_bucket_prefix,
                                              auth0_domain=args.auth0_domain,
                                              auth0_client=args.auth0_client,
                                              auth0_secret=args.auth0_secret,
                                              auth0_allowed_connections=args.auth0_allowed_connections,
                                              re_captcha_key=args.recaptcha_key, re_captcha_secret=args.recaptcha_secret,
                                              redis_server=args.redis_server,
+                                             google_api_key=args.google_api_key,
                                              file_upload_bucket=args.file_upload_bucket,
                                              file_wfout_bucket=args.file_wfout_bucket,
                                              blob_bucket=args.blob_bucket, system_bucket=args.system_bucket,
                                              metadata_bundles_bucket=args.metadata_bundles_bucket)
         except Exception as e:
             PRINT("Error (%s): %s" % (e.__class__.__name__, e))
             sys.exit(1)
```

### Comparing `dcicutils-8.8.2.1b7/dcicutils/diff_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/docker_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/ecr_scripts.py` & `dcicutils-8.8.2.1b8/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/ecr_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/ecs_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/env_base.py` & `dcicutils-8.8.2.1b8/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/env_manager.py` & `dcicutils-8.8.2.1b8/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/env_scripts.py` & `dcicutils-8.8.2.1b8/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/env_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/env_utils_legacy.py` & `dcicutils-8.8.2.1b8/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/es_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/exceptions.py` & `dcicutils-8.8.2.1b8/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/ff_mocks.py` & `dcicutils-8.8.2.1b8/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/ff_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/file_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/function_cache_decorator.py` & `dcicutils-8.8.2.1b8/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/glacier_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/jh_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/kibana/dashboards.json` & `dcicutils-8.8.2.1b8/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/kibana/readme.md` & `dcicutils-8.8.2.1b8/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/lang_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/license_policies/park-lab-common-server.jsonc` & `dcicutils-8.8.2.1b8/dcicutils/license_policies/park-lab-common-server.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/license_policies/park-lab-common.jsonc` & `dcicutils-8.8.2.1b8/dcicutils/license_policies/park-lab-common.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc` & `dcicutils-8.8.2.1b8/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/license_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/license_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/log_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/misc_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/obfuscation_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/opensearch_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/portal_object_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/portal_object_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/portal_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/portal_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/progress_bar.py` & `dcicutils-8.8.2.1b8/dcicutils/progress_bar.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         self._disabled = False
         self._done = False
         self._printf = printf if callable(printf) else print
         self._tidy_output_hack = (tidy_output_hack is True)
         self._started = time.time()
         self._stop_requested = False
         # Interrupt handling. We do not do the actual (signal) interrupt setup
-        # in self._initialiaze as that could be called from a (sub) thread; and in
+        # in self._initialize as that could be called from a (sub) thread; and in
         # Python we can only set a signal (SIGINT in our case) on the main thread.
         self._catch_interrupt = (catch_interrupt is True)
         self._interrupt = interrupt if callable(interrupt) else None
         self._interrupt_continue = interrupt_continue if callable(interrupt_continue) else None
         self._interrupt_stop = interrupt_stop if callable(interrupt_stop) else None
         if interrupt_exit in [True, False]:
             if not self._interrupt_stop:
```

### Comparing `dcicutils-8.8.2.1b7/dcicutils/project_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/qa_checkers.py` & `dcicutils-8.8.2.1b8/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/qa_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/redis_tools.py` & `dcicutils-8.8.2.1b8/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/redis_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/s3_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/schema_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-8.8.2.1b8/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/scripts/run_license_checker.py` & `dcicutils-8.8.2.1b8/dcicutils/scripts/run_license_checker.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/scripts/view_portal_object.py` & `dcicutils-8.8.2.1b8/dcicutils/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/secrets_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/sheet_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/sheet_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/snapshot_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/ssl_certificate_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/structured_data.py` & `dcicutils-8.8.2.1b8/dcicutils/structured_data.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/submitr/progress_constants.py` & `dcicutils-8.8.2.1b8/dcicutils/submitr/progress_constants.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/submitr/ref_lookup_strategy.py` & `dcicutils-8.8.2.1b8/dcicutils/submitr/ref_lookup_strategy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/task_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/tmpfile_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/tmpfile_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/trace_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/validation_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/variant_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/variant_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/dcicutils/zip_utils.py` & `dcicutils-8.8.2.1b8/dcicutils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.2.1b7/pyproject.toml` & `dcicutils-8.8.2.1b8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "8.8.2.1b7"  # TODO: To become 8.8.3
+version = "8.8.2.1b8"  # TODO: To become 8.8.3
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-8.8.2.1b7/PKG-INFO` & `dcicutils-8.8.2.1b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 8.8.2.1b7
+Version: 8.8.2.1b8
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
```

