# Comparing `tmp/qdrant_haystack-3.2.1.tar.gz` & `tmp/qdrant_haystack-3.3.0.tar.gz`

## Comparing `qdrant_haystack-3.2.1.tar` & `qdrant_haystack-3.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/pydoc/config.yml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/src/haystack_integrations/components/retrievers/qdrant/__init__.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/src/haystack_integrations/components/retrievers/qdrant/retriever.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/src/haystack_integrations/document_stores/qdrant/__init__.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/src/haystack_integrations/document_stores/qdrant/converters.py
--rw-r--r--   0        0        0    18939 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/src/haystack_integrations/document_stores/qdrant/document_store.py
--rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/src/haystack_integrations/document_stores/qdrant/filters.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/tests/__init__.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/tests/test_converters.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/tests/test_dict_converters.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/tests/test_document_store.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/tests/test_filters.py
--rw-r--r--   0        0        0    20208 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/tests/test_legacy_filters.py
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/tests/test_retriever.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/LICENSE.txt
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/README.md
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/pydoc/config.yml
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/src/haystack_integrations/components/retrievers/qdrant/__init__.py
+-rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/src/haystack_integrations/components/retrievers/qdrant/retriever.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/src/haystack_integrations/document_stores/qdrant/__init__.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/src/haystack_integrations/document_stores/qdrant/converters.py
+-rw-r--r--   0        0        0    22800 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/src/haystack_integrations/document_stores/qdrant/document_store.py
+-rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/src/haystack_integrations/document_stores/qdrant/filters.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/tests/test_converters.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/tests/test_dict_converters.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/tests/test_filters.py
+-rw-r--r--   0        0        0    20208 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/tests/test_legacy_filters.py
+-rw-r--r--   0        0        0    11065 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/tests/test_retriever.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/README.md
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 qdrant_haystack-3.3.0/PKG-INFO
```

### Comparing `qdrant_haystack-3.2.1/pydoc/config.yml` & `qdrant_haystack-3.3.0/pydoc/config.yml`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.1/src/haystack_integrations/document_stores/qdrant/document_store.py` & `qdrant_haystack-3.3.0/src/haystack_integrations/document_stores/qdrant/document_store.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,25 +4,32 @@
 from typing import Any, ClassVar, Dict, Generator, List, Optional, Set, Union
 
 import numpy as np
 import qdrant_client
 from grpc import RpcError
 from haystack import default_from_dict, default_to_dict
 from haystack.dataclasses import Document
+from haystack.dataclasses.sparse_embedding import SparseEmbedding
 from haystack.document_stores.errors import DocumentStoreError, DuplicateDocumentError
 from haystack.document_stores.types import DuplicatePolicy
 from haystack.utils import Secret, deserialize_secrets_inplace
-from haystack.utils.filters import convert
+from haystack.utils.filters import convert as convert_legacy_filters
 from qdrant_client import grpc
 from qdrant_client.http import models as rest
 from qdrant_client.http.exceptions import UnexpectedResponse
 from tqdm import tqdm
 
-from .converters import HaystackToQdrant, QdrantToHaystack
-from .filters import QdrantFilterConverter
+from .converters import (
+    DENSE_VECTORS_NAME,
+    SPARSE_VECTORS_NAME,
+    convert_haystack_documents_to_qdrant_points,
+    convert_id,
+    convert_qdrant_point_to_haystack_document,
+)
+from .filters import convert_filters_to_qdrant
 
 logger = logging.getLogger(__name__)
 
 
 class QdrantStoreError(DocumentStoreError):
     pass
 
@@ -50,42 +57,43 @@
 
     def __init__(
         self,
         location: Optional[str] = None,
         url: Optional[str] = None,
         port: int = 6333,
         grpc_port: int = 6334,
-        prefer_grpc: bool = False,  # noqa: FBT001, FBT002
+        prefer_grpc: bool = False,
         https: Optional[bool] = None,
         api_key: Optional[Secret] = None,
         prefix: Optional[str] = None,
         timeout: Optional[float] = None,
         host: Optional[str] = None,
         path: Optional[str] = None,
         index: str = "Document",
         embedding_dim: int = 768,
-        on_disk: bool = False,  # noqa: FBT001, FBT002
+        on_disk: bool = False,
         content_field: str = "content",
         name_field: str = "name",
         embedding_field: str = "embedding",
+        use_sparse_embeddings: bool = False,
         similarity: str = "cosine",
-        return_embedding: bool = False,  # noqa: FBT001, FBT002
-        progress_bar: bool = True,  # noqa: FBT001, FBT002
+        return_embedding: bool = False,
+        progress_bar: bool = True,
         duplicate_documents: str = "overwrite",
-        recreate_index: bool = False,  # noqa: FBT001, FBT002
+        recreate_index: bool = False,
         shard_number: Optional[int] = None,
         replication_factor: Optional[int] = None,
         write_consistency_factor: Optional[int] = None,
         on_disk_payload: Optional[bool] = None,
         hnsw_config: Optional[dict] = None,
         optimizers_config: Optional[dict] = None,
         wal_config: Optional[dict] = None,
         quantization_config: Optional[dict] = None,
         init_from: Optional[dict] = None,
-        wait_result_from_api: bool = True,  # noqa: FBT001, FBT002
+        wait_result_from_api: bool = True,
         metadata: Optional[dict] = None,
         write_batch_size: int = 100,
         scroll_size: int = 10_000,
         payload_fields_to_index: Optional[List[dict]] = None,
     ):
         super().__init__()
 
@@ -129,35 +137,31 @@
         self.optimizers_config = optimizers_config
         self.wal_config = wal_config
         self.quantization_config = quantization_config
         self.init_from = init_from
         self.wait_result_from_api = wait_result_from_api
         self.recreate_index = recreate_index
         self.payload_fields_to_index = payload_fields_to_index
+        self.use_sparse_embeddings = use_sparse_embeddings
 
         # Make sure the collection is properly set up
-        self._set_up_collection(index, embedding_dim, recreate_index, similarity, on_disk, payload_fields_to_index)
+        self._set_up_collection(
+            index, embedding_dim, recreate_index, similarity, use_sparse_embeddings, on_disk, payload_fields_to_index
+        )
 
         self.embedding_dim = embedding_dim
         self.on_disk = on_disk
         self.content_field = content_field
         self.name_field = name_field
         self.embedding_field = embedding_field
         self.similarity = similarity
         self.index = index
         self.return_embedding = return_embedding
         self.progress_bar = progress_bar
         self.duplicate_documents = duplicate_documents
-        self.qdrant_filter_converter = QdrantFilterConverter()
-        self.haystack_to_qdrant_converter = HaystackToQdrant()
-        self.qdrant_to_haystack = QdrantToHaystack(
-            content_field,
-            name_field,
-            embedding_field,
-        )
         self.write_batch_size = write_batch_size
         self.scroll_size = scroll_size
 
     def count_documents(self) -> int:
         try:
             response = self.client.count(
                 collection_name=self.index,
@@ -174,15 +178,15 @@
         filters: Optional[Dict[str, Any]] = None,
     ) -> List[Document]:
         if filters and not isinstance(filters, dict):
             msg = "Filter must be a dictionary"
             raise ValueError(msg)
 
         if filters and "operator" not in filters:
-            filters = convert(filters)
+            filters = convert_legacy_filters(filters)
         return list(
             self.get_documents_generator(
                 filters,
             )
         )
 
     def write_documents(
@@ -190,45 +194,46 @@
         documents: List[Document],
         policy: DuplicatePolicy = DuplicatePolicy.FAIL,
     ):
         for doc in documents:
             if not isinstance(doc, Document):
                 msg = f"DocumentStore.write_documents() expects a list of Documents but got an element of {type(doc)}."
                 raise ValueError(msg)
-        self._set_up_collection(self.index, self.embedding_dim, False, self.similarity)
+        self._set_up_collection(self.index, self.embedding_dim, False, self.similarity, self.use_sparse_embeddings)
 
         if len(documents) == 0:
             logger.warning("Calling QdrantDocumentStore.write_documents() with empty list")
             return
 
         document_objects = self._handle_duplicate_documents(
             documents=documents,
             index=self.index,
             policy=policy,
         )
 
         batched_documents = get_batches_from_generator(document_objects, self.write_batch_size)
         with tqdm(total=len(document_objects), disable=not self.progress_bar) as progress_bar:
             for document_batch in batched_documents:
-                batch = self.haystack_to_qdrant_converter.documents_to_batch(
+                batch = convert_haystack_documents_to_qdrant_points(
                     document_batch,
                     embedding_field=self.embedding_field,
+                    use_sparse_embeddings=self.use_sparse_embeddings,
                 )
 
                 self.client.upsert(
                     collection_name=self.index,
                     points=batch,
                     wait=self.wait_result_from_api,
                 )
 
                 progress_bar.update(self.write_batch_size)
         return len(document_objects)
 
     def delete_documents(self, ids: List[str]):
-        ids = [self.haystack_to_qdrant_converter.convert_id(_id) for _id in ids]
+        ids = [convert_id(_id) for _id in ids]
         try:
             self.client.delete(
                 collection_name=self.index,
                 points_selector=ids,
                 wait=self.wait_result_from_api,
             )
         except KeyError:
@@ -253,15 +258,15 @@
         )
 
     def get_documents_generator(
         self,
         filters: Optional[Dict[str, Any]] = None,
     ) -> Generator[Document, None, None]:
         index = self.index
-        qdrant_filters = self.qdrant_filter_converter.convert(filters)
+        qdrant_filters = convert_filters_to_qdrant(filters)
 
         next_offset = None
         stop_scrolling = False
         while not stop_scrolling:
             records, next_offset = self.client.scroll(
                 collection_name=index,
                 scroll_filter=qdrant_filters,
@@ -271,56 +276,107 @@
                 with_vectors=True,
             )
             stop_scrolling = next_offset is None or (
                 isinstance(next_offset, grpc.PointId) and next_offset.num == 0 and next_offset.uuid == ""
             )
 
             for record in records:
-                yield self.qdrant_to_haystack.point_to_document(record)
+                yield convert_qdrant_point_to_haystack_document(
+                    record, use_sparse_embeddings=self.use_sparse_embeddings
+                )
 
     def get_documents_by_id(
         self,
         ids: List[str],
         index: Optional[str] = None,
     ) -> List[Document]:
         index = index or self.index
 
         documents: List[Document] = []
 
-        ids = [self.haystack_to_qdrant_converter.convert_id(_id) for _id in ids]
+        ids = [convert_id(_id) for _id in ids]
         records = self.client.retrieve(
             collection_name=index,
             ids=ids,
             with_payload=True,
             with_vectors=True,
         )
 
         for record in records:
-            documents.append(self.qdrant_to_haystack.point_to_document(record))
+            documents.append(
+                convert_qdrant_point_to_haystack_document(record, use_sparse_embeddings=self.use_sparse_embeddings)
+            )
         return documents
 
+    def query_by_sparse(
+        self,
+        query_sparse_embedding: SparseEmbedding,
+        filters: Optional[Dict[str, Any]] = None,
+        top_k: int = 10,
+        scale_score: bool = True,
+        return_embedding: bool = False,
+    ) -> List[Document]:
+        if not self.use_sparse_embeddings:
+            message = (
+                "You are trying to query using sparse embeddings, but the Document Store "
+                "was initialized with `use_sparse_embeddings=False`. "
+            )
+            raise QdrantStoreError(message)
+
+        qdrant_filters = convert_filters_to_qdrant(filters)
+        query_indices = query_sparse_embedding.indices
+        query_values = query_sparse_embedding.values
+        points = self.client.search(
+            collection_name=self.index,
+            query_vector=rest.NamedSparseVector(
+                name=SPARSE_VECTORS_NAME,
+                vector=rest.SparseVector(
+                    indices=query_indices,
+                    values=query_values,
+                ),
+            ),
+            query_filter=qdrant_filters,
+            limit=top_k,
+            with_vectors=return_embedding,
+        )
+        results = [
+            convert_qdrant_point_to_haystack_document(point, use_sparse_embeddings=self.use_sparse_embeddings)
+            for point in points
+        ]
+        if scale_score:
+            for document in results:
+                score = document.score
+                score = float(1 / (1 + np.exp(-score / 100)))
+                document.score = score
+        return results
+
     def query_by_embedding(
         self,
         query_embedding: List[float],
         filters: Optional[Dict[str, Any]] = None,
         top_k: int = 10,
-        scale_score: bool = True,  # noqa: FBT001, FBT002
-        return_embedding: bool = False,  # noqa: FBT001, FBT002
+        scale_score: bool = True,
+        return_embedding: bool = False,
     ) -> List[Document]:
-        qdrant_filters = self.qdrant_filter_converter.convert(filters)
+        qdrant_filters = convert_filters_to_qdrant(filters)
 
         points = self.client.search(
             collection_name=self.index,
-            query_vector=query_embedding,
+            query_vector=rest.NamedVector(
+                name=DENSE_VECTORS_NAME if self.use_sparse_embeddings else "",
+                vector=query_embedding,
+            ),
             query_filter=qdrant_filters,
             limit=top_k,
             with_vectors=return_embedding,
         )
-
-        results = [self.qdrant_to_haystack.point_to_document(point) for point in points]
+        results = [
+            convert_qdrant_point_to_haystack_document(point, use_sparse_embeddings=self.use_sparse_embeddings)
+            for point in points
+        ]
         if scale_score:
             for document in results:
                 score = document.score
                 if self.similarity == "cosine":
                     score = (score + 1) / 2
                 else:
                     score = float(1 / (1 + np.exp(-score / 100)))
@@ -351,25 +407,26 @@
                     field_schema=payload_index["field_schema"],
                 )
 
     def _set_up_collection(
         self,
         collection_name: str,
         embedding_dim: int,
-        recreate_collection: bool,  # noqa: FBT001
+        recreate_collection: bool,
         similarity: str,
-        on_disk: bool = False,  # noqa: FBT001, FBT002
+        use_sparse_embeddings: bool,
+        on_disk: bool = False,
         payload_fields_to_index: Optional[List[dict]] = None,
     ):
         distance = self._get_distance(similarity)
 
         if recreate_collection:
             # There is no need to verify the current configuration of that
             # collection. It might be just recreated again.
-            self._recreate_collection(collection_name, distance, embedding_dim, on_disk)
+            self._recreate_collection(collection_name, distance, embedding_dim, on_disk, use_sparse_embeddings)
             # Create Payload index if payload_fields_to_index is provided
             self._create_payload_index(collection_name, payload_fields_to_index)
             return
 
         try:
             # Check if the collection already exists and validate its
             # current configuration with the parameters.
@@ -377,21 +434,47 @@
         except (UnexpectedResponse, RpcError, ValueError):
             # That indicates the collection does not exist, so it can be
             # safely created with any configuration.
             #
             # Qdrant local raises ValueError if the collection is not found, but
             # with the remote server UnexpectedResponse / RpcError is raised.
             # Until that's unified, we need to catch both.
-            self._recreate_collection(collection_name, distance, embedding_dim, on_disk)
+            self._recreate_collection(collection_name, distance, embedding_dim, on_disk, use_sparse_embeddings)
             # Create Payload index if payload_fields_to_index is provided
             self._create_payload_index(collection_name, payload_fields_to_index)
             return
 
-        current_distance = collection_info.config.params.vectors.distance
-        current_vector_size = collection_info.config.params.vectors.size
+        has_named_vectors = (
+            isinstance(collection_info.config.params.vectors, dict)
+            and DENSE_VECTORS_NAME in collection_info.config.params.vectors
+        )
+
+        if self.use_sparse_embeddings and not has_named_vectors:
+            msg = (
+                f"Collection '{collection_name}' already exists in Qdrant, "
+                f"but it has been originally created without sparse embedding vectors. "
+                f"If you want to use that collection, you can set `use_sparse_embeddings=False`. "
+                f"To use sparse embeddings, you need to recreate the collection or migrate the existing one."
+            )
+            raise QdrantStoreError(msg)
+
+        elif not self.use_sparse_embeddings and has_named_vectors:
+            msg = (
+                f"Collection '{collection_name}' already exists in Qdrant, "
+                f"but it has been originally created with sparse embedding vectors."
+                f"If you want to use that collection, please set `use_sparse_embeddings=True`."
+            )
+            raise QdrantStoreError(msg)
+
+        if self.use_sparse_embeddings:
+            current_distance = collection_info.config.params.vectors[DENSE_VECTORS_NAME].distance
+            current_vector_size = collection_info.config.params.vectors[DENSE_VECTORS_NAME].size
+        else:
+            current_distance = collection_info.config.params.vectors.distance
+            current_vector_size = collection_info.config.params.vectors.size
 
         if current_distance != distance:
             msg = (
                 f"Collection '{collection_name}' already exists in Qdrant, "
                 f"but it is configured with a similarity '{current_distance.name}'. "
                 f"If you want to use that collection, but with a different "
                 f"similarity, please set `recreate_collection=True` argument."
@@ -403,22 +486,41 @@
                 f"Collection '{collection_name}' already exists in Qdrant, "
                 f"but it is configured with a vector size '{current_vector_size}'. "
                 f"If you want to use that collection, but with a different "
                 f"vector size, please set `recreate_collection=True` argument."
             )
             raise ValueError(msg)
 
-    def _recreate_collection(self, collection_name: str, distance, embedding_dim: int, on_disk: bool):  # noqa: FBT001
+    def _recreate_collection(
+        self,
+        collection_name: str,
+        distance,
+        embedding_dim: int,
+        on_disk: bool,
+        use_sparse_embeddings: bool,
+    ):
+        # dense vectors configuration
+        vectors_config = rest.VectorParams(size=embedding_dim, on_disk=on_disk, distance=distance)
+
+        if use_sparse_embeddings:
+            # in this case, we need to define named vectors
+            vectors_config = {DENSE_VECTORS_NAME: vectors_config}
+
+            sparse_vectors_config = {
+                SPARSE_VECTORS_NAME: rest.SparseVectorParams(
+                    index=rest.SparseIndexParams(
+                        on_disk=on_disk,
+                    )
+                ),
+            }
+
         self.client.recreate_collection(
             collection_name=collection_name,
-            vectors_config=rest.VectorParams(
-                size=embedding_dim,
-                on_disk=on_disk,
-                distance=distance,
-            ),
+            vectors_config=vectors_config,
+            sparse_vectors_config=sparse_vectors_config if use_sparse_embeddings else None,
             shard_number=self.shard_number,
             replication_factor=self.replication_factor,
             write_consistency_factor=self.write_consistency_factor,
             on_disk_payload=self.on_disk_payload,
             hnsw_config=self.hnsw_config,
             optimizers_config=self.optimizers_config,
             wal_config=self.wal_config,
```

