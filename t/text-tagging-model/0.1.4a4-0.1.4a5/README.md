# Comparing `tmp/text_tagging_model-0.1.4a4.tar.gz` & `tmp/text_tagging_model-0.1.4a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_tagging_model-0.1.4a4.tar", max compression
+gzip compressed data, was "text_tagging_model-0.1.4a5.tar", max compression
```

## Comparing `text_tagging_model-0.1.4a4.tar` & `text_tagging_model-0.1.4a5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0       41 2024-04-11 20:15:26.658891 text_tagging_model-0.1.4a4/README.md
--rw-r--r--   0        0        0     1573 2024-04-12 00:21:34.462838 text_tagging_model-0.1.4a4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 20:15:26.662053 text_tagging_model-0.1.4a4/text_tagging_model/__init__.py
--rw-r--r--   0        0        0     1247 2024-04-11 22:07:22.313440 text_tagging_model-0.1.4a4/text_tagging_model/logger_config.py
--rw-r--r--   0        0        0        0 2024-04-11 20:15:26.662246 text_tagging_model-0.1.4a4/text_tagging_model/models/__init__.py
--rw-r--r--   0        0        0       61 2024-04-11 22:32:30.780888 text_tagging_model-0.1.4a4/text_tagging_model/models/attention_based_model/__init__.py
--rw-r--r--   0        0        0     3655 2024-04-12 00:12:07.814103 text_tagging_model-0.1.4a4/text_tagging_model/models/attention_based_model/attention_extractor.py
--rw-r--r--   0        0        0       89 2024-04-11 20:15:26.662508 text_tagging_model-0.1.4a4/text_tagging_model/models/bart_based_model/__init__.py
--rw-r--r--   0        0        0     2594 2024-04-11 20:15:26.662636 text_tagging_model-0.1.4a4/text_tagging_model/models/bart_based_model/tag_sum_extractor.py
--rw-r--r--   0        0        0      575 2024-04-11 20:15:26.662732 text_tagging_model-0.1.4a4/text_tagging_model/models/base_extractor.py
--rw-r--r--   0        0        0     1230 2024-04-11 20:15:26.662826 text_tagging_model-0.1.4a4/text_tagging_model/models/metrics.py
--rw-r--r--   0        0        0       84 2024-04-11 20:15:26.662964 text_tagging_model-0.1.4a4/text_tagging_model/models/rake_based_model/__init__.py
--rw-r--r--   0        0        0     1526 2024-04-11 20:15:26.663056 text_tagging_model-0.1.4a4/text_tagging_model/models/rake_based_model/keyphrases_extractor.py
--rw-r--r--   0        0        0     2537 2024-04-11 20:15:26.663352 text_tagging_model-0.1.4a4/text_tagging_model/models/rake_based_model/tags_extractor.py
--rw-r--r--   0        0        0      216 2024-04-11 20:15:26.663569 text_tagging_model-0.1.4a4/text_tagging_model/processing/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 20:15:26.663668 text_tagging_model-0.1.4a4/text_tagging_model/processing/embedder/__init__.py
--rw-r--r--   0        0        0      556 2024-04-11 20:15:26.663790 text_tagging_model-0.1.4a4/text_tagging_model/processing/embedder/base_embedder.py
--rw-r--r--   0        0        0      675 2024-04-11 20:15:26.663901 text_tagging_model-0.1.4a4/text_tagging_model/processing/embedder/fasttext_embedder.py
--rw-r--r--   0        0        0     1097 2024-04-11 20:15:26.664002 text_tagging_model-0.1.4a4/text_tagging_model/processing/embedder/hg_embedder.py
--rw-r--r--   0        0        0      365 2024-04-11 20:15:26.664149 text_tagging_model-0.1.4a4/text_tagging_model/processing/normalizers/__init__.py
--rw-r--r--   0        0        0      166 2024-04-11 20:15:26.664238 text_tagging_model-0.1.4a4/text_tagging_model/processing/normalizers/base_normalizer.py
--rw-r--r--   0        0        0      996 2024-04-11 20:15:26.664335 text_tagging_model-0.1.4a4/text_tagging_model/processing/normalizers/nouns_keeper.py
--rw-r--r--   0        0        0      624 2024-04-11 20:15:26.664426 text_tagging_model-0.1.4a4/text_tagging_model/processing/normalizers/pipe.py
--rw-r--r--   0        0        0      456 2024-04-11 22:03:58.493567 text_tagging_model-0.1.4a4/text_tagging_model/processing/normalizers/punctuation_deleter.py
--rw-r--r--   0        0        0     1025 2024-04-11 22:21:45.482586 text_tagging_model-0.1.4a4/text_tagging_model/processing/normalizers/stopwords_deleter.py
--rw-r--r--   0        0        0        0 2024-04-11 20:15:26.664701 text_tagging_model-0.1.4a4/text_tagging_model/processing/ranker/__init__.py
--rw-r--r--   0        0        0     1193 2024-04-11 20:15:26.664804 text_tagging_model-0.1.4a4/text_tagging_model/processing/ranker/base_ranker.py
--rw-r--r--   0        0        0     1021 2024-04-11 20:15:26.664888 text_tagging_model-0.1.4a4/text_tagging_model/processing/ranker/max_distance_ranker.py
--rw-r--r--   0        0        0      543 2024-04-11 20:15:26.664979 text_tagging_model-0.1.4a4/text_tagging_model/processing/ranker/text_sim_ranker.py
--rw-r--r--   0        0        0        0 2024-04-11 20:15:26.665067 text_tagging_model-0.1.4a4/text_tagging_model/processing/summarizator/__init__.py
--rw-r--r--   0        0        0     1089 2024-04-11 20:15:26.665176 text_tagging_model-0.1.4a4/text_tagging_model/processing/summarizator/bart_summarization.py
--rw-r--r--   0        0        0       58 2024-04-11 20:15:26.665253 text_tagging_model-0.1.4a4/text_tagging_model/processing/utils.py
--rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 text_tagging_model-0.1.4a4/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-04-11 20:15:26.658891 text_tagging_model-0.1.4a5/README.md
+-rw-r--r--   0        0        0     1573 2024-04-12 01:11:44.449869 text_tagging_model-0.1.4a5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 20:15:26.662053 text_tagging_model-0.1.4a5/text_tagging_model/__init__.py
+-rw-r--r--   0        0        0     1247 2024-04-11 22:07:22.313440 text_tagging_model-0.1.4a5/text_tagging_model/logger_config.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:15:26.662246 text_tagging_model-0.1.4a5/text_tagging_model/models/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-11 22:32:30.780888 text_tagging_model-0.1.4a5/text_tagging_model/models/attention_based_model/__init__.py
+-rw-r--r--   0        0        0     3655 2024-04-12 00:12:07.814103 text_tagging_model-0.1.4a5/text_tagging_model/models/attention_based_model/attention_extractor.py
+-rw-r--r--   0        0        0       89 2024-04-11 20:15:26.662508 text_tagging_model-0.1.4a5/text_tagging_model/models/bart_based_model/__init__.py
+-rw-r--r--   0        0        0     2594 2024-04-11 20:15:26.662636 text_tagging_model-0.1.4a5/text_tagging_model/models/bart_based_model/tag_sum_extractor.py
+-rw-r--r--   0        0        0      575 2024-04-11 20:15:26.662732 text_tagging_model-0.1.4a5/text_tagging_model/models/base_extractor.py
+-rw-r--r--   0        0        0     1230 2024-04-11 20:15:26.662826 text_tagging_model-0.1.4a5/text_tagging_model/models/metrics.py
+-rw-r--r--   0        0        0       84 2024-04-11 20:15:26.662964 text_tagging_model-0.1.4a5/text_tagging_model/models/rake_based_model/__init__.py
+-rw-r--r--   0        0        0     1526 2024-04-11 20:15:26.663056 text_tagging_model-0.1.4a5/text_tagging_model/models/rake_based_model/keyphrases_extractor.py
+-rw-r--r--   0        0        0     2537 2024-04-11 20:15:26.663352 text_tagging_model-0.1.4a5/text_tagging_model/models/rake_based_model/tags_extractor.py
+-rw-r--r--   0        0        0      216 2024-04-11 20:15:26.663569 text_tagging_model-0.1.4a5/text_tagging_model/processing/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:15:26.663668 text_tagging_model-0.1.4a5/text_tagging_model/processing/embedder/__init__.py
+-rw-r--r--   0        0        0      556 2024-04-11 20:15:26.663790 text_tagging_model-0.1.4a5/text_tagging_model/processing/embedder/base_embedder.py
+-rw-r--r--   0        0        0      675 2024-04-11 20:15:26.663901 text_tagging_model-0.1.4a5/text_tagging_model/processing/embedder/fasttext_embedder.py
+-rw-r--r--   0        0        0     1097 2024-04-11 20:15:26.664002 text_tagging_model-0.1.4a5/text_tagging_model/processing/embedder/hg_embedder.py
+-rw-r--r--   0        0        0      365 2024-04-11 20:15:26.664149 text_tagging_model-0.1.4a5/text_tagging_model/processing/normalizers/__init__.py
+-rw-r--r--   0        0        0      166 2024-04-11 20:15:26.664238 text_tagging_model-0.1.4a5/text_tagging_model/processing/normalizers/base_normalizer.py
+-rw-r--r--   0        0        0     2806 2024-04-12 01:11:39.106958 text_tagging_model-0.1.4a5/text_tagging_model/processing/normalizers/nouns_keeper.py
+-rw-r--r--   0        0        0      624 2024-04-11 20:15:26.664426 text_tagging_model-0.1.4a5/text_tagging_model/processing/normalizers/pipe.py
+-rw-r--r--   0        0        0      456 2024-04-11 22:03:58.493567 text_tagging_model-0.1.4a5/text_tagging_model/processing/normalizers/punctuation_deleter.py
+-rw-r--r--   0        0        0     1025 2024-04-11 22:21:45.482586 text_tagging_model-0.1.4a5/text_tagging_model/processing/normalizers/stopwords_deleter.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:15:26.664701 text_tagging_model-0.1.4a5/text_tagging_model/processing/ranker/__init__.py
+-rw-r--r--   0        0        0     1193 2024-04-11 20:15:26.664804 text_tagging_model-0.1.4a5/text_tagging_model/processing/ranker/base_ranker.py
+-rw-r--r--   0        0        0     1021 2024-04-11 20:15:26.664888 text_tagging_model-0.1.4a5/text_tagging_model/processing/ranker/max_distance_ranker.py
+-rw-r--r--   0        0        0      543 2024-04-11 20:15:26.664979 text_tagging_model-0.1.4a5/text_tagging_model/processing/ranker/text_sim_ranker.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:15:26.665067 text_tagging_model-0.1.4a5/text_tagging_model/processing/summarizator/__init__.py
+-rw-r--r--   0        0        0     1089 2024-04-11 20:15:26.665176 text_tagging_model-0.1.4a5/text_tagging_model/processing/summarizator/bart_summarization.py
+-rw-r--r--   0        0        0       58 2024-04-11 20:15:26.665253 text_tagging_model-0.1.4a5/text_tagging_model/processing/utils.py
+-rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 text_tagging_model-0.1.4a5/PKG-INFO
```

### Comparing `text_tagging_model-0.1.4a4/pyproject.toml` & `text_tagging_model-0.1.4a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "text-tagging-model"
-version = "0.1.4a4"
+version = "0.1.4a5"
 description = "Here we collected some online and offline models for text tagging."
 authors = [
     "Pavel Kochkin <kochkin27@gmail.com>",
     "Shamil Nurkaev <nurkaievs1204@gmail.com>",
     "Denis <denison03@mail.ru>",
     "Stephan Olizko <stepa.olizko@yandex.ru>"
 ]
