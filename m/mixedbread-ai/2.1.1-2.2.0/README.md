# Comparing `tmp/mixedbread_ai-2.1.1.tar.gz` & `tmp/mixedbread_ai-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixedbread_ai-2.1.1.tar", max compression
+gzip compressed data, was "mixedbread_ai-2.2.0.tar", max compression
```

## Comparing `mixedbread_ai-2.1.1.tar` & `mixedbread_ai-2.2.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    11348 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/LICENSE.md
--rw-r--r--   0        0        0     4368 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/README.md
--rw-r--r--   0        0        0     2049 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/__init__.py
--rw-r--r--   0        0        0    24258 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/client.py
--rw-r--r--   0        0        0      790 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/api_error.py
--rw-r--r--   0        0        0     1081 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/file.py
--rw-r--r--   0        0        0     4882 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/core/request_options.py
--rw-r--r--   0        0        0      163 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/environment.py
--rw-r--r--   0        0        0      620 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/__init__.py
--rw-r--r--   0        0        0      305 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/bad_request_error.py
--rw-r--r--   0        0        0      300 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/forbidden_error.py
--rw-r--r--   0        0        0      289 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/internal_server_error.py
--rw-r--r--   0        0        0      297 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/not_found_error.py
--rw-r--r--   0        0        0      326 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      312 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/unauthorized_error.py
--rw-r--r--   0        0        0      300 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     2445 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/__init__.py
--rw-r--r--   0        0        0     1163 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/bad_request_error_body.py
--rw-r--r--   0        0        0      268 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/data.py
--rw-r--r--   0        0        0     1202 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/embedding.py
--rw-r--r--   0        0        0      152 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/embedding_item.py
--rw-r--r--   0        0        0      217 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/embeddings_request_encoding_format.py
--rw-r--r--   0        0        0     1613 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/embeddings_response.py
--rw-r--r--   0        0        0      218 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/embeddings_response_encoding_format.py
--rw-r--r--   0        0        0     1052 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/encoding_format.py
--rw-r--r--   0        0        0     1160 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/forbidden_error_body.py
--rw-r--r--   0        0        0      187 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/input.py
--rw-r--r--   0        0        0     1152 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/internal_error.py
--rw-r--r--   0        0        0     1194 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/invalid_matryoshka_dimensions_error.py
--rw-r--r--   0        0        0     1184 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/invalid_matryoshka_model_error.py
--rw-r--r--   0        0        0     1166 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/model_not_found_error.py
--rw-r--r--   0        0        0      216 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/multi_modal_input.py
--rw-r--r--   0        0        0     1411 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/multiple_encodings_embedding.py
--rw-r--r--   0        0        0     1465 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/multiple_encodings_embedding_item.py
--rw-r--r--   0        0        0     1125 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/mxbai_api_error.py
--rw-r--r--   0        0        0      171 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/mxbai_api_error_details.py
--rw-r--r--   0        0        0     1159 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/not_found_error_body.py
--rw-r--r--   0        0        0      837 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/object_type.py
--rw-r--r--   0        0        0      161 2024-04-05 14:40:30.875906 mixedbread_ai-2.1.1/mixedbread_ai/types/query.py
--rw-r--r--   0        0        0     1223 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/ranked_document.py
--rw-r--r--   0        0        0     1558 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/reranking_response.py
--rw-r--r--   0        0        0      970 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/text_document.py
--rw-r--r--   0        0        0     1174 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/too_many_requests_error_body.py
--rw-r--r--   0        0        0      689 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/truncation_strategy.py
--rw-r--r--   0        0        0     1166 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/unauthorized_error_body.py
--rw-r--r--   0        0        0     1134 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/usage.py
--rw-r--r--   0        0        0      141 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/validation_error.py
--rw-r--r--   0        0        0     1161 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/mixedbread_ai/types/web_truncation_error.py
--rw-r--r--   0        0        0      544 2024-04-05 14:40:30.879906 mixedbread_ai-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     5369 1970-01-01 00:00:00.000000 mixedbread_ai-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11348 2024-04-11 22:00:20.610632 mixedbread_ai-2.2.0/LICENSE.md
+-rw-r--r--   0        0        0     4368 2024-04-11 22:00:20.610632 mixedbread_ai-2.2.0/README.md
+-rw-r--r--   0        0        0     2087 2024-04-11 22:00:20.610632 mixedbread_ai-2.2.0/mixedbread_ai/__init__.py
+-rw-r--r--   0        0        0    24755 2024-04-11 22:00:20.610632 mixedbread_ai-2.2.0/mixedbread_ai/client.py
+-rw-r--r--   0        0        0      790 2024-04-11 22:00:20.610632 mixedbread_ai-2.2.0/mixedbread_ai/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-11 22:00:20.610632 mixedbread_ai-2.2.0/mixedbread_ai/core/api_error.py
+-rw-r--r--   0        0        0     1081 2024-04-11 22:00:20.610632 mixedbread_ai-2.2.0/mixedbread_ai/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/core/file.py
+-rw-r--r--   0        0        0     4882 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/core/request_options.py
+-rw-r--r--   0        0        0      163 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/environment.py
+-rw-r--r--   0        0        0      620 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/errors/__init__.py
+-rw-r--r--   0        0        0      305 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/errors/bad_request_error.py
+-rw-r--r--   0        0        0      300 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/errors/forbidden_error.py
+-rw-r--r--   0        0        0      289 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/errors/internal_server_error.py
+-rw-r--r--   0        0        0      297 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/errors/not_found_error.py
+-rw-r--r--   0        0        0      326 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      312 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      300 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     2505 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/__init__.py
+-rw-r--r--   0        0        0     1163 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/bad_request_error_body.py
+-rw-r--r--   0        0        0      268 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/data.py
+-rw-r--r--   0        0        0     1202 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/embedding.py
+-rw-r--r--   0        0        0      152 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/embedding_item.py
+-rw-r--r--   0        0        0      217 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/embeddings_request_encoding_format.py
+-rw-r--r--   0        0        0     1613 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/embeddings_response.py
+-rw-r--r--   0        0        0      218 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/embeddings_response_encoding_format.py
+-rw-r--r--   0        0        0     1052 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/encoding_format.py
+-rw-r--r--   0        0        0     1160 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/forbidden_error_body.py
+-rw-r--r--   0        0        0     1152 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/internal_error.py
+-rw-r--r--   0        0        0     1194 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/invalid_matryoshka_dimensions_error.py
+-rw-r--r--   0        0        0     1184 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/invalid_matryoshka_model_error.py
+-rw-r--r--   0        0        0     1166 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/model_not_found_error.py
+-rw-r--r--   0        0        0      216 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/multi_modal_input.py
+-rw-r--r--   0        0        0      181 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/multi_modal_reranking_input.py
+-rw-r--r--   0        0        0     1411 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/multiple_encodings_embedding.py
+-rw-r--r--   0        0        0     1465 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/multiple_encodings_embedding_item.py
+-rw-r--r--   0        0        0     1125 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/mxbai_api_error.py
+-rw-r--r--   0        0        0      171 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/mxbai_api_error_details.py
+-rw-r--r--   0        0        0     1159 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/not_found_error_body.py
+-rw-r--r--   0        0        0      837 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/object_type.py
+-rw-r--r--   0        0        0      161 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/query.py
+-rw-r--r--   0        0        0     1223 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/ranked_document.py
+-rw-r--r--   0        0        0     1558 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/reranking_response.py
+-rw-r--r--   0        0        0      970 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/text_document.py
+-rw-r--r--   0        0        0     1174 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/too_many_requests_error_body.py
+-rw-r--r--   0        0        0      689 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/truncation_strategy.py
+-rw-r--r--   0        0        0     1166 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/unauthorized_error_body.py
+-rw-r--r--   0        0        0     1134 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/usage.py
+-rw-r--r--   0        0        0      141 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/validation_error.py
+-rw-r--r--   0        0        0     1161 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/mixedbread_ai/types/web_truncation_error.py
+-rw-r--r--   0        0        0      544 2024-04-11 22:00:20.614632 mixedbread_ai-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5369 1970-01-01 00:00:00.000000 mixedbread_ai-2.2.0/PKG-INFO
```

### Comparing `mixedbread_ai-2.1.1/LICENSE.md` & `mixedbread_ai-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/README.md` & `mixedbread_ai-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/__init__.py` & `mixedbread_ai-2.2.0/mixedbread_ai/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     Embedding,
     EmbeddingItem,
     EmbeddingsRequestEncodingFormat,
     EmbeddingsResponse,
     EmbeddingsResponseEncodingFormat,
     EncodingFormat,
     ForbiddenErrorBody,