### Comparing `qdrant_haystack-3.2.1/src/haystack_integrations/document_stores/qdrant/filters.py` & `qdrant_haystack-3.3.0/src/haystack_integrations/document_stores/qdrant/filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,233 +1,237 @@
 from datetime import datetime
 from typing import List, Optional, Union
 
 from haystack.utils.filters import COMPARISON_OPERATORS, LOGICAL_OPERATORS, FilterError
 from qdrant_client.http import models
 
-from .converters import HaystackToQdrant
+from .converters import convert_id
 
 COMPARISON_OPERATORS = COMPARISON_OPERATORS.keys()
 LOGICAL_OPERATORS = LOGICAL_OPERATORS.keys()
 
 
-class QdrantFilterConverter:
+def convert_filters_to_qdrant(
+    filter_term: Optional[Union[List[dict], dict]] = None,
+) -> Optional[models.Filter]:
     """Converts Haystack filters to the format used by Qdrant."""
 
-    def __init__(self):
-        self.haystack_to_qdrant_converter = HaystackToQdrant()
+    if not filter_term:
+        return None
 
-    def convert(
-        self,
-        filter_term: Optional[Union[List[dict], dict]] = None,
-    ) -> Optional[models.Filter]:
-        if not filter_term:
-            return None
-
-        must_clauses, should_clauses, must_not_clauses = [], [], []
-
-        if isinstance(filter_term, dict):
-            filter_term = [filter_term]
-
-        for item in filter_term:
-            operator = item.get("operator")
-            if operator is None:
-                msg = "Operator not found in filters"
-                raise FilterError(msg)
+    must_clauses, should_clauses, must_not_clauses = [], [], []
 
