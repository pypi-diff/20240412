# Comparing `tmp/parsee_core-0.1.4.2.tar.gz` & `tmp/parsee_core-0.1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsee_core-0.1.4.2.tar", max compression
+gzip compressed data, was "parsee_core-0.1.4.3.tar", max compression
```

## Comparing `parsee_core-0.1.4.2.tar` & `parsee_core-0.1.4.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1066 2024-03-21 12:33:53.103983 parsee_core-0.1.4.2/LICENSE
--rw-r--r--   0        0        0      529 2024-03-27 13:19:30.023928 parsee_core-0.1.4.2/parsee/__init__.py
--rw-r--r--   0        0        0     3252 2024-04-11 09:44:46.126854 parsee_core-0.1.4.2/parsee/cloud/api.py
--rw-r--r--   0        0        0        0 2023-07-26 14:50:21.298000 parsee_core-0.1.4.2/parsee/converters/__init__.py
--rw-r--r--   0        0        0     6063 2024-03-29 10:54:00.293459 parsee_core-0.1.4.2/parsee/converters/html_extraction.py
--rw-r--r--   0        0        0     3210 2024-04-11 09:44:46.122580 parsee_core-0.1.4.2/parsee/converters/image_creation.py
--rw-r--r--   0        0        0      399 2024-03-27 13:22:36.894150 parsee_core-0.1.4.2/parsee/converters/interfaces.py
--rw-r--r--   0        0        0     1806 2024-04-10 14:57:20.432097 parsee_core-0.1.4.2/parsee/converters/json_to_raw.py
--rw-r--r--   0        0        0     1069 2024-04-10 14:57:20.432511 parsee_core-0.1.4.2/parsee/converters/langchain.py
--rw-r--r--   0        0        0     3015 2024-04-10 14:57:20.432769 parsee_core-0.1.4.2/parsee/converters/main.py
--rw-r--r--   0        0        0     4324 2024-03-27 13:19:30.029388 parsee_core-0.1.4.2/parsee/converters/pdf_extraction.py
--rw-r--r--   0        0        0      491 2024-03-27 13:22:36.895882 parsee_core-0.1.4.2/parsee/converters/simple_text.py
--rw-r--r--   0        0        0     6680 2024-03-25 10:47:46.831244 parsee_core-0.1.4.2/parsee/datasets/dataset_dataclasses.py
--rw-r--r--   0        0        0     7820 2024-03-20 10:51:40.783264 parsee_core-0.1.4.2/parsee/datasets/evaluation/main.py
--rw-r--r--   0        0        0     2645 2024-03-01 12:41:34.973375 parsee_core-0.1.4.2/parsee/datasets/main.py
--rw-r--r--   0        0        0     3538 2024-02-15 11:15:28.539480 parsee_core-0.1.4.2/parsee/datasets/readers/disk_reader.py
--rw-r--r--   0        0        0     1422 2024-02-14 09:53:17.733410 parsee_core-0.1.4.2/parsee/datasets/readers/interfaces.py
--rw-r--r--   0        0        0     1883 2024-02-14 10:08:53.958308 parsee_core-0.1.4.2/parsee/datasets/writers/disk_writer.py
--rw-r--r--   0        0        0     1084 2024-02-14 09:53:17.701394 parsee_core-0.1.4.2/parsee/datasets/writers/interfaces.py
--rw-r--r--   0        0        0        0 2022-08-08 15:31:09.039000 parsee_core-0.1.4.2/parsee/extraction/__init__.py
--rw-r--r--   0        0        0     4138 2024-04-10 14:57:20.433043 parsee_core-0.1.4.2/parsee/extraction/extractor_dataclasses.py
--rw-r--r--   0        0        0    29463 2024-04-11 11:20:23.988527 parsee_core-0.1.4.2/parsee/extraction/extractor_elements.py
--rw-r--r--   0        0        0     9472 2024-04-05 15:38:22.487342 parsee_core-0.1.4.2/parsee/extraction/final_structuring.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.4.2/parsee/extraction/models/__init__.py
--rw-r--r--   0        0        0     2062 2024-04-10 14:57:20.433864 parsee_core-0.1.4.2/parsee/extraction/models/helpers.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.4.2/parsee/extraction/models/llm_models/__init__.py
--rw-r--r--   0        0        0     2882 2024-04-10 14:57:20.434116 parsee_core-0.1.4.2/parsee/extraction/models/llm_models/anthropic_model.py
--rw-r--r--   0        0        0     2866 2024-04-10 14:57:20.434321 parsee_core-0.1.4.2/parsee/extraction/models/llm_models/chatgpt_model.py
--rw-r--r--   0        0        0      888 2024-04-10 14:57:20.434563 parsee_core-0.1.4.2/parsee/extraction/models/llm_models/llm_base_model.py
--rw-r--r--   0        0        0     1694 2024-04-10 14:57:20.434940 parsee_core-0.1.4.2/parsee/extraction/models/llm_models/ollama_model.py
--rw-r--r--   0        0        0      875 2024-04-10 14:57:20.435213 parsee_core-0.1.4.2/parsee/extraction/models/llm_models/prompts.py
--rw-r--r--   0        0        0     1971 2024-04-10 14:57:20.435485 parsee_core-0.1.4.2/parsee/extraction/models/llm_models/replicate_model.py
--rw-r--r--   0        0        0     7875 2024-03-19 14:15:12.265884 parsee_core-0.1.4.2/parsee/extraction/models/llm_models/structuring_schema.py
--rw-r--r--   0        0        0      985 2024-04-10 14:57:20.435851 parsee_core-0.1.4.2/parsee/extraction/models/model_dataclasses.py
--rw-r--r--   0        0        0     8163 2024-03-20 12:24:18.192932 parsee_core-0.1.4.2/parsee/extraction/models/model_loader.py
--rw-r--r--   0        0        0     3358 2024-04-09 11:54:32.370368 parsee_core-0.1.4.2/parsee/extraction/run.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.2/parsee/extraction/tasks/__init__.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.2/parsee/extraction/tasks/element_classification/__init__.py
--rw-r--r--   0        0        0     1756 2024-02-22 09:52:47.322977 parsee_core-0.1.4.2/parsee/extraction/tasks/element_classification/element_model.py
--rw-r--r--   0        0        0     2199 2024-04-10 14:57:20.436266 parsee_core-0.1.4.2/parsee/extraction/tasks/element_classification/element_model_llm.py
--rw-r--r--   0        0        0     8051 2024-04-10 14:57:20.436667 parsee_core-0.1.4.2/parsee/extraction/tasks/element_classification/features.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.2/parsee/extraction/tasks/mappings/__init__.py
--rw-r--r--   0        0        0     6108 2024-04-04 15:01:44.484913 parsee_core-0.1.4.2/parsee/extraction/tasks/mappings/features.py
--rw-r--r--   0        0        0     1493 2024-02-22 09:52:47.319414 parsee_core-0.1.4.2/parsee/extraction/tasks/mappings/mapping_model.py
--rw-r--r--   0        0        0     2519 2024-04-10 14:57:20.436928 parsee_core-0.1.4.2/parsee/extraction/tasks/mappings/mapping_model_llm.py
--rw-r--r--   0        0        0      894 2024-03-28 20:25:58.634238 parsee_core-0.1.4.2/parsee/extraction/tasks/mappings/utils.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.4.2/parsee/extraction/tasks/meta_info_structuring/__init__.py
--rw-r--r--   0        0        0    13073 2024-04-10 14:57:20.437207 parsee_core-0.1.4.2/parsee/extraction/tasks/meta_info_structuring/features.py
--rw-r--r--   0        0        0      729 2024-02-22 09:52:47.324193 parsee_core-0.1.4.2/parsee/extraction/tasks/meta_info_structuring/meta_info.py
--rw-r--r--   0        0        0     2641 2024-04-10 14:57:20.437514 parsee_core-0.1.4.2/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.4.2/parsee/extraction/tasks/questions/__init__.py
--rw-r--r--   0        0        0     6136 2024-04-10 14:57:20.437823 parsee_core-0.1.4.2/parsee/extraction/tasks/questions/features.py
--rw-r--r--   0        0        0     1430 2024-03-01 12:41:34.971601 parsee_core-0.1.4.2/parsee/extraction/tasks/questions/question_model.py
--rw-r--r--   0        0        0     4031 2024-04-10 14:57:20.438067 parsee_core-0.1.4.2/parsee/extraction/tasks/questions/question_model_llm.py
--rw-r--r--   0        0        0     2678 2024-03-12 17:16:10.730178 parsee_core-0.1.4.2/parsee/extraction/tasks/questions/utils.py
--rw-r--r--   0        0        0        0 2023-08-08 14:40:07.901000 parsee_core-0.1.4.2/parsee/storage/__init__.py
--rw-r--r--   0        0        0     2366 2024-04-10 14:57:20.438310 parsee_core-0.1.4.2/parsee/storage/in_memory_storage.py
--rw-r--r--   0        0        0     1212 2024-04-10 14:57:20.438565 parsee_core-0.1.4.2/parsee/storage/interfaces.py
--rw-r--r--   0        0        0      317 2024-02-21 09:46:14.327121 parsee_core-0.1.4.2/parsee/storage/vector_stores/interfaces.py
--rw-r--r--   0        0        0     3204 2024-03-22 17:12:35.963569 parsee_core-0.1.4.2/parsee/storage/vector_stores/simple_faiss.py
--rw-r--r--   0        0        0        0 2023-08-03 13:44:22.929000 parsee_core-0.1.4.2/parsee/templates/__init__.py
--rw-r--r--   0        0        0     1360 2024-04-05 15:38:22.487748 parsee_core-0.1.4.2/parsee/templates/element_schema.py
--rw-r--r--   0        0        0     1959 2024-02-22 09:42:26.246323 parsee_core-0.1.4.2/parsee/templates/general_structuring_schema.py
--rw-r--r--   0        0        0     4019 2024-04-05 15:38:22.488067 parsee_core-0.1.4.2/parsee/templates/helpers.py
--rw-r--r--   0        0        0     1288 2024-02-22 09:33:07.394404 parsee_core-0.1.4.2/parsee/templates/job_template.py
--rw-r--r--   0        0        0     1011 2024-02-14 09:53:17.727343 parsee_core-0.1.4.2/parsee/templates/mappings.py
--rw-r--r--   0        0        0      384 2024-02-14 09:50:55.308500 parsee_core-0.1.4.2/parsee/templates/template_from_json.py
--rw-r--r--   0        0        0        0 2023-07-26 14:15:43.630000 parsee_core-0.1.4.2/parsee/utils/__init__.py
--rw-r--r--   0        0        0      405 2024-02-15 14:56:20.018887 parsee_core-0.1.4.2/parsee/utils/constants.py
--rw-r--r--   0        0        0      781 2024-03-27 13:19:30.038637 parsee_core-0.1.4.2/parsee/utils/enums.py
--rw-r--r--   0        0        0     6632 2024-04-08 08:51:44.149915 parsee_core-0.1.4.2/parsee/utils/helper.py
--rw-r--r--   0        0        0     2030 2024-03-26 12:40:38.547700 parsee_core-0.1.4.2/parsee/utils/sample_items.py
--rw-r--r--   0        0        0      827 2024-04-11 11:20:23.992920 parsee_core-0.1.4.2/pyproject.toml
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 parsee_core-0.1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-21 12:33:53.103983 parsee_core-0.1.4.3/LICENSE
+-rw-r--r--   0        0        0      529 2024-03-27 13:19:30.023928 parsee_core-0.1.4.3/parsee/__init__.py
+-rw-r--r--   0        0        0     4298 2024-04-11 14:23:00.335740 parsee_core-0.1.4.3/parsee/cloud/api.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:50:21.298000 parsee_core-0.1.4.3/parsee/converters/__init__.py
+-rw-r--r--   0        0        0     6063 2024-03-29 10:54:00.293459 parsee_core-0.1.4.3/parsee/converters/html_extraction.py
+-rw-r--r--   0        0        0     3210 2024-04-11 09:44:46.122580 parsee_core-0.1.4.3/parsee/converters/image_creation.py
+-rw-r--r--   0        0        0      399 2024-03-27 13:22:36.894150 parsee_core-0.1.4.3/parsee/converters/interfaces.py
+-rw-r--r--   0        0        0     1806 2024-04-10 14:57:20.432097 parsee_core-0.1.4.3/parsee/converters/json_to_raw.py
+-rw-r--r--   0        0        0     1069 2024-04-10 14:57:20.432511 parsee_core-0.1.4.3/parsee/converters/langchain.py
+-rw-r--r--   0        0        0     3015 2024-04-10 14:57:20.432769 parsee_core-0.1.4.3/parsee/converters/main.py
+-rw-r--r--   0        0        0     4324 2024-03-27 13:19:30.029388 parsee_core-0.1.4.3/parsee/converters/pdf_extraction.py
+-rw-r--r--   0        0        0      491 2024-03-27 13:22:36.895882 parsee_core-0.1.4.3/parsee/converters/simple_text.py
+-rw-r--r--   0        0        0     6680 2024-03-25 10:47:46.831244 parsee_core-0.1.4.3/parsee/datasets/dataset_dataclasses.py
+-rw-r--r--   0        0        0     7820 2024-03-20 10:51:40.783264 parsee_core-0.1.4.3/parsee/datasets/evaluation/main.py
+-rw-r--r--   0        0        0     2645 2024-03-01 12:41:34.973375 parsee_core-0.1.4.3/parsee/datasets/main.py
+-rw-r--r--   0        0        0     3538 2024-02-15 11:15:28.539480 parsee_core-0.1.4.3/parsee/datasets/readers/disk_reader.py
+-rw-r--r--   0        0        0     1422 2024-02-14 09:53:17.733410 parsee_core-0.1.4.3/parsee/datasets/readers/interfaces.py
+-rw-r--r--   0        0        0     1883 2024-02-14 10:08:53.958308 parsee_core-0.1.4.3/parsee/datasets/writers/disk_writer.py
+-rw-r--r--   0        0        0     1084 2024-02-14 09:53:17.701394 parsee_core-0.1.4.3/parsee/datasets/writers/interfaces.py
+-rw-r--r--   0        0        0        0 2022-08-08 15:31:09.039000 parsee_core-0.1.4.3/parsee/extraction/__init__.py
+-rw-r--r--   0        0        0     4138 2024-04-11 14:09:13.370382 parsee_core-0.1.4.3/parsee/extraction/extractor_dataclasses.py
+-rw-r--r--   0        0        0    29463 2024-04-11 11:20:23.988527 parsee_core-0.1.4.3/parsee/extraction/extractor_elements.py
+-rw-r--r--   0        0        0     9472 2024-04-05 15:38:22.487342 parsee_core-0.1.4.3/parsee/extraction/final_structuring.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.4.3/parsee/extraction/models/__init__.py
+-rw-r--r--   0        0        0     2062 2024-04-10 14:57:20.433864 parsee_core-0.1.4.3/parsee/extraction/models/helpers.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.4.3/parsee/extraction/models/llm_models/__init__.py
+-rw-r--r--   0        0        0     2882 2024-04-10 14:57:20.434116 parsee_core-0.1.4.3/parsee/extraction/models/llm_models/anthropic_model.py
+-rw-r--r--   0        0        0     2866 2024-04-10 14:57:20.434321 parsee_core-0.1.4.3/parsee/extraction/models/llm_models/chatgpt_model.py
+-rw-r--r--   0        0        0      888 2024-04-10 14:57:20.434563 parsee_core-0.1.4.3/parsee/extraction/models/llm_models/llm_base_model.py
+-rw-r--r--   0        0        0     1694 2024-04-10 14:57:20.434940 parsee_core-0.1.4.3/parsee/extraction/models/llm_models/ollama_model.py
+-rw-r--r--   0        0        0      875 2024-04-10 14:57:20.435213 parsee_core-0.1.4.3/parsee/extraction/models/llm_models/prompts.py
+-rw-r--r--   0        0        0     1971 2024-04-10 14:57:20.435485 parsee_core-0.1.4.3/parsee/extraction/models/llm_models/replicate_model.py
+-rw-r--r--   0        0        0     7875 2024-03-19 14:15:12.265884 parsee_core-0.1.4.3/parsee/extraction/models/llm_models/structuring_schema.py
+-rw-r--r--   0        0        0      985 2024-04-10 14:57:20.435851 parsee_core-0.1.4.3/parsee/extraction/models/model_dataclasses.py
+-rw-r--r--   0        0        0     8163 2024-03-20 12:24:18.192932 parsee_core-0.1.4.3/parsee/extraction/models/model_loader.py
+-rw-r--r--   0        0        0     3358 2024-04-09 11:54:32.370368 parsee_core-0.1.4.3/parsee/extraction/run.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.3/parsee/extraction/tasks/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.3/parsee/extraction/tasks/element_classification/__init__.py
+-rw-r--r--   0        0        0     1756 2024-02-22 09:52:47.322977 parsee_core-0.1.4.3/parsee/extraction/tasks/element_classification/element_model.py
+-rw-r--r--   0        0        0     2199 2024-04-10 14:57:20.436266 parsee_core-0.1.4.3/parsee/extraction/tasks/element_classification/element_model_llm.py
+-rw-r--r--   0        0        0     8051 2024-04-10 14:57:20.436667 parsee_core-0.1.4.3/parsee/extraction/tasks/element_classification/features.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.3/parsee/extraction/tasks/mappings/__init__.py
+-rw-r--r--   0        0        0     6108 2024-04-04 15:01:44.484913 parsee_core-0.1.4.3/parsee/extraction/tasks/mappings/features.py
+-rw-r--r--   0        0        0     1493 2024-02-22 09:52:47.319414 parsee_core-0.1.4.3/parsee/extraction/tasks/mappings/mapping_model.py
+-rw-r--r--   0        0        0     2519 2024-04-10 14:57:20.436928 parsee_core-0.1.4.3/parsee/extraction/tasks/mappings/mapping_model_llm.py
+-rw-r--r--   0        0        0      894 2024-03-28 20:25:58.634238 parsee_core-0.1.4.3/parsee/extraction/tasks/mappings/utils.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.4.3/parsee/extraction/tasks/meta_info_structuring/__init__.py
+-rw-r--r--   0        0        0    13073 2024-04-10 14:57:20.437207 parsee_core-0.1.4.3/parsee/extraction/tasks/meta_info_structuring/features.py
+-rw-r--r--   0        0        0      729 2024-02-22 09:52:47.324193 parsee_core-0.1.4.3/parsee/extraction/tasks/meta_info_structuring/meta_info.py
+-rw-r--r--   0        0        0     2641 2024-04-10 14:57:20.437514 parsee_core-0.1.4.3/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.4.3/parsee/extraction/tasks/questions/__init__.py
+-rw-r--r--   0        0        0     6136 2024-04-10 14:57:20.437823 parsee_core-0.1.4.3/parsee/extraction/tasks/questions/features.py
+-rw-r--r--   0        0        0     1430 2024-03-01 12:41:34.971601 parsee_core-0.1.4.3/parsee/extraction/tasks/questions/question_model.py
+-rw-r--r--   0        0        0     4031 2024-04-10 14:57:20.438067 parsee_core-0.1.4.3/parsee/extraction/tasks/questions/question_model_llm.py
+-rw-r--r--   0        0        0     2678 2024-03-12 17:16:10.730178 parsee_core-0.1.4.3/parsee/extraction/tasks/questions/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 14:40:07.901000 parsee_core-0.1.4.3/parsee/storage/__init__.py
+-rw-r--r--   0        0        0     2366 2024-04-10 14:57:20.438310 parsee_core-0.1.4.3/parsee/storage/in_memory_storage.py
+-rw-r--r--   0        0        0     1212 2024-04-10 14:57:20.438565 parsee_core-0.1.4.3/parsee/storage/interfaces.py
+-rw-r--r--   0        0        0      317 2024-02-21 09:46:14.327121 parsee_core-0.1.4.3/parsee/storage/vector_stores/interfaces.py
+-rw-r--r--   0        0        0     3204 2024-03-22 17:12:35.963569 parsee_core-0.1.4.3/parsee/storage/vector_stores/simple_faiss.py
+-rw-r--r--   0        0        0        0 2023-08-03 13:44:22.929000 parsee_core-0.1.4.3/parsee/templates/__init__.py
+-rw-r--r--   0        0        0     1360 2024-04-05 15:38:22.487748 parsee_core-0.1.4.3/parsee/templates/element_schema.py
+-rw-r--r--   0        0        0     1959 2024-02-22 09:42:26.246323 parsee_core-0.1.4.3/parsee/templates/general_structuring_schema.py
+-rw-r--r--   0        0        0     4019 2024-04-05 15:38:22.488067 parsee_core-0.1.4.3/parsee/templates/helpers.py
+-rw-r--r--   0        0        0     1288 2024-02-22 09:33:07.394404 parsee_core-0.1.4.3/parsee/templates/job_template.py
+-rw-r--r--   0        0        0     1011 2024-02-14 09:53:17.727343 parsee_core-0.1.4.3/parsee/templates/mappings.py
+-rw-r--r--   0        0        0      384 2024-02-14 09:50:55.308500 parsee_core-0.1.4.3/parsee/templates/template_from_json.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:15:43.630000 parsee_core-0.1.4.3/parsee/utils/__init__.py
+-rw-r--r--   0        0        0      405 2024-02-15 14:56:20.018887 parsee_core-0.1.4.3/parsee/utils/constants.py
+-rw-r--r--   0        0        0      781 2024-03-27 13:19:30.038637 parsee_core-0.1.4.3/parsee/utils/enums.py
+-rw-r--r--   0        0        0     6632 2024-04-08 08:51:44.149915 parsee_core-0.1.4.3/parsee/utils/helper.py
+-rw-r--r--   0        0        0     2030 2024-03-26 12:40:38.547700 parsee_core-0.1.4.3/parsee/utils/sample_items.py
+-rw-r--r--   0        0        0      827 2024-04-11 14:26:51.187498 parsee_core-0.1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 parsee_core-0.1.4.3/PKG-INFO
```

### Comparing `parsee_core-0.1.4.2/LICENSE` & `parsee_core-0.1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/__init__.py` & `parsee_core-0.1.4.3/parsee/__init__.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/cloud/api.py` & `parsee_core-0.1.4.3/parsee/cloud/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import requests
 
 from parsee.templates.job_template import JobTemplate
 from parsee.templates.template_from_json import from_json_dict
 from parsee.extraction.extractor_elements import StandardDocumentFormat
 from parsee.converters.json_to_raw import load_document_from_json
