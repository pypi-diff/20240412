# Comparing `tmp/rerankers-0.1.2.post1.tar.gz` & `tmp/rerankers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rerankers-0.1.2.post1.tar", last modified: Mon Apr  8 10:02:06 2024, max compression
+gzip compressed data, was "rerankers-0.2.0.tar", last modified: Fri Apr 12 15:35:50 2024, max compression
```

## Comparing `rerankers-0.1.2.post1.tar` & `rerankers-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-08 10:02:06.963711 rerankers-0.1.2.post1/
--rw-r--r--   0 bclavie    (501) staff       (20)    11309 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/LICENSE
--rw-r--r--   0 bclavie    (501) staff       (20)    21389 2024-04-08 10:02:06.963495 rerankers-0.1.2.post1/PKG-INFO
--rw-r--r--   0 bclavie    (501) staff       (20)     6732 2024-03-20 13:21:15.000000 rerankers-0.1.2.post1/README.md
--rw-r--r--   0 bclavie    (501) staff       (20)     1557 2024-04-08 10:01:49.000000 rerankers-0.1.2.post1/pyproject.toml
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-08 10:02:06.958892 rerankers-0.1.2.post1/rerankers/
--rw-r--r--   0 bclavie    (501) staff       (20)       86 2024-03-20 13:21:15.000000 rerankers-0.1.2.post1/rerankers/__init__.py
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-08 10:02:06.959805 rerankers-0.1.2.post1/rerankers/integrations/
--rw-r--r--   0 bclavie    (501) staff       (20)        0 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/integrations/__init__.py
--rw-r--r--   0 bclavie    (501) staff       (20)     1153 2024-03-19 21:00:12.000000 rerankers-0.1.2.post1/rerankers/integrations/langchain.py
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-08 10:02:06.961740 rerankers-0.1.2.post1/rerankers/models/
--rw-r--r--   0 bclavie    (501) staff       (20)      766 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/models/__init__.py
--rw-r--r--   0 bclavie    (501) staff       (20)     2871 2024-03-20 13:21:15.000000 rerankers-0.1.2.post1/rerankers/models/api_rankers.py
--rw-r--r--   0 bclavie    (501) staff       (20)     8695 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/models/colbert_ranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     1111 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/models/ranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     5654 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/models/rankgpt_rankers.py
--rw-r--r--   0 bclavie    (501) staff       (20)       28 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/models/rankllm.py
--rw-r--r--   0 bclavie    (501) staff       (20)    10177 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/models/t5ranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     3185 2024-04-08 10:00:14.000000 rerankers-0.1.2.post1/rerankers/models/transformer_ranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     6470 2024-03-20 13:21:15.000000 rerankers-0.1.2.post1/rerankers/reranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     1478 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/results.py
--rw-r--r--   0 bclavie    (501) staff       (20)     2394 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/rerankers/utils.py
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-08 10:02:06.962400 rerankers-0.1.2.post1/rerankers.egg-info/
--rw-r--r--   0 bclavie    (501) staff       (20)    21389 2024-04-08 10:02:06.000000 rerankers-0.1.2.post1/rerankers.egg-info/PKG-INFO
--rw-r--r--   0 bclavie    (501) staff       (20)      651 2024-04-08 10:02:06.000000 rerankers-0.1.2.post1/rerankers.egg-info/SOURCES.txt
--rw-r--r--   0 bclavie    (501) staff       (20)        1 2024-04-08 10:02:06.000000 rerankers-0.1.2.post1/rerankers.egg-info/dependency_links.txt
--rw-r--r--   0 bclavie    (501) staff       (20)      237 2024-04-08 10:02:06.000000 rerankers-0.1.2.post1/rerankers.egg-info/requires.txt
--rw-r--r--   0 bclavie    (501) staff       (20)       10 2024-04-08 10:02:06.000000 rerankers-0.1.2.post1/rerankers.egg-info/top_level.txt
--rw-r--r--   0 bclavie    (501) staff       (20)       38 2024-04-08 10:02:06.963776 rerankers-0.1.2.post1/setup.cfg
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-08 10:02:06.962224 rerankers-0.1.2.post1/tests/
--rw-r--r--   0 bclavie    (501) staff       (20)     1225 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/tests/test_crossenc.py
--rw-r--r--   0 bclavie    (501) staff       (20)      943 2024-03-14 14:24:04.000000 rerankers-0.1.2.post1/tests/test_results.py
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-12 15:35:50.095461 rerankers-0.2.0/
+-rw-r--r--   0 bclavie    (501) staff       (20)    11309 2024-03-14 14:24:04.000000 rerankers-0.2.0/LICENSE
+-rw-r--r--   0 bclavie    (501) staff       (20)    21497 2024-04-12 15:35:50.095249 rerankers-0.2.0/PKG-INFO
+-rw-r--r--   0 bclavie    (501) staff       (20)     6732 2024-03-20 13:21:15.000000 rerankers-0.2.0/README.md
+-rw-r--r--   0 bclavie    (501) staff       (20)     1591 2024-04-12 15:35:29.000000 rerankers-0.2.0/pyproject.toml
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-12 15:35:50.090579 rerankers-0.2.0/rerankers/
+-rw-r--r--   0 bclavie    (501) staff       (20)       86 2024-04-12 15:35:36.000000 rerankers-0.2.0/rerankers/__init__.py
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-12 15:35:50.091372 rerankers-0.2.0/rerankers/integrations/
+-rw-r--r--   0 bclavie    (501) staff       (20)        0 2024-03-14 14:24:04.000000 rerankers-0.2.0/rerankers/integrations/__init__.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     1153 2024-03-19 21:00:12.000000 rerankers-0.2.0/rerankers/integrations/langchain.py
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-12 15:35:50.093300 rerankers-0.2.0/rerankers/models/
+-rw-r--r--   0 bclavie    (501) staff       (20)      927 2024-04-12 15:23:15.000000 rerankers-0.2.0/rerankers/models/__init__.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     3537 2024-04-12 15:23:15.000000 rerankers-0.2.0/rerankers/models/api_rankers.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     8695 2024-03-14 14:24:04.000000 rerankers-0.2.0/rerankers/models/colbert_ranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     2052 2024-04-12 15:23:15.000000 rerankers-0.2.0/rerankers/models/flashrank_ranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     1466 2024-04-12 15:35:13.000000 rerankers-0.2.0/rerankers/models/ranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     5654 2024-03-14 14:24:04.000000 rerankers-0.2.0/rerankers/models/rankgpt_rankers.py
+-rw-r--r--   0 bclavie    (501) staff       (20)       28 2024-03-14 14:24:04.000000 rerankers-0.2.0/rerankers/models/rankllm.py
+-rw-r--r--   0 bclavie    (501) staff       (20)    10177 2024-03-14 14:24:04.000000 rerankers-0.2.0/rerankers/models/t5ranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     3185 2024-04-12 14:38:14.000000 rerankers-0.2.0/rerankers/models/transformer_ranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     6921 2024-04-12 15:23:15.000000 rerankers-0.2.0/rerankers/reranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     1478 2024-03-14 14:24:04.000000 rerankers-0.2.0/rerankers/results.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     2394 2024-03-14 14:24:04.000000 rerankers-0.2.0/rerankers/utils.py
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-12 15:35:50.094049 rerankers-0.2.0/rerankers.egg-info/
+-rw-r--r--   0 bclavie    (501) staff       (20)    21497 2024-04-12 15:35:50.000000 rerankers-0.2.0/rerankers.egg-info/PKG-INFO
+-rw-r--r--   0 bclavie    (501) staff       (20)      688 2024-04-12 15:35:50.000000 rerankers-0.2.0/rerankers.egg-info/SOURCES.txt
+-rw-r--r--   0 bclavie    (501) staff       (20)        1 2024-04-12 15:35:50.000000 rerankers-0.2.0/rerankers.egg-info/dependency_links.txt
+-rw-r--r--   0 bclavie    (501) staff       (20)      270 2024-04-12 15:35:50.000000 rerankers-0.2.0/rerankers.egg-info/requires.txt
+-rw-r--r--   0 bclavie    (501) staff       (20)       10 2024-04-12 15:35:50.000000 rerankers-0.2.0/rerankers.egg-info/top_level.txt
+-rw-r--r--   0 bclavie    (501) staff       (20)       38 2024-04-12 15:35:50.095663 rerankers-0.2.0/setup.cfg
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-12 15:35:50.093880 rerankers-0.2.0/tests/
+-rw-r--r--   0 bclavie    (501) staff       (20)     1225 2024-03-14 14:24:04.000000 rerankers-0.2.0/tests/test_crossenc.py
+-rw-r--r--   0 bclavie    (501) staff       (20)      943 2024-03-14 14:24:04.000000 rerankers-0.2.0/tests/test_results.py
```

### Comparing `rerankers-0.1.2.post1/LICENSE` & `rerankers-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2.post1/PKG-INFO` & `rerankers-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rerankers
-Version: 0.1.2.post1
+Version: 0.2.0
 Summary: A unified API for various document re-ranking models.
 Author-email: Ben Clavié <bc@answer.ai>
 Maintainer-email: Ben Clavié <bc@answer.ai>
 License:  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -222,23 +222,26 @@
 Provides-Extra: all
 Requires-Dist: transformers; extra == "all"
 Requires-Dist: torch; extra == "all"
 Requires-Dist: litellm; extra == "all"
 Requires-Dist: requests; extra == "all"
 Requires-Dist: sentencepiece; extra == "all"
 Requires-Dist: protobuf; extra == "all"