-            if operator in LOGICAL_OPERATORS and "conditions" not in item:
-                msg = f"'conditions' not found for '{operator}'"
-                raise FilterError(msg)
+    if isinstance(filter_term, dict):
+        filter_term = [filter_term]
 
-            if operator == "AND":
-                must_clauses.append(self.convert(item.get("conditions", [])))
-            elif operator == "OR":
-                should_clauses.append(self.convert(item.get("conditions", [])))
-            elif operator == "NOT":
-                must_not_clauses.append(self.convert(item.get("conditions", [])))
-            elif operator in COMPARISON_OPERATORS:
-                field = item.get("field")
-                value = item.get("value")
-                if field is None or value is None:
-                    msg = f"'field' or 'value' not found for '{operator}'"
-                    raise FilterError(msg)
-
-                must_clauses.extend(
-                    self._parse_comparison_operation(comparison_operation=operator, key=field, value=value)
-                )
-            else:
-                msg = f"Unknown operator {operator} used in filters"
-                raise FilterError(msg)
+    for item in filter_term:
+        operator = item.get("operator")
+        if operator is None:
+            msg = "Operator not found in filters"
+            raise FilterError(msg)
 
-        payload_filter = models.Filter(
-            must=must_clauses or None,
-            should=should_clauses or None,
-            must_not=must_not_clauses or None,
-        )
-
-        filter_result = self._squeeze_filter(payload_filter)
-
-        return filter_result
-
-    def _parse_comparison_operation(
-        self, comparison_operation: str, key: str, value: Union[dict, List, str, float]
-    ) -> List[models.Condition]:
-        conditions: List[models.Condition] = []
-
-        condition_builder_mapping = {
-            "==": self._build_eq_condition,
-            "in": self._build_in_condition,
-            "!=": self._build_ne_condition,
-            "not in": self._build_nin_condition,
-            ">": self._build_gt_condition,
-            ">=": self._build_gte_condition,
-            "<": self._build_lt_condition,
-            "<=": self._build_lte_condition,
-        }
-
-        condition_builder = condition_builder_mapping.get(comparison_operation)
-
-        if condition_builder is None:
-            msg = f"Unknown operator {comparison_operation} used in filters"
-            raise ValueError(msg)
-
-        conditions.append(condition_builder(key, value))
-
-        return conditions
-
-    def _build_eq_condition(self, key: str, value: models.ValueVariants) -> models.Condition:
-        if isinstance(value, str) and " " in value:
-            models.FieldCondition(key=key, match=models.MatchText(text=value))
-        return models.FieldCondition(key=key, match=models.MatchValue(value=value))
-
-    def _build_in_condition(self, key: str, value: List[models.ValueVariants]) -> models.Condition:
-        if not isinstance(value, list):
-            msg = f"Value {value} is not a list"
+        if operator in LOGICAL_OPERATORS and "conditions" not in item:
+            msg = f"'conditions' not found for '{operator}'"
             raise FilterError(msg)