-from parsee.extraction.extractor_dataclasses import ParseeAnswer, ParseeMeta, source_from_json
+from parsee.extraction.extractor_dataclasses import ParseeAnswer, ParseeMeta, source_from_json, AssignedAnswer, ExtractedSource
 
 
 class ParseeCloud:
 
     def __init__(self, api_key: str, custom_host: Optional[str] = None):
 
         self.api_key = api_key
@@ -51,22 +51,47 @@
                 meta_answers = []
                 for item in entry["text"]["metaInfo"]:
                     meta_answers.append(ParseeMeta(item["model"], 0, [], item["class_id"], item["value"], item["prob"]))
                 sources = [source_from_json(x) for x in entry["sources"]]
                 output.append(ParseeAnswer(entry["model"], sources, class_id, class_value, "", True, meta_answers))
         return output
 
-    """
-    upload a PDF, HTML or image file to Parsee Cloud
-    """
     def upload_file(self, file_path: str) -> str:
+        """
+        upload a PDF, HTML or image file to Parsee Cloud
+        """
         with open(file_path, "rb") as f:
             data = f.read()
         file_data = {'file': (os.path.basename(file_path), data)}
 
         extractor_url = f"{self.host}/api/document/upload?method=simple"
 
         r = requests.post(extractor_url, {}, files=file_data, headers=self._headers())
 
         data = r.json()
 
         return list(data[0].values())[0]
