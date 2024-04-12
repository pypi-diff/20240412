# Comparing `tmp/exasol_transformers_extension-0.10.0.tar.gz` & `tmp/exasol_transformers_extension-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol_transformers_extension-0.10.0.tar", max compression
+gzip compressed data, was "exasol_transformers_extension-1.0.0.tar", max compression
```

## Comparing `exasol_transformers_extension-0.10.0.tar` & `exasol_transformers_extension-1.0.0.tar`

### file list

```diff
@@ -1,59 +1,57 @@
--rw-r--r--   0        0        0     1063 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/LICENSE
--rw-r--r--   0        0        0      503 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/README.md
--rw-r--r--   0        0        0       22 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/__init__.py
--rw-r--r--   0        0        0     1019 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/deploy.py
--rw-r--r--   0        0        0        0 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/__init__.py
--rw-r--r--   0        0        0     1092 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/constants.py
--rw-r--r--   0        0        0     1083 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/deployment_utils.py
--rw-r--r--   0        0        0     3813 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/language_container.py
--rw-r--r--   0        0        0    13328 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/language_container_deployer.py
--rw-r--r--   0        0        0     7899 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/language_container_deployer_cli.py
--rw-r--r--   0        0        0     2376 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/scripts_deployer.py
--rw-r--r--   0        0        0     1379 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/scripts_deployer_cli.py
--rw-r--r--   0        0        0     1155 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/te_language_container_deployer.py
--rw-r--r--   0        0        0        0 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/resources/__init__.py
--rw-r--r--   0        0        0      659 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/resources/templates/filling_mask_udf.jinja.sql
--rw-r--r--   0        0        0      339 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/resources/templates/model_downloader_udf.jinja.sql
--rw-r--r--   0        0        0      728 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/resources/templates/question_answering_udf.jinja.sql
--rw-r--r--   0        0        0      620 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/resources/templates/sequence_classification_single_text_udf.jinja.sql
--rw-r--r--   0        0        0      688 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/resources/templates/sequence_classification_text_pair_udf.jinja.sql
--rw-r--r--   0        0        0      698 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/resources/templates/text_generation_udf.jinja.sql
--rw-r--r--   0        0        0      763 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/resources/templates/token_classification_udf.jinja.sql
--rw-r--r--   0        0        0      788 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/resources/templates/translation_udf.jinja.sql
--rw-r--r--   0        0        0      710 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/resources/templates/zero_shot_text_classification_udf.jinja.sql
--rw-r--r--   0        0        0        0 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/__init__.py
--rw-r--r--   0        0        0        0 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/callers/__init__.py
--rw-r--r--   0        0        0      154 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/callers/filling_mask_udf_call.py
--rw-r--r--   0        0        0      170 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/callers/model_downloader_udf_call.py
--rw-r--r--   0        0        0      177 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/callers/question_answering_udf_call.py
--rw-r--r--   0        0        0      224 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/callers/sequence_classification_single_text_udf_call.py
--rw-r--r--   0        0        0      218 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/callers/sequence_classification_text_pair_udf_call.py
--rw-r--r--   0        0        0      168 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/callers/text_generation_udf_call.py
--rw-r--r--   0        0        0      183 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/callers/token_classification_udf_call.py
--rw-r--r--   0        0        0      158 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/callers/translation_udf_call.py
--rw-r--r--   0        0        0      206 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/callers/zero_shot_text_classification_udf.py
--rw-r--r--   0        0        0        0 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/__init__.py
--rw-r--r--   0        0        0    10464 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/base_model_udf.py
--rw-r--r--   0        0        0     4483 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/filling_mask_udf.py
--rw-r--r--   0        0        0     2889 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/model_downloader_udf.py
--rw-r--r--   0        0        0     4258 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/question_answering_udf.py
--rw-r--r--   0        0        0     3251 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/sequence_classification_single_text_udf.py
--rw-r--r--   0        0        0     3509 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/sequence_classification_text_pair_udf.py
--rw-r--r--   0        0        0     3712 2024-02-22 10:06:10.553301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/text_generation_udf.py
--rw-r--r--   0        0        0     4714 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/token_classification_udf.py
--rw-r--r--   0        0        0     3806 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/translation_udf.py
--rw-r--r--   0        0        0     4047 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/zero_shot_text_classification_udf.py
--rw-r--r--   0        0        0     2033 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/upload_model.py
--rw-r--r--   0        0        0        0 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/__init__.py
--rw-r--r--   0        0        0      806 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/bucketfs_model_uploader.py
--rw-r--r--   0        0        0     3015 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/bucketfs_operations.py
--rw-r--r--   0        0        0     1126 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/dataframe_operations.py
--rw-r--r--   0        0        0      383 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/device_management.py
--rw-r--r--   0        0        0     2516 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/huggingface_hub_bucketfs_model_transfer.py
--rw-r--r--   0        0        0     4124 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/huggingface_hub_bucketfs_model_transfer_sp.py
--rw-r--r--   0        0        0     2456 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/load_local_model.py
--rw-r--r--   0        0        0     1983 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/load_model.py
--rw-r--r--   0        0        0      893 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/model_factory_protocol.py
--rw-r--r--   0        0        0      150 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/temporary_directory_factory.py
--rw-r--r--   0        0        0     1097 2024-02-22 10:06:10.557301 exasol_transformers_extension-0.10.0/pyproject.toml
--rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 exasol_transformers_extension-0.10.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-12 11:14:18.044924 exasol_transformers_extension-1.0.0/LICENSE
+-rw-r--r--   0        0        0      653 2024-04-12 11:14:18.044924 exasol_transformers_extension-1.0.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/__init__.py
+-rw-r--r--   0        0        0     1019 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deploy.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/__init__.py
+-rw-r--r--   0        0        0     1078 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/constants.py
+-rw-r--r--   0        0        0     1083 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/deployment_utils.py
+-rw-r--r--   0        0        0     3813 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/language_container.py
+-rw-r--r--   0        0        0    13328 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/language_container_deployer.py
+-rw-r--r--   0        0        0     7899 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/language_container_deployer_cli.py
+-rw-r--r--   0        0        0     2376 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/scripts_deployer.py
+-rw-r--r--   0        0        0     1379 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/scripts_deployer_cli.py
+-rw-r--r--   0        0        0     1155 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/te_language_container_deployer.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/__init__.py
+-rw-r--r--   0        0        0      593 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/filling_mask_udf.jinja.sql
+-rw-r--r--   0        0        0      339 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/model_downloader_udf.jinja.sql
+-rw-r--r--   0        0        0      662 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/question_answering_udf.jinja.sql
+-rw-r--r--   0        0        0      554 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/sequence_classification_single_text_udf.jinja.sql
+-rw-r--r--   0        0        0      622 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/sequence_classification_text_pair_udf.jinja.sql
+-rw-r--r--   0        0        0      632 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/text_generation_udf.jinja.sql
+-rw-r--r--   0        0        0      697 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/token_classification_udf.jinja.sql
+-rw-r--r--   0        0        0      722 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/translation_udf.jinja.sql
+-rw-r--r--   0        0        0      644 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/zero_shot_text_classification_udf.jinja.sql
+-rw-r--r--   0        0        0        0 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/filling_mask_udf_call.py
+-rw-r--r--   0        0        0      170 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/model_downloader_udf_call.py
+-rw-r--r--   0        0        0      177 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/question_answering_udf_call.py
+-rw-r--r--   0        0        0      224 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/sequence_classification_single_text_udf_call.py
+-rw-r--r--   0        0        0      218 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/sequence_classification_text_pair_udf_call.py
+-rw-r--r--   0        0        0      168 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/text_generation_udf_call.py
+-rw-r--r--   0        0        0      183 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/token_classification_udf_call.py
+-rw-r--r--   0        0        0      158 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/translation_udf_call.py
+-rw-r--r--   0        0        0      206 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/zero_shot_text_classification_udf.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/__init__.py
+-rw-r--r--   0        0        0    10362 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/base_model_udf.py
+-rw-r--r--   0        0        0     4483 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/filling_mask_udf.py
+-rw-r--r--   0        0        0     3779 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/model_downloader_udf.py
+-rw-r--r--   0        0        0     4258 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/question_answering_udf.py
+-rw-r--r--   0        0        0     3251 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/sequence_classification_single_text_udf.py
+-rw-r--r--   0        0        0     3509 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/sequence_classification_text_pair_udf.py
+-rw-r--r--   0        0        0     3712 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/text_generation_udf.py
+-rw-r--r--   0        0        0     4714 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/token_classification_udf.py
+-rw-r--r--   0        0        0     3806 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/translation_udf.py
+-rw-r--r--   0        0        0     4047 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/zero_shot_text_classification_udf.py
+-rw-r--r--   0        0        0     2268 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/upload_model.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/__init__.py
+-rw-r--r--   0        0        0      899 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/bucketfs_model_uploader.py
+-rw-r--r--   0        0        0     3246 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/bucketfs_operations.py
+-rw-r--r--   0        0        0     1126 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/dataframe_operations.py
+-rw-r--r--   0        0        0      383 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/device_management.py
+-rw-r--r--   0        0        0     4412 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/huggingface_hub_bucketfs_model_transfer_sp.py
+-rw-r--r--   0        0        0     2438 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/load_local_model.py
+-rw-r--r--   0        0        0      893 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/model_factory_protocol.py
+-rw-r--r--   0        0        0      150 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/temporary_directory_factory.py
+-rw-r--r--   0        0        0     1112 2024-04-12 11:14:18.052924 exasol_transformers_extension-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1824 1970-01-01 00:00:00.000000 exasol_transformers_extension-1.0.0/PKG-INFO
```

### Comparing `exasol_transformers_extension-0.10.0/LICENSE` & `exasol_transformers_extension-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/deploy.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deploy.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/constants.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,8 +22,8 @@
         "token_classification_udf.jinja.sql",
     "translation_udf_call.py":
         "translation_udf.jinja.sql",
     "zero_shot_text_classification_udf.py":
         "zero_shot_text_classification_udf.jinja.sql"
 }
 