-        return models.Filter(
-            should=[
-                (
-                    models.FieldCondition(key=key, match=models.MatchText(text=item))
-                    if isinstance(item, str) and " " not in item
-                    else models.FieldCondition(key=key, match=models.MatchValue(value=item))
-                )
-                for item in value
-            ]
-        )
-
-    def _build_ne_condition(self, key: str, value: models.ValueVariants) -> models.Condition:
-        return models.Filter(
-            must_not=[
-                (
-                    models.FieldCondition(key=key, match=models.MatchText(text=value))
-                    if isinstance(value, str) and " " not in value
-                    else models.FieldCondition(key=key, match=models.MatchValue(value=value))
-                )
-            ]
-        )
-
-    def _build_nin_condition(self, key: str, value: List[models.ValueVariants]) -> models.Condition:
-        if not isinstance(value, list):
-            msg = f"Value {value} is not a list"
+
+        if operator == "AND":
+            must_clauses.append(convert_filters_to_qdrant(item.get("conditions", [])))
+        elif operator == "OR":
+            should_clauses.append(convert_filters_to_qdrant(item.get("conditions", [])))
+        elif operator == "NOT":
+            must_not_clauses.append(convert_filters_to_qdrant(item.get("conditions", [])))
+        elif operator in COMPARISON_OPERATORS:
+            field = item.get("field")
+            value = item.get("value")
+            if field is None or value is None:
+                msg = f"'field' or 'value' not found for '{operator}'"
+                raise FilterError(msg)
+
+            must_clauses.extend(_parse_comparison_operation(comparison_operation=operator, key=field, value=value))
+        else:
+            msg = f"Unknown operator {operator} used in filters"
             raise FilterError(msg)