+
+    def add_assigned_answers(self, template_id: str, source_identifier: str, answers: List[AssignedAnswer]) -> bool:
+        """
+        adds one or more assigned answers to the Parsee Cloud database
+        """
+        failed = False
+        for answer in answers:
+            data = {
+                "sourceIdentifier": source_identifier,
+                "templateId": template_id,
+                "itemId": answer.class_id,
+                "newValue": answer.class_value,
+                "newMeta": [
+                    {"model": "manual", "class_id": meta_item.class_id, "value": meta_item.class_value, "prob": 1.0} for meta_item in answer.meta
+                ],
+                "sources": [source.to_json_dict() for source in answer.sources]
+            }
+
+            url = f"{self.host}/api/extraction/output/general-query"
+
+            r = requests.post(url, json=data, headers=self._headers())
+
+            if r.status_code != 200:
+                failed = True
+        return not failed
```

### Comparing `parsee_core-0.1.4.2/parsee/converters/html_extraction.py` & `parsee_core-0.1.4.3/parsee/converters/html_extraction.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/converters/image_creation.py` & `parsee_core-0.1.4.3/parsee/converters/image_creation.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/converters/json_to_raw.py` & `parsee_core-0.1.4.3/parsee/converters/json_to_raw.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/converters/langchain.py` & `parsee_core-0.1.4.3/parsee/converters/langchain.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/converters/main.py` & `parsee_core-0.1.4.3/parsee/converters/main.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/converters/pdf_extraction.py` & `parsee_core-0.1.4.3/parsee/converters/pdf_extraction.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/datasets/dataset_dataclasses.py` & `parsee_core-0.1.4.3/parsee/datasets/dataset_dataclasses.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/datasets/evaluation/main.py` & `parsee_core-0.1.4.3/parsee/datasets/evaluation/main.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/datasets/main.py` & `parsee_core-0.1.4.3/parsee/datasets/main.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/datasets/readers/disk_reader.py` & `parsee_core-0.1.4.3/parsee/datasets/readers/disk_reader.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/datasets/readers/interfaces.py` & `parsee_core-0.1.4.3/parsee/datasets/readers/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/datasets/writers/disk_writer.py` & `parsee_core-0.1.4.3/parsee/datasets/writers/disk_writer.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/datasets/writers/interfaces.py` & `parsee_core-0.1.4.3/parsee/datasets/writers/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/extractor_dataclasses.py` & `parsee_core-0.1.4.3/parsee/extraction/extractor_dataclasses.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/extractor_elements.py` & `parsee_core-0.1.4.3/parsee/extraction/extractor_elements.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/final_structuring.py` & `parsee_core-0.1.4.3/parsee/extraction/final_structuring.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/models/helpers.py` & `parsee_core-0.1.4.3/parsee/extraction/models/helpers.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/models/llm_models/anthropic_model.py` & `parsee_core-0.1.4.3/parsee/extraction/models/llm_models/anthropic_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/models/llm_models/chatgpt_model.py` & `parsee_core-0.1.4.3/parsee/extraction/models/llm_models/chatgpt_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/models/llm_models/llm_base_model.py` & `parsee_core-0.1.4.3/parsee/extraction/models/llm_models/llm_base_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/models/llm_models/ollama_model.py` & `parsee_core-0.1.4.3/parsee/extraction/models/llm_models/ollama_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/models/llm_models/prompts.py` & `parsee_core-0.1.4.3/parsee/extraction/models/llm_models/prompts.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/models/llm_models/replicate_model.py` & `parsee_core-0.1.4.3/parsee/extraction/models/llm_models/replicate_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/models/llm_models/structuring_schema.py` & `parsee_core-0.1.4.3/parsee/extraction/models/llm_models/structuring_schema.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/models/model_dataclasses.py` & `parsee_core-0.1.4.3/parsee/extraction/models/model_dataclasses.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/models/model_loader.py` & `parsee_core-0.1.4.3/parsee/extraction/models/model_loader.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/run.py` & `parsee_core-0.1.4.3/parsee/extraction/run.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/tasks/element_classification/element_model.py` & `parsee_core-0.1.4.3/parsee/extraction/tasks/element_classification/element_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/tasks/element_classification/element_model_llm.py` & `parsee_core-0.1.4.3/parsee/extraction/tasks/element_classification/element_model_llm.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/tasks/element_classification/features.py` & `parsee_core-0.1.4.3/parsee/extraction/tasks/element_classification/features.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/tasks/mappings/features.py` & `parsee_core-0.1.4.3/parsee/extraction/tasks/mappings/features.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/tasks/mappings/mapping_model.py` & `parsee_core-0.1.4.3/parsee/extraction/tasks/mappings/mapping_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/tasks/mappings/mapping_model_llm.py` & `parsee_core-0.1.4.3/parsee/extraction/tasks/mappings/mapping_model_llm.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/tasks/mappings/utils.py` & `parsee_core-0.1.4.3/parsee/extraction/tasks/mappings/utils.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/tasks/meta_info_structuring/features.py` & `parsee_core-0.1.4.3/parsee/extraction/tasks/meta_info_structuring/features.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/tasks/meta_info_structuring/meta_info.py` & `parsee_core-0.1.4.3/parsee/extraction/tasks/meta_info_structuring/meta_info.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py` & `parsee_core-0.1.4.3/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/tasks/questions/features.py` & `parsee_core-0.1.4.3/parsee/extraction/tasks/questions/features.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/tasks/questions/question_model.py` & `parsee_core-0.1.4.3/parsee/extraction/tasks/questions/question_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/tasks/questions/question_model_llm.py` & `parsee_core-0.1.4.3/parsee/extraction/tasks/questions/question_model_llm.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/extraction/tasks/questions/utils.py` & `parsee_core-0.1.4.3/parsee/extraction/tasks/questions/utils.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/storage/in_memory_storage.py` & `parsee_core-0.1.4.3/parsee/storage/in_memory_storage.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/storage/interfaces.py` & `parsee_core-0.1.4.3/parsee/storage/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/storage/vector_stores/simple_faiss.py` & `parsee_core-0.1.4.3/parsee/storage/vector_stores/simple_faiss.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/templates/element_schema.py` & `parsee_core-0.1.4.3/parsee/templates/element_schema.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/templates/general_structuring_schema.py` & `parsee_core-0.1.4.3/parsee/templates/general_structuring_schema.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/templates/helpers.py` & `parsee_core-0.1.4.3/parsee/templates/helpers.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/templates/job_template.py` & `parsee_core-0.1.4.3/parsee/templates/job_template.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/templates/mappings.py` & `parsee_core-0.1.4.3/parsee/templates/mappings.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/utils/enums.py` & `parsee_core-0.1.4.3/parsee/utils/enums.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/utils/helper.py` & `parsee_core-0.1.4.3/parsee/utils/helper.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/parsee/utils/sample_items.py` & `parsee_core-0.1.4.3/parsee/utils/sample_items.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.2/pyproject.toml` & `parsee_core-0.1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parsee-core"
-version = "0.1.4.2"
+version = "0.1.4.3"
 description = ""
 authors = ["Parsee.ai <info@parsee.ai>"]
 homepage = "https://parsee.ai"
 packages = [{include = "parsee"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
```

### Comparing `parsee_core-0.1.4.2/PKG-INFO` & `parsee_core-0.1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsee-core
-Version: 0.1.4.2
+Version: 0.1.4.3
 Summary: 
 Home-page: https://parsee.ai
 Author: Parsee.ai
 Author-email: info@parsee.ai
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

