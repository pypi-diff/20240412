# Comparing `tmp/unstract_adapters-0.8.1.tar.gz` & `tmp/unstract_adapters-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstract_adapters-0.8.1.tar", last modified: Tue Apr  9 06:23:41 2024, max compression
+gzip compressed data, was "unstract_adapters-0.9.0.tar", last modified: Fri Apr 12 05:09:57 2024, max compression
```

## Comparing `unstract_adapters-0.8.1.tar` & `unstract_adapters-0.9.0.tar`

### file list

```diff
@@ -1,153 +1,153 @@
--rw-r--r--   0        0        0    34523 2024-04-09 06:23:17.493884 unstract_adapters-0.8.1/LICENSE
--rw-r--r--   0        0        0     1598 2024-04-09 06:23:17.493884 unstract_adapters-0.8.1/README.md
--rw-r--r--   0        0        0     2271 2024-04-09 06:23:41.681894 unstract_adapters-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      297 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/__init__.py
--rw-r--r--   0        0        0     2665 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/adapterkit.py
--rw-r--r--   0        0        0     1745 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/base.py
--rw-r--r--   0        0        0      282 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/constants.py
--rw-r--r--   0        0        0      183 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/__init__.py
--rw-r--r--   0        0        0      154 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/azure_open_ai/README.md
--rw-r--r--   0        0        0      514 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/azure_open_ai/pyproject.toml
--rw-r--r--   0        0        0      216 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/azure_open_ai/src/__init__.py
--rw-r--r--   0        0        0     2511 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py
--rw-r--r--   0        0        0     1548 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0      899 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/embedding_adapter.py
--rw-r--r--   0        0        0     1324 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/helper.py
--rw-r--r--   0        0        0       42 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/hugging_face/README.md
--rw-r--r--   0        0        0      517 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/hugging_face/pyproject.toml
--rw-r--r--   0        0        0      215 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/hugging_face/src/__init__.py
--rw-r--r--   0        0        0     2876 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py
--rw-r--r--   0        0        0      940 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json
--rw-r--r--   0        0        0       30 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/open_ai/README.md
--rw-r--r--   0        0        0      503 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/open_ai/pyproject.toml
--rw-r--r--   0        0        0      190 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/open_ai/src/__init__.py
--rw-r--r--   0        0        0     2091 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/open_ai/src/open_ai.py
--rw-r--r--   0        0        0      719 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0       35 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/palm/README.md
--rw-r--r--   0        0        0      510 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/palm/pyproject.toml
--rw-r--r--   0        0        0      179 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/palm/src/__init__.py
--rw-r--r--   0        0        0     2041 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/palm/src/palm.py
--rw-r--r--   0        0        0      804 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/palm/src/static/json_schema.json
--rw-r--r--   0        0        0       46 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/qdrant_fast_embed/README.md
--rw-r--r--   0        0        0      524 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/qdrant_fast_embed/pyproject.toml
--rw-r--r--   0        0        0      239 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/__init__.py
--rw-r--r--   0        0        0     1827 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py
--rw-r--r--   0        0        0      553 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json
--rw-r--r--   0        0        0     2086 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/register.py
--rw-r--r--   0        0        0      184 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/enums.py
--rw-r--r--   0        0        0      502 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/exceptions.py
--rw-r--r--   0        0        0      165 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/__init__.py
--rw-r--r--   0        0        0       33 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/anthropic/README.md
--rw-r--r--   0        0        0      498 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/anthropic/pyproject.toml
--rw-r--r--   0        0        0      207 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/anthropic/src/__init__.py
--rw-r--r--   0        0        0     2324 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/anthropic/src/anthropic.py
--rw-r--r--   0        0        0     1017 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/anthropic/src/static/json_schema.json
--rw-r--r--   0        0        0       33 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/any_scale/README.md
--rw-r--r--   0        0        0      498 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/any_scale/pyproject.toml
--rw-r--r--   0        0        0      202 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/any_scale/src/__init__.py
--rw-r--r--   0        0        0     2520 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/any_scale/src/anyscale.py
--rw-r--r--   0        0        0     1327 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/any_scale/src/static/json_schema.json
--rw-r--r--   0        0        0       37 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/azure_open_ai/README.md
--rw-r--r--   0        0        0      503 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/azure_open_ai/pyproject.toml
--rw-r--r--   0        0        0      219 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/azure_open_ai/src/__init__.py
--rw-r--r--   0        0        0     2312 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py
--rw-r--r--   0        0        0     1681 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0       41 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/constants.py
--rw-r--r--   0        0        0      844 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/helper.py
--rw-r--r--   0        0        0     1544 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/llm_adapter.py
--rw-r--r--   0        0        0       34 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/mistral/README.md
--rw-r--r--   0        0        0      500 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/mistral/pyproject.toml
--rw-r--r--   0        0        0      197 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/mistral/src/__init__.py
--rw-r--r--   0        0        0     1824 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/mistral/src/mistral.py
--rw-r--r--   0        0        0      852 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/mistral/src/static/json_schema.json
--rw-r--r--   0        0        0       31 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/open_ai/README.md
--rw-r--r--   0        0        0      491 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/open_ai/pyproject.toml
--rw-r--r--   0        0        0      193 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/open_ai/src/__init__.py
--rw-r--r--   0        0        0     2763 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/open_ai/src/open_ai.py
--rw-r--r--   0        0        0     1489 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0       26 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/palm/README.md
--rw-r--r--   0        0        0      496 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/palm/pyproject.toml
--rw-r--r--   0        0        0      182 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/palm/src/__init__.py
--rw-r--r--   0        0        0     2136 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/palm/src/palm.py
--rw-r--r--   0        0        0      989 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/palm/src/static/json_schema.json
--rw-r--r--   0        0        0     1963 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/register.py
--rw-r--r--   0        0        0       33 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/replicate/README.md
--rw-r--r--   0        0        0      499 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/replicate/pyproject.toml
--rw-r--r--   0        0        0      207 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/replicate/src/__init__.py
--rw-r--r--   0        0        0     1766 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/replicate/src/replicate.py
--rw-r--r--   0        0        0      840 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/replicate/src/static/json_schema.json
--rw-r--r--   0        0        0      273 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/vertex_ai/README.md
--rw-r--r--   0        0        0      480 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/vertex_ai/pyproject.toml
--rw-r--r--   0        0        0      203 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/vertex_ai/src/__init__.py
--rw-r--r--   0        0        0      964 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json
--rw-r--r--   0        0        0     2137 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py
--rw-r--r--   0        0        0      165 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/__init__.py
--rw-r--r--   0        0        0      430 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/constants.py
--rw-r--r--   0        0        0       42 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/README.md
--rw-r--r--   0        0        0      491 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/src/README.md
--rw-r--r--   0        0        0      237 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/src/__init__.py
--rw-r--r--   0        0        0     5994 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py
--rw-r--r--   0        0        0      817 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json
--rw-r--r--   0        0        0      978 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/ocr_adapter.py
--rw-r--r--   0        0        0     1964 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/register.py
--rw-r--r--   0        0        0      277 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/registry.py
--rw-r--r--   0        0        0     1745 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/utils.py
--rw-r--r--   0        0        0      181 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/__init__.py
--rw-r--r--   0        0        0      225 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/constants.py
--rw-r--r--   0        0        0     4187 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/helper.py
--rw-r--r--   0        0        0       27 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/milvus/README.md
--rw-r--r--   0        0        0      508 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/milvus/pyproject.toml
--rw-r--r--   0        0        0      188 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/milvus/src/__init__.py
--rw-r--r--   0        0        0     2775 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/milvus/src/milvus.py
--rw-r--r--   0        0        0      805 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json
--rw-r--r--   0        0        0       29 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/pinecone/README.md
--rw-r--r--   0        0        0      519 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/pinecone/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/pinecone/src/__init__.py
--rw-r--r--   0        0        0     3572 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/pinecone/src/pinecone.py
--rw-r--r--   0        0        0      771 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json
--rw-r--r--   0        0        0       29 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/postgres/README.md
--rw-r--r--   0        0        0      512 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/postgres/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/postgres/src/__init__.py
--rw-r--r--   0        0        0     3930 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/postgres/src/postgres.py
--rw-r--r--   0        0        0      912 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json
--rw-r--r--   0        0        0       27 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/qdrant/README.md
--rw-r--r--   0        0        0      513 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/qdrant/pyproject.toml
--rw-r--r--   0        0        0      188 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/qdrant/src/__init__.py
--rw-r--r--   0        0        0     3019 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/qdrant/src/qdrant.py
--rw-r--r--   0        0        0      571 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json
--rw-r--r--   0        0        0     2039 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/register.py
--rw-r--r--   0        0        0    75042 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/samples/sample1.txt
--rw-r--r--   0        0        0       29 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/supabase/README.md
--rw-r--r--   0        0        0      512 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/supabase/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/supabase/src/__init__.py
--rw-r--r--   0        0        0      937 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json
--rw-r--r--   0        0        0     3349 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/supabase/src/supabase.py
--rw-r--r--   0        0        0      947 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/vectordb_adapter.py
--rw-r--r--   0        0        0       29 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/weaviate/README.md
--rw-r--r--   0        0        0      520 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/weaviate/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/weaviate/src/__init__.py
--rw-r--r--   0        0        0      678 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json
--rw-r--r--   0        0        0     3722 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/weaviate/src/weaviate.py
--rw-r--r--   0        0        0      174 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/__init__.py
--rw-r--r--   0        0        0      145 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/constants.py
--rw-r--r--   0        0        0     5407 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/helper.py
--rw-r--r--   0        0        0       40 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/README.md
--rw-r--r--   0        0        0      495 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/pyproject.toml
--rw-r--r--   0        0        0      217 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/src/__init__.py
--rw-r--r--   0        0        0      981 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/src/constants.py
--rw-r--r--   0        0        0     6562 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py
--rw-r--r--   0        0        0     3115 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json
--rw-r--r--   0        0        0     1991 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/register.py
--rw-r--r--   0        0        0       51 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_community/README.md
--rw-r--r--   0        0        0      499 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_community/pyproject.toml
--rw-r--r--   0        0        0      255 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_community/src/__init__.py
--rw-r--r--   0        0        0      583 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json
--rw-r--r--   0        0        0     1463 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py
--rw-r--r--   0        0        0       52 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_enterprise/README.md
--rw-r--r--   0        0        0      499 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_enterprise/pyproject.toml
--rw-r--r--   0        0        0      259 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_enterprise/src/__init__.py
--rw-r--r--   0        0        0      805 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json
--rw-r--r--   0        0        0     1468 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py
--rw-r--r--   0        0        0     1006 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/x2text_adapter.py
--rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 unstract_adapters-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-12 05:09:37.376570 unstract_adapters-0.9.0/LICENSE
+-rw-r--r--   0        0        0      849 2024-04-12 05:09:37.376570 unstract_adapters-0.9.0/README.md
+-rw-r--r--   0        0        0     2632 2024-04-12 05:09:57.816741 unstract_adapters-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      298 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/__init__.py
+-rw-r--r--   0        0        0     2805 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/adapterkit.py
+-rw-r--r--   0        0        0     1830 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/base.py
+-rw-r--r--   0        0        0      282 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/constants.py
+-rw-r--r--   0        0        0      183 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/azure_open_ai/README.md
+-rw-r--r--   0        0        0      494 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/azure_open_ai/pyproject.toml
+-rw-r--r--   0        0        0      216 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/azure_open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2468 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py
+-rw-r--r--   0        0        0     1548 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0     1145 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/embedding_adapter.py
+-rw-r--r--   0        0        0     1319 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/helper.py
+-rw-r--r--   0        0        0       42 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/hugging_face/README.md
+-rw-r--r--   0        0        0      491 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/hugging_face/pyproject.toml
+-rw-r--r--   0        0        0      216 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/hugging_face/src/__init__.py
+-rw-r--r--   0        0        0     2449 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py
+-rw-r--r--   0        0        0      940 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json
+-rw-r--r--   0        0        0       30 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/open_ai/README.md
+-rw-r--r--   0        0        0      482 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/open_ai/pyproject.toml
+-rw-r--r--   0        0        0      190 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2055 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/open_ai/src/open_ai.py
+-rw-r--r--   0        0        0      719 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0       35 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/palm/README.md
+-rw-r--r--   0        0        0      476 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/palm/pyproject.toml
+-rw-r--r--   0        0        0      179 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/palm/src/__init__.py
+-rw-r--r--   0        0        0     1993 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/palm/src/palm.py
+-rw-r--r--   0        0        0      804 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/palm/src/static/json_schema.json
+-rw-r--r--   0        0        0       46 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/qdrant_fast_embed/README.md
+-rw-r--r--   0        0        0      500 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/qdrant_fast_embed/pyproject.toml
+-rw-r--r--   0        0        0      240 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/__init__.py
+-rw-r--r--   0        0        0     1784 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py
+-rw-r--r--   0        0        0      553 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json
+-rw-r--r--   0        0        0     2086 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/embedding/register.py
+-rw-r--r--   0        0        0      184 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/enums.py
+-rw-r--r--   0        0        0      502 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/exceptions.py
+-rw-r--r--   0        0        0      165 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/anthropic/README.md
+-rw-r--r--   0        0        0      474 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/anthropic/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/anthropic/src/__init__.py
+-rw-r--r--   0        0        0     2000 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/anthropic/src/anthropic.py
+-rw-r--r--   0        0        0     1017 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/anthropic/src/static/json_schema.json
+-rw-r--r--   0        0        0       33 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/any_scale/README.md
+-rw-r--r--   0        0        0      473 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/any_scale/pyproject.toml
+-rw-r--r--   0        0        0      202 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/any_scale/src/__init__.py
+-rw-r--r--   0        0        0     2054 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/any_scale/src/anyscale.py
+-rw-r--r--   0        0        0     1327 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/any_scale/src/static/json_schema.json
+-rw-r--r--   0        0        0       37 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/azure_open_ai/README.md
+-rw-r--r--   0        0        0      482 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/azure_open_ai/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/azure_open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2290 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py
+-rw-r--r--   0        0        0     1681 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0       69 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/constants.py
+-rw-r--r--   0        0        0      850 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/helper.py
+-rw-r--r--   0        0        0     1573 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/llm_adapter.py
+-rw-r--r--   0        0        0       34 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/mistral/README.md
+-rw-r--r--   0        0        0      473 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/mistral/pyproject.toml
+-rw-r--r--   0        0        0      197 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/mistral/src/__init__.py
+-rw-r--r--   0        0        0     1774 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/mistral/src/mistral.py
+-rw-r--r--   0        0        0      852 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/mistral/src/static/json_schema.json
+-rw-r--r--   0        0        0       31 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/open_ai/README.md
+-rw-r--r--   0        0        0      470 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/open_ai/pyproject.toml
+-rw-r--r--   0        0        0      193 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2240 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/open_ai/src/open_ai.py
+-rw-r--r--   0        0        0     1489 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0       26 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/palm/README.md
+-rw-r--r--   0        0        0      462 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/palm/pyproject.toml
+-rw-r--r--   0        0        0      182 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/palm/src/__init__.py
+-rw-r--r--   0        0        0     1871 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/palm/src/palm.py
+-rw-r--r--   0        0        0      989 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/palm/src/static/json_schema.json
+-rw-r--r--   0        0        0     1963 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/register.py
+-rw-r--r--   0        0        0       33 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/replicate/README.md
+-rw-r--r--   0        0        0      474 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/replicate/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/replicate/src/__init__.py
+-rw-r--r--   0        0        0     1714 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/replicate/src/replicate.py
+-rw-r--r--   0        0        0      840 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/replicate/src/static/json_schema.json
+-rw-r--r--   0        0        0      273 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/vertex_ai/README.md
+-rw-r--r--   0        0        0      444 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/vertex_ai/pyproject.toml
+-rw-r--r--   0        0        0      203 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/vertex_ai/src/__init__.py
+-rw-r--r--   0        0        0      964 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0     2085 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py
+-rw-r--r--   0        0        0      165 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/__init__.py
+-rw-r--r--   0        0        0      430 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/constants.py
+-rw-r--r--   0        0        0       42 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/README.md
+-rw-r--r--   0        0        0      491 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/src/README.md
+-rw-r--r--   0        0        0      237 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/src/__init__.py
+-rw-r--r--   0        0        0     5955 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py
+-rw-r--r--   0        0        0      817 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0      978 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/ocr_adapter.py
+-rw-r--r--   0        0        0     1964 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/ocr/register.py
+-rw-r--r--   0        0        0      277 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/registry.py
+-rw-r--r--   0        0        0     1745 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/utils.py
+-rw-r--r--   0        0        0      181 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/constants.py
+-rw-r--r--   0        0        0     4289 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/helper.py
+-rw-r--r--   0        0        0       27 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/milvus/README.md
+-rw-r--r--   0        0        0      485 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/milvus/pyproject.toml
+-rw-r--r--   0        0        0      188 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/milvus/src/__init__.py
+-rw-r--r--   0        0        0     2795 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/milvus/src/milvus.py
+-rw-r--r--   0        0        0      805 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json
+-rw-r--r--   0        0        0       29 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/pinecone/README.md
+-rw-r--r--   0        0        0      489 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/pinecone/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/pinecone/src/__init__.py
+-rw-r--r--   0        0        0     3732 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/pinecone/src/pinecone.py
+-rw-r--r--   0        0        0      771 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json
+-rw-r--r--   0        0        0       29 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/postgres/README.md
+-rw-r--r--   0        0        0      489 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/postgres/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/postgres/src/__init__.py
+-rw-r--r--   0        0        0     3923 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/postgres/src/postgres.py
+-rw-r--r--   0        0        0      912 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json
+-rw-r--r--   0        0        0       27 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/qdrant/README.md
+-rw-r--r--   0        0        0      485 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/qdrant/pyproject.toml
+-rw-r--r--   0        0        0      188 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/qdrant/src/__init__.py
+-rw-r--r--   0        0        0     2719 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/qdrant/src/qdrant.py
+-rw-r--r--   0        0        0      571 2024-04-12 05:09:37.380570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json
+-rw-r--r--   0        0        0     2039 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/register.py
+-rw-r--r--   0        0        0    75042 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/samples/sample1.txt
+-rw-r--r--   0        0        0       30 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/supabase/README.md
+-rw-r--r--   0        0        0      489 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/supabase/pyproject.toml
+-rw-r--r--   0        0        0      199 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/supabase/src/__init__.py
+-rw-r--r--   0        0        0      937 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json
+-rw-r--r--   0        0        0     3371 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/supabase/src/supabase.py
+-rw-r--r--   0        0        0     1328 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/vectordb_adapter.py
+-rw-r--r--   0        0        0       29 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/weaviate/README.md
+-rw-r--r--   0        0        0      489 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/weaviate/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/weaviate/src/__init__.py
+-rw-r--r--   0        0        0      678 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json
+-rw-r--r--   0        0        0     3715 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/vectordb/weaviate/src/weaviate.py
+-rw-r--r--   0        0        0      174 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/constants.py
+-rw-r--r--   0        0        0     5407 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/helper.py
+-rw-r--r--   0        0        0       40 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/README.md
+-rw-r--r--   0        0        0      495 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/pyproject.toml
+-rw-r--r--   0        0        0      217 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/src/__init__.py
+-rw-r--r--   0        0        0      981 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/src/constants.py
+-rw-r--r--   0        0        0     6559 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py
+-rw-r--r--   0        0        0     3115 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json
+-rw-r--r--   0        0        0     1991 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/register.py
+-rw-r--r--   0        0        0       51 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_community/README.md
+-rw-r--r--   0        0        0      499 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_community/pyproject.toml
+-rw-r--r--   0        0        0      255 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_community/src/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json
+-rw-r--r--   0        0        0     1460 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py
+-rw-r--r--   0        0        0       52 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_enterprise/README.md
+-rw-r--r--   0        0        0      499 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_enterprise/pyproject.toml
+-rw-r--r--   0        0        0      259 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_enterprise/src/__init__.py
+-rw-r--r--   0        0        0      805 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json
+-rw-r--r--   0        0        0     1465 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py
+-rw-r--r--   0        0        0     1006 2024-04-12 05:09:37.384570 unstract_adapters-0.9.0/src/unstract/adapters/x2text/x2text_adapter.py
+-rw-r--r--   0        0        0     2673 1970-01-01 00:00:00.000000 unstract_adapters-0.9.0/PKG-INFO
```

### Comparing `unstract_adapters-0.8.1/LICENSE` & `unstract_adapters-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/adapterkit.py` & `unstract_adapters-0.9.0/src/unstract/adapters/adapterkit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import logging
 from typing import Any
 