-ORDERED_COLUMNS = ['model_name', 'bucketfs_conn', 'token_conn', 'sub_dir']
+ORDERED_COLUMNS = ['model_name', 'bucketfs_conn', 'sub_dir']
```

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/deployment_utils.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/language_container.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/language_container.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/language_container_deployer.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/language_container_deployer.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/language_container_deployer_cli.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/language_container_deployer_cli.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/scripts_deployer.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/scripts_deployer.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/scripts_deployer_cli.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/scripts_deployer_cli.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/deployment/te_language_container_deployer.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/te_language_container_deployer.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/resources/templates/filling_mask_udf.jinja.sql` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/question_answering_udf.jinja.sql`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-CREATE OR REPLACE {{ language_alias }} SET SCRIPT "TE_FILLING_MASK_UDF"(
+CREATE OR REPLACE {{ language_alias }} SET SCRIPT "TE_QUESTION_ANSWERING_UDF"(
     device_id INTEGER,
     bucketfs_conn VARCHAR(2000000),
-    token_conn VARCHAR(2000000),
     sub_dir VARCHAR(2000000),
     model_name VARCHAR(2000000),
-    text_data VARCHAR(2000000),
+    question VARCHAR(2000000),
+    context_text VARCHAR(2000000),
     top_k INTEGER
     ORDER BY {{ ordered_columns | join(" ASC,") }} ASC
 )EMITS (
     bucketfs_conn VARCHAR(2000000),
-    token_conn VARCHAR(2000000),
     sub_dir VARCHAR(2000000),
     model_name VARCHAR(2000000),
-    text_data VARCHAR(2000000),
+    question VARCHAR(2000000),
+    context_text VARCHAR(2000000),
     top_k INTEGER,
-    filled_text VARCHAR(2000000),
+    answer VARCHAR(2000000),
     score DOUBLE,
     rank INTEGER,
     error_message VARCHAR(2000000) ) AS
 
 {{ script_content }}
 
 /
```

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/resources/templates/question_answering_udf.jinja.sql` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/token_classification_udf.jinja.sql`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-CREATE OR REPLACE {{ language_alias }} SET SCRIPT "TE_QUESTION_ANSWERING_UDF"(
+CREATE OR REPLACE {{ language_alias }} SET SCRIPT "TE_TOKEN_CLASSIFICATION_UDF"(
     device_id INTEGER,
     bucketfs_conn VARCHAR(2000000),
-    token_conn VARCHAR(2000000),
     sub_dir VARCHAR(2000000),
     model_name VARCHAR(2000000),
-    question VARCHAR(2000000),
-    context_text VARCHAR(2000000),
-    top_k INTEGER
+    text_data VARCHAR(2000000),
+    aggregation_strategy VARCHAR(2000000)
     ORDER BY {{ ordered_columns | join(" ASC,") }} ASC
 )EMITS (
     bucketfs_conn VARCHAR(2000000),
-    token_conn VARCHAR(2000000),
     sub_dir VARCHAR(2000000),
     model_name VARCHAR(2000000),
-    question VARCHAR(2000000),
-    context_text VARCHAR(2000000),
-    top_k INTEGER,
-    answer VARCHAR(2000000),
+    text_data VARCHAR(2000000),
+    aggregation_strategy VARCHAR(2000000),
+    start_pos INTEGER,
+    end_pos INTEGER,
+    word VARCHAR(2000000),
+    entity VARCHAR(2000000),
     score DOUBLE,
-    rank INTEGER,
     error_message VARCHAR(2000000) ) AS
 
 {{ script_content }}
 
 /
```

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/resources/templates/sequence_classification_single_text_udf.jinja.sql` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/sequence_classification_text_pair_udf.jinja.sql`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-CREATE OR REPLACE {{ language_alias }} SET SCRIPT "TE_SEQUENCE_CLASSIFICATION_SINGLE_TEXT_UDF"(
+CREATE OR REPLACE {{ language_alias }} SET SCRIPT "TE_SEQUENCE_CLASSIFICATION_TEXT_PAIR_UDF"(
     device_id INTEGER,
     bucketfs_conn VARCHAR(2000000),
-    token_conn VARCHAR(2000000),
     sub_dir VARCHAR(2000000),
     model_name VARCHAR(2000000),
-    text_data VARCHAR(2000000)
+    first_text VARCHAR(2000000),
+    second_text VARCHAR(2000000)
     ORDER BY {{ ordered_columns | join(" ASC,") }} ASC
 )EMITS (
     bucketfs_conn VARCHAR(2000000),
-    token_conn VARCHAR(2000000),
     sub_dir VARCHAR(2000000),
     model_name VARCHAR(2000000),
-    text_data VARCHAR(2000000),
+    first_text VARCHAR(2000000),
+    second_text VARCHAR(2000000),
     label VARCHAR(2000000),
     score DOUBLE,
     error_message VARCHAR(2000000) ) AS
 
 {{ script_content }}
 
 /
```

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/resources/templates/text_generation_udf.jinja.sql` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/sequence_classification_single_text_udf.jinja.sql`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-CREATE OR REPLACE {{ language_alias }} SET SCRIPT "TE_TEXT_GENERATION_UDF"(
+CREATE OR REPLACE {{ language_alias }} SET SCRIPT "TE_SEQUENCE_CLASSIFICATION_SINGLE_TEXT_UDF"(
     device_id INTEGER,
     bucketfs_conn VARCHAR(2000000),
-    token_conn VARCHAR(2000000),
     sub_dir VARCHAR(2000000),
     model_name VARCHAR(2000000),
-    text_data VARCHAR(2000000),
-    max_length INTEGER,
-    return_full_text BOOLEAN
+    text_data VARCHAR(2000000)
     ORDER BY {{ ordered_columns | join(" ASC,") }} ASC
 )EMITS (
     bucketfs_conn VARCHAR(2000000),
-    token_conn VARCHAR(2000000),
     sub_dir VARCHAR(2000000),
     model_name VARCHAR(2000000),
     text_data VARCHAR(2000000),
-    max_length INTEGER,
-    return_full_text BOOLEAN,
-    generated_text VARCHAR(2000000),
-    error_message VARCHAR(2000000)) AS
+    label VARCHAR(2000000),
+    score DOUBLE,
+    error_message VARCHAR(2000000) ) AS
 
 {{ script_content }}
 
 /
```

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/resources/templates/translation_udf.jinja.sql` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/translation_udf.jinja.sql`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 CREATE OR REPLACE {{ language_alias }} SET SCRIPT "TE_TRANSLATION_UDF"(
     device_id INTEGER,
     bucketfs_conn VARCHAR(2000000),
-    token_conn VARCHAR(2000000),
     sub_dir VARCHAR(2000000),
     model_name VARCHAR(2000000),
     text_data VARCHAR(2000000),
     source_language VARCHAR(2000000),
     target_language VARCHAR(2000000),
     max_length INTEGER
     ORDER BY {{ ordered_columns | join(" ASC,") }} ASC
 )EMITS (
     bucketfs_conn VARCHAR(2000000),
-    token_conn VARCHAR(2000000),
     sub_dir VARCHAR(2000000),
     model_name VARCHAR(2000000),
     text_data VARCHAR(2000000),
     source_language VARCHAR(2000000),
     target_language VARCHAR(2000000),
     max_length INTEGER,
     translation_text VARCHAR(2000000),
```

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/base_model_udf.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/base_model_udf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,48 @@
+import os
 from abc import abstractmethod, ABC
 from typing import Iterator, List, Any
 import torch
 import traceback
 import pandas as pd
 import numpy as np
+import transformers
+
 from exasol_transformers_extension.deployment import constants
 from exasol_transformers_extension.utils import device_management, \
     bucketfs_operations, dataframe_operations
-from exasol_transformers_extension.utils.load_model import LoadModel
+from exasol_transformers_extension.utils.load_local_model import LoadLocalModel
+from exasol_transformers_extension.utils.model_factory_protocol import ModelFactoryProtocol
 
 
 class BaseModelUDF(ABC):
     """
     This base class should be extended by each UDF class containing model logic.
-    This class contains common operations for all prediction UDFs. The following
-    methods should be implemented specifically for each UDF class:
+    This class contains common operations for all prediction UDFs:
         - accesses data part-by-part based on predefined batch size
-        - manages the script cache
+        - manages the model cache
         - reads the corresponding model from BucketFS into cache
         - creates model pipeline through transformer api
         - manages the creation of predictions and the preparation of results.
+
+    Additionally, the following
+    methods should be implemented specifically for each UDF class:
+        - create_dataframes_from_predictions
+        - extract_unique_param_based_dataframes
+        - execute_prediction
+        - append_predictions_to_input_dataframe
+
     """
     def __init__(self,
                  exa,
-                 batch_size,
-                 pipeline,
-                 base_model,
-                 tokenizer,
-                 task_name):
+                 batch_size: int,
+                 pipeline: transformers.Pipeline,
+                 base_model: ModelFactoryProtocol,
+                 tokenizer: ModelFactoryProtocol,
+                 task_name: str):
         self.exa = exa
         self.batch_size = batch_size
         self.pipeline = pipeline
         self.base_model = base_model
         self.tokenizer = tokenizer
         self.task_name = task_name
         self.device = None
