# Comparing `tmp/text_tagging_model-0.1.2a9.tar.gz` & `tmp/text_tagging_model-0.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_tagging_model-0.1.2a9.tar", max compression
+gzip compressed data, was "text_tagging_model-0.1.4a0.tar", max compression
```

## Comparing `text_tagging_model-0.1.2a9.tar` & `text_tagging_model-0.1.4a0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0       41 2024-04-05 18:27:57.393842 text_tagging_model-0.1.2a9/README.md
--rw-r--r--   0        0        0     1540 2024-04-11 10:07:05.228849 text_tagging_model-0.1.2a9/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 13:26:29.785403 text_tagging_model-0.1.2a9/text_tagging_model/__init__.py
--rw-r--r--   0        0        0     1248 2024-04-10 17:38:45.908803 text_tagging_model-0.1.2a9/text_tagging_model/logger_config.py
--rw-r--r--   0        0        0        0 2024-04-10 14:59:49.958211 text_tagging_model-0.1.2a9/text_tagging_model/models/__init__.py
--rw-r--r--   0        0        0       89 2024-04-10 21:18:16.240769 text_tagging_model-0.1.2a9/text_tagging_model/models/bart_based_model/__init__.py
--rw-r--r--   0        0        0     3622 2024-04-11 10:06:53.010074 text_tagging_model-0.1.2a9/text_tagging_model/models/bart_based_model/tag_sum_extractor.py
--rw-r--r--   0        0        0     1230 2024-04-10 13:26:29.785889 text_tagging_model-0.1.2a9/text_tagging_model/models/metrics.py
--rw-r--r--   0        0        0       84 2024-04-10 19:51:48.269012 text_tagging_model-0.1.2a9/text_tagging_model/models/rake_based_model/__init__.py
--rw-r--r--   0        0        0     1526 2024-04-10 17:03:50.201269 text_tagging_model-0.1.2a9/text_tagging_model/models/rake_based_model/keyphrases_extractor.py
--rw-r--r--   0        0        0     3741 2024-04-11 00:11:22.852114 text_tagging_model-0.1.2a9/text_tagging_model/models/rake_based_model/tags_extractor.py
--rw-r--r--   0        0        0      216 2024-04-10 15:00:17.918296 text_tagging_model-0.1.2a9/text_tagging_model/processing/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 15:49:15.254929 text_tagging_model-0.1.2a9/text_tagging_model/processing/embedder/__init__.py
--rw-r--r--   0        0        0      376 2024-04-10 20:39:51.551412 text_tagging_model-0.1.2a9/text_tagging_model/processing/embedder/base_embedder.py
--rw-r--r--   0        0        0      509 2024-04-10 20:00:44.503406 text_tagging_model-0.1.2a9/text_tagging_model/processing/embedder/fasttext_embedder.py
--rw-r--r--   0        0        0      822 2024-04-11 00:09:17.764085 text_tagging_model-0.1.2a9/text_tagging_model/processing/embedder/hg_embedder.py
--rw-r--r--   0        0        0      365 2024-04-10 17:07:38.801435 text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/__init__.py
--rw-r--r--   0        0        0      166 2024-04-10 16:36:32.623920 text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/base_normalizer.py
--rw-r--r--   0        0        0      996 2024-04-10 20:00:44.506705 text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/nouns_keeper.py
--rw-r--r--   0        0        0      624 2024-04-10 20:06:17.954874 text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/pipe.py
--rw-r--r--   0        0        0      456 2024-04-10 20:00:44.508075 text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/punctuation_deleter.py
--rw-r--r--   0        0        0      746 2024-04-10 20:00:44.508861 text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/stopwords_deleter.py
--rw-r--r--   0        0        0        0 2024-04-10 15:47:50.375775 text_tagging_model-0.1.2a9/text_tagging_model/processing/ranker/__init__.py
--rw-r--r--   0        0        0      843 2024-04-11 00:02:41.411968 text_tagging_model-0.1.2a9/text_tagging_model/processing/ranker/base_ranker.py
--rw-r--r--   0        0        0      781 2024-04-11 00:01:12.682816 text_tagging_model-0.1.2a9/text_tagging_model/processing/ranker/max_distance_ranker.py
--rw-r--r--   0        0        0        0 2024-04-10 20:50:54.437113 text_tagging_model-0.1.2a9/text_tagging_model/processing/summarizator/__init__.py
--rw-r--r--   0        0        0     1126 2024-04-10 22:49:41.812642 text_tagging_model-0.1.2a9/text_tagging_model/processing/summarizator/bart_summarization.py
--rw-r--r--   0        0        0       58 2024-04-10 13:26:29.787998 text_tagging_model-0.1.2a9/text_tagging_model/processing/utils.py
--rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 text_tagging_model-0.1.2a9/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-04-11 20:15:26.658891 text_tagging_model-0.1.4a0/README.md
+-rw-r--r--   0        0        0     1573 2024-04-11 22:09:13.193366 text_tagging_model-0.1.4a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 20:15:26.662053 text_tagging_model-0.1.4a0/text_tagging_model/__init__.py
+-rw-r--r--   0        0        0     1247 2024-04-11 22:07:22.313440 text_tagging_model-0.1.4a0/text_tagging_model/logger_config.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:15:26.662246 text_tagging_model-0.1.4a0/text_tagging_model/models/__init__.py
+-rw-r--r--   0        0        0       89 2024-04-11 20:15:26.662508 text_tagging_model-0.1.4a0/text_tagging_model/models/bart_based_model/__init__.py
+-rw-r--r--   0        0        0     2594 2024-04-11 20:15:26.662636 text_tagging_model-0.1.4a0/text_tagging_model/models/bart_based_model/tag_sum_extractor.py
+-rw-r--r--   0        0        0      575 2024-04-11 20:15:26.662732 text_tagging_model-0.1.4a0/text_tagging_model/models/base_extractor.py
+-rw-r--r--   0        0        0     1230 2024-04-11 20:15:26.662826 text_tagging_model-0.1.4a0/text_tagging_model/models/metrics.py
+-rw-r--r--   0        0        0       84 2024-04-11 20:15:26.662964 text_tagging_model-0.1.4a0/text_tagging_model/models/rake_based_model/__init__.py
+-rw-r--r--   0        0        0     1526 2024-04-11 20:15:26.663056 text_tagging_model-0.1.4a0/text_tagging_model/models/rake_based_model/keyphrases_extractor.py
+-rw-r--r--   0        0        0     2537 2024-04-11 20:15:26.663352 text_tagging_model-0.1.4a0/text_tagging_model/models/rake_based_model/tags_extractor.py
+-rw-r--r--   0        0        0      216 2024-04-11 20:15:26.663569 text_tagging_model-0.1.4a0/text_tagging_model/processing/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:15:26.663668 text_tagging_model-0.1.4a0/text_tagging_model/processing/embedder/__init__.py
+-rw-r--r--   0        0        0      556 2024-04-11 20:15:26.663790 text_tagging_model-0.1.4a0/text_tagging_model/processing/embedder/base_embedder.py
+-rw-r--r--   0        0        0      675 2024-04-11 20:15:26.663901 text_tagging_model-0.1.4a0/text_tagging_model/processing/embedder/fasttext_embedder.py
+-rw-r--r--   0        0        0     1097 2024-04-11 20:15:26.664002 text_tagging_model-0.1.4a0/text_tagging_model/processing/embedder/hg_embedder.py
+-rw-r--r--   0        0        0      365 2024-04-11 20:15:26.664149 text_tagging_model-0.1.4a0/text_tagging_model/processing/normalizers/__init__.py
+-rw-r--r--   0        0        0      166 2024-04-11 20:15:26.664238 text_tagging_model-0.1.4a0/text_tagging_model/processing/normalizers/base_normalizer.py
+-rw-r--r--   0        0        0      996 2024-04-11 20:15:26.664335 text_tagging_model-0.1.4a0/text_tagging_model/processing/normalizers/nouns_keeper.py
+-rw-r--r--   0        0        0      624 2024-04-11 20:15:26.664426 text_tagging_model-0.1.4a0/text_tagging_model/processing/normalizers/pipe.py
+-rw-r--r--   0        0        0      456 2024-04-11 22:03:58.493567 text_tagging_model-0.1.4a0/text_tagging_model/processing/normalizers/punctuation_deleter.py
+-rw-r--r--   0        0        0     1024 2024-04-11 22:00:06.117686 text_tagging_model-0.1.4a0/text_tagging_model/processing/normalizers/stopwords_deleter.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:15:26.664701 text_tagging_model-0.1.4a0/text_tagging_model/processing/ranker/__init__.py
+-rw-r--r--   0        0        0     1193 2024-04-11 20:15:26.664804 text_tagging_model-0.1.4a0/text_tagging_model/processing/ranker/base_ranker.py
+-rw-r--r--   0        0        0     1021 2024-04-11 20:15:26.664888 text_tagging_model-0.1.4a0/text_tagging_model/processing/ranker/max_distance_ranker.py
+-rw-r--r--   0        0        0      543 2024-04-11 20:15:26.664979 text_tagging_model-0.1.4a0/text_tagging_model/processing/ranker/text_sim_ranker.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:15:26.665067 text_tagging_model-0.1.4a0/text_tagging_model/processing/summarizator/__init__.py
+-rw-r--r--   0        0        0     1089 2024-04-11 20:15:26.665176 text_tagging_model-0.1.4a0/text_tagging_model/processing/summarizator/bart_summarization.py
+-rw-r--r--   0        0        0       58 2024-04-11 20:15:26.665253 text_tagging_model-0.1.4a0/text_tagging_model/processing/utils.py
+-rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 text_tagging_model-0.1.4a0/PKG-INFO
```

### Comparing `text_tagging_model-0.1.2a9/pyproject.toml` & `text_tagging_model-0.1.4a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "text-tagging-model"
-version = "0.1.2a9"
+version = "0.1.4a0"
 description = "Here we collected some online and offline models for text tagging."
 authors = [
     "Pavel Kochkin <kochkin27@gmail.com>",
     "Shamil Nurkaev <nurkaievs1204@gmail.com>",
     "Denis <denison03@mail.ru>",
     "Stephan Olizko <stepa.olizko@yandex.ru>"
 ]
 readme = "README.md"
 packages = [{include = "text_tagging_model"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rouge = "^1.0.1"
-numpy = "~1.25.2"
 scikit-learn = "^1.4.1.post1"
 pymorphy2 = "^0.9.1"
 nltk = "^3.8.1"
 rake-nltk = "^1.0.6"
 coloredlogs = "^15.0.1"
 tqdm = "^4.66.2"
 fasttext-wheel = "^0.9.2"
 transformers = "^4.39.3"
 sentencepiece = "^0.2.0"
+sentence-transformers = "^2.6.1"
+numpy = "^1.24.4"
 
 
 [tool.poetry.group.dev.dependencies]
 pandas = "~2.0.3"
 pylint = "^2.17.4"
 flake8 = "^6.0.0"
 mypy = "^1.2.0"
```

### Comparing `text_tagging_model-0.1.2a9/text_tagging_model/logger_config.py` & `text_tagging_model-0.1.4a0/text_tagging_model/logger_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-
 # import sys
 from logging import Logger
 
 import coloredlogs
 
 
 class LoggerFactory:
```

### Comparing `text_tagging_model-0.1.2a9/text_tagging_model/models/bart_based_model/tag_sum_extractor.py` & `text_tagging_model-0.1.4a0/text_tagging_model/models/bart_based_model/tag_sum_extractor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-from collections import Counter
-from typing import List
-
 import numpy as np
-from tqdm import tqdm
 
+from text_tagging_model.models.base_extractor import BaseExtractor
 from text_tagging_model.processing.embedder.hg_embedder import HGEmbedder
 from text_tagging_model.processing.normalizers import NounsKeeper, PunctDeleter, StopwordsDeleter
 from text_tagging_model.processing.normalizers.pipe import NormalizersPipe
-from text_tagging_model.processing.ranker.max_distance_ranker import MaxDistanceRanker
+from text_tagging_model.processing.ranker.text_sim_ranker import TextSimRanker
 from text_tagging_model.processing.summarizator.bart_summarization import MBartSummarizator
 
 
-class TagSumExtractor:
+class TagSumExtractor(BaseExtractor):
     """
     The class is used to extract keywords from the text.
 
     Attributes
     ----------
     language : str
         language that will be used. available: 'russian', 'english'
@@ -30,56 +27,28 @@
     """
 
     def __init__(
         self,
         summarizator_model: str = "IlyaGusev/mbart_ru_sum_gazeta",
         embedder_model: str = "cointegrated/rubert-tiny2",
         language: str = "russian",
-        min_cnt_keyword: int = 2,
         device: str = "cpu",
     ) -> None:
         self.summarizator = MBartSummarizator(summarizator_model, device=device)
         self.normalizer = NormalizersPipe(
             [
                 PunctDeleter(),
                 StopwordsDeleter(language),
-                NounsKeeper(language),
+                NounsKeeper(language, keep_latn=True),
             ],
             final_split=True,
         )
 
         embedder = HGEmbedder(embedder_model)
-        self.ranker = MaxDistanceRanker(embedder)
-        self.min_cnt_keyword = min_cnt_keyword
-
-    def extract_for_corpus(
-        self,
-        texts: List[str],
-        top_n: int,
-    ) -> np.ndarray:
-        """Returns extracted keywords for corpus of texts
-
-        Args:
-            texts (List[str]): list with texts
-            top_n (int): number of words to extract
-            min_keyword_cnt (int): min number of words in the extracted phrases
-            distance_metric (str, optional): distance metric,
-            available ['cityblock', 'cosine', 'euclidean', 'l1', 'l2', 'manhattan'].
-            Defaults to "cosine".
-
-        Returns:
-            np.ndarray: array with arrays extracted keywords
-        """
-        extracted_keywords = list()
-
-        for text in tqdm(texts):
-            keywords = self.extract(text, top_n)
-            extracted_keywords.append(keywords)
-
-        return extracted_keywords
+        self.ranker = TextSimRanker(embedder)
 
     def extract(
         self,
         text: str,
         top_n: int,
     ) -> np.ndarray:
         """Returns extracted keywords from the text
@@ -94,16 +63,14 @@
 
         Returns:
             np.ndarray: array with extracted keywords
         """
 
         keyphrase = self.summarizator.get_summary(text.lower())
         normalized_keyphrase = self.normalizer.normalize(keyphrase)
-        most_co_occurring_words = [
-            word
-            for word, cnt in Counter(normalized_keyphrase).most_common(2 * top_n)
-            # if cnt >= self.min_cnt_keyword
-        ]
-
-        keywords = self.ranker.get_top_n_keywords(np.array(most_co_occurring_words), top_n)
+        keywords = self.ranker.get_top_n_keywords(
+            text=keyphrase,
+            words=np.unique(normalized_keyphrase),
+            top_n=top_n,
+        )
 
         return keywords
```

### Comparing `text_tagging_model-0.1.2a9/text_tagging_model/models/metrics.py` & `text_tagging_model-0.1.4a0/text_tagging_model/models/metrics.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a9/text_tagging_model/models/rake_based_model/keyphrases_extractor.py` & `text_tagging_model-0.1.4a0/text_tagging_model/models/rake_based_model/keyphrases_extractor.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a9/text_tagging_model/models/rake_based_model/tags_extractor.py` & `text_tagging_model-0.1.4a0/text_tagging_model/models/rake_based_model/tags_extractor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,21 @@
 from collections import Counter
 from itertools import chain
-from typing import List
 
 import numpy as np
-from tqdm import tqdm
 
+from text_tagging_model.models.base_extractor import BaseExtractor
 from text_tagging_model.models.rake_based_model.keyphrases_extractor import RakeKeyphrasesExtractor
 from text_tagging_model.processing.embedder.fasttext_embedder import FastTextEmbedder
 from text_tagging_model.processing.normalizers import NounsKeeper, PunctDeleter, StopwordsDeleter
 from text_tagging_model.processing.normalizers.pipe import NormalizersPipe
 from text_tagging_model.processing.ranker.max_distance_ranker import MaxDistanceRanker
 
 
-class TagsExtractor:
-    """
-    The class is used to extract keywords from the text.
-
-    Attributes
-    ----------
-    language : str
-        language that will be used. available: 'russian', 'english'
-    model_name : str
-        Name of model from fasttext (will be download if not exists)
-        or path to already downloaded .bin file with embeddings.
-
-    Methods
-    -------
-    extract(text, top_n, min_keyword_cnt, distance_metric)
-        Returns list with extracted keywords
-    """
-
+class TagsExtractor(BaseExtractor):
     def __init__(
         self,
         language: str = "russian",
         fasttext_model_path: str = "cc.ru.300.bin",
         min_cnt_keyword: int = 2,
     ) -> None:
         self.extractor = RakeKeyphrasesExtractor(language=language)
@@ -46,40 +28,14 @@
             final_split=True,
         )
 
         embedder = FastTextEmbedder(fasttext_model_path)
         self.ranker = MaxDistanceRanker(embedder)
         self.min_cnt_keyword = min_cnt_keyword
 
-    def extract_for_corpus(
-        self,
-        texts: List[str],
-        top_n: int,
-    ) -> np.ndarray:
-        """Returns extracted keywords for corpus of texts
-
-        Args:
-            texts (List[str]): list with texts
-            top_n (int): number of words to extract
-            min_keyword_cnt (int): min number of words in the extracted phrases
-            distance_metric (str, optional): distance metric,
-            available ['cityblock', 'cosine', 'euclidean', 'l1', 'l2', 'manhattan'].
-            Defaults to "cosine".
-
-        Returns:
-            np.ndarray: array with arrays extracted keywords
-        """
-        extracted_keywords = list()
-
-        for text in tqdm(texts):
-            keywords = self.extract(text, top_n)
-            extracted_keywords.append(keywords)
-
-        return extracted_keywords
-
     def extract(
         self,
         text: str,
         top_n: int,
     ) -> np.ndarray:
         """Returns extracted keywords from the text
 
@@ -105,10 +61,11 @@
             [
                 word
                 for word, cnt in Counter(normalized_words).most_common(top_n)
                 if cnt >= self.min_cnt_keyword
             ]
         )
 
-        keywords = self.ranker.get_top_n_keywords(most_co_occurring_words, top_n)
+        # keywords = most_co_occurring_words.tolist()
+        keywords = self.ranker.get_top_n_keywords(normalized_words, most_co_occurring_words, top_n)
 
         return keywords
```

### Comparing `text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/nouns_keeper.py` & `text_tagging_model-0.1.4a0/text_tagging_model/processing/normalizers/nouns_keeper.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/pipe.py` & `text_tagging_model-0.1.4a0/text_tagging_model/processing/normalizers/pipe.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/stopwords_deleter.py` & `text_tagging_model-0.1.4a0/text_tagging_model/processing/normalizers/stopwords_deleter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,31 @@
+import re
+
 import nltk
 from nltk.corpus import stopwords
 
 from text_tagging_model.processing.normalizers.base_normalizer import BaseNormalizer
 from text_tagging_model.processing.utils import languages
 
 
 class StopwordsDeleter(BaseNormalizer):
-    def __init__(self, language: str) -> None:
+    def __init__(self, language: str, drop_english=False, remove_non_alpha=True) -> None:
         if language not in languages:
             raise ValueError(f"Wrong language!\nAvailable languages: {languages.keys()}")
 
         nltk.download("stopwords")
         self.stop_words = set(stopwords.words(language))
 
+        if drop_english:
+            self.stop_words = self.stop_words.union(set(stopwords.words("english")))
+
+        self.remove_non_alpha = remove_non_alpha
+
     def normalize(self, text: str) -> str:
-        clear_text = []
-        for word in text.split():
-            if word.lower() not in self.stop_words and word != "":
-                clear_text.append(word)
+        if self.remove_non_alpha:
+            text = re.sub(r"[^a-zA-Zа-яА-Я\s]", " ", text)
+
+        words = text.split()
+
+        clear_text = [word for word in words if word.lower() not in self.stop_words and word != ""]
 
         return " ".join(clear_text)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `text_tagging_model-0.1.2a9/text_tagging_model/processing/ranker/base_ranker.py` & `text_tagging_model-0.1.4a0/text_tagging_model/processing/ranker/base_ranker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 from abc import ABC, abstractmethod
-from typing import List
+from typing import List, Union
 
 import numpy as np
 
 from text_tagging_model.processing.embedder.base_embedder import BaseEmbeddingModel
 
 
 class BaseRanker(ABC):
     def __init__(self, embedding_model: BaseEmbeddingModel):
         self.embedding_model = embedding_model
 
     def get_top_n_keywords(
         self,
+        text: Union[str, List[str]],
         words: np.ndarray[str],
         top_n: int,
     ) -> List[str]:
         embeddings = self.embedding_model(words)
-
         if len(embeddings) == 0:
             return []
 
-        top_n_indices = self.get_ranked_embedding(embeddings)
+        text_embedding = self.get_text_embedding(text)
+        top_n_indices = self.get_ranked_embedding(text_embedding, embeddings)
         top_n_keywords: List[str] = words[top_n_indices][:top_n].tolist()
 
         return top_n_keywords
 
+    def get_text_embedding(self, text: Union[str, List[str]]) -> np.ndarray:
+        return self.embedding_model.get_sentence_emb(" ".join(text))
+
     @abstractmethod
-    def get_ranked_embedding(self, embeddings: np.ndarray[np.ndarray[float]]) -> np.ndarray[int]:
-        """Ranking the embeddings."""
+    def get_ranked_embedding(
+        self,
+        text_embedding: np.ndarray,
+        embeddings: np.ndarray,
+    ) -> np.ndarray[int]:
+        """Ranking the embeddings. The method to be implemented by derived classes."""
```

### Comparing `text_tagging_model-0.1.2a9/text_tagging_model/processing/ranker/max_distance_ranker.py` & `text_tagging_model-0.1.4a0/text_tagging_model/processing/ranker/max_distance_ranker.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 class MaxDistanceRanker(BaseRanker):
     def __init__(self, embedding_model: BaseEmbeddingModel, distance_metric: str = "cosine"):
         super().__init__(embedding_model)
         self.distance_metric = distance_metric
 
     def get_ranked_embedding(
         self,
-        embeddings: np.ndarray[np.ndarray[float]],
+        text_embedding: np.ndarray,
+        embeddings: np.ndarray,
     ) -> np.ndarray[int]:
-        distances = pairwise_distances(
-            embeddings,
-            metric=self.distance_metric,
-        ).mean(axis=1)
+        distances = pairwise_distances(embeddings, metric=self.distance_metric).mean(axis=1)
         top_n_indices = (-distances).argsort()
-
         return top_n_indices
+
+    # def get_text_embedding(self, text: List[str]) -> np.ndarray:
+    #     # Переопределение не требуется, если ранжирование не зависит от текста.
+    #     return super().get_text_embedding(text)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `text_tagging_model-0.1.2a9/text_tagging_model/processing/summarizator/bart_summarization.py` & `text_tagging_model-0.1.4a0/text_tagging_model/processing/summarizator/bart_summarization.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         )["input_ids"]
 
         output_ids = self.model.generate(
             input_ids=input_ids.to(self.device),
             max_length=128,
             no_repeat_ngram_size=3,
             num_beams=10,
-            #             top_p=0.95
         )[0]
 
         if self.device == "cpu":
             output_ids.detach().cpu().numpy()
 
         summary: str = self.tokenizer.decode(output_ids, skip_special_tokens=True)
```

### Comparing `text_tagging_model-0.1.2a9/PKG-INFO` & `text_tagging_model-0.1.4a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: text-tagging-model
-Version: 0.1.2a9
+Version: 0.1.4a0
 Summary: Here we collected some online and offline models for text tagging.
 Author: Pavel Kochkin
 Author-email: kochkin27@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: fasttext-wheel (>=0.9.2,<0.10.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
-Requires-Dist: numpy (>=1.25.2,<1.26.0)
+Requires-Dist: numpy (>=1.24.4,<2.0.0)
 Requires-Dist: pymorphy2 (>=0.9.1,<0.10.0)
 Requires-Dist: rake-nltk (>=1.0.6,<2.0.0)
 Requires-Dist: rouge (>=1.0.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
+Requires-Dist: sentence-transformers (>=2.6.1,<3.0.0)
 Requires-Dist: sentencepiece (>=0.2.0,<0.3.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: transformers (>=4.39.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # text-tagging-model
 Text tagging model.
```