-        return models.Filter(
-            must_not=[
-                (
-                    models.FieldCondition(key=key, match=models.MatchText(text=item))
-                    if isinstance(item, str) and " " in item
-                    else models.FieldCondition(key=key, match=models.MatchValue(value=item))
-                )
-                for item in value
-            ]
-        )
-
-    def _build_lt_condition(self, key: str, value: Union[str, float, int]) -> models.Condition:
-        if isinstance(value, str) and is_datetime_string(value):
-            return models.FieldCondition(key=key, range=models.DatetimeRange(lt=value))
 
-        if isinstance(value, (int, float)):
-            return models.FieldCondition(key=key, range=models.Range(lt=value))
+    payload_filter = models.Filter(
+        must=must_clauses or None,
+        should=should_clauses or None,
+        must_not=must_not_clauses or None,
+    )
 
-        msg = f"Value {value} is not an int or float or datetime string"
-        raise FilterError(msg)
+    filter_result = _squeeze_filter(payload_filter)
 
-    def _build_lte_condition(self, key: str, value: Union[str, float, int]) -> models.Condition:
-        if isinstance(value, str) and is_datetime_string(value):
-            return models.FieldCondition(key=key, range=models.DatetimeRange(lte=value))
+    return filter_result
 
-        if isinstance(value, (int, float)):
-            return models.FieldCondition(key=key, range=models.Range(lte=value))
 