@@ -55,19 +66,19 @@
 
         self.model_loader.clear_device_memory()
 
     def create_model_loader(self):
         """
         Creates the model_loader.
         """
-        self.model_loader = LoadModel(self.pipeline,
-                                      self.base_model,
-                                      self.tokenizer,
-                                      self.task_name,
-                                      self.device)
+        self.model_loader = LoadLocalModel(pipeline_factory=self.pipeline,
+                                           base_model_factory=self.base_model,
+                                           tokenizer_factory=self.tokenizer,
+                                           task_name=self.task_name,
+                                           device=self.device)
 
     def get_predictions_from_batch(self, batch_df: pd.DataFrame) -> pd.DataFrame:
         """
         Perform separate predictions for each model in the dataframe.
 
         :param batch_df: A batch of dataframe retrieved from context
 
@@ -137,15 +148,15 @@
         :return: Unique model dataframe having same model_name,
         bucketfs_connection, and sub_dir
         """
 
         unique_values = dataframe_operations.get_unique_values(
             batch_df, constants.ORDERED_COLUMNS, sort=True)
 
-        for model_name, bucketfs_conn, token_conn, sub_dir in unique_values:
+        for model_name, bucketfs_conn, sub_dir in unique_values:
             try:
                 self._check_values_not_null(model_name, bucketfs_conn, sub_dir)
             except ValueError:
                 stack_trace = traceback.format_exc()
                 result_with_error_df = self.get_result_with_error(
                     batch_df, stack_trace)
                 yield result_with_error_df