+Requires-Dist: flashrank; extra == "all"
 Provides-Extra: transformers
 Requires-Dist: transformers; extra == "transformers"
 Requires-Dist: torch; extra == "transformers"
 Requires-Dist: sentencepiece; extra == "transformers"
 Requires-Dist: protobuf; extra == "transformers"
 Provides-Extra: api
 Requires-Dist: requests; extra == "api"
 Provides-Extra: gpt
 Requires-Dist: litellm; extra == "gpt"
+Provides-Extra: flashrank
+Requires-Dist: flashrank; extra == "flashrank"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ipyprogress; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: ranx; extra == "dev"
```

### Comparing `rerankers-0.1.2.post1/README.md` & `rerankers-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2.post1/pyproject.toml` & `rerankers-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "rerankers.integrations",
 ]
 
 [project]
 name = "rerankers" 
 
 
-version = "0.1.2post1"
+version = "0.2.0"
 
 description = "A unified API for various document re-ranking models."
 
 readme = "README.md"
 
 requires-python = ">=3.8"
 
@@ -48,15 +48,16 @@
 
 dependencies = [
   "pydantic",
   "tqdm",
 ]
 
 [project.optional-dependencies]
-all = ["transformers", "torch", "litellm", "requests", "sentencepiece", "protobuf"]
+all = ["transformers", "torch", "litellm", "requests", "sentencepiece", "protobuf", "flashrank"]
 transformers = ["transformers", "torch", "sentencepiece", "protobuf"]
 api = ["requests"]
 gpt = ["litellm"]