-        msg = f"Value {value} is not an int or float or datetime string"
-        raise FilterError(msg)
+def _parse_comparison_operation(
+    comparison_operation: str, key: str, value: Union[dict, List, str, float]
+) -> List[models.Condition]:
+    conditions: List[models.Condition] = []
 
-    def _build_gt_condition(self, key: str, value: Union[str, float, int]) -> models.Condition:
-        if isinstance(value, str) and is_datetime_string(value):
-            return models.FieldCondition(key=key, range=models.DatetimeRange(gt=value))
+    condition_builder_mapping = {
+        "==": _build_eq_condition,
+        "in": _build_in_condition,
+        "!=": _build_ne_condition,
+        "not in": _build_nin_condition,
+        ">": _build_gt_condition,
+        ">=": _build_gte_condition,
+        "<": _build_lt_condition,
+        "<=": _build_lte_condition,
+    }
 
-        if isinstance(value, (int, float)):
-            return models.FieldCondition(key=key, range=models.Range(gt=value))
+    condition_builder = condition_builder_mapping.get(comparison_operation)
 
-        msg = f"Value {value} is not an int or float or datetime string"
-        raise FilterError(msg)
+    if condition_builder is None:
+        msg = f"Unknown operator {comparison_operation} used in filters"
+        raise ValueError(msg)
+
+    conditions.append(condition_builder(key, value))
+
+    return conditions
 
-    def _build_gte_condition(self, key: str, value: Union[str, float, int]) -> models.Condition:
-        if isinstance(value, str) and is_datetime_string(value):
-            return models.FieldCondition(key=key, range=models.DatetimeRange(gte=value))
 
-        if isinstance(value, (int, float)):
-            return models.FieldCondition(key=key, range=models.Range(gte=value))
+def _build_eq_condition(key: str, value: models.ValueVariants) -> models.Condition:
+    if isinstance(value, str) and " " in value:
+        models.FieldCondition(key=key, match=models.MatchText(text=value))
+    return models.FieldCondition(key=key, match=models.MatchValue(value=value))
 