-    Input,
     InternalError,
     InvalidMatryoshkaDimensionsError,
     InvalidMatryoshkaModelError,
     ModelNotFoundError,
     MultiModalInput,
+    MultiModalRerankingInput,
     MultipleEncodingsEmbedding,
     MultipleEncodingsEmbeddingItem,
     MxbaiApiError,
     MxbaiApiErrorDetails,
     NotFoundErrorBody,
     ObjectType,
     Query,
@@ -52,22 +52,22 @@
     "EmbeddingItem",
     "EmbeddingsRequestEncodingFormat",
     "EmbeddingsResponse",
     "EmbeddingsResponseEncodingFormat",
     "EncodingFormat",
     "ForbiddenError",
     "ForbiddenErrorBody",
-    "Input",
     "InternalError",
     "InternalServerError",
     "InvalidMatryoshkaDimensionsError",
     "InvalidMatryoshkaModelError",
     "MixedbreadAIEnvironment",
     "ModelNotFoundError",
     "MultiModalInput",
+    "MultiModalRerankingInput",
     "MultipleEncodingsEmbedding",
     "MultipleEncodingsEmbeddingItem",
     "MxbaiApiError",
     "MxbaiApiErrorDetails",
     "NotFoundError",
     "NotFoundErrorBody",
     "ObjectType",
