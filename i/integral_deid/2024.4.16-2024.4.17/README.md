# Comparing `tmp/integral_deid-2024.4.16.tar.gz` & `tmp/integral_deid-2024.4.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integral_deid-2024.4.16.tar", max compression
+gzip compressed data, was "integral_deid-2024.4.17.tar", max compression
```

## Comparing `integral_deid-2024.4.16.tar` & `integral_deid-2024.4.17.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     7126 2024-04-05 16:49:03.600397 integral_deid-2024.4.16/integral_deid/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-11 16:09:06.913504 integral_deid-2024.4.16/integral_deid/argmax_process.py
--rw-r--r--   0        0        0      665 2024-03-27 18:41:58.721027 integral_deid-2024.4.16/integral_deid/check_consistent_length.py
--rw-r--r--   0        0        0     3178 2024-03-27 18:41:58.721206 integral_deid-2024.4.16/integral_deid/clean_regex.py
--rw-r--r--   0        0        0    14684 2024-03-27 18:41:58.721410 integral_deid-2024.4.16/integral_deid/clinical_regex.py
--rw-r--r--   0        0        0     3274 2024-04-11 16:09:06.917170 integral_deid-2024.4.16/integral_deid/clinical_spacy_tokenizer.py
--rw-r--r--   0        0        0     2017 2024-03-27 18:41:58.721936 integral_deid-2024.4.16/integral_deid/conditional_random_field_sub.py
--rw-r--r--   0        0        0     2385 2024-03-27 18:41:58.722088 integral_deid-2024.4.16/integral_deid/core_nlp_tokenizer.py
--rw-r--r--   0        0        0     1130 2024-04-11 16:09:06.921313 integral_deid-2024.4.16/integral_deid/crf_argmax_process.py
--rw-r--r--   0        0        0     3378 2024-04-11 16:09:06.923955 integral_deid-2024.4.16/integral_deid/crf_bert_model_for_token_classification.py
--rw-r--r--   0        0        0     3956 2024-04-11 16:09:06.926157 integral_deid-2024.4.16/integral_deid/crf_process.py
--rw-r--r--   0        0        0      659 2024-03-27 18:41:58.722929 integral_deid-2024.4.16/integral_deid/crf_token_classifier_output.py
--rw-r--r--   0        0        0     5886 2024-03-27 18:41:58.723170 integral_deid-2024.4.16/integral_deid/crf_utils.py
--rw-r--r--   0        0        0     4066 2024-03-27 18:41:58.723347 integral_deid-2024.4.16/integral_deid/data_training_arguments.py
--rw-r--r--   0        0        0     6840 2024-04-11 16:09:06.928227 integral_deid-2024.4.16/integral_deid/dataset.py
--rw-r--r--   0        0        0     9001 2024-04-11 16:09:06.930502 integral_deid-2024.4.16/integral_deid/dataset_creator.py
--rw-r--r--   0        0        0    10063 2024-03-27 18:41:58.724005 integral_deid-2024.4.16/integral_deid/dataset_tokenizer.py
--rw-r--r--   0        0        0     3827 2024-03-27 18:41:58.724178 integral_deid-2024.4.16/integral_deid/date_regex.py
--rw-r--r--   0        0        0     1055 2024-03-27 18:41:58.724416 integral_deid-2024.4.16/integral_deid/evaluation_arguments.py
--rw-r--r--   0        0        0     4073 2024-04-11 16:09:06.933240 integral_deid-2024.4.16/integral_deid/label_mapper.py
--rw-r--r--   0        0        0     2255 2024-03-27 18:41:58.724927 integral_deid-2024.4.16/integral_deid/logits_process.py
--rw-r--r--   0        0        0      326 2024-03-27 18:41:58.725115 integral_deid-2024.4.16/integral_deid/mismatch_error.py
--rw-r--r--   0        0        0     1527 2024-03-27 18:41:58.725304 integral_deid-2024.4.16/integral_deid/model_arguments.py
--rw-r--r--   0        0        0     3572 2024-04-11 16:09:06.935112 integral_deid-2024.4.16/integral_deid/model_picker.py
--rw-r--r--   0        0        0     3637 2024-03-27 18:41:58.725725 integral_deid-2024.4.16/integral_deid/ner_dataset.py
--rw-r--r--   0        0        0     2937 2024-03-27 18:41:58.725893 integral_deid-2024.4.16/integral_deid/ner_labels.py
--rw-r--r--   0        0        0     1072 2024-03-27 18:41:58.726064 integral_deid-2024.4.16/integral_deid/ner_predict_token_labels.py
--rw-r--r--   0        0        0     7782 2024-04-11 16:09:06.949311 integral_deid-2024.4.16/integral_deid/ner_token_labels.py
--rw-r--r--   0        0        0     8420 2024-03-27 18:41:58.726521 integral_deid-2024.4.16/integral_deid/note_level_aggregator.py
--rw-r--r--   0        0        0     1053 2024-03-27 18:41:58.726707 integral_deid-2024.4.16/integral_deid/note_sentencizer.py
--rw-r--r--   0        0        0     2659 2024-04-11 16:09:06.951048 integral_deid-2024.4.16/integral_deid/post_process_picker.py
--rw-r--r--   0        0        0     2380 2024-04-11 16:09:06.952852 integral_deid-2024.4.16/integral_deid/preprocessing_loader.py
--rw-r--r--   0        0        0    24393 2024-03-27 18:41:58.727527 integral_deid-2024.4.16/integral_deid/sentence_dataset.py
--rw-r--r--   0        0        0    25731 2024-04-11 16:09:06.955005 integral_deid-2024.4.16/integral_deid/sequence_tagging.py
--rw-r--r--   0        0        0     1258 2024-03-27 18:41:58.728155 integral_deid-2024.4.16/integral_deid/spacy_sentencizer.py
--rw-r--r--   0        0        0     1864 2024-03-27 18:41:58.728303 integral_deid-2024.4.16/integral_deid/spacy_tokenizer.py
--rw-r--r--   0        0        0     9042 2024-04-11 16:09:06.957370 integral_deid-2024.4.16/integral_deid/text_deid.py
--rw-r--r--   0        0        0     1079 2024-03-27 18:41:58.728699 integral_deid-2024.4.16/integral_deid/text_deid_utils.py
--rw-r--r--   0        0        0     2444 2024-04-11 16:09:06.959161 integral_deid-2024.4.16/integral_deid/threshold_process_max.py
--rw-r--r--   0        0        0     2358 2024-04-11 16:09:06.961033 integral_deid-2024.4.16/integral_deid/threshold_process_sum.py
--rw-r--r--   0        0        0      761 2024-04-11 18:46:01.291676 integral_deid-2024.4.16/pyproject.toml
--rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 integral_deid-2024.4.16/PKG-INFO
+-rw-r--r--   0        0        0     7126 2024-04-05 16:49:03.600397 integral_deid-2024.4.17/integral_deid/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-11 16:09:06.913504 integral_deid-2024.4.17/integral_deid/argmax_process.py
+-rw-r--r--   0        0        0      665 2024-03-27 18:41:58.721027 integral_deid-2024.4.17/integral_deid/check_consistent_length.py
+-rw-r--r--   0        0        0     3178 2024-03-27 18:41:58.721206 integral_deid-2024.4.17/integral_deid/clean_regex.py
+-rw-r--r--   0        0        0    14684 2024-03-27 18:41:58.721410 integral_deid-2024.4.17/integral_deid/clinical_regex.py
+-rw-r--r--   0        0        0     3274 2024-04-11 16:09:06.917170 integral_deid-2024.4.17/integral_deid/clinical_spacy_tokenizer.py
+-rw-r--r--   0        0        0     2017 2024-03-27 18:41:58.721936 integral_deid-2024.4.17/integral_deid/conditional_random_field_sub.py
+-rw-r--r--   0        0        0     2385 2024-03-27 18:41:58.722088 integral_deid-2024.4.17/integral_deid/core_nlp_tokenizer.py
+-rw-r--r--   0        0        0     1130 2024-04-11 16:09:06.921313 integral_deid-2024.4.17/integral_deid/crf_argmax_process.py
+-rw-r--r--   0        0        0     3378 2024-04-11 16:09:06.923955 integral_deid-2024.4.17/integral_deid/crf_bert_model_for_token_classification.py
+-rw-r--r--   0        0        0     3956 2024-04-11 16:09:06.926157 integral_deid-2024.4.17/integral_deid/crf_process.py
+-rw-r--r--   0        0        0      659 2024-03-27 18:41:58.722929 integral_deid-2024.4.17/integral_deid/crf_token_classifier_output.py
+-rw-r--r--   0        0        0     5886 2024-03-27 18:41:58.723170 integral_deid-2024.4.17/integral_deid/crf_utils.py
+-rw-r--r--   0        0        0     4066 2024-03-27 18:41:58.723347 integral_deid-2024.4.17/integral_deid/data_training_arguments.py
+-rw-r--r--   0        0        0     6840 2024-04-11 16:09:06.928227 integral_deid-2024.4.17/integral_deid/dataset.py
+-rw-r--r--   0        0        0     9001 2024-04-11 16:09:06.930502 integral_deid-2024.4.17/integral_deid/dataset_creator.py
+-rw-r--r--   0        0        0    10063 2024-03-27 18:41:58.724005 integral_deid-2024.4.17/integral_deid/dataset_tokenizer.py
+-rw-r--r--   0        0        0     3827 2024-03-27 18:41:58.724178 integral_deid-2024.4.17/integral_deid/date_regex.py
+-rw-r--r--   0        0        0     1055 2024-03-27 18:41:58.724416 integral_deid-2024.4.17/integral_deid/evaluation_arguments.py
+-rw-r--r--   0        0        0     4073 2024-04-11 16:09:06.933240 integral_deid-2024.4.17/integral_deid/label_mapper.py
+-rw-r--r--   0        0        0     2255 2024-03-27 18:41:58.724927 integral_deid-2024.4.17/integral_deid/logits_process.py
+-rw-r--r--   0        0        0      326 2024-03-27 18:41:58.725115 integral_deid-2024.4.17/integral_deid/mismatch_error.py
+-rw-r--r--   0        0        0     1527 2024-03-27 18:41:58.725304 integral_deid-2024.4.17/integral_deid/model_arguments.py
+-rw-r--r--   0        0        0     3572 2024-04-11 16:09:06.935112 integral_deid-2024.4.17/integral_deid/model_picker.py
+-rw-r--r--   0        0        0     3637 2024-03-27 18:41:58.725725 integral_deid-2024.4.17/integral_deid/ner_dataset.py
+-rw-r--r--   0        0        0     2937 2024-03-27 18:41:58.725893 integral_deid-2024.4.17/integral_deid/ner_labels.py
+-rw-r--r--   0        0        0     1072 2024-03-27 18:41:58.726064 integral_deid-2024.4.17/integral_deid/ner_predict_token_labels.py
+-rw-r--r--   0        0        0     7782 2024-04-11 16:09:06.949311 integral_deid-2024.4.17/integral_deid/ner_token_labels.py
+-rw-r--r--   0        0        0     8420 2024-03-27 18:41:58.726521 integral_deid-2024.4.17/integral_deid/note_level_aggregator.py
+-rw-r--r--   0        0        0     1053 2024-03-27 18:41:58.726707 integral_deid-2024.4.17/integral_deid/note_sentencizer.py
+-rw-r--r--   0        0        0     2659 2024-04-11 16:09:06.951048 integral_deid-2024.4.17/integral_deid/post_process_picker.py
+-rw-r--r--   0        0        0     2380 2024-04-11 16:09:06.952852 integral_deid-2024.4.17/integral_deid/preprocessing_loader.py
+-rw-r--r--   0        0        0    24393 2024-03-27 18:41:58.727527 integral_deid-2024.4.17/integral_deid/sentence_dataset.py
+-rw-r--r--   0        0        0    25731 2024-04-11 16:09:06.955005 integral_deid-2024.4.17/integral_deid/sequence_tagging.py
+-rw-r--r--   0        0        0     1258 2024-03-27 18:41:58.728155 integral_deid-2024.4.17/integral_deid/spacy_sentencizer.py
+-rw-r--r--   0        0        0     1864 2024-03-27 18:41:58.728303 integral_deid-2024.4.17/integral_deid/spacy_tokenizer.py
+-rw-r--r--   0        0        0     9042 2024-04-11 16:09:06.957370 integral_deid-2024.4.17/integral_deid/text_deid.py
+-rw-r--r--   0        0        0     1079 2024-03-27 18:41:58.728699 integral_deid-2024.4.17/integral_deid/text_deid_utils.py
+-rw-r--r--   0        0        0     2444 2024-04-11 16:09:06.959161 integral_deid-2024.4.17/integral_deid/threshold_process_max.py
+-rw-r--r--   0        0        0     2358 2024-04-11 16:09:06.961033 integral_deid-2024.4.17/integral_deid/threshold_process_sum.py
+-rw-r--r--   0        0        0      760 2024-04-11 21:20:32.183224 integral_deid-2024.4.17/pyproject.toml
+-rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 integral_deid-2024.4.17/PKG-INFO
```

### Comparing `integral_deid-2024.4.16/integral_deid/__init__.py` & `integral_deid-2024.4.17/integral_deid/__init__.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/argmax_process.py` & `integral_deid-2024.4.17/integral_deid/argmax_process.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/check_consistent_length.py` & `integral_deid-2024.4.17/integral_deid/check_consistent_length.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/clean_regex.py` & `integral_deid-2024.4.17/integral_deid/clean_regex.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/clinical_regex.py` & `integral_deid-2024.4.17/integral_deid/clinical_regex.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/clinical_spacy_tokenizer.py` & `integral_deid-2024.4.17/integral_deid/clinical_spacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/conditional_random_field_sub.py` & `integral_deid-2024.4.17/integral_deid/conditional_random_field_sub.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/core_nlp_tokenizer.py` & `integral_deid-2024.4.17/integral_deid/core_nlp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/crf_argmax_process.py` & `integral_deid-2024.4.17/integral_deid/crf_argmax_process.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/crf_bert_model_for_token_classification.py` & `integral_deid-2024.4.17/integral_deid/crf_bert_model_for_token_classification.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/crf_process.py` & `integral_deid-2024.4.17/integral_deid/crf_process.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/crf_token_classifier_output.py` & `integral_deid-2024.4.17/integral_deid/crf_token_classifier_output.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/crf_utils.py` & `integral_deid-2024.4.17/integral_deid/crf_utils.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/data_training_arguments.py` & `integral_deid-2024.4.17/integral_deid/data_training_arguments.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/dataset.py` & `integral_deid-2024.4.17/integral_deid/dataset.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/dataset_creator.py` & `integral_deid-2024.4.17/integral_deid/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/dataset_tokenizer.py` & `integral_deid-2024.4.17/integral_deid/dataset_tokenizer.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/date_regex.py` & `integral_deid-2024.4.17/integral_deid/date_regex.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/evaluation_arguments.py` & `integral_deid-2024.4.17/integral_deid/evaluation_arguments.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/label_mapper.py` & `integral_deid-2024.4.17/integral_deid/label_mapper.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/logits_process.py` & `integral_deid-2024.4.17/integral_deid/logits_process.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/model_arguments.py` & `integral_deid-2024.4.17/integral_deid/model_arguments.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/model_picker.py` & `integral_deid-2024.4.17/integral_deid/model_picker.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/ner_dataset.py` & `integral_deid-2024.4.17/integral_deid/ner_dataset.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/ner_labels.py` & `integral_deid-2024.4.17/integral_deid/ner_labels.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/ner_predict_token_labels.py` & `integral_deid-2024.4.17/integral_deid/ner_predict_token_labels.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/ner_token_labels.py` & `integral_deid-2024.4.17/integral_deid/ner_token_labels.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/note_level_aggregator.py` & `integral_deid-2024.4.17/integral_deid/note_level_aggregator.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/note_sentencizer.py` & `integral_deid-2024.4.17/integral_deid/note_sentencizer.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/post_process_picker.py` & `integral_deid-2024.4.17/integral_deid/post_process_picker.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/preprocessing_loader.py` & `integral_deid-2024.4.17/integral_deid/preprocessing_loader.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/sentence_dataset.py` & `integral_deid-2024.4.17/integral_deid/sentence_dataset.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/sequence_tagging.py` & `integral_deid-2024.4.17/integral_deid/sequence_tagging.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/spacy_sentencizer.py` & `integral_deid-2024.4.17/integral_deid/spacy_sentencizer.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/spacy_tokenizer.py` & `integral_deid-2024.4.17/integral_deid/spacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/text_deid.py` & `integral_deid-2024.4.17/integral_deid/text_deid.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/text_deid_utils.py` & `integral_deid-2024.4.17/integral_deid/text_deid_utils.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/threshold_process_max.py` & `integral_deid-2024.4.17/integral_deid/threshold_process_max.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/integral_deid/threshold_process_sum.py` & `integral_deid-2024.4.17/integral_deid/threshold_process_sum.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.16/pyproject.toml` & `integral_deid-2024.4.17/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "integral_deid"
-version = "2024.04.16"
+version = "2024.04.17"
 description = "PHI taggging and redaction"
 authors = ["Kevin DeSimone <kevin@useintegral.com>", "Dominick Villano <dominick@useintegral.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 transformers = "4.39.1"
 spacy = "3.7.4"
@@ -14,15 +14,14 @@
 tensorboard = "2.16.2"
 seqeval = "1.2.2"
 accelerate = "0.28.0"
 allennlp-light = "1.0.0"
 databricks-sdk = "0.23.0"
 markupsafe = "2.0.1"
 
-
 [tool.poetry.dev-dependencies]
 black = "23.12.1"
 coverage = "7.4.3"
 flake8 = "7.0.0"
 mypy = "1.8.0"
 pandas-stubs = "2.1.4.231227"
 pre-commit = "3.6.0"
```

### Comparing `integral_deid-2024.4.16/PKG-INFO` & `integral_deid-2024.4.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integral_deid
-Version: 2024.4.16
+Version: 2024.4.17
 Summary: PHI taggging and redaction
 Author: Kevin DeSimone
 Author-email: kevin@useintegral.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