+flashrank = ["flashrank"]
 dev = ["ruff", "isort", "pytest", "ipyprogress", "ipython", "ranx", "ir_datasets", "srsly"]
 
 [project.urls]
 "Homepage" = "https://github.com/bclavie/rerankers"
```

### Comparing `rerankers-0.1.2.post1/rerankers/integrations/langchain.py` & `rerankers-0.2.0/rerankers/integrations/langchain.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2.post1/rerankers/models/__init__.py` & `rerankers-0.2.0/rerankers/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,7 +27,14 @@
 
 try:
     from rerankers.models.colbert_ranker import ColBERTRanker
 
     AVAILABLE_RANKERS["ColBERTRanker"] = ColBERTRanker
 except ImportError:
     pass
+
+try:
+    from rerankers.models.flashrank_ranker import FlashRankRanker
+
+    AVAILABLE_RANKERS["FlashRankRanker"] = FlashRankRanker
+except ImportError:
+    pass
```

### Comparing `rerankers-0.1.2.post1/rerankers/models/api_rankers.py` & `rerankers-0.2.0/rerankers/models/api_rankers.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import json
 
 
 URLS = {
     "cohere": "https://api.cohere.ai/v1/rerank",
     "jina": "https://api.jina.ai/v1/rerank",
     "voyage": "https://api.voyageai.com/v1/rerank",
-    "mixedbread": NotImplemented,
+    "mixedbread.ai": "https://api.mixedbread.ai/v1/reranking",
 }
 
 
 class APIRanker(BaseRanker):
     def __init__(self, model: str, api_key: str, api_provider: str, verbose: int = 1):
         self.api_key = api_key
         self.model = model
@@ -25,32 +25,44 @@
         self.headers = {
             "accept": "application/json",
             "content-type": "application/json",
             "Authorization": f"Bearer {self.api_key}",
         }
         self.url = URLS[self.api_provider]
 
+    def _get_document_text(self, r: dict) -> str:
+        if self.api_provider == "voyage":
+            return r["document"]
+        elif self.api_provider == "mixedbread.ai":
+            return r["input"]
+        else:
+            return r["document"]["text"]
+
+    def _get_score(self, r: dict) -> float:
+        if self.api_provider == "mixedbread.ai":
+            return r["score"]
+        return r["relevance_score"]
+
     def _parse_response(
         self, response: dict, doc_ids: Union[List[str], List[int]]
     ) -> RankedResults:
         ranked_docs = []