```

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/client.py` & `mixedbread_ai-2.2.0/mixedbread_ai/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 from .errors.too_many_requests_error import TooManyRequestsError
 from .errors.unauthorized_error import UnauthorizedError
 from .errors.unprocessable_entity_error import UnprocessableEntityError
 from .types.bad_request_error_body import BadRequestErrorBody
 from .types.embeddings_request_encoding_format import EmbeddingsRequestEncodingFormat
 from .types.embeddings_response import EmbeddingsResponse
 from .types.forbidden_error_body import ForbiddenErrorBody
-from .types.input import Input
 from .types.internal_error import InternalError
 from .types.multi_modal_input import MultiModalInput
+from .types.multi_modal_reranking_input import MultiModalRerankingInput
 from .types.not_found_error_body import NotFoundErrorBody
 from .types.query import Query
 from .types.reranking_response import RerankingResponse
 from .types.too_many_requests_error_body import TooManyRequestsErrorBody
 from .types.truncation_strategy import TruncationStrategy
 from .types.unauthorized_error_body import UnauthorizedErrorBody
 from .types.validation_error import ValidationError
@@ -188,41 +188,46 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def reranking(
         self,
         *,
         model: str,
-        input: Input,
         query: Query,
+        input: MultiModalRerankingInput,
+        rank_fields: typing.Optional[typing.Sequence[str]] = OMIT,
         top_k: typing.Optional[int] = OMIT,
         return_input: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> RerankingResponse:
         """
         Parameters:
-            - model: str. The model to use for creating embeddings
-
-            - input: Input. The input documents to rerank
+            - model: str. The model to use for reranking documents
 
             - query: Query. The query to rerank the documents
 
+            - input: MultiModalRerankingInput.
+
+            - rank_fields: typing.Optional[typing.Sequence[str]].
+
             - top_k: typing.Optional[int]. The number of documents to return
 
             - return_input: typing.Optional[bool]. Whether to return the documents
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from mixedbread-ai import TextDocument
         from mixedbread-ai.client import MixedbreadAI
 
         client = MixedbreadAI(api_key="YOUR_API_KEY", )
-        client.reranking(model="model", input=["input"], query=TextDocument(text="text", ), top_k=10, return_input=False, )
+        client.reranking(model="model", query=TextDocument(text="text", ), input=["input"], top_k=10, return_input=False, )
         """
-        _request: typing.Dict[str, typing.Any] = {"model": model, "input": input, "query": query}
+        _request: typing.Dict[str, typing.Any] = {"model": model, "query": query, "input": input}
+        if rank_fields is not OMIT:
+            _request["rank_fields"] = rank_fields
         if top_k is not OMIT:
             _request["top_k"] = top_k
         if return_input is not OMIT:
             _request["return_input"] = return_input
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/reranking"),
@@ -419,41 +424,46 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def reranking(
         self,
         *,
         model: str,
-        input: Input,
         query: Query,
+        input: MultiModalRerankingInput,
+        rank_fields: typing.Optional[typing.Sequence[str]] = OMIT,
         top_k: typing.Optional[int] = OMIT,
         return_input: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> RerankingResponse:
         """
         Parameters:
-            - model: str. The model to use for creating embeddings
-
-            - input: Input. The input documents to rerank
+            - model: str. The model to use for reranking documents
 
             - query: Query. The query to rerank the documents
 
+            - input: MultiModalRerankingInput.
+
+            - rank_fields: typing.Optional[typing.Sequence[str]].
+
             - top_k: typing.Optional[int]. The number of documents to return
 
             - return_input: typing.Optional[bool]. Whether to return the documents
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from mixedbread-ai import TextDocument
         from mixedbread-ai.client import AsyncMixedbreadAI
 
         client = AsyncMixedbreadAI(api_key="YOUR_API_KEY", )
-        await client.reranking(model="model", input=["input"], query=TextDocument(text="text", ), top_k=10, return_input=False, )
+        await client.reranking(model="model", query=TextDocument(text="text", ), input=["input"], top_k=10, return_input=False, )
         """
-        _request: typing.Dict[str, typing.Any] = {"model": model, "input": input, "query": query}
+        _request: typing.Dict[str, typing.Any] = {"model": model, "query": query, "input": input}
+        if rank_fields is not OMIT:
+            _request["rank_fields"] = rank_fields
         if top_k is not OMIT:
             _request["top_k"] = top_k
         if return_input is not OMIT:
             _request["return_input"] = return_input
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/reranking"),
```

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/core/__init__.py` & `mixedbread_ai-2.2.0/mixedbread_ai/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/core/client_wrapper.py` & `mixedbread_ai-2.2.0/mixedbread_ai/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/core/datetime_utils.py` & `mixedbread_ai-2.2.0/mixedbread_ai/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/core/file.py` & `mixedbread_ai-2.2.0/mixedbread_ai/core/file.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/core/http_client.py` & `mixedbread_ai-2.2.0/mixedbread_ai/core/http_client.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/core/jsonable_encoder.py` & `mixedbread_ai-2.2.0/mixedbread_ai/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/core/request_options.py` & `mixedbread_ai-2.2.0/mixedbread_ai/core/request_options.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/errors/__init__.py` & `mixedbread_ai-2.2.0/mixedbread_ai/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/__init__.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from .embedding import Embedding
 from .embedding_item import EmbeddingItem
 from .embeddings_request_encoding_format import EmbeddingsRequestEncodingFormat
 from .embeddings_response import EmbeddingsResponse
 from .embeddings_response_encoding_format import EmbeddingsResponseEncodingFormat
 from .encoding_format import EncodingFormat
 from .forbidden_error_body import ForbiddenErrorBody