@@ -153,18 +164,14 @@
 
             selections = (
                     (batch_df['model_name'] == model_name) &
                     (batch_df['bucketfs_conn'] == bucketfs_conn) &
                     (batch_df['sub_dir'] == sub_dir)
             )
 
-            if token_conn is None:
-                selections = selections & pd.isnull(batch_df['token_conn'])
-            else:
-                selections = selections & (batch_df['token_conn'] == token_conn)
             model_df = batch_df[
                 selections]
 
             yield model_df
 
     def check_cache(self, model_df: pd.DataFrame) -> None:
         """
@@ -173,28 +180,21 @@
 
         :param model_df: Unique model dataframe having same model_name,
         bucketfs_connection, and sub_dir
         """
         model_name = model_df["model_name"].iloc[0]
         bucketfs_conn = model_df["bucketfs_conn"].iloc[0]
         sub_dir = model_df["sub_dir"].iloc[0]
-        token_conn = model_df["token_conn"].iloc[0]
 
-        current_model_key = (bucketfs_conn, sub_dir, model_name, token_conn)
-        if self.model_loader.last_loaded_model_key != current_model_key:
+        current_model_key = (bucketfs_conn, sub_dir, model_name)
+        if self.model_loader.loaded_model_key != current_model_key:
             self.set_cache_dir(model_name, bucketfs_conn, sub_dir)
             self.model_loader.clear_device_memory()