+from singleton_decorator import singleton
+
 from unstract.adapters import AdapterDict
 from unstract.adapters.base import Adapter
 from unstract.adapters.constants import Common
 from unstract.adapters.embedding import adapters as embedding_adapters
 from unstract.adapters.llm import adapters as llm_adapters
 from unstract.adapters.ocr import adapters as ocr_adapters
 from unstract.adapters.vectordb import adapters as vectordb_adapters
 from unstract.adapters.x2text import adapters as x2text_adapters
 
 logger = logging.getLogger(__name__)
 
 
+# Declaring this class as a Singleton to avoid initialising
+# adapters list everytime
+@singleton
 class Adapterkit:
     def __init__(self) -> None:
         self._adapters: AdapterDict = (
             embedding_adapters
             | llm_adapters
             | vectordb_adapters
             | x2text_adapters
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/base.py` & `unstract_adapters-0.9.0/src/unstract/adapters/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import logging
 from abc import ABC, abstractmethod
-from typing import Any, Optional, Union
+from typing import Any, Union
+
+from llama_index.core import MockEmbedding
+from llama_index.core.embeddings import BaseEmbedding
+from llama_index.core.llms import LLM, MockLLM
+from llama_index.core.vector_stores import SimpleVectorStore
+from llama_index.core.vector_stores.types import (
+    BasePydanticVectorStore,
+    VectorStore,
+)
 
-from llama_index.embeddings.base import BaseEmbedding
-from llama_index.llms.llm import LLM
-from llama_index.vector_stores.types import BasePydanticVectorStore, VectorStore
 from unstract.adapters.enums import AdapterTypes
 
 logger = logging.getLogger(__name__)
 
 
 class Adapter(ABC):
     def __init__(self, name: str):
@@ -40,29 +46,28 @@
         return ""
 
     @staticmethod
     @abstractmethod
     def get_adapter_type() -> AdapterTypes:
         return ""
 
-    def get_llm_instance(self, llm_config: dict[str, Any]) -> Optional[LLM]:
+    def get_llm_instance(self, llm_config: dict[str, Any]) -> LLM:
         # Overriding implementations use llm_config
-        return None
+        return MockLLM()
 
     def get_vector_db_instance(
         self, vector_db_config: dict[str, Any]
-    ) -> Union[BasePydanticVectorStore, VectorStore, None]:
+    ) -> Union[BasePydanticVectorStore, VectorStore]:
         # Overriding implementations use vector_db_config