-from .input import Input
 from .internal_error import InternalError
 from .invalid_matryoshka_dimensions_error import InvalidMatryoshkaDimensionsError
 from .invalid_matryoshka_model_error import InvalidMatryoshkaModelError
 from .model_not_found_error import ModelNotFoundError
 from .multi_modal_input import MultiModalInput
+from .multi_modal_reranking_input import MultiModalRerankingInput
 from .multiple_encodings_embedding import MultipleEncodingsEmbedding
 from .multiple_encodings_embedding_item import MultipleEncodingsEmbeddingItem
 from .mxbai_api_error import MxbaiApiError
 from .mxbai_api_error_details import MxbaiApiErrorDetails
 from .not_found_error_body import NotFoundErrorBody
 from .object_type import ObjectType
 from .query import Query
@@ -38,20 +38,20 @@
     "Embedding",
     "EmbeddingItem",
     "EmbeddingsRequestEncodingFormat",
     "EmbeddingsResponse",
     "EmbeddingsResponseEncodingFormat",
     "EncodingFormat",
     "ForbiddenErrorBody",
-    "Input",
     "InternalError",
     "InvalidMatryoshkaDimensionsError",
     "InvalidMatryoshkaModelError",
     "ModelNotFoundError",
     "MultiModalInput",
+    "MultiModalRerankingInput",
     "MultipleEncodingsEmbedding",
     "MultipleEncodingsEmbeddingItem",
     "MxbaiApiError",
     "MxbaiApiErrorDetails",
     "NotFoundErrorBody",
     "ObjectType",
     "Query",