-            if token_conn:
-                token_conn_obj = self.exa.get_connection(token_conn)
-            else:
-                token_conn_obj = None
-            self.last_created_pipeline = self.model_loader.load_models(model_name,
-                                                                       current_model_key,
-                                                                       self.cache_dir,
-                                                                       token_conn_obj)
+            self.last_created_pipeline = self.model_loader.load_models(self.cache_dir,
+                                                                       current_model_key)
 
     def set_cache_dir(
             self, model_name: str, bucketfs_conn_name: str,
             sub_dir: str) -> None:
         """
         Set the cache directory in bucketfs of the specified model.
 
@@ -202,19 +202,18 @@
         :param bucketfs_conn_name: Name of the bucketFS connection
         :param sub_dir: Directory where the model is cached
         """
         bucketfs_location = \
             bucketfs_operations.create_bucketfs_location_from_conn_object(
                 self.exa.get_connection(bucketfs_conn_name))
 
-        model_path = bucketfs_operations.get_model_path(sub_dir, model_name)
+        model_path = bucketfs_operations.get_model_path_with_pretrained(sub_dir, model_name)
         self.cache_dir = bucketfs_operations.get_local_bucketfs_path(
             bucketfs_location=bucketfs_location, model_path=str(model_path))
 
-
     def get_prediction(self, model_df: pd.DataFrame) -> pd.DataFrame:
         """
         Perform prediction of the given model and preparation of the prediction
         results according to the format that the UDF can emit.
 
         :param model_df: The dataframe to be predicted
```

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/filling_mask_udf.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/filling_mask_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/model_downloader_udf.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/model_downloader_udf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 from typing import Tuple
 
 import transformers
 from exasol_bucketfs_utils_python.bucketfs_factory import BucketFSFactory
 
 from exasol_transformers_extension.utils import bucketfs_operations
-from exasol_transformers_extension.utils.huggingface_hub_bucketfs_model_transfer import ModelFactoryProtocol, \
-    HuggingFaceHubBucketFSModelTransferFactory
+from exasol_transformers_extension.utils.model_factory_protocol import ModelFactoryProtocol
+from exasol_transformers_extension.utils.huggingface_hub_bucketfs_model_transfer_sp import \
+    HuggingFaceHubBucketFSModelTransferSPFactory
 
 
 class ModelDownloaderUDF:
+    """
+    UDF which downloads a pretrained model from Huggingface using Huggingface's transformers API,
+    and uploads it to the BucketFS, from where it can then be loaded without accessing Huggingface again.
+    Must be called with the following Input Parameter:
+
+    model_name                | sub_dir                 | bfs_conn            | token_conn
+    ---------------------------------------------------------------------------------------------------
+    name of Huggingface model | directory to save model | BucketFS connection | name of token connection
+
+    returns <sub_dir/model_name> , <path of model BucketFS>
+    """
     def __init__(self,
                  exa,
                  base_model_factory: ModelFactoryProtocol = transformers.AutoModel,
                  tokenizer_factory: ModelFactoryProtocol = transformers.AutoTokenizer,
-                 huggingface_hub_bucketfs_model_transfer: HuggingFaceHubBucketFSModelTransferFactory =
-                 HuggingFaceHubBucketFSModelTransferFactory(),
+                 huggingface_hub_bucketfs_model_transfer: HuggingFaceHubBucketFSModelTransferSPFactory =
+                 HuggingFaceHubBucketFSModelTransferSPFactory(),
                  bucketfs_factory: BucketFSFactory = BucketFSFactory()):
         self._exa = exa
         self._base_model_factory = base_model_factory
         self._tokenizer_factory = tokenizer_factory
         self._huggingface_hub_bucketfs_model_transfer = huggingface_hub_bucketfs_model_transfer
         self._bucketfs_factory = bucketfs_factory
 
@@ -27,18 +39,18 @@
             model_path = self._download_model(ctx)
             ctx.emit(*model_path)
             if not ctx.next():
                 break
 
     def _download_model(self, ctx) -> Tuple[str, str]:
         # parameters
-        model_name = ctx.model_name
-        sub_dir = ctx.sub_dir
-        bfs_conn = ctx.bfs_conn
-        token_conn = ctx.token_conn
+        model_name = ctx.model_name     # name of Huggingface model
+        sub_dir = ctx.sub_dir           # directory to save model
+        bfs_conn = ctx.bfs_conn         # BucketFS connection
+        token_conn = ctx.token_conn     # name of token connection
 
         # extract token from the connection if token connection name is given.
         # note that, token is required for private models. It doesn't matter
         # whether there is a token for public model or even what the token is.
         token = False
         if token_conn:
             token_conn_obj = self._exa.get_connection(token_conn)
@@ -60,10 +72,11 @@
                 bucketfs_location=bucketfs_location,
                 model_name=model_name,
                 model_path=model_path,
                 token=token
         ) as downloader:
             for model in [self._base_model_factory, self._tokenizer_factory]:
                 downloader.download_from_huggingface_hub(model)
+            # upload model files to BucketFS
             model_tar_file_path = downloader.upload_to_bucketfs()
 
         return str(model_path), str(model_tar_file_path)
```

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/question_answering_udf.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/question_answering_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/sequence_classification_single_text_udf.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/sequence_classification_single_text_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/sequence_classification_text_pair_udf.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/sequence_classification_text_pair_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/text_generation_udf.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/text_generation_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/token_classification_udf.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/token_classification_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/translation_udf.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/translation_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/udfs/models/zero_shot_text_classification_udf.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/zero_shot_text_classification_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/upload_model.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/upload_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,20 +29,25 @@
         bucketfs_user: str,
         bucketfs_password: str,
         bucket: str,
         path_in_bucket: str,
         model_name: str,
         sub_dir: str,
         local_model_path: str):
+    """
+    Script for uploading locally saved model files to BucketFS. Files should have been saved locally
+    using Transformers save_pretrained function. This ensures proper loading from the BucketFS later
+    """
     # create bucketfs location
     bucketfs_location = bucketfs_operations.create_bucketfs_location(
         bucketfs_name, bucketfs_host, bucketfs_port, bucketfs_use_https,
         bucketfs_user, bucketfs_password, bucket, path_in_bucket)
 
     # upload the downloaded model files into bucketfs
-    upload_path = bucketfs_operations.get_model_path(sub_dir, model_name)
+    upload_path = bucketfs_operations.get_model_path_with_pretrained(sub_dir, model_name)
+
     bucketfs_operations.upload_model_files_to_bucketfs(
         local_model_path, upload_path, bucketfs_location)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/bucketfs_operations.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/bucketfs_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,18 +37,21 @@
         bucket_config=_bucket_config,
         base_path=PurePosixPath(path_in_bucket))
 
 
 def upload_model_files_to_bucketfs(
         tmpdir_name: str, model_path: Path,
         bucketfs_location: AbstractBucketFSLocation) -> Path:
+    """
+    uploads model in tmpdir_name to model_path in bucketfs_location
+    """
     with tempfile.TemporaryFile() as fileobj:
         create_tar_of_directory(Path(tmpdir_name), fileobj)
-        model_tar_file = model_path.with_suffix(".tar.gz")
-        return upload_file_to_bucketfs_with_retry(bucketfs_location, fileobj, model_tar_file)
+        model_upload_tar_file_path = model_path.with_suffix(".tar.gz")
+        return upload_file_to_bucketfs_with_retry(bucketfs_location, fileobj, model_upload_tar_file_path)
 
 
 @retry(wait=wait_fixed(2), stop=stop_after_attempt(10))
 def upload_file_to_bucketfs_with_retry(bucketfs_location: AbstractBucketFSLocation,
                                        fileobj: BinaryIO,
                                        file_path: Path) -> Path:
     fileobj.seek(0)
@@ -65,8 +68,12 @@
 def get_local_bucketfs_path(
         bucketfs_location: BucketFSLocation, model_path: str) -> PurePosixPath:
     bucketfs_local_path = bucketfs_location.generate_bucket_udf_path(model_path)
     return bucketfs_local_path
 
 
 def get_model_path(sub_dir: str, model_name: str) -> Path:
-    return Path(sub_dir, model_name.replace('-', '_'))
+    return Path(sub_dir, model_name)
+
+
+def get_model_path_with_pretrained(sub_dir: str, model_name: str) -> Path:
+    return Path(sub_dir, model_name, "pretrained" , model_name)
```

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/dataframe_operations.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/dataframe_operations.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/huggingface_hub_bucketfs_model_transfer_sp.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/huggingface_hub_bucketfs_model_transfer_sp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from pathlib import Path
 
+from exasol_bucketfs_utils_python.abstract_bucketfs_location import AbstractBucketFSLocation
 from exasol_bucketfs_utils_python.bucketfs_location import BucketFSLocation
 
 from exasol_transformers_extension.utils.model_factory_protocol import ModelFactoryProtocol
 from exasol_transformers_extension.utils.bucketfs_model_uploader import BucketFSModelUploaderFactory
 from exasol_transformers_extension.utils.temporary_directory_factory import TemporaryDirectoryFactory
 
 
-
-
-
 class HuggingFaceHubBucketFSModelTransferSP:
     """