-        msg = f"Value {value} is not an int or float or datetime string"
+
+def _build_in_condition(key: str, value: List[models.ValueVariants]) -> models.Condition:
+    if not isinstance(value, list):
+        msg = f"Value {value} is not a list"
+        raise FilterError(msg)
+    return models.Filter(
+        should=[
+            (
+                models.FieldCondition(key=key, match=models.MatchText(text=item))
+                if isinstance(item, str) and " " not in item
+                else models.FieldCondition(key=key, match=models.MatchValue(value=item))
+            )
+            for item in value
+        ]
+    )
+
+
+def _build_ne_condition(key: str, value: models.ValueVariants) -> models.Condition:
+    return models.Filter(
+        must_not=[
+            (
+                models.FieldCondition(key=key, match=models.MatchText(text=value))
+                if isinstance(value, str) and " " not in value
+                else models.FieldCondition(key=key, match=models.MatchValue(value=value))
+            )
+        ]
+    )
+
+
+def _build_nin_condition(key: str, value: List[models.ValueVariants]) -> models.Condition:
+    if not isinstance(value, list):
+        msg = f"Value {value} is not a list"
         raise FilterError(msg)
+    return models.Filter(
+        must_not=[
+            (
+                models.FieldCondition(key=key, match=models.MatchText(text=item))
+                if isinstance(item, str) and " " in item
+                else models.FieldCondition(key=key, match=models.MatchValue(value=item))
+            )
+            for item in value
+        ]
+    )
+
+
+def _build_lt_condition(key: str, value: Union[str, float, int]) -> models.Condition:
+    if isinstance(value, str) and is_datetime_string(value):
+        return models.FieldCondition(key=key, range=models.DatetimeRange(lt=value))
+
+    if isinstance(value, (int, float)):
+        return models.FieldCondition(key=key, range=models.Range(lt=value))
+
+    msg = f"Value {value} is not an int or float or datetime string"
+    raise FilterError(msg)
 
-    def _build_has_id_condition(self, id_values: List[models.ExtendedPointId]) -> models.HasIdCondition:
-        return models.HasIdCondition(
-            has_id=[
-                # Ids are converted into their internal representation
-                self.haystack_to_qdrant_converter.convert_id(item)
-                for item in id_values
-            ]
-        )
-
-    def _squeeze_filter(self, payload_filter: models.Filter) -> models.Filter:
-        """
-        Simplify given payload filter, if the nested structure might be unnested.
-        That happens if there is a single clause in that filter.
-        :param payload_filter:
-        :returns:
-        """
-        filter_parts = {
-            "must": payload_filter.must,
-            "should": payload_filter.should,
-            "must_not": payload_filter.must_not,
-        }
-
-        total_clauses = sum(len(x) for x in filter_parts.values() if x is not None)
-        if total_clauses == 0 or total_clauses > 1:
-            return payload_filter
-
-        # Payload filter has just a single clause provided (either must, should
-        # or must_not). If that single clause is also of a models.Filter type,
-        # then it might be returned instead.
-        for part_name, filter_part in filter_parts.items():
-            if not filter_part:
-                continue
-
-            subfilter = filter_part[0]
-            if not isinstance(subfilter, models.Filter):
-                # The inner statement is a simple condition like models.FieldCondition
-                # so it cannot be simplified.
-                continue
 
-            if subfilter.must:
-                return models.Filter(**{part_name: subfilter.must})
+def _build_lte_condition(key: str, value: Union[str, float, int]) -> models.Condition:
+    if isinstance(value, str) and is_datetime_string(value):
+        return models.FieldCondition(key=key, range=models.DatetimeRange(lte=value))
 
+    if isinstance(value, (int, float)):
+        return models.FieldCondition(key=key, range=models.Range(lte=value))
+
+    msg = f"Value {value} is not an int or float or datetime string"
+    raise FilterError(msg)
+
+
+def _build_gt_condition(key: str, value: Union[str, float, int]) -> models.Condition:
+    if isinstance(value, str) and is_datetime_string(value):
+        return models.FieldCondition(key=key, range=models.DatetimeRange(gt=value))
+
+    if isinstance(value, (int, float)):
+        return models.FieldCondition(key=key, range=models.Range(gt=value))
+
+    msg = f"Value {value} is not an int or float or datetime string"
+    raise FilterError(msg)
+
+
+def _build_gte_condition(key: str, value: Union[str, float, int]) -> models.Condition:
+    if isinstance(value, str) and is_datetime_string(value):
+        return models.FieldCondition(key=key, range=models.DatetimeRange(gte=value))
+
+    if isinstance(value, (int, float)):
+        return models.FieldCondition(key=key, range=models.Range(gte=value))
+
+    msg = f"Value {value} is not an int or float or datetime string"
+    raise FilterError(msg)
+
+
+def _build_has_id_condition(id_values: List[models.ExtendedPointId]) -> models.HasIdCondition:
+    return models.HasIdCondition(
+        has_id=[
+            # Ids are converted into their internal representation
+            convert_id(item)
+            for item in id_values
+        ]
+    )
+
+
+def _squeeze_filter(payload_filter: models.Filter) -> models.Filter:
+    """
+    Simplify given payload filter, if the nested structure might be unnested.
+    That happens if there is a single clause in that filter.
+    :param payload_filter:
+    :returns:
+    """
+    filter_parts = {
+        "must": payload_filter.must,
+        "should": payload_filter.should,
+        "must_not": payload_filter.must_not,
+    }
+
+    total_clauses = sum(len(x) for x in filter_parts.values() if x is not None)
+    if total_clauses == 0 or total_clauses > 1:
         return payload_filter
 