-        results_key = "results" if self.api_provider != "voyage" else "data"
+        results_key = (
+            "results"
+            if self.api_provider not in ["voyage", "mixedbread.ai"]
+            else "data"
+        )
         print(response)
 
         for i, r in enumerate(response[results_key]):
-            document_text = (
-                r["document"]
-                if self.api_provider == "voyage"
-                else r["document"]["text"]
-            )
             ranked_docs.append(
                 Result(
                     doc_id=doc_ids[r["index"]],
-                    text=document_text,
-                    score=r["relevance_score"],
+                    text=self._get_document_text(r),
+                    score=self._get_score(r),
                     rank=i + 1,
                 )
             )
 
         return ranked_docs
 
     def rank(
@@ -63,21 +75,30 @@
         doc_ids = ensure_docids(doc_ids, len(docs))
         payload = self._format_payload(query, docs)
         response = requests.post(self.url, headers=self.headers, data=payload)
         results = self._parse_response(response.json(), doc_ids)
         return RankedResults(results=results, query=query, has_scores=True)
 
     def _format_payload(self, query: str, docs: List[str]) -> str:
-        top_key = "top_n" if self.api_provider != "voyage" else "top_k"
+        top_key = (
+            "top_n" if self.api_provider not in ["voyage", "mixedbread.ai"] else "top_k"
+        )
+        documents_key = "documents" if self.api_provider != "mixedbread.ai" else "input"
+        return_documents_key = (
+            "return_documents"
+            if self.api_provider != "mixedbread.ai"
+            else "return_input"
+        )
+
         payload = {
             "model": self.model,
             "query": query,
-            "documents": docs,
+            documents_key: docs,
             top_key: len(docs),
-            "return_documents": True,
+            return_documents_key: True,
         }
         return json.dumps(payload)
 
     def score(self, query: str, doc: str) -> float:
         payload = self._format_payload(query, [doc])
         response = requests.post(self.url, headers=self.headers, data=payload)
         results = self._parse_response(response.json(), [doc])
```

### Comparing `rerankers-0.1.2.post1/rerankers/models/colbert_ranker.py` & `rerankers-0.2.0/rerankers/models/colbert_ranker.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2.post1/rerankers/models/rankgpt_rankers.py` & `rerankers-0.2.0/rerankers/models/rankgpt_rankers.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2.post1/rerankers/models/t5ranker.py` & `rerankers-0.2.0/rerankers/models/t5ranker.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2.post1/rerankers/models/transformer_ranker.py` & `rerankers-0.2.0/rerankers/models/transformer_ranker.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2.post1/rerankers/reranker.py` & `rerankers-0.2.0/rerankers/reranker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Optional
 from rerankers.models import AVAILABLE_RANKERS
 from rerankers.models.ranker import BaseRanker
 from rerankers.utils import vprint
 
 DEFAULTS = {
     "jina": {"en": "jina-reranker-v1-base-en"},
-    "cohere": {"en": "rerank-english-v2.0", "other": "rerank-multilingual-v2.0"},
+    "cohere": {"en": "rerank-english-v3.0", "other": "rerank-multilingual-v3.0"},
     "voyage": {"en": "rerank-lite-1"},
+    "mixedbread.ai": {"en": "mixedbread-ai/mxbai-rerank-large-v1"},
     "cross-encoder": {
         "en": "mixedbread-ai/mxbai-rerank-base-v1",
         "fr": "antoinelouis/crossencoder-camembert-base-mmarcoFR",
         "zh": "BAAI/bge-reranker-base",
         "other": "corrius/cross-encoder-mmarco-mMiniLMv2-L12-H384-v1",
     },
     "t5": {"en": "unicamp-dl/InRanker-base", "other": "unicamp-dl/mt5-base-mmarco-v2"},
@@ -22,26 +23,28 @@
     "rankgpt4": {"en": "gpt-4", "other": "gpt-4"},
     "colbert": {
         "en": "colbert-ir/colbertv2.0",
         "fr": "bclavie/FraColBERTv2",
         "ja": "bclavie/JaColBERTv2",
         "es": "AdrienB134/ColBERTv2.0-spanish-mmarcoES",
     },
+    "flashrank": {"en": "ms-marco-MiniLM-L-12-v2", "other": "ms-marco-MultiBERT-L-12"},
 }
 
 DEPS_MAPPING = {
     "TransformerRanker": "transformers",
     "T5Ranker": "transformers",
     "LiT5Ranker": "lit5",
     "RankGPTRanker": "gpt",
     "APIRanker": "api",
     "ColBERTRanker": "transformers",
+    "FlashRankRanker": "flashrank",
 }
 
-PROVIDERS = ["cohere", "jina", "voyage"]
+PROVIDERS = ["cohere", "jina", "voyage", "mixedbread.ai"]
 
 
 def _get_api_provider(model_name: str, model_type: Optional[str] = None) -> str:
     if model_type in PROVIDERS or any(provider in model_name for provider in PROVIDERS):
         return model_type or next(
             (provider for provider in PROVIDERS if provider in model_name), None
         )
@@ -64,34 +67,41 @@
             "jina": "APIRanker",
             "voyage": "APIRanker",
             "rankgpt": "RankGPTRanker",
             "lit5": "LiT5Ranker",
             "t5": "T5Ranker",
             "colbert": "ColBERTRanker",
             "cross-encoder": "TransformerRanker",
+            "flashrank": "FlashRankRanker",
         }
         return model_mapping.get(explicit_model_type, explicit_model_type)
     else:
         model_name = model_name.lower()
         model_mapping = {
             "lit5": "LiT5Ranker",
             "t5": "T5Ranker",
             "inranker": "T5Ranker",
             "gpt": "RankGPTRanker",
             "zephyr": "RankZephyr",
             "colbert": "ColBERTRanker",
             "cohere": "APIRanker",
             "jina": "APIRanker",
             "voyage": "APIRanker",
+            "ms-marco-minilm-l-12-v2": "FlashRankRanker",
+            "ms-marco-multibert-l-12": "FlashRankRanker",
         }
         for key, value in model_mapping.items():
             if key in model_name:
                 return value