-    Class for downloading a model using the Huggingface Transformers API, and loading it into the BucketFS
-    using save_pretrained.
+    Class for downloading a model using the Huggingface Transformers API, saving it locally using
+    transformers save_pretrained, and loading the saved model files into the BucketFS.
 
-    :bucketfs_location:     BucketFSLocation the model should be loaded to
-    :model_name:            Name of the model to be downloaded using Huggingface Transformers API
-    :model_path:            Path the model will be loaded into the BucketFS at
-    :token:                 Huggingface token, only needed for private models
+    :bucketfs_location:                 BucketFSLocation the model should be loaded to
+    :model_name:                        Name of the model to be downloaded using Huggingface Transformers API
+    :model_path:                        Path the model will be loaded into the BucketFS at
+    :token:                             Huggingface token, only needed for private models
     :temporary_directory_factory:       Optional. Default is TemporaryDirectoryFactory. Mainly change for testing.
     :bucketfs_model_uploader_factory:   Optional. Default is BucketFSModelUploaderFactory. Mainly change for testing.
     """
     def __init__(self,
                  bucketfs_location: BucketFSLocation,
                  model_name: str,
                  model_path: Path,
@@ -46,26 +44,27 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._tmpdir.__exit__(exc_type, exc_val, exc_tb)
 
     def download_from_huggingface_hub(self, model_factory: ModelFactoryProtocol):
         """
         Download a model from HuggingFace Hub into a temporary directory and save it with save_pretrained