-        return None
+        return SimpleVectorStore()
 
     def get_embedding_instance(
         self, embed_config: dict[str, Any]
-    ) -> Optional[BaseEmbedding]:
-        # Overriding implementations use embed_config
-        return None
+    ) -> BaseEmbedding:
+        return MockEmbedding(embed_dim=1)
 
     @abstractmethod
     def test_connection(self) -> bool:
         """Override to test connection for a adapter.
 
         Returns:
             bool: Flag indicating if the credentials are valid or not
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py` & `unstract_adapters-0.9.0/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 import json
 import os
 from typing import Any, Optional
 
-from llama_index.embeddings.azure_openai import AzureOpenAIEmbedding
-from llama_index.embeddings.base import BaseEmbedding
+from llama_index.core.embeddings import BaseEmbedding
+from llama_index.embeddings.huggingface import HuggingFaceEmbedding
+
 from unstract.adapters.embedding.embedding_adapter import EmbeddingAdapter
 from unstract.adapters.embedding.helper import EmbeddingHelper
 from unstract.adapters.exceptions import AdapterError
 
 
 class Constants:
     ADAPTER_NAME = "adapter_name"
-    MODEL = "model"
-    API_KEY = "api_key"
-    API_VERSION = "api_version"
-    AZURE_ENDPOINT = "azure_endpoint"
-    DEPLOYMENT_NAME = "deployment_name"
-    API_TYPE = "azure"
+    MODEL = "model_name"
+    TOKENIZER_NAME = "tokenizer_name"
+    MAX_LENGTH = "max_length"
+    NORMALIZE = "normalize"
 
 
-class AzureOpenAI(EmbeddingAdapter):
+class HuggingFace(EmbeddingAdapter):
     def __init__(self, settings: dict[str, Any]):
-        super().__init__("AzureOpenAIEmbedding")
+        super().__init__("HuggingFace")
         self.config = settings
         self.json_credentials = json.loads(
             settings.get("json_credentials", "{}")
         )
 
     @staticmethod
     def get_id() -> str:
-        return "azureopenai|9770f3f6-f8ba-4fa0-bb3a-bef48a00e66f"
+        return "huggingface|90ec9ec2-1768-4d69-8fb1-c88b95de5e5a"
 
     @staticmethod
     def get_name() -> str:
-        return "AzureOpenAIEmbedding"
+        return "HuggingFace"
 
     @staticmethod
     def get_description() -> str:
-        return "AzureOpenAI Embedding"
+        return "HuggingFace LLM"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/AzureopenAI.png"
-        )
+        return "/icons/adapter-icons/huggingface.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_embedding_instance(self) -> Optional[BaseEmbedding]:
+    def get_embedding_instance(self) -> BaseEmbedding:
         try:
             embedding_batch_size = EmbeddingHelper.get_embedding_batch_size(
                 config=self.config
             )
-            embedding = AzureOpenAIEmbedding(
-                model=str(self.config.get(Constants.MODEL)),
-                deployment_name=str(self.config.get(Constants.DEPLOYMENT_NAME)),
-                api_key=str(self.config.get(Constants.API_KEY)),
-                api_version=str(self.config.get(Constants.API_VERSION)),
-                azure_endpoint=str(self.config.get(Constants.AZURE_ENDPOINT)),
+            max_length: Optional[int] = (
+                int(self.config.get(Constants.MAX_LENGTH, 0))
+                if self.config.get(Constants.MAX_LENGTH)
+                else None
+            )
+            embedding: BaseEmbedding = HuggingFaceEmbedding(
+                model_name=str(self.config.get(Constants.MODEL)),
+                tokenizer_name=str(self.config.get(Constants.TOKENIZER_NAME)),
+                normalize=bool(self.config.get(Constants.NORMALIZE)),
                 embed_batch_size=embedding_batch_size,
-                api_type=Constants.API_TYPE,
+                max_length=max_length,
             )
+
             return embedding
         except Exception as e:
             raise AdapterError(str(e))
 
     def test_connection(self) -> bool:
         embedding = self.get_embedding_instance()
         test_result: bool = EmbeddingHelper.test_embedding_instance(embedding)
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/embedding/embedding_adapter.py` & `unstract_adapters-0.9.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,61 @@
-from abc import ABC
-from typing import Any, Optional
-
-from llama_index.core.embeddings.base import BaseEmbedding
-from unstract.adapters.base import Adapter
-from unstract.adapters.enums import AdapterTypes
-
-
-class EmbeddingAdapter(Adapter, ABC):
-    def __init__(self, name: str):
-        super().__init__(name)
-        self.name = name
+import json
+import os
+from typing import Any
+
+from llama_index.core.embeddings import BaseEmbedding
+from llama_index.embeddings.fastembed import FastEmbedEmbedding
+
+from unstract.adapters.embedding.embedding_adapter import EmbeddingAdapter
+from unstract.adapters.embedding.helper import EmbeddingHelper
+from unstract.adapters.exceptions import AdapterError
+
+
+class Constants:
+    MODEL = "model_name"
+    ADAPTER_NAME = "adapter_name"
+
+
+class QdrantFastEmbedM(EmbeddingAdapter):
+    def __init__(self, settings: dict[str, Any]):
+        super().__init__("QdrantFastEmbedM")
+        self.config = settings
+        self.json_credentials = json.loads(
+            settings.get("json_credentials", "{}")
+        )
 
     @staticmethod
     def get_id() -> str:
-        return ""
+        return "qdrantfastembed|31e83eee-a416-4c07-9c9c-02392d5bcf7f"
 
     @staticmethod
     def get_name() -> str:
-        return ""
+        return "QdrantFastEmbedM"
 
     @staticmethod
     def get_description() -> str:
-        return ""
+        return "QdrantFastEmbedM LLM"
 
     @staticmethod
     def get_icon() -> str:
-        return ""
+        return "/icons/adapter-icons/qdrant.png"
 
     @staticmethod
     def get_json_schema() -> str:
-        return ""
-
-    @staticmethod
-    def get_adapter_type() -> AdapterTypes:
-        return AdapterTypes.EMBEDDING
-
-    def get_embedding_instance(
-        self, embed_config: dict[str, Any]
-    ) -> Optional[BaseEmbedding]:
-        return None
+        f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
+        schema = f.read()
+        f.close()
+        return schema
+
+    def get_embedding_instance(self) -> BaseEmbedding:
+        try:
+            embedding: BaseEmbedding = FastEmbedEmbedding(
+                model_name=str(self.config.get(Constants.MODEL))
+            )
+            return embedding
+        except Exception as e:
+            raise AdapterError(str(e))
+
+    def test_connection(self) -> bool:
+        embedding = self.get_embedding_instance()
+        test_result: bool = EmbeddingHelper.test_embedding_instance(embedding)
+        return test_result
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/embedding/helper.py` & `unstract_adapters-0.9.0/src/unstract/adapters/embedding/helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from typing import Any, Optional
 
-from llama_index.core.embeddings.base import BaseEmbedding
+from llama_index.core.embeddings import BaseEmbedding
 
 from unstract.adapters.exceptions import AdapterError
 
 logger = logging.getLogger(__name__)
 
 
 class EmbeddingConstants:
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py` & `unstract_adapters-0.9.0/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,74 @@
 import json
 import os
-from typing import Any, Optional
+from typing import Any
+
+from llama_index.core.embeddings import BaseEmbedding
+from llama_index.embeddings.azure_openai import AzureOpenAIEmbedding
 
-from llama_index.embeddings.base import BaseEmbedding
-from llama_index.embeddings.huggingface import HuggingFaceEmbedding
 from unstract.adapters.embedding.embedding_adapter import EmbeddingAdapter
 from unstract.adapters.embedding.helper import EmbeddingHelper
 from unstract.adapters.exceptions import AdapterError
 
 
 class Constants:
     ADAPTER_NAME = "adapter_name"
-    MODEL = "model_name"
-    TOKENIZER_NAME = "tokenizer_name"
-    MAX_LENGTH = "max_length"
-    NORMALIZE = "normalize"
+    MODEL = "model"
+    API_KEY = "api_key"
+    API_VERSION = "api_version"
+    AZURE_ENDPOINT = "azure_endpoint"
+    DEPLOYMENT_NAME = "deployment_name"
+    API_TYPE = "azure"
 
 
-class HuggingFace(EmbeddingAdapter):
+class AzureOpenAI(EmbeddingAdapter):
     def __init__(self, settings: dict[str, Any]):
-        super().__init__("HuggingFace")
+        super().__init__("AzureOpenAIEmbedding")
         self.config = settings
         self.json_credentials = json.loads(
             settings.get("json_credentials", "{}")
         )
 
     @staticmethod
     def get_id() -> str:
-        return "huggingface|90ec9ec2-1768-4d69-8fb1-c88b95de5e5a"
+        return "azureopenai|9770f3f6-f8ba-4fa0-bb3a-bef48a00e66f"
 
     @staticmethod
     def get_name() -> str:
-        return "HuggingFace"
+        return "AzureOpenAIEmbedding"
 
     @staticmethod
     def get_description() -> str:
-        return "HuggingFace LLM"
+        return "AzureOpenAI Embedding"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/huggingface.png"
-        )
+        return "/icons/adapter-icons/AzureopenAI.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_embedding_instance(self) -> Optional[BaseEmbedding]:
+    def get_embedding_instance(self) -> BaseEmbedding:
         try:
             embedding_batch_size = EmbeddingHelper.get_embedding_batch_size(
                 config=self.config
             )
-            if (self.config.get(Constants.MAX_LENGTH)) is not None:
-                embedding = HuggingFaceEmbedding(
-                    model_name=str(self.config.get(Constants.MODEL)),
-                    tokenizer_name=str(
-                        self.config.get(Constants.TOKENIZER_NAME)
-                    ),
-                    normalize=bool(self.config.get(Constants.NORMALIZE)),
-                    embed_batch_size=embedding_batch_size,
-                    max_length=int(self.config.get(Constants.MAX_LENGTH, 10)),
-                )
-            else:
-                embedding = HuggingFaceEmbedding(
-                    model_name=str(self.config.get(Constants.MODEL)),
-                    tokenizer_name=str(
-                        self.config.get(Constants.TOKENIZER_NAME)
-                    ),
-                    normalize=bool(self.config.get(Constants.NORMALIZE)),
-                    embed_batch_size=embedding_batch_size,
-                )
+            embedding: BaseEmbedding = AzureOpenAIEmbedding(
+                model=str(self.config.get(Constants.MODEL)),
+                deployment_name=str(self.config.get(Constants.DEPLOYMENT_NAME)),
+                api_key=str(self.config.get(Constants.API_KEY)),
+                api_version=str(self.config.get(Constants.API_VERSION)),
+                azure_endpoint=str(self.config.get(Constants.AZURE_ENDPOINT)),
+                embed_batch_size=embedding_batch_size,
+                api_type=Constants.API_TYPE,
+            )
             return embedding
         except Exception as e:
             raise AdapterError(str(e))
 
     def test_connection(self) -> bool:
         embedding = self.get_embedding_instance()
         test_result: bool = EmbeddingHelper.test_embedding_instance(embedding)
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/embedding/open_ai/src/open_ai.py` & `unstract_adapters-0.9.0/src/unstract/adapters/embedding/open_ai/src/open_ai.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import os
-from typing import Any, Optional
+from typing import Any
+
+from llama_index.core.embeddings import BaseEmbedding
+from llama_index.embeddings.openai import OpenAIEmbedding
 
-from llama_index.embeddings import OpenAIEmbedding
-from llama_index.embeddings.base import BaseEmbedding
 from unstract.adapters.embedding.embedding_adapter import EmbeddingAdapter
 from unstract.adapters.embedding.helper import EmbeddingHelper
 from unstract.adapters.exceptions import AdapterError
 
 
 class Constants:
     API_KEY = "api_key"
@@ -35,29 +36,26 @@
 
     @staticmethod
     def get_description() -> str:
         return "OpenAI LLM"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/OpenAI.png"
-        )
+        return "/icons/adapter-icons/OpenAI.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_embedding_instance(self) -> Optional[BaseEmbedding]:
+    def get_embedding_instance(self) -> BaseEmbedding:
         try:
-            embedding = OpenAIEmbedding(
+            embedding: BaseEmbedding = OpenAIEmbedding(
                 api_key=str(self.config.get(Constants.API_KEY)),
                 api_base=str(
                     self.config.get(
                         Constants.API_BASE_KEY, Constants.API_BASE_VALUE
                     )
                 ),
                 api_type=Constants.API_TYPE,
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/embedding/palm/src/palm.py` & `unstract_adapters-0.9.0/src/unstract/adapters/embedding/palm/src/palm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import os
-from typing import Any, Optional
+from typing import Any
+
+from llama_index.core.embeddings import BaseEmbedding
+from llama_index.embeddings.google import GooglePaLMEmbedding
 
-from llama_index.embeddings.base import BaseEmbedding
-from llama_index.embeddings.google_palm import GooglePaLMEmbedding
 from unstract.adapters.embedding.embedding_adapter import EmbeddingAdapter
 from unstract.adapters.embedding.helper import EmbeddingHelper
 from unstract.adapters.exceptions import AdapterError
 
 
 class Constants:
     MODEL = "model_name"
@@ -33,32 +34,29 @@
 
     @staticmethod
     def get_description() -> str:
         return "PaLM LLM"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/PaLM.png"
-        )
+        return "/icons/adapter-icons/PaLM.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_embedding_instance(self) -> Optional[BaseEmbedding]:
+    def get_embedding_instance(self) -> BaseEmbedding:
         try:
             embedding_batch_size = EmbeddingHelper.get_embedding_batch_size(
                 config=self.config
             )
-            embedding = GooglePaLMEmbedding(
+            embedding: BaseEmbedding = GooglePaLMEmbedding(
                 model_name=str(self.config.get(Constants.MODEL)),
                 api_key=str(self.config.get(Constants.API_KEY)),
                 embed_batch_size=embedding_batch_size,
             )
             return embedding
         except Exception as e:
             raise AdapterError(str(e))
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/embedding/palm/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/embedding/palm/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py` & `unstract_adapters-0.9.0/src/unstract/adapters/embedding/embedding_adapter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,49 @@
-import json
-import os
-from typing import Any, Optional
-
-from llama_index.embeddings.base import BaseEmbedding
-from llama_index.embeddings.fastembed import FastEmbedEmbedding
-from unstract.adapters.embedding.embedding_adapter import EmbeddingAdapter
-from unstract.adapters.embedding.helper import EmbeddingHelper
-from unstract.adapters.exceptions import AdapterError
-
-
-class Constants:
-    MODEL = "model_name"
-    ADAPTER_NAME = "adapter_name"
-
-
-class QdrantFastEmbedM(EmbeddingAdapter):
-    def __init__(self, settings: dict[str, Any]):
-        super().__init__("QdrantFastEmbedM")
-        self.config = settings
-        self.json_credentials = json.loads(
-            settings.get("json_credentials", "{}")
-        )
+from abc import ABC
+from typing import Any
+
+from llama_index.core import MockEmbedding
+from llama_index.core.embeddings import BaseEmbedding
+
+from unstract.adapters.base import Adapter
+from unstract.adapters.enums import AdapterTypes
+
+
+class EmbeddingAdapter(Adapter, ABC):
+    def __init__(self, name: str):
+        super().__init__(name)
+        self.name = name
 
     @staticmethod
     def get_id() -> str:
-        return "qdrantfastembed|31e83eee-a416-4c07-9c9c-02392d5bcf7f"
+        return ""
 
     @staticmethod
     def get_name() -> str:
-        return "QdrantFastEmbedM"
+        return ""
 
     @staticmethod
     def get_description() -> str:
-        return "QdrantFastEmbedM LLM"
+        return ""
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/qdrant.png"
-        )
+        return ""
 
     @staticmethod
     def get_json_schema() -> str:
-        f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
-        schema = f.read()
-        f.close()
-        return schema
-
-    def get_embedding_instance(self) -> Optional[BaseEmbedding]:
-        try:
-            embedding = FastEmbedEmbedding(
-                model_name=str(self.config.get(Constants.MODEL))
-            )
-            return embedding
-        except Exception as e:
-            raise AdapterError(str(e))
-
-    def test_connection(self) -> bool:
-        embedding = self.get_embedding_instance()
-        test_result: bool = EmbeddingHelper.test_embedding_instance(embedding)
-        return test_result
+        return ""
+
+    @staticmethod
+    def get_adapter_type() -> AdapterTypes:
+        return AdapterTypes.EMBEDDING
+
+    def get_embedding_instance(
+        self, embed_config: dict[str, Any]
+    ) -> BaseEmbedding:
+        """Instantiate the llama index BaseEmbedding class.
+
+        Returns:
+            BaseEmbedding: llama index implementation of the Embedding
+            Raises exceptions for any error
+        """
+        return MockEmbedding(embed_dim=1)
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/embedding/register.py` & `unstract_adapters-0.9.0/src/unstract/adapters/embedding/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/anthropic/src/anthropic.py` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/anthropic/src/anthropic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
-from typing import Any, Optional
+from typing import Any
+
+from llama_index.core.llms import LLM
+from llama_index.llms.anthropic import Anthropic
 
-from llama_index.llms import Anthropic
-from llama_index.llms.llm import LLM
 from unstract.adapters.exceptions import AdapterError
 from unstract.adapters.llm.constants import LLMKeys
 from unstract.adapters.llm.helper import LLMHelper
 from unstract.adapters.llm.llm_adapter import LLMAdapter
 
 
 class Constants:
@@ -31,46 +32,38 @@
 
     @staticmethod
     def get_description() -> str:
         return "Anthropic LLM"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/Anthropic.png"
-        )
+        return "/icons/adapter-icons/Anthropic.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_llm_instance(self) -> Optional[LLM]:
+    def get_llm_instance(self) -> LLM:
         try:
-            timeout = float(
-                self.config.get(Constants.TIMEOUT, LLMKeys.DEFAULT_TIMEOUT)
+            llm: LLM = Anthropic(
+                model=str(self.config.get(Constants.MODEL)),
+                api_key=str(self.config.get(Constants.API_KEY)),
+                timeout=float(
+                    self.config.get(Constants.TIMEOUT, LLMKeys.DEFAULT_TIMEOUT)
+                ),
+                max_retries=int(
+                    self.config.get(
+                        Constants.MAX_RETIRES, LLMKeys.DEFAULT_MAX_RETRIES
+                    )
+                ),
+                temperature=0,
             )
-            if self.config.get(Constants.MAX_RETIRES) is not None:
-                llm = Anthropic(
-                    model=str(self.config.get(Constants.MODEL)),
-                    api_key=str(self.config.get(Constants.API_KEY)),
-                    timeout=timeout,
-                    max_retries=int(self.config.get(Constants.MAX_RETIRES, 3)),
-                    temperature=0,
-                )
-            else:
-                llm = Anthropic(
-                    model=str(self.config.get(Constants.MODEL)),
-                    api_key=str(self.config.get(Constants.API_KEY)),
-                    timeout=timeout,
-                    temperature=0,
-                )
             return llm
         except Exception as e:
             raise AdapterError(str(e))
 
     def test_connection(self) -> bool:
         llm = self.get_llm_instance()
         test_result: bool = LLMHelper.test_llm_instance(llm=llm)
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/anthropic/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/anthropic/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/any_scale/src/anyscale.py` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/any_scale/src/anyscale.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
-from typing import Any, Optional
+from typing import Any
+
+from llama_index.core.llms import LLM
+from llama_index.llms.anyscale import Anyscale
 
-from llama_index.llms import Anyscale
-from llama_index.llms.llm import LLM
 from unstract.adapters.exceptions import AdapterError
+from unstract.adapters.llm.constants import LLMKeys
 from unstract.adapters.llm.helper import LLMHelper
 from unstract.adapters.llm.llm_adapter import LLMAdapter
 
 
 class Constants:
     MODEL = "model"
     API_KEY = "api_key"
@@ -31,50 +33,37 @@
 
     @staticmethod
     def get_description() -> str:
         return "AnyScale LLM"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/anyscale.png"
-        )
+        return "/icons/adapter-icons/anyscale.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_llm_instance(self) -> Optional[LLM]:
+    def get_llm_instance(self) -> LLM:
         try:
-            if self.config.get(Constants.MAX_RETIRES) is not None:
-                llm = Anyscale(
-                    model=str(self.config.get(Constants.MODEL)),
-                    api_key=str(self.config.get(Constants.API_KEY)),
-                    api_base=str(self.config.get(Constants.API_BASE)),
-                    additional_kwargs=self.config.get(
-                        Constants.ADDITIONAL_KWARGS
-                    ),
-                    max_retries=int(self.config.get(Constants.MAX_RETIRES, 10)),
-                    temperature=0,
-                )
-            else:
-                llm = Anyscale(
-                    model=str(self.config.get(Constants.MODEL)),
-                    api_key=str(self.config.get(Constants.API_KEY)),
-                    api_base=str(self.config.get(Constants.API_BASE)),
-                    additional_kwargs=self.config.get(
-                        Constants.ADDITIONAL_KWARGS
-                    ),
-                    temperature=0,
-                )
-
+            llm: LLM = Anyscale(
+                model=str(self.config.get(Constants.MODEL)),
+                api_key=str(self.config.get(Constants.API_KEY)),
+                api_base=str(self.config.get(Constants.API_BASE)),
+                additional_kwargs=self.config.get(Constants.ADDITIONAL_KWARGS),
+                max_retries=int(
+                    self.config.get(
+                        Constants.MAX_RETIRES, LLMKeys.DEFAULT_MAX_RETRIES
+                    )
+                ),
+                temperature=0,
+            )
             return llm
         except Exception as e:
             raise AdapterError(str(e))
 
     def test_connection(self) -> bool:
         llm = self.get_llm_instance()
         test_result: bool = LLMHelper.test_llm_instance(llm=llm)
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/any_scale/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/any_scale/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
-from typing import Any, Optional
+from typing import Any
 
+from llama_index.core.llms import LLM
 from llama_index.llms.azure_openai import AzureOpenAI
-from llama_index.llms.llm import LLM
 
 from unstract.adapters.exceptions import AdapterError
 from unstract.adapters.llm.constants import LLMKeys
 from unstract.adapters.llm.helper import LLMHelper
 from unstract.adapters.llm.llm_adapter import LLMAdapter
 
 
@@ -15,14 +15,15 @@
     DEPLOYMENT_NAME = "deployment_name"
     API_KEY = "api_key"
     API_VERSION = "api_version"
     MAX_RETIRES = "max_retries"
     AZURE_ENDPONT = "azure_endpoint"
     API_TYPE = "azure"
     TIMEOUT = "timeout"
+    DEFAULT_MODEL = "gpt-35-turbo"
 
 
 class AzureOpenAILLM(LLMAdapter):
     def __init__(self, settings: dict[str, Any]):
         super().__init__("AzureOpenAI")
         self.config = settings
 
@@ -45,30 +46,28 @@
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_llm_instance(self) -> Optional[LLM]:
+    def get_llm_instance(self) -> LLM:
         try:
-            model: Optional[str] = self.config.get(Constants.MODEL)
-            llm = AzureOpenAI(
+            llm: LLM = AzureOpenAI(
+                model=self.config.get(Constants.MODEL, Constants.DEFAULT_MODEL),
                 deployment_name=str(self.config.get(Constants.DEPLOYMENT_NAME)),
                 api_key=str(self.config.get(Constants.API_KEY)),
                 api_version=str(self.config.get(Constants.API_VERSION)),
                 azure_endpoint=str(self.config.get(Constants.AZURE_ENDPONT)),
                 api_type=Constants.API_TYPE,
                 temperature=0,
                 timeout=self.config.get(
                     Constants.TIMEOUT, LLMKeys.DEFAULT_TIMEOUT
                 ),
             )
-            if model:
-                llm.model = model
             return llm
         except Exception as e:
             raise AdapterError(str(e))
 
     def test_connection(self) -> bool:
         llm = self.get_llm_instance()
         test_result: bool = LLMHelper.test_llm_instance(llm=llm)
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/helper.py` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/helper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import re
 from typing import Optional
 
-from llama_index.llms import LLM
+from llama_index.core.llms import LLM
+
 from unstract.adapters.exceptions import AdapterError
 
 logger = logging.getLogger(__name__)
 
 
 class LLMHelper:
     @staticmethod
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/llm_adapter.py` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/llm_adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from abc import ABC
-from typing import Any, Optional
+from typing import Any
 
-from llama_index.llms.llm import LLM
+from llama_index.core.llms import LLM, MockLLM
 
 from unstract.adapters.base import Adapter
 from unstract.adapters.enums import AdapterTypes
 
 logger = logging.getLogger(__name__)
 
 
@@ -35,21 +35,22 @@
     def get_json_schema() -> str:
         return ""
 
     @staticmethod
     def get_adapter_type() -> AdapterTypes:
         return AdapterTypes.LLM
 
-    def get_llm_instance(self) -> Optional[LLM]:
+    def get_llm_instance(self) -> LLM:
         """Instantiate the llama index LLM class.
 
         Returns:
-            Optional[LLM]: llama index implementation of the LLM
+            LLM: llama index implementation of the LLM
+            Raises exceptions for any error
         """
-        return None
+        return MockLLM()
 
     def test_connection(self, llm_metadata: dict[str, Any]) -> bool:
         return False
 
     def get_context_window_size(self) -> int:
         """Get the context window size supported by the LLM.
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/mistral/src/mistral.py` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/mistral/src/mistral.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
-from typing import Any, Optional
+from typing import Any
+
+from llama_index.core.llms import LLM
+from llama_index.llms.mistralai import MistralAI
 
-from llama_index.llms.llm import LLM
-from llama_index.llms.mistral import MistralAI
 from unstract.adapters.exceptions import AdapterError
 from unstract.adapters.llm.constants import LLMKeys
 from unstract.adapters.llm.helper import LLMHelper
 from unstract.adapters.llm.llm_adapter import LLMAdapter
 
 
 class Constants:
@@ -30,29 +31,26 @@
 
     @staticmethod
     def get_description() -> str:
         return "Mistral AI LLM"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/Mistral%20AI.png"
-        )
+        return "/icons/adapter-icons/Mistral%20AI.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_llm_instance(self) -> Optional[LLM]:
+    def get_llm_instance(self) -> LLM:
         try:
-            llm = MistralAI(
+            llm: LLM = MistralAI(
                 model=str(self.config.get(Constants.MODEL)),
                 api_key=str(self.config.get(Constants.API_KEY)),
                 temperature=0,
                 timeout=self.config.get(
                     Constants.TIMEOUT, LLMKeys.DEFAULT_TIMEOUT
                 ),
             )
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/mistral/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/mistral/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/open_ai/src/open_ai.py` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/open_ai/src/open_ai.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
-from typing import Any, Optional
+from typing import Any
+
+from llama_index.core.llms import LLM
+from llama_index.llms.openai import OpenAI
 