+    # Payload filter has just a single clause provided (either must, should
+    # or must_not). If that single clause is also of a models.Filter type,
+    # then it might be returned instead.
+    for part_name, filter_part in filter_parts.items():
+        if not filter_part:
+            continue
+
+        subfilter = filter_part[0]
+        if not isinstance(subfilter, models.Filter):
+            # The inner statement is a simple condition like models.FieldCondition
+            # so it cannot be simplified.
+            continue
+
+        if subfilter.must:
+            return models.Filter(**{part_name: subfilter.must})
+
+    return payload_filter
+
 
 def is_datetime_string(value: str) -> bool:
     try:
         datetime.fromisoformat(value)
         return True
     except ValueError:
         return False
```

### Comparing `qdrant_haystack-3.2.1/tests/test_dict_converters.py` & `qdrant_haystack-3.3.0/tests/test_dict_converters.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
             "path": None,
             "index": "test",
             "embedding_dim": 768,
             "on_disk": False,
             "content_field": "content",
             "name_field": "name",
             "embedding_field": "embedding",
+            "use_sparse_embeddings": False,
             "similarity": "cosine",
             "return_embedding": False,
             "progress_bar": True,
             "duplicate_documents": "overwrite",
             "recreate_index": False,
             "shard_number": None,
             "replication_factor": None,
@@ -59,14 +60,15 @@
                 "location": ":memory:",
                 "index": "test",
                 "embedding_dim": 768,
                 "on_disk": False,
                 "content_field": "content",
                 "name_field": "name",
                 "embedding_field": "embedding",
+                "use_sparse_embeddings": True,
                 "similarity": "cosine",
                 "return_embedding": False,
                 "progress_bar": True,
                 "duplicate_documents": "overwrite",
                 "recreate_index": True,
                 "shard_number": None,
                 "quantization_config": None,
@@ -82,14 +84,15 @@
 
     assert all(
         [
             document_store.index == "test",
             document_store.content_field == "content",
             document_store.name_field == "name",
             document_store.embedding_field == "embedding",
+            document_store.use_sparse_embeddings is True,
             document_store.on_disk is False,
             document_store.similarity == "cosine",
             document_store.return_embedding is False,
             document_store.progress_bar,
             document_store.duplicate_documents == "overwrite",
             document_store.recreate_index is True,
             document_store.shard_number is None,
```

### Comparing `qdrant_haystack-3.2.1/tests/test_document_store.py` & `qdrant_haystack-3.3.0/tests/test_document_store.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.1/tests/test_filters.py` & `qdrant_haystack-3.3.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.1/tests/test_legacy_filters.py` & `qdrant_haystack-3.3.0/tests/test_legacy_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.1/.gitignore` & `qdrant_haystack-3.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.1/LICENSE.txt` & `qdrant_haystack-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.1/README.md` & `qdrant_haystack-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.1/pyproject.toml` & `qdrant_haystack-3.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ["haystack-ai", "qdrant-client"]
+dependencies = ["haystack-ai>=2.0.1", "qdrant-client"]
 
 [project.urls]
 Source = "https://github.com/deepset-ai/haystack-core-integrations"
 Documentation = "https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/qdrant/README.md"
 Issues = "https://github.com/deepset-ai/haystack-core-integrations/issues"
 
 [tool.hatch.build.targets.wheel]
@@ -99,14 +99,16 @@
   "YTT",
 ]
 ignore = [
   # Allow non-abstract empty methods in abstract base classes
   "B027",
   # Allow boolean positional values in function calls, like `dict.get(... True)`
   "FBT003",
+  # Allow boolean arguments in function definition
+  "FBT001", "FBT002",
   # Ignore checks for possible passwords
   "S105",
   "S106",
   "S107",
   # Ignore complexity
   "C901",
   "PLR0911",
```

### Comparing `qdrant_haystack-3.2.1/PKG-INFO` & `qdrant_haystack-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: qdrant-haystack
-Version: 3.2.1
+Version: 3.3.0
 Summary: An integration of Qdrant ANN vector database backend with Haystack
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/qdrant/README.md
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Author-email: Kacper Łukawski <kacper.lukawski@qdrant.com>, Anush Shetty <anush.shetty@qdrant.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: haystack-ai
+Requires-Dist: haystack-ai>=2.0.1
 Requires-Dist: qdrant-client
 Description-Content-Type: text/markdown
 
 # qdrant-haystack
 
 [![PyPI - Version](https://img.shields.io/pypi/v/qdrant-haystack.svg)](https://pypi.org/project/qdrant-haystack)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qdrant-haystack.svg)](https://pypi.org/project/qdrant-haystack)
```