-        in temporary directory / pretrained .
+        in temporary directory / pretrained / model_name.
         """
-        model = model_factory.from_pretrained(self._model_name, cache_dir=self._tmpdir_name / "cache", use_auth_token=self._token)
+        model = model_factory.from_pretrained(self._model_name, cache_dir=self._tmpdir_name / "cache",
+                                              use_auth_token=self._token)
         model.save_pretrained(self._tmpdir_name / "pretrained" / self._model_name)
 
     def upload_to_bucketfs(self) -> Path:
         """
         Upload the downloaded models into the BucketFS.
 
         returns: Path of the uploaded model in the BucketFS
         """
-        return self._bucketfs_model_uploader.upload_directory(self._tmpdir_name / "pretrained" / self._model_name)
+        return self._bucketfs_model_uploader.upload_directory(self._tmpdir_name / "pretrained" / self._model_name) #todo should we do replace(-,_) here to?
 
 
 class HuggingFaceHubBucketFSModelTransferSPFactory:
     """
     Class for creating a HuggingFaceHubBucketFSModelTransferSP object.
     """
     def create(self,
```

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/load_local_model.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/load_local_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 
 class LoadLocalModel:
     """
     Class for loading locally saved models and tokenizers. Also stores information regarding the model and pipeline.
 
     :_pipeline_factory:      a function to create a transformers pipeline