```

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/logger_config.py` & `text_tagging_model-0.1.4a5/text_tagging_model/logger_config.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/models/attention_based_model/attention_extractor.py` & `text_tagging_model-0.1.4a5/text_tagging_model/models/attention_based_model/attention_extractor.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/models/bart_based_model/tag_sum_extractor.py` & `text_tagging_model-0.1.4a5/text_tagging_model/models/bart_based_model/tag_sum_extractor.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/models/base_extractor.py` & `text_tagging_model-0.1.4a5/text_tagging_model/models/base_extractor.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/models/metrics.py` & `text_tagging_model-0.1.4a5/text_tagging_model/models/metrics.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/models/rake_based_model/keyphrases_extractor.py` & `text_tagging_model-0.1.4a5/text_tagging_model/models/rake_based_model/keyphrases_extractor.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/models/rake_based_model/tags_extractor.py` & `text_tagging_model-0.1.4a5/text_tagging_model/models/rake_based_model/tags_extractor.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/processing/embedder/base_embedder.py` & `text_tagging_model-0.1.4a5/text_tagging_model/processing/embedder/base_embedder.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/processing/embedder/fasttext_embedder.py` & `text_tagging_model-0.1.4a5/text_tagging_model/processing/embedder/fasttext_embedder.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/processing/embedder/hg_embedder.py` & `text_tagging_model-0.1.4a5/text_tagging_model/processing/embedder/hg_embedder.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/processing/normalizers/pipe.py` & `text_tagging_model-0.1.4a5/text_tagging_model/processing/normalizers/pipe.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/processing/normalizers/stopwords_deleter.py` & `text_tagging_model-0.1.4a5/text_tagging_model/processing/normalizers/stopwords_deleter.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/processing/ranker/base_ranker.py` & `text_tagging_model-0.1.4a5/text_tagging_model/processing/ranker/base_ranker.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/processing/ranker/max_distance_ranker.py` & `text_tagging_model-0.1.4a5/text_tagging_model/processing/ranker/max_distance_ranker.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/processing/ranker/text_sim_ranker.py` & `text_tagging_model-0.1.4a5/text_tagging_model/processing/ranker/text_sim_ranker.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/text_tagging_model/processing/summarizator/bart_summarization.py` & `text_tagging_model-0.1.4a5/text_tagging_model/processing/summarizator/bart_summarization.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.4a4/PKG-INFO` & `text_tagging_model-0.1.4a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-tagging-model
-Version: 0.1.4a4
+Version: 0.1.4a5
 Summary: Here we collected some online and offline models for text tagging.
 Author: Pavel Kochkin
 Author-email: kochkin27@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