-        if any(
-            keyword in model_name for keyword in ["minilm", "bert", "cross-encoders/"]
+        if (
+            any(
+                keyword in model_name
+                for keyword in ["minilm", "bert", "cross-encoders/"]
+            )
+            and "/" in model_name
         ):
             return "TransformerRanker"
         print(
             "Warning: Model type could not be auto-mapped with the defaults list. Defaulting to TransformerRanker."
         )
         print(
             "If your model is NOT intended to be ran as a one-label cross-encoder, please reload it and specify the model_type!",
```

### Comparing `rerankers-0.1.2.post1/rerankers/results.py` & `rerankers-0.2.0/rerankers/results.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2.post1/rerankers/utils.py` & `rerankers-0.2.0/rerankers/utils.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2.post1/rerankers.egg-info/PKG-INFO` & `rerankers-0.2.0/rerankers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rerankers
-Version: 0.1.2.post1
+Version: 0.2.0
 Summary: A unified API for various document re-ranking models.
 Author-email: Ben Clavié <bc@answer.ai>
 Maintainer-email: Ben Clavié <bc@answer.ai>
 License:  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -222,23 +222,26 @@
 Provides-Extra: all
 Requires-Dist: transformers; extra == "all"
 Requires-Dist: torch; extra == "all"
 Requires-Dist: litellm; extra == "all"
 Requires-Dist: requests; extra == "all"
 Requires-Dist: sentencepiece; extra == "all"
 Requires-Dist: protobuf; extra == "all"
+Requires-Dist: flashrank; extra == "all"
 Provides-Extra: transformers
 Requires-Dist: transformers; extra == "transformers"
 Requires-Dist: torch; extra == "transformers"
 Requires-Dist: sentencepiece; extra == "transformers"
 Requires-Dist: protobuf; extra == "transformers"
 Provides-Extra: api
 Requires-Dist: requests; extra == "api"
 Provides-Extra: gpt
 Requires-Dist: litellm; extra == "gpt"
+Provides-Extra: flashrank
+Requires-Dist: flashrank; extra == "flashrank"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ipyprogress; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: ranx; extra == "dev"
```

### Comparing `rerankers-0.1.2.post1/rerankers.egg-info/SOURCES.txt` & `rerankers-0.2.0/rerankers.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 rerankers.egg-info/requires.txt
 rerankers.egg-info/top_level.txt
 rerankers/integrations/__init__.py
 rerankers/integrations/langchain.py
 rerankers/models/__init__.py
 rerankers/models/api_rankers.py
 rerankers/models/colbert_ranker.py
+rerankers/models/flashrank_ranker.py
 rerankers/models/ranker.py
 rerankers/models/rankgpt_rankers.py
 rerankers/models/rankllm.py
 rerankers/models/t5ranker.py
 rerankers/models/transformer_ranker.py
 tests/test_crossenc.py
 tests/test_results.py
```

### Comparing `rerankers-0.1.2.post1/tests/test_crossenc.py` & `rerankers-0.2.0/tests/test_crossenc.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.1.2.post1/tests/test_results.py` & `rerankers-0.2.0/tests/test_results.py`

 * *Files identical despite different names*