-from llama_index.llms import OpenAI
-from llama_index.llms.llm import LLM
 from unstract.adapters.exceptions import AdapterError
 from unstract.adapters.llm.constants import LLMKeys
 from unstract.adapters.llm.helper import LLMHelper
 from unstract.adapters.llm.llm_adapter import LLMAdapter
 
 
 class Constants:
@@ -34,52 +35,41 @@
 
     @staticmethod
     def get_description() -> str:
         return "OpenAI LLM"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/OpenAI.png"
-        )
+        return "/icons/adapter-icons/OpenAI.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_llm_instance(self) -> Optional[LLM]:
+    def get_llm_instance(self) -> LLM:
         try:
-            timeout = float(
-                self.config.get(Constants.TIMEOUT, LLMKeys.DEFAULT_TIMEOUT)
+            llm: LLM = OpenAI(
+                model=str(self.config.get(Constants.MODEL)),
+                api_key=str(self.config.get(Constants.API_KEY)),
+                api_base=str(self.config.get(Constants.API_BASE)),
+                api_version=str(self.config.get(Constants.API_VERSION)),
+                max_retries=int(
+                    self.config.get(
+                        Constants.MAX_RETIRES, LLMKeys.DEFAULT_MAX_RETRIES
+                    )
+                ),
+                api_type="openai",
+                temperature=0,
+                timeout=float(
+                    self.config.get(Constants.TIMEOUT, LLMKeys.DEFAULT_TIMEOUT)
+                ),
             )
-            if self.config.get(Constants.MAX_RETIRES) is not None:
-                llm = OpenAI(
-                    model=str(self.config.get(Constants.MODEL)),
-                    api_key=str(self.config.get(Constants.API_KEY)),
-                    api_base=str(self.config.get(Constants.API_BASE)),
-                    api_version=str(self.config.get(Constants.API_VERSION)),
-                    max_retries=int(self.config.get(Constants.MAX_RETIRES, 3)),
-                    api_type="openai",
-                    temperature=0,
-                    timeout=timeout,
-                )
-            else:
-                llm = OpenAI(
-                    model=str(self.config.get(Constants.MODEL)),
-                    api_key=str(self.config.get(Constants.API_KEY)),
-                    api_base=str(self.config.get(Constants.API_BASE)),
-                    api_version=str(self.config.get(Constants.API_VERSION)),
-                    api_type="openai",
-                    temperature=0,
-                    timeout=timeout,
-                )
             return llm
         except Exception as e:
             raise AdapterError(str(e))
 
     def test_connection(self) -> bool:
         llm = self.get_llm_instance()
         test_result: bool = LLMHelper.test_llm_instance(llm=llm)
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/open_ai/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/palm/src/palm.py` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/palm/src/palm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
-from typing import Any, Optional
+from typing import Any
 
-from llama_index.llms.llm import LLM
+from llama_index.core.llms import LLM
 from llama_index.llms.palm import PaLM
+
 from unstract.adapters.exceptions import AdapterError
 from unstract.adapters.llm.helper import LLMHelper
 from unstract.adapters.llm.llm_adapter import LLMAdapter
 
 
 class Constants:
     MODEL = "model_name"
@@ -30,43 +31,37 @@
 
     @staticmethod
     def get_description() -> str:
         return "Palm LLM"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/PaLM.png"
-        )
+        return "/icons/adapter-icons/PaLM.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_llm_instance(self) -> Optional[LLM]:
+    def get_llm_instance(self) -> LLM:
         try:
-            if self.config.get(Constants.NUM_OUTPUT) is not None:
-                llm = PaLM(
-                    model=str(self.config.get(Constants.MODEL)),
-                    api_key=str(self.config.get(Constants.API_KEY)),
-                    num_output=int(self.config.get(Constants.NUM_OUTPUT, 50)),
-                    api_type=Constants.API_TYPE,
-                    temperature=0,
-                )
-            else:
-                llm = PaLM(
-                    model=str(self.config.get(Constants.MODEL)),
-                    api_key=str(self.config.get(Constants.API_KEY)),
-                    api_type=Constants.API_TYPE,
-                    temperature=0,
-                )
+            num_output = (
+                int(self.config.get(Constants.NUM_OUTPUT, 50))
+                if self.config.get(Constants.NUM_OUTPUT) is not None
+                else None
+            )
+            llm: LLM = PaLM(
+                model=str(self.config.get(Constants.MODEL)),
+                api_key=str(self.config.get(Constants.API_KEY)),
+                num_output=num_output,
+                api_type=Constants.API_TYPE,
+                temperature=0,
+            )
             return llm
         except Exception as e:
             raise AdapterError(str(e))
 
     def test_connection(self) -> bool:
         llm = self.get_llm_instance()
         test_result: bool = LLMHelper.test_llm_instance(llm=llm)
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/palm/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/palm/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/register.py` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/replicate/src/replicate.py` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/replicate/src/replicate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
-from typing import Any, Optional
+from typing import Any
 
-from llama_index.llms.llm import LLM
+from llama_index.core.llms import LLM
 from llama_index.llms.replicate import Replicate
+
 from unstract.adapters.exceptions import AdapterError
 from unstract.adapters.llm.helper import LLMHelper
 from unstract.adapters.llm.llm_adapter import LLMAdapter
 
 
 class Constants:
     MODEL = "model"
@@ -28,18 +29,15 @@
 
     @staticmethod
     def get_description() -> str:
         return "Replicate LLM"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/Replicate.png"
-        )
+        return "/icons/adapter-icons/Replicate.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
@@ -48,17 +46,17 @@
     def can_write() -> bool:
         return True
 
     @staticmethod
     def can_read() -> bool:
         return True
 
-    def get_llm_instance(self) -> Optional[LLM]:
+    def get_llm_instance(self) -> LLM:
         try:
-            llm = Replicate(
+            llm: LLM = Replicate(
                 model=str(self.config.get(Constants.MODEL)),
                 prompt_key=str(self.config.get(Constants.API_KEY)),
                 temperature=0,
             )
             return llm
         except Exception as e:
             raise AdapterError(str(e))
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/replicate/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/replicate/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py` & `unstract_adapters-0.9.0/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import os
-from typing import Any, Optional
+from typing import Any
 
 from google.auth.transport import requests as google_requests
 from google.oauth2 import service_account
-from llama_index.llms.llm import LLM
+from llama_index.core.llms import LLM
 from llama_index.llms.vertex import Vertex
+
 from unstract.adapters.llm.helper import LLMHelper
 from unstract.adapters.llm.llm_adapter import LLMAdapter
 
 
 class Constants:
     MODEL = "model"
     PROJECT = "project"
@@ -31,37 +32,34 @@
 
     @staticmethod
     def get_description() -> str:
         return "Vertex Gemini LLM"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/VertexAI.png"
-        )
+        return "/icons/adapter-icons/VertexAI.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_llm_instance(self) -> Optional[LLM]:
+    def get_llm_instance(self) -> LLM:
         input_credentials = self.config.get(Constants.JSON_CREDENTIALS)
         if not input_credentials:
             input_credentials = "{}"
         json_credentials = json.loads(input_credentials)
         credentials = service_account.Credentials.from_service_account_info(
             info=json_credentials,
             scopes=["https://www.googleapis.com/auth/cloud-platform"],
         )
         credentials.refresh(google_requests.Request())
-        llm = Vertex(
+        llm: LLM = Vertex(
             project=str(self.config.get(Constants.PROJECT)),
             model=str(self.config.get(Constants.MODEL)),
             credentials=credentials,
             temperature=0,
             additional_kwargs={},
         )
         return llm
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py` & `unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,15 @@
 
     @staticmethod
     def get_description() -> str:
         return "Google Document AI OCR"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/GoogleDocumentAI.png"
-        )
+        return "/icons/adapter-icons/GoogleDocumentAI.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/ocr/ocr_adapter.py` & `unstract_adapters-0.9.0/src/unstract/adapters/ocr/ocr_adapter.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/ocr/register.py` & `unstract_adapters-0.9.0/src/unstract/adapters/ocr/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/utils.py` & `unstract_adapters-0.9.0/src/unstract/adapters/utils.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/helper.py` & `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import logging
 import os
 from typing import Union
 
-from llama_index import (
-    ServiceContext,
+from llama_index.core import (
+    MockEmbedding,
     SimpleDirectoryReader,
     StorageContext,
     VectorStoreIndex,
 )
-from llama_index.vector_stores.types import BasePydanticVectorStore, VectorStore
+from llama_index.core.llms import MockLLM
+from llama_index.core.vector_stores.types import (
+    BasePydanticVectorStore,
+    VectorStore,
+)
 
 from unstract.adapters.exceptions import AdapterError
 from unstract.adapters.vectordb.constants import VectorDbConstants
 
 logger = logging.getLogger(__name__)
 
 
@@ -21,39 +25,39 @@
     def test_vector_db_instance(
         vector_store: Union[VectorStore, BasePydanticVectorStore, None]
     ) -> bool:
         try:
             if vector_store is None:
                 return False
 
-            # For custom embedding args will be:
-            #     embed_model - InstructorEmbeddings(embed_batch_size=2)
-            #     chunk_size - 512
-            #     llm=None
-            service_context = ServiceContext.from_defaults(
-                llm=None, embed_model=None
-            )
-
             storage_context = StorageContext.from_defaults(
                 vector_store=vector_store
             )
             local_path = f"{os.path.dirname(__file__)}/samples/"
+            # Using mock llm and embedding here.
+            # For custom embedding args will be:
+            #     embed_model - InstructorEmbeddings(embed_batch_size=2)
+            #     chunk_size - 512
+            #     llm=None
+            llm = MockLLM()
+            embed_model = MockEmbedding(embed_dim=1)
             index = VectorStoreIndex.from_documents(
-                # By default SimpleDirectoryReader discards paths which
+                # By default, SimpleDirectoryReader discards paths which
                 # contain one or more parts that are hidden.
                 # In local, packages could be installed in a venv. This
                 # means a path can contain a ".venv" in it which will
                 # then be treated as hidden and subsequently discarded.
                 documents=SimpleDirectoryReader(
-                    local_path,exclude_hidden=False
+                    local_path, exclude_hidden=False
                 ).load_data(),
                 storage_context=storage_context,
-                service_context=service_context,
+                llm=llm,
+                embed_model=embed_model,
             )
-            query_engine = index.as_query_engine()
+            query_engine = index.as_query_engine(llm=llm)
 
             query_engine.query("What did the author learn?")
             return True
 
         except Exception as e:
             logger.error(f"Error occured while testing adapter {e}")
             raise AdapterError(str(e))
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/milvus/src/milvus.py` & `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/milvus/src/milvus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from typing import Any, Optional
 
-from llama_index.vector_stores import MilvusVectorStore
-from llama_index.vector_stores.types import VectorStore
+from llama_index.core.vector_stores.types import VectorStore
+from llama_index.vector_stores.milvus import MilvusVectorStore
 from pymilvus import MilvusClient
 
 from unstract.adapters.exceptions import AdapterError
 from unstract.adapters.vectordb.constants import VectorDbConstants
 from unstract.adapters.vectordb.helper import VectorDBHelper
 from unstract.adapters.vectordb.vectordb_adapter import VectorDBAdapter
 
@@ -34,51 +34,49 @@
 
     @staticmethod
     def get_description() -> str:
         return "Milvus VectorDB"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/Milvus.png"
-        )
+        return "/icons/adapter-icons/Milvus.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_vector_db_instance(self) -> Optional[VectorStore]:
+    def get_vector_db_instance(self) -> VectorStore:
         try:
             self.collection_name = VectorDBHelper.get_collection_name(
                 self.config.get(VectorDbConstants.VECTOR_DB_NAME),
                 self.config.get(VectorDbConstants.EMBEDDING_DIMENSION),
             )
             dimension = self.config.get(
                 VectorDbConstants.EMBEDDING_DIMENSION,
                 VectorDbConstants.DEFAULT_EMBEDDING_SIZE,
             )
-            vector_db = MilvusVectorStore(
+            vector_db: VectorStore = MilvusVectorStore(
                 uri=self.config.get(Constants.URI, ""),
                 collection_name=self.collection_name,
                 token=self.config.get(Constants.TOKEN, ""),
                 dim=dimension,
             )
-            self.client = vector_db.client
+            if vector_db is not None:
+                self.client = vector_db.client
             return vector_db
         except Exception as e:
             raise AdapterError(str(e))
 
     def test_connection(self) -> bool:
-        self.config[
-            VectorDbConstants.EMBEDDING_DIMENSION
-        ] = VectorDbConstants.TEST_CONNECTION_EMBEDDING_SIZE
+        self.config[VectorDbConstants.EMBEDDING_DIMENSION] = (
+            VectorDbConstants.TEST_CONNECTION_EMBEDDING_SIZE
+        )
         vector_db = self.get_vector_db_instance()
         test_result: bool = VectorDBHelper.test_vector_db_instance(
             vector_store=vector_db
         )
         # Delete the collection that was created for testing
         if self.client is not None:
             self.client.drop_collection(self.collection_name)
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/pinecone/src/pinecone.py` & `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/pinecone/src/pinecone.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import logging
 import os
-import time
 from typing import Any, Optional
 
-import pinecone
+from llama_index.core.vector_stores.types import BasePydanticVectorStore
 from llama_index.vector_stores.pinecone import PineconeVectorStore
-from llama_index.vector_stores.types import BasePydanticVectorStore
 from pinecone import NotFoundException
+from pinecone import Pinecone as LLamaIndexPinecone
+from pinecone import PodSpec
 
 from unstract.adapters.exceptions import AdapterError
 from unstract.adapters.vectordb.constants import VectorDbConstants
 from unstract.adapters.vectordb.helper import VectorDBHelper
 from unstract.adapters.vectordb.vectordb_adapter import VectorDBAdapter
 
 logger = logging.getLogger(__name__)
 
+
 class Constants:
     API_KEY = "api_key"
     ENVIRONMENT = "environment"
     NAMESPACE = "namespace"
     DIMENSION = 1536
     METRIC = "euclidean"
 
 
 class Pinecone(VectorDBAdapter):
     def __init__(self, settings: dict[str, Any]):
         super().__init__("Pinecone")
         self.config = settings
+        self.client: Optional[LLamaIndexPinecone] = None
         self.collection_name: str = VectorDbConstants.DEFAULT_VECTOR_DB_NAME
 
     @staticmethod
     def get_id() -> str:
         return "pinecone|83881133-485d-4ecc-b1f7-0009f96dc74a"
 
     @staticmethod
@@ -39,65 +41,65 @@
 
     @staticmethod
     def get_description() -> str:
         return "Pinecone VectorDB"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/pinecone.png"
-        )
+        return "/icons/adapter-icons/pinecone.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_vector_db_instance(self) -> Optional[BasePydanticVectorStore]:
+    def get_vector_db_instance(self) -> BasePydanticVectorStore:
         try:
-            pinecone.init(
-                api_key=str(self.config.get(Constants.API_KEY)),
-                environment=str(self.config.get(Constants.ENVIRONMENT)),
+            self.client = LLamaIndexPinecone(
+                api_key=str(self.config.get(Constants.API_KEY))
             )
             collection_name = VectorDBHelper.get_collection_name(
                 self.config.get(VectorDbConstants.VECTOR_DB_NAME),
                 self.config.get(VectorDbConstants.EMBEDDING_DIMENSION),
             )
-            # Pinecone allows only lowercase alphanumeric & hyphens for
-            # collection name
             self.collection_name = collection_name.replace("_", "-").lower()
             dimension = self.config.get(
                 VectorDbConstants.EMBEDDING_DIMENSION,
                 VectorDbConstants.DEFAULT_EMBEDDING_SIZE,
             )
             try:
-                pinecone.describe_index(name=self.collection_name)
-            except NotFoundException as e:
-                logger.info(f"Index:{self.collection_name} does not exist. Creating it.")
-                pinecone.create_index(
-                name=self.collection_name,
-                dimension=dimension,
-                metric=Constants.METRIC,
-            )
-            vector_db = PineconeVectorStore(
+                self.client.describe_index(name=self.collection_name)
+            except NotFoundException:
+                logger.info(
+                    f"Index:{self.collection_name} does not exist. Creating it."
+                )
+                self.client.create_index(
+                    name=self.collection_name,
+                    dimension=dimension,
+                    metric=Constants.METRIC,
+                    spec=PodSpec(
+                        environment=str(self.config.get(Constants.ENVIRONMENT))
+                    ),
+                )
+            vector_db: BasePydanticVectorStore = PineconeVectorStore(
                 index_name=self.collection_name,
                 api_key=str(self.config.get(Constants.API_KEY)),
                 environment=str(self.config.get(Constants.ENVIRONMENT)),
             )
             return vector_db
         except Exception as e:
             raise AdapterError(str(e))
 
     def test_connection(self) -> bool:
-        self.config[
-            VectorDbConstants.EMBEDDING_DIMENSION
-        ] = VectorDbConstants.TEST_CONNECTION_EMBEDDING_SIZE
+        self.config[VectorDbConstants.EMBEDDING_DIMENSION] = (
+            VectorDbConstants.TEST_CONNECTION_EMBEDDING_SIZE
+        )
         vector_db = self.get_vector_db_instance()
         test_result: bool = VectorDBHelper.test_vector_db_instance(
             vector_store=vector_db
         )
         # Delete the collection that was created for testing
-        pinecone.delete_index(self.collection_name)
+        if self.client:
+            self.client.delete_index(self.collection_name)
         return test_result
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/postgres/src/postgres.py` & `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/postgres/src/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from typing import Any, Optional
 
 import psycopg2
-from llama_index.vector_stores import PGVectorStore
-from llama_index.vector_stores.types import BasePydanticVectorStore
+from llama_index.core.vector_stores.types import BasePydanticVectorStore
+from llama_index.vector_stores.postgres import PGVectorStore
 from psycopg2._psycopg import connection
+
 from unstract.adapters.exceptions import AdapterError
 from unstract.adapters.vectordb.constants import VectorDbConstants
 from unstract.adapters.vectordb.helper import VectorDBHelper
 from unstract.adapters.vectordb.vectordb_adapter import VectorDBAdapter
 
 
 class Constants:
@@ -38,41 +39,38 @@
 
     @staticmethod
     def get_description() -> str:
         return "Postgres VectorDB"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/postgres.png"
-        )
+        return "/icons/adapter-icons/postgres.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_vector_db_instance(self) -> Optional[BasePydanticVectorStore]:
+    def get_vector_db_instance(self) -> BasePydanticVectorStore:
         try:
             self.collection_name = VectorDBHelper.get_collection_name(
                 self.config.get(VectorDbConstants.VECTOR_DB_NAME),
                 self.config.get(VectorDbConstants.EMBEDDING_DIMENSION),
             )
             self.schema_name = self.config.get(
                 Constants.SCHEMA,
                 VectorDbConstants.DEFAULT_VECTOR_DB_NAME,
             )
             dimension = self.config.get(
                 VectorDbConstants.EMBEDDING_DIMENSION,
                 VectorDbConstants.DEFAULT_EMBEDDING_SIZE,
             )
-            vector_db = PGVectorStore.from_params(
+            vector_db: BasePydanticVectorStore = PGVectorStore.from_params(
                 database=self.config.get(Constants.DATABASE),
                 schema_name=self.schema_name,
                 host=self.config.get(Constants.HOST),
                 password=self.config.get(Constants.PASSWORD),
                 port=str(self.config.get(Constants.PORT)),
                 user=self.config.get(Constants.USER),
                 table_name=self.collection_name,
@@ -87,17 +85,17 @@
             )
 
             return vector_db
         except Exception as e:
             raise AdapterError(str(e))
 
     def test_connection(self) -> bool:
-        self.config[
-            VectorDbConstants.EMBEDDING_DIMENSION
-        ] = VectorDbConstants.TEST_CONNECTION_EMBEDDING_SIZE
+        self.config[VectorDbConstants.EMBEDDING_DIMENSION] = (
+            VectorDbConstants.TEST_CONNECTION_EMBEDDING_SIZE
+        )
         vector_db = self.get_vector_db_instance()
         test_result: bool = VectorDBHelper.test_vector_db_instance(
             vector_store=vector_db
         )
 
         # Delete the collection that was created for testing
         if self.client is not None:
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/qdrant/src/qdrant.py` & `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/qdrant/src/qdrant.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 from typing import Any, Optional
 
+from llama_index.core.vector_stores.types import BasePydanticVectorStore
 from llama_index.vector_stores.qdrant import QdrantVectorStore
-from llama_index.vector_stores.types import BasePydanticVectorStore
 from qdrant_client import QdrantClient
+
 from unstract.adapters.exceptions import AdapterError
 from unstract.adapters.vectordb.constants import VectorDbConstants
 from unstract.adapters.vectordb.helper import VectorDBHelper
 from unstract.adapters.vectordb.vectordb_adapter import VectorDBAdapter
 
 logger = logging.getLogger(__name__)
 
@@ -35,50 +36,41 @@
 
     @staticmethod
     def get_description() -> str:
         return "Qdrant LLM"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/qdrant.png"
-        )
+        return "/icons/adapter-icons/qdrant.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_vector_db_instance(self) -> Optional[BasePydanticVectorStore]:
+    def get_vector_db_instance(self) -> BasePydanticVectorStore:
         try:
             self.collection_name = VectorDBHelper.get_collection_name(
                 self.config.get(VectorDbConstants.VECTOR_DB_NAME),
                 self.config.get(VectorDbConstants.EMBEDDING_DIMENSION),
             )
             url = self.config.get(Constants.URL)
-            if (
-                self.config.get(Constants.API_KEY) is not None
-                or self.config.get(Constants.API_KEY) == ""
-            ):
-                self.client = QdrantClient(
-                    url=url, api_key=self.config.get(Constants.API_KEY)
-                )
-                vector_db = QdrantVectorStore(
-                    collection_name=self.collection_name,
-                    client=self.client,
-                    api_key=self.config.get(Constants.API_KEY),
-                )
+            api_key: Optional[str] = self.config.get(Constants.API_KEY, None)
+            if api_key:
+                self.client = QdrantClient(url=url, api_key=api_key)
             else:
                 self.client = QdrantClient(url=url)
-                vector_db = QdrantVectorStore(
-                    collection_name=self.collection_name, client=self.client
-                )
+            vector_db: BasePydanticVectorStore = QdrantVectorStore(
+                collection_name=self.collection_name,
+                client=self.client,
+                url=url,
+                api_key=api_key,
+            )
             return vector_db
         except Exception as e:
             raise AdapterError(str(e))
 
     def test_connection(self) -> bool:
         vector_db = self.get_vector_db_instance()
         test_result: bool = VectorDBHelper.test_vector_db_instance(
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/register.py` & `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/samples/sample1.txt` & `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/samples/sample1.txt`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/supabase/src/supabase.py` & `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/supabase/src/supabase.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from typing import Any, Optional
 
-from llama_index.vector_stores import SupabaseVectorStore
-from llama_index.vector_stores.types import VectorStore
+from llama_index.core.vector_stores.types import VectorStore
+from llama_index.vector_stores.supabase import SupabaseVectorStore
 from vecs import Client
 
 from unstract.adapters.exceptions import AdapterError
 from unstract.adapters.vectordb.constants import VectorDbConstants
 from unstract.adapters.vectordb.helper import VectorDBHelper
 from unstract.adapters.vectordb.vectordb_adapter import VectorDBAdapter
 
@@ -37,27 +37,24 @@
 
     @staticmethod
     def get_description() -> str:
         return "Supabase VectorDB"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/supabase.png"
-        )
+        return "/icons/adapter-icons/supabase.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_vector_db_instance(self) -> Optional[VectorStore]:
+    def get_vector_db_instance(self) -> VectorStore:
         try:
             self.collection_name = VectorDBHelper.get_collection_name(
                 self.config.get(VectorDbConstants.VECTOR_DB_NAME),
                 self.config.get(
                     VectorDbConstants.EMBEDDING_DIMENSION,
                     VectorDbConstants.DEFAULT_EMBEDDING_SIZE,
                 ),
@@ -71,28 +68,29 @@
             postgres_connection_string = (
                 f"postgresql://{user}:{password}@{host}:{port}/{db_name}"
             )
             dimension = self.config.get(
                 VectorDbConstants.EMBEDDING_DIMENSION,
                 VectorDbConstants.DEFAULT_EMBEDDING_SIZE,
             )
-            vector_db = SupabaseVectorStore(
+            vector_db: VectorStore = SupabaseVectorStore(
                 postgres_connection_string=postgres_connection_string,
                 collection_name=self.collection_name,
                 dimension=dimension,
             )
-            self.client = vector_db.client
+            if vector_db is not None:
+                self.client = vector_db.client
             return vector_db
         except Exception as e:
             raise AdapterError(str(e))
 
     def test_connection(self) -> bool:
-        self.config[
-            VectorDbConstants.EMBEDDING_DIMENSION
-        ] = VectorDbConstants.TEST_CONNECTION_EMBEDDING_SIZE
+        self.config[VectorDbConstants.EMBEDDING_DIMENSION] = (
+            VectorDbConstants.TEST_CONNECTION_EMBEDDING_SIZE
+        )
         vector_db = self.get_vector_db_instance()
         test_result: bool = VectorDBHelper.test_vector_db_instance(
             vector_store=vector_db
         )
         # Delete the collection that was created for testing
         if self.client is not None:
             self.client.delete_collection(self.collection_name)
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/vectordb_adapter.py` & `unstract_adapters-0.9.0/src/unstract/adapters/x2text/x2text_adapter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from abc import ABC
-from typing import Any, Union
+from typing import Any, Optional
 
-from llama_index.vector_stores.types import BasePydanticVectorStore, VectorStore
 from unstract.adapters.base import Adapter
 from unstract.adapters.enums import AdapterTypes
 
 
-class VectorDBAdapter(Adapter, ABC):
+class X2TextAdapter(Adapter, ABC):
     def __init__(self, name: str):
         super().__init__(name)
         self.name = name
 
     @staticmethod
     def get_id() -> str:
         return ""
@@ -29,13 +28,20 @@
 
     @staticmethod
     def get_json_schema() -> str:
         return ""
 
     @staticmethod
     def get_adapter_type() -> AdapterTypes:
-        return AdapterTypes.VECTOR_DB
+        return AdapterTypes.X2TEXT
 
-    def get_vector_db_instance(
-        self, vector_db_config: dict[str, Any]
-    ) -> Union[BasePydanticVectorStore, VectorStore, None]:
-        return None
+    def test_connection(self) -> bool:
+        return False
+
+    def process(
+        self,
+        input_file_path: str,
+        output_file_path: Optional[str] = None,
+        **kwargs: dict[Any, Any],
+    ) -> str:
+        # Overriding methods will have the actual implementation
+        return ""
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/weaviate/src/weaviate.py` & `unstract_adapters-0.9.0/src/unstract/adapters/vectordb/weaviate/src/weaviate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 import os
 from typing import Any, Optional
 
 import weaviate
-from llama_index.vector_stores import WeaviateVectorStore
-from llama_index.vector_stores.types import BasePydanticVectorStore
+from llama_index.core.vector_stores.types import BasePydanticVectorStore
+from llama_index.vector_stores.weaviate import WeaviateVectorStore
+from weaviate import UnexpectedStatusCodeException
+
 from unstract.adapters.exceptions import AdapterError
 from unstract.adapters.vectordb.constants import VectorDbConstants
 from unstract.adapters.vectordb.helper import VectorDBHelper
 from unstract.adapters.vectordb.vectordb_adapter import VectorDBAdapter
-from weaviate import UnexpectedStatusCodeException
 
 logger = logging.getLogger(__name__)
 
 
 class Constants:
     URL = "url"
     API_KEY = "api_key"
@@ -36,27 +37,24 @@
 
     @staticmethod
     def get_description() -> str:
         return "Weaviate VectorDB"
 
     @staticmethod
     def get_icon() -> str:
-        return (
-            "/icons/"
-            "adapter-icons/Weaviate.png"
-        )
+        return "/icons/adapter-icons/Weaviate.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
 
-    def get_vector_db_instance(self) -> Optional[BasePydanticVectorStore]:
+    def get_vector_db_instance(self) -> BasePydanticVectorStore:
         try:
             collection_name = VectorDBHelper.get_collection_name(
                 self.config.get(VectorDbConstants.VECTOR_DB_NAME),
                 self.config.get(VectorDbConstants.EMBEDDING_DIMENSION),
             )
             # Capitalise the frst letter as Weaviate expects this
             # LLama-index throws the error if not capitalised while using
@@ -80,26 +78,26 @@
                 self.client.schema.create_class(class_obj)
             except Exception as e:
                 if isinstance(e, UnexpectedStatusCodeException):
                     if "already exists" in e.message:
                         logger.warning(f"Collection already exists: {e}")
                 else:
                     raise e
-            vector_db = WeaviateVectorStore(
+            vector_db: BasePydanticVectorStore = WeaviateVectorStore(
                 weaviate_client=self.client,
                 index_name=self.collection_name,
             )
             return vector_db
         except Exception as e:
             raise AdapterError(str(e))
 
     def test_connection(self) -> bool:
-        self.config[
-            VectorDbConstants.EMBEDDING_DIMENSION
-        ] = VectorDbConstants.TEST_CONNECTION_EMBEDDING_SIZE
+        self.config[VectorDbConstants.EMBEDDING_DIMENSION] = (
+            VectorDbConstants.TEST_CONNECTION_EMBEDDING_SIZE
+        )
         vector_db = self.get_vector_db_instance()
         test_result: bool = VectorDBHelper.test_vector_db_instance(
             vector_store=vector_db
         )
         # Delete the collection that was created for testing
         if self.client is not None:
             self.client.schema.delete_class(self.collection_name)
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/x2text/helper.py` & `unstract_adapters-0.9.0/src/unstract/adapters/x2text/helper.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/src/constants.py` & `unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/src/constants.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py` & `unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     @staticmethod
     def get_description() -> str:
         return "LLMWhisperer X2Text"
 
     @staticmethod
     def get_icon() -> str:
-        return "/icons/" "adapter-icons/LLMWhisperer.png"
+        return "/icons/adapter-icons/LLMWhisperer.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/x2text/register.py` & `unstract_adapters-0.9.0/src/unstract/adapters/x2text/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py` & `unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     @staticmethod
     def get_description() -> str:
         return "Unstructured IO Community X2Text"
 
     @staticmethod
     def get_icon() -> str:
-        return "/icons/" "adapter-icons/UnstructuredIO.png"
+        return "/icons/adapter-icons/UnstructuredIO.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
```

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json` & `unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py` & `unstract_adapters-0.9.0/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     @staticmethod
     def get_description() -> str:
         return "Unstructured IO Enterprise X2Text"
 
     @staticmethod
     def get_icon() -> str:
-        return "/icons/" "adapter-icons/UnstructuredIO.png"
+        return "/icons/adapter-icons/UnstructuredIO.png"
 
     @staticmethod
     def get_json_schema() -> str:
         f = open(f"{os.path.dirname(__file__)}/static/json_schema.json")
         schema = f.read()
         f.close()
         return schema
```

### Comparing `unstract_adapters-0.8.1/PKG-INFO` & `unstract_adapters-0.9.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstract-adapters
-Version: 0.8.1
+Version: 0.9.0
 Summary: Unstract interface for LLMs, Embeddings and VectorDBs
 Author-Email: Zipstack Inc. <devsupport@zipstack.com>
 License: AGPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
@@ -13,85 +13,47 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Homepage, https://unstract.com
 Project-URL: Release notes, https://github.com/Zipstack/unstract-adapters/releases
 Project-URL: Source, https://github.com/Zipstack/unstract-adapters
 Requires-Python: <3.12,>=3.9
-Requires-Dist: llama-index==0.9.28
-Requires-Dist: requests>=2.31.0
-Requires-Dist: openai==1.3.9
-Requires-Dist: google-generativeai==0.3.1
-Requires-Dist: google-cloud-aiplatform==1.40.0
-Requires-Dist: fastembed==0.1.3
-Requires-Dist: huggingface==0.0.1
-Requires-Dist: pymilvus==2.3.4
-Requires-Dist: vecs==0.4.3
-Requires-Dist: pinecone-client==2.2.4
-Requires-Dist: psycopg2-binary==2.9.9
-Requires-Dist: qdrant-client~=1.8.0
-Requires-Dist: supabase==2.2.1
-Requires-Dist: weaviate-client==3.25.3
-Requires-Dist: asyncpg==0.29.0
-Requires-Dist: SQLAlchemy==2.0.26
-Requires-Dist: anthropic==0.7.8
-Requires-Dist: replicate==0.22.0
-Requires-Dist: anyscale==0.5.165
-Requires-Dist: mistralai==0.0.8
+Requires-Dist: llama-index==0.10.28
+Requires-Dist: llama-index-embeddings-google==0.1.4
+Requires-Dist: llama-index-embeddings-azure-openai==0.1.6
+Requires-Dist: llama-index-embeddings-azure-openai==0.1.6
+Requires-Dist: llama-index-vector-stores-postgres==0.1.3
+Requires-Dist: llama-index-vector-stores-milvus==0.1.6
+Requires-Dist: llama-index-vector-stores-weaviate==0.1.4
+Requires-Dist: llama-index-vector-stores-pinecone==0.1.4
+Requires-Dist: llama-index-vector-stores-qdrant==0.1.4
+Requires-Dist: llama-index-llms-palm==0.1.4
+Requires-Dist: llama-index-llms-mistralai==0.1.10
+Requires-Dist: llama-index-llms-anyscale==0.1.3
+Requires-Dist: llama-index-llms-anthropic==0.1.5
+Requires-Dist: llama-index-llms-azure-openai==0.1.5
+Requires-Dist: llama-index-llms-vertex==0.1.5
+Requires-Dist: llama-index-llms-replicate==0.1.3
 Requires-Dist: filetype~=1.2.0
+Requires-Dist: singleton-decorator~=1.0.0
 Description-Content-Type: text/markdown
 
 <div align="center">
 <img src="docs/assets/unstract_u_logo.png" style="height: 120px">
 
 # Unstract
 
 ## No-code LLM Platform to launch APIs and ETL Pipelines to structure unstructured documents
 
 </div>
 
 # Unstract Adapters
 
 This is Unstract's python package which helps to configure to a number of different LLMs, Embeddings and VectorDBs.
-
-## LLMs
-The following LLMs are supported:
-
-| LLM          | Version |
-|--------------|---------|
-| OpenAI       | 1.3.9   |
-| Azure OpenAI | 1.3.9   |
-| Anthropic    | 0.7.8   |
-| PaLM         | 0.3.1   |
-| Replicate    | 0.22.0  |
-| AnyScale     | 0.5.165 |
-| Mistral      | 0.0.8   |
-
-## Embeddings
-The following Embeddings are supported:
-
-| Embedding   | Version |
-|-------------|---------|
-| OpenAI      |   1.3.9      |
-| Azure OpenAI |    1.3.9     |
-| Qdrant FastEmbed   |    0.1.3     |
-| HuggingFace        |    0.0.1     |
-| PaLM    |    0.3.1     |
-
-## VectorDBs
-The following VectorDBs are supported:
-
-| Vector DB        | Version |
-|------------------|--------|
-| Milvus           |   2.3.4     |
-| Pinecone    |    2.2.4    |
-| Postgres |    0.2.4    |
-| Qdrant      |    1.7.0    |
-| Supabase             |    2.2.1     |
-| Weaviate             |    3.25.3    |
+For further details on the list of supported LLMs, Embeddings and Vector DBs,, please visit https://github.com/Zipstack/unstract
 
 ## Installation
 
 ### Local Development
 
 To get started with local development, 
 - Create and source a virtual environment if you haven't already following [these steps](/README.md#create-your-virtual-env).
```