-    :task_name:             name of the current task
-    :device:                device to be used for pipeline creation
+    :task_name:              name of the current task
+    :device:                 device to be used for pipeline creation, i.e "CPU"
     :_base_model_factory:    a ModelFactoryProtocol for creating the loaded model
     :_tokenizer_factory:     a ModelFactoryProtocol for creating the loaded tokenizer
     """
     def __init__(self,
-                 _pipeline_factory,
+                 pipeline_factory,
                  task_name: str,
                  device: str,
                  base_model_factory: ModelFactoryProtocol,
                  tokenizer_factory: ModelFactoryProtocol
                  ):
-        self.pipeline_factory = _pipeline_factory
+        self.pipeline_factory = pipeline_factory
         self.task_name = task_name
         self.device = device
         self._base_model_factory = base_model_factory
         self._tokenizer_factory = tokenizer_factory
         self._loaded_model_key = None
 
     @property
@@ -35,15 +35,15 @@
         return self._loaded_model_key
 
     def load_models(self,
                     model_path: Path,
                     current_model_key: str
                     ) -> transformers.pipelines.Pipeline:
         """
-        Loads a locally saved model and tokenizer from "cache_dir / "pretrained" / model_name".
+        Loads a locally saved model and tokenizer from model_path.
         Returns new pipeline corresponding to the model and task.
 
         :model_path:            location of the saved model and tokenizer
         :current_model_key:     key of the model to be loaded
         """
 
         loaded_model = self._base_model_factory.from_pretrained(str(model_path))
```

### Comparing `exasol_transformers_extension-0.10.0/exasol_transformers_extension/utils/model_factory_protocol.py` & `exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/model_factory_protocol.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-0.10.0/pyproject.toml` & `exasol_transformers_extension-1.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "exasol-transformers-extension"
-version = "0.10.0"
-description = "An Exasol extension to use state-of-the-art pretrained machine learning models via the transformers api."
+version = "1.0.0"
+description = "An Exasol extension for using state-of-the-art pretrained machine learning models via the Hugging Face Transformers API."
 
 authors = [
     	"Umit Buyuksahin <umit.buyuksahin@exasol.com>",
     	"Torsten Kilias <torsten.kilias@exasol.com>"
 ]
 
 readme = 'README.md'
```

### Comparing `exasol_transformers_extension-0.10.0/PKG-INFO` & `exasol_transformers_extension-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: exasol-transformers-extension
-Version: 0.10.0
-Summary: An Exasol extension to use state-of-the-art pretrained machine learning models via the transformers api.
+Version: 1.0.0
+Summary: An Exasol extension for using state-of-the-art pretrained machine learning models via the Hugging Face Transformers API.
 Home-page: https://github.com/exasol/transformers-extension
 Keywords: exasol
 Author: Umit Buyuksahin
 Author-email: umit.buyuksahin@exasol.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -26,14 +26,17 @@
 Description-Content-Type: text/markdown
 
 # Exasol Transformers Extension
 
 An Exasol extension to use state-of-the-art pretrained machine learning models 
 via the [transformers api](https://github.com/huggingface/transformers).
 
+This Extension is build and tested for Linux OS, and does not have Windows or MacOS support. 
+It might work regardless but proceed at your own risk.
+
 
 ## Table of Contents
 
 ### Information for Users
 
 * [User Guide](doc/user_guide/user_guide.md)
 * [Developer Guide](doc/developer_guide/developer_guide.md)
```