```

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/bad_request_error_body.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/bad_request_error_body.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/embedding.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/embedding.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/embeddings_response.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/embeddings_response.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/encoding_format.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/encoding_format.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/forbidden_error_body.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/forbidden_error_body.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/internal_error.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/internal_error.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/invalid_matryoshka_dimensions_error.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/invalid_matryoshka_dimensions_error.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/invalid_matryoshka_model_error.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/invalid_matryoshka_model_error.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/model_not_found_error.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/model_not_found_error.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/multiple_encodings_embedding.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/multiple_encodings_embedding.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/multiple_encodings_embedding_item.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/multiple_encodings_embedding_item.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/mxbai_api_error.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/mxbai_api_error.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/not_found_error_body.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/not_found_error_body.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/object_type.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/object_type.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/ranked_document.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/ranked_document.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/reranking_response.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/reranking_response.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/text_document.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/text_document.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/too_many_requests_error_body.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/too_many_requests_error_body.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/truncation_strategy.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/truncation_strategy.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/unauthorized_error_body.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/unauthorized_error_body.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/usage.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/usage.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/mixedbread_ai/types/web_truncation_error.py` & `mixedbread_ai-2.2.0/mixedbread_ai/types/web_truncation_error.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.1.1/pyproject.toml` & `mixedbread_ai-2.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mixedbread-ai"
-version = "2.1.1"
+version = "2.2.0"
 description = "mixedbread ai (https://www.mixedbread.ai)"
 authors = ["mixedbread.ai <support@mixedbread.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/mixedbread-ai/python-sdk.git"
 keywords = ["Embeddings", "NLP", "mixedbread.ai"]
 packages = [
```

### Comparing `mixedbread_ai-2.1.1/PKG-INFO` & `mixedbread_ai-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixedbread-ai
-Version: 2.1.1
+Version: 2.2.0
 Summary: mixedbread ai (https://www.mixedbread.ai)
 Home-page: https://github.com/mixedbread-ai/python-sdk.git
 License: Apache-2.0
 Keywords: Embeddings,NLP,mixedbread.ai
 Author: mixedbread.ai
 Author-email: support@mixedbread.ai
 Requires-Python: >=3.8,<4.0
```

