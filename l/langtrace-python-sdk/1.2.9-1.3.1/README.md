# Comparing `tmp/langtrace_python_sdk-1.2.9.tar.gz` & `tmp/langtrace_python_sdk-1.3.1.tar.gz`

## Comparing `langtrace_python_sdk-1.2.9.tar` & `langtrace_python_sdk-1.3.1.tar`

### file list

```diff
@@ -1,72 +1,86 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/run_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/anthropic_example/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/anthropic_example/completion.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/chroma_example/__init__.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/chroma_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/langchain_example/__init__.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/langchain_example/basic.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/langchain_example/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/llamaindex_example/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/llamaindex_example/basic.py
--rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/llamaindex_example/data/abramov.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/openai/__init__.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/openai/chat_completion.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/openai/embeddings_create.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/openai/function_calling.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/openai/images_generate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/pinecone_example/__init__.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/pinecone_example/basic.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/__init__.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/langtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/__init__.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/chroma.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/common.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/openai.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/extensions/__init__.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/extensions/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0     7115 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/chroma/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/openai/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/utils/llm.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/utils/with_root_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/tests/__init__.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/tests/utils.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/tests/chroma/test_chroma.py
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/tests/openai/test_chat_completion.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/tests/openai/test_image_generation.py
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/tests/pinecone/test_pinecone.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/LICENSE
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/README.md
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/pyproject.toml
--rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/__init__.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/run_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/anthropic_example/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/anthropic_example/completion.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/chroma_example/__init__.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/chroma_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/cohere_example/__init__.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/cohere_example/chat.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/cohere_example/chat_stream.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/cohere_example/embed_create.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/fastapi_example/basic_route.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/langchain_example/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/langchain_example/basic.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/langchain_example/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/llamaindex_example/__init__.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/llamaindex_example/basic.py
+-rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/llamaindex_example/data/abramov.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/openai/__init__.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/openai/chat_completion.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/openai/embeddings_create.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/openai/function_calling.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/openai/images_generate.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/perplexity_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/pinecone_example/__init__.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/pinecone_example/basic.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/__init__.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/langtrace.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/chroma.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/cohere.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/common.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/openai.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/extensions/__init__.py
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/extensions/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/chroma/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/cohere/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0    15463 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/openai/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/utils/llm.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/utils/with_root_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/__init__.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/utils.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/anthropic/test_anthropic.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/chroma/test_chroma.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/langchain/test_langchain.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/langchain/test_langchain_community.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/langchain/test_langchain_core.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/openai/test_chat_completion.py
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/openai/test_image_generation.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/pinecone/test_pinecone.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/LICENSE
+-rw-r--r--   0        0        0     8044 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/README.md
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/PKG-INFO
```

### Comparing `langtrace_python_sdk-1.2.9/src/examples/anthropic_example/completion.py` & `langtrace_python_sdk-1.3.1/src/examples/anthropic_example/completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/examples/chroma_example/basic.py` & `langtrace_python_sdk-1.3.1/src/examples/chroma_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/examples/langchain_example/basic.py` & `langtrace_python_sdk-1.3.1/src/examples/langchain_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/examples/langchain_example/tool.py` & `langtrace_python_sdk-1.3.1/src/examples/langchain_example/tool.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/examples/llamaindex_example/basic.py` & `langtrace_python_sdk-1.3.1/src/examples/llamaindex_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/examples/llamaindex_example/data/abramov.txt` & `langtrace_python_sdk-1.3.1/src/examples/llamaindex_example/data/abramov.txt`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/examples/openai/chat_completion.py` & `langtrace_python_sdk-1.3.1/src/examples/openai/chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/examples/openai/embeddings_create.py` & `langtrace_python_sdk-1.3.1/src/examples/openai/embeddings_create.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/examples/openai/function_calling.py` & `langtrace_python_sdk-1.3.1/src/examples/openai/function_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/examples/pinecone_example/basic.py` & `langtrace_python_sdk-1.3.1/src/examples/pinecone_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/langtrace.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/langtrace.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+from typing import Optional
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import (
     BatchSpanProcessor,
     ConsoleSpanExporter,
     SimpleSpanProcessor,
 )
@@ -28,28 +28,31 @@
 )
 from langtrace_python_sdk.instrumentation.openai.instrumentation import (
     OpenAIInstrumentation,
 )
 from langtrace_python_sdk.instrumentation.pinecone.instrumentation import (
     PineconeInstrumentation,
 )
+from langtrace_python_sdk.instrumentation.cohere.instrumentation import (
+    CohereInstrumentation,
+)
 
 
 def init(
     api_key: str = None,
     batch: bool = True,
     write_to_langtrace_cloud: bool = True,
     debug_log_to_console: bool = False,
     custom_remote_exporter=None,
+    api_host: Optional[str] = None,
 ):
-
     provider = TracerProvider()
 
     remote_write_exporter = (
-        LangTraceExporter(api_key, write_to_langtrace_cloud)
+        LangTraceExporter(api_key, write_to_langtrace_cloud, api_host=api_host)
         if custom_remote_exporter is None
         else custom_remote_exporter
     )
     console_exporter = ConsoleSpanExporter()
     batch_processor_remote = BatchSpanProcessor(remote_write_exporter)
     batch_processor_console = BatchSpanProcessor(console_exporter)
     simple_processor_console = SimpleSpanProcessor(console_exporter)
@@ -73,17 +76,19 @@
     pinecone_instrumentation = PineconeInstrumentation()
     llamaindex_instrumentation = LlamaindexInstrumentation()
     chroma_instrumentation = ChromaInstrumentation()
     langchain_instrumentation = LangchainInstrumentation()
     langchain_core_instrumentation = LangchainCoreInstrumentation()
     langchain_community_instrumentation = LangchainCommunityInstrumentation()
     anthropic_instrumentation = AnthropicInstrumentation()
+    cohere_instrumentation = CohereInstrumentation()
 
     # Call the instrument method with some arguments
     openai_instrumentation.instrument()
     pinecone_instrumentation.instrument()
     llamaindex_instrumentation.instrument()
     chroma_instrumentation.instrument()
     langchain_instrumentation.instrument()
     langchain_core_instrumentation.instrument()
     langchain_community_instrumentation.instrument()
     anthropic_instrumentation.instrument()
+    cohere_instrumentation.instrument()
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/chroma.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/common.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,10 +12,12 @@
     "CHROMA": "Chroma",
     "LANGCHAIN": "Langchain",
     "LANGCHAIN_COMMUNITY": "Langchain Community",
     "LANGCHAIN_CORE": "Langchain Core",
     "LLAMAINDEX": "LlamaIndex",
     "OPENAI": "OpenAI",
     "PINECONE": "Pinecone",
+    "COHERE": "Cohere",
+    "PPLX": "Perplexity",
 }
 
 LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY = "langtrace_additional_attributes"
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/openai.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/extensions/langtrace_exporter.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/extensions/langtrace_exporter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import json
 import os
 import typing
 
-from langtrace_python_sdk.constants.exporter.langtrace_exporter import (
-    LANGTRACE_REMOTE_URL,
-)
 import requests
 from opentelemetry.sdk.trace.export import ReadableSpan, SpanExporter, SpanExportResult
 from opentelemetry.trace.span import format_trace_id
 
+from langtrace_python_sdk.constants.exporter.langtrace_exporter import LANGTRACE_REMOTE_URL
+
 
 class LangTraceExporter(SpanExporter):
     """
     **LangTraceExporter Class**
 
     This class exports telemetry data in the LangTrace format to a remote URL. It inherits from the `SpanExporter` class in OpenTelemetry.
 
@@ -45,32 +44,32 @@
 
     * `ValueError`: If the API key is not provided or the URL is missing when `write_to_remote_url` is True.
     """
 
     api_key: str
     write_to_remote_url: bool
 
-    def __init__(self, api_key: str = None, write_to_remote_url: bool = False) -> None:
-        self.api_key = api_key if api_key else os.environ.get("LANGTRACE_API_KEY")
+    def __init__(self, api_key: str = None, write_to_remote_url: bool = False, api_host: typing.Optional[str] = None) -> None:
+        self.api_key = api_key or os.environ.get("LANGTRACE_API_KEY")
         self.write_to_remote_url = write_to_remote_url
+        self.api_host: str = api_host or LANGTRACE_REMOTE_URL
 
         if self.write_to_remote_url and not self.api_key:
             raise ValueError("No API key provided")
 
     def export(self, spans: typing.Sequence[ReadableSpan]) -> SpanExportResult:
         """
         Exports a batch of telemetry data.
 
         Args:
             spans: The list of `opentelemetry.trace.Span` objects to be exported
 
         Returns:
             The result of the export SUCCESS or FAILURE
         """
-
         data = [
             {
                 "traceId": format_trace_id(span.get_span_context().trace_id),
                 "instrumentationLibrary": span.instrumentation_info.__repr__(),
                 "droppedEventsCount": span.dropped_events,
                 "droppedAttributesCount": span.dropped_attributes,
                 "droppedLinksCount": span.dropped_links,
@@ -82,19 +81,17 @@
 
         if not self.write_to_remote_url:
             return
 
         # Send data to remote URL
         try:
             requests.post(
-                url=LANGTRACE_REMOTE_URL,
+                url=f"{self.api_host}/api/trace",
                 data=json.dumps(data),
                 headers={"Content-Type": "application/json", "x-api-key": self.api_key},
             )
-            print(f"Traces sent To {LANGTRACE_REMOTE_URL}")
             return SpanExportResult.SUCCESS
         except Exception as e:
-            print("Error sending data to remote URL", e)
             return SpanExportResult.FAILURE
 
     def shutdown(self) -> None:
         pass
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
 from langtrace_python_sdk.instrumentation.anthropic.patch import messages_create
 
+import logging
+
+logging.basicConfig(level=logging.FATAL)
+
 
 class AnthropicInstrumentation(BaseInstrumentor):
     """
     The AnthropicInstrumentation class represents the Anthropic instrumentation
     """
 
     def instrumentation_dependencies(self) -> Collection[str]:
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/anthropic/patch.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/anthropic/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         if system:
             prompts = json.dumps(
                 [{"role": "system", "content": system}] + kwargs.get("messages", [])
             )
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": base_url,
             "llm.api": APIS["MESSAGES_CREATE"]["ENDPOINT"],
             "llm.model": kwargs.get("model"),
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
 from langtrace_python_sdk.constants.instrumentation.chroma import APIS
 from langtrace_python_sdk.instrumentation.chroma.patch import collection_patch
+import logging
+
+logging.basicConfig(level=logging.FATAL)
 
 
 class ChromaInstrumentation(BaseInstrumentor):
     """
     The ChromaInstrumentation class represents the ChromaDB instrumentation
     """
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/chroma/patch.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/chroma/patch.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
     def traced_method(wrapped, instance, args, kwargs):
         api = APIS[method]
         service_provider = SERVICE_PROVIDERS["CHROMA"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "vectordb",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "db.system": "chromadb",
             "db.operation": api["OPERATION"],
             **(extra_attributes if extra_attributes is not None else {})
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
 from langtrace_python_sdk.instrumentation.langchain.patch import generic_patch
 
+import logging
+
+logging.basicConfig(level=logging.FATAL)
+
 
 def patch_module_classes(
     module_name, tracer, version, task, trace_output=True, trace_input=True
 ):
     """
     Generic function to patch all public methods of all classes in a given module.
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain/patch.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain/patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     """
 
     def traced_method(wrapped, instance, args, kwargs):
         service_provider = SERVICE_PROVIDERS["LANGCHAIN"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "langchain.task.name": task,
             **(extra_attributes if extra_attributes is not None else {})
         }
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     method_name, task, tracer, version, trace_output=True, trace_input=True
 ):
     def traced_method(wrapped, instance, args, kwargs):
         service_provider = SERVICE_PROVIDERS["LANGCHAIN_COMMUNITY"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "langchain.task.name": task,
             **(extra_attributes if extra_attributes is not None else {})
         }
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     """
 
     def traced_method(wrapped, instance, args, kwargs):
         service_provider = SERVICE_PROVIDERS["LANGCHAIN_CORE"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "langchain.task.name": task,
             **(extra_attributes if extra_attributes is not None else {})
         }
@@ -92,14 +93,15 @@
     trace_output: Whether to trace the output of the patched methods.
     trace_input: Whether to trace the input of the patched methods.
     """
 
     def traced_method(wrapped, instance, args, kwargs):
         service_provider = SERVICE_PROVIDERS["LANGCHAIN_CORE"]
         span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "langchain.task.name": task,
         }
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
 from langtrace_python_sdk.instrumentation.llamaindex.patch import generic_patch
 
+import logging
+
+logging.basicConfig(level=logging.FATAL)
+
 
 class LlamaindexInstrumentation(BaseInstrumentor):
     """
     The LlamaindexInstrumentation class represents the LlamaIndex instrumentation
     """
 
     def instrumentation_dependencies(self) -> Collection[str]:
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     A generic patch method that wraps a function with a span"""
 
     def traced_method(wrapped, instance, args, kwargs):
         service_provider = SERVICE_PROVIDERS["LLAMAINDEX"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "llamaindex.task.name": task,
             **(extra_attributes if extra_attributes is not None else {})
         }
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 import importlib.metadata
 from typing import Collection
 
-import openai
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
 from langtrace_python_sdk.instrumentation.openai.patch import (
     chat_completions_create,
     embeddings_create,
     images_generate,
 )
 
+import logging
+
+logging.basicConfig(level=logging.FATAL)
+
 
 class OpenAIInstrumentation(BaseInstrumentor):
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return ["openai >= 0.27.0"]
 
     def _instrument(self, **kwargs):
         tracer_provider = kwargs.get("tracer_provider")
         tracer = get_tracer(__name__, "", tracer_provider)
         version = importlib.metadata.version("openai")
         wrap_function_wrapper(
             "openai.resources.chat.completions",
             "Completions.create",
-            chat_completions_create(openai.chat.completions.create, version, tracer),
+            chat_completions_create("openai.chat.completions.create", version, tracer),
         )
         wrap_function_wrapper(
             "openai.resources.images",
             "Images.generate",
-            images_generate(openai.images.generate, version, tracer),
+            images_generate("openai.images.generate", version, tracer),
         )
         wrap_function_wrapper(
             "openai.resources.embeddings",
             "Embeddings.create",
-            embeddings_create(openai.embeddings.create, version, tracer),
+            embeddings_create("openai.embeddings.create", version, tracer),
         )
 
     def _uninstrument(self, **kwargs):
         pass
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/openai/patch.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/openai/patch.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             if hasattr(instance, "_client") and hasattr(instance._client, "_base_url")
             else ""
         )
         service_provider = SERVICE_PROVIDERS["OPENAI"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": base_url,
             "llm.api": APIS["IMAGES_GENERATION"]["ENDPOINT"],
             "llm.model": kwargs.get("model"),
@@ -48,15 +49,15 @@
             APIS["IMAGES_GENERATION"]["METHOD"], kind=SpanKind.CLIENT
         ) as span:
             for field, value in attributes.model_dump(by_alias=True).items():
                 if value is not None:
                     span.set_attribute(field, value)
             try:
                 # Attempt to call the original method
-                result = original_method(*args, **kwargs)
+                result = wrapped(*args, **kwargs)
                 if kwargs.get("stream") is False or kwargs.get("stream") is None:
                     data = (
                         result.data[0]
                         if hasattr(result, "data") and len(result.data) > 0
                         else {}
                     )
                     response = [
@@ -92,17 +93,24 @@
     def traced_method(wrapped, instance, args, kwargs):
         base_url = (
             str(instance._client._base_url)
             if hasattr(instance, "_client") and hasattr(instance._client, "_base_url")
             else ""
         )
         service_provider = SERVICE_PROVIDERS["OPENAI"]
+        # If base url contains perplexity or azure, set the service provider accordingly
+        if "perplexity" in base_url:
+            service_provider = SERVICE_PROVIDERS["PPLX"]
+        elif "azure" in base_url:
+            service_provider = SERVICE_PROVIDERS["AZURE"]
+
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": base_url,
             "llm.api": APIS["CHAT_COMPLETION"]["ENDPOINT"],
             "llm.prompts": json.dumps(kwargs.get("messages", [])),
@@ -128,16 +136,16 @@
             APIS["CHAT_COMPLETION"]["METHOD"], kind=SpanKind.CLIENT
         )
         for field, value in attributes.model_dump(by_alias=True).items():
             if value is not None:
                 span.set_attribute(field, value)
         try:
             # Attempt to call the original method
-            result = original_method(*args, **kwargs)
-            if kwargs.get("stream") is False:
+            result = wrapped(*args, **kwargs)
+            if kwargs.get("stream") is False or kwargs.get("stream") is None:
                 span.set_attribute("llm.model", result.model)
                 if hasattr(result, "choices") and result.choices is not None:
                     responses = [
                         {
                             "message": {
                                 "role": (
                                     choice.message.role
@@ -188,39 +196,50 @@
                             "total_tokens": usage.total_tokens,
                         }
                         span.set_attribute("llm.token.counts", json.dumps(usage_dict))
                 span.set_status(StatusCode.OK)
                 span.end()
                 return result
             else:
-                prompt_tokens = calculate_prompt_tokens(
-                    json.dumps(kwargs.get("messages", {})[0]), kwargs.get("model")
-                )
+                # iterate over kwargs.get("messages", {}) and calculate the prompt tokens
+                prompt_tokens = 0
+                for message in kwargs.get("messages", {}):
+                    prompt_tokens += calculate_prompt_tokens(
+                        json.dumps(message), kwargs.get("model")
+                    )
+
+                # iterate over kwargs.get("functions") and calculate the prompt tokens
+                if kwargs.get("functions") is not None:
+                    for function in kwargs.get("functions"):
+                        prompt_tokens += calculate_prompt_tokens(
+                            json.dumps(function), kwargs.get("model")
+                        )
+
                 return handle_streaming_response(
                     result,
                     span,
                     prompt_tokens,
                     function_call=kwargs.get("functions") is not None,
                 )
-        except Exception as e:
-            # Record the exception in the span
-            span.record_exception(e)
-            # Set the span status to indicate an error
-            span.set_status(Status(StatusCode.ERROR, str(e)))
-            # Reraise the exception to ensure it's not swallowed
+
+        except Exception as error:
+            span.record_exception(error)
+            span.set_status(Status(StatusCode.ERROR, str(error)))
             span.end()
             raise
 
     def handle_streaming_response(result, span, prompt_tokens, function_call=False):
         """Process and yield streaming response chunks."""
         result_content = []
         span.add_event(Event.STREAM_START.value)
         completion_tokens = 0
         try:
             for chunk in result:
+                if hasattr(chunk, "model") and chunk.model is not None:
+                    span.set_attribute("llm.model", chunk.model)
                 if hasattr(chunk, "choices") and chunk.choices is not None:
                     token_counts = [
                         (
                             estimate_tokens(choice.delta.content)
                             if choice.delta and choice.delta.content
                             else (
                                 estimate_tokens(choice.delta.function_call.arguments)
@@ -262,38 +281,27 @@
                     {
                         "input_tokens": prompt_tokens,
                         "output_tokens": completion_tokens,
                         "total_tokens": prompt_tokens + completion_tokens,
                     }
                 ),
             )
-            if function_call is False:
-                span.set_attribute(
-                    "llm.responses",
-                    json.dumps(
+            span.set_attribute(
+                "llm.responses",
+                json.dumps(
+                    [
                         {
                             "message": {
                                 "role": "assistant",
                                 "content": "".join(result_content),
                             }
                         }
-                    ),
-                )
-            else:
-                span.set_attribute(
-                    "llm.responses",
-                    json.dumps(
-                        {
-                            "message": {
-                                "role": "assistant",
-                                "function_call": "".join(result_content),
-                            }
-                        }
-                    ),
-                )
+                    ]
+                ),
+            )
             span.set_status(StatusCode.OK)
             span.end()
 
     # return the wrapped method
     return traced_method
 
 
@@ -309,14 +317,15 @@
             else ""
         )
 
         service_provider = SERVICE_PROVIDERS["OPENAI"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": base_url,
             "llm.api": APIS["EMBEDDINGS_CREATE"]["ENDPOINT"],
             "llm.model": kwargs.get("model"),
@@ -334,22 +343,20 @@
         if kwargs.get("user") is not None:
             attributes["llm.user"] = kwargs.get("user")
 
         with tracer.start_as_current_span(
             APIS["EMBEDDINGS_CREATE"]["METHOD"], kind=SpanKind.CLIENT
         ) as span:
 
-            print("Inside embeddings_create", trace.get_current_span())
-
             for field, value in attributes.model_dump(by_alias=True).items():
                 if value is not None:
                     span.set_attribute(field, value)
             try:
                 # Attempt to call the original method
-                result = original_method(*args, **kwargs)
+                result = wrapped(*args, **kwargs)
                 span.set_status(StatusCode.OK)
                 return result
             except Exception as e:
                 # Record the exception in the span
                 span.record_exception(e)
 
                 # Set the span status to indicate an error
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
 from langtrace_python_sdk.constants.instrumentation.pinecone import APIS
 from langtrace_python_sdk.instrumentation.pinecone.patch import generic_patch
 
+import logging
+
+logging.basicConfig(level=logging.FATAL)
+
 
 class PineconeInstrumentation(BaseInstrumentor):
     """
     The PineconeInstrumentation class represents the Pinecone instrumentation"""
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return ["pinecone-client >= 3.1.0"]
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/pinecone/patch.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/pinecone/patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     def traced_method(wrapped, instance, args, kwargs):
         api = APIS[method]
         service_provider = SERVICE_PROVIDERS["PINECONE"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "vectordb",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "db.system": "pinecone",
             "db.operation": api["OPERATION"],
             **(extra_attributes if extra_attributes is not None else {})
```

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/utils/llm.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/utils/llm.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/utils/with_root_span.py` & `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/utils/with_root_span.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/src/tests/utils.py` & `langtrace_python_sdk-1.3.1/src/tests/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-import importlib.metadata
 from unittest.mock import MagicMock, patch
 import json
-
-def common_setup(data, method_to_mock):
-    service_mock = patch(method_to_mock)
-    mock_image_generate = service_mock.start()
-    mock_image_generate.return_value = json.dumps(data)
+   
+def common_setup(data, method_to_mock=None):
+    if method_to_mock:
+        service_mock = patch(method_to_mock)
+        mock_method = service_mock.start()
+        mock_method.return_value = json.dumps(data)
+    else:
+        service_mock = MagicMock()
+        service_mock.return_value = MagicMock(**data)
+       
 
     tracer = MagicMock()
     span = MagicMock()
 
     context_manager_mock = MagicMock()
     context_manager_mock.__enter__.return_value = span
     tracer.start_as_current_span.return_value = context_manager_mock
 
-    return service_mock, tracer, span
+    return service_mock, tracer, span
```

### Comparing `langtrace_python_sdk-1.2.9/src/tests/chroma/test_chroma.py` & `langtrace_python_sdk-1.3.1/src/tests/chroma/test_chroma.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,24 +35,30 @@
         self.assertEqual(result, "mocked method result")
 
         # Assert the span is started with the correct parameters
         self.assertTrue(self.tracer.start_as_current_span.called_once_with("chromadb.Collection.add", kind=SpanKind.CLIENT))
 
         # Verify span attributes are set as expected
         expected_attributes = {
+            'langtrace.sdk.name': 'langtrace-python-sdk',
             'langtrace.service.name': 'Chroma',
             'langtrace.service.type': 'vectordb',
             'langtrace.service.version': '1.2.3',
             'langtrace.version': '1.0.0',
             'db.system': 'chromadb',
             'db.operation': 'add',
             'db.collection.name': 'aa',
         }
         for key, value in expected_attributes.items():
             self.span.set_attribute.assert_has_calls([call(key, value)], any_order=True)
+
+        actual_calls = self.span.set_attribute.call_args_list
+
+        for key, value in expected_attributes.items():
+            self.assertIn(call(key, value), actual_calls)
         
         # Assert the span status is set to OK
         self.span.set_status.assert_called_with(StatusCode.OK)
         
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `langtrace_python_sdk-1.2.9/src/tests/openai/test_chat_completion.py` & `langtrace_python_sdk-1.3.1/src/tests/anthropic/test_anthropic.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,95 +1,73 @@
 import unittest
-from unittest.mock import MagicMock, Mock, patch, call
-from langtrace_python_sdk.instrumentation.openai.patch import chat_completions_create
+from unittest.mock import MagicMock, call
+from langtrace_python_sdk.instrumentation.anthropic.patch import messages_create
 from opentelemetry.trace import SpanKind
-from opentelemetry.trace import get_tracer
 import importlib.metadata
-import openai
-from langtrace_python_sdk.constants.instrumentation.openai import APIS
+from langtrace_python_sdk.constants.instrumentation.anthropic import APIS
 from opentelemetry.trace.status import Status, StatusCode
 import json
+from langtrace.trace_attributes import Event, LLMSpanAttributes
+
 from tests.utils import common_setup
-class TestChatCompletion(unittest.TestCase):
+
+class TestAnthropic(unittest.TestCase):
+
     data = {
-        "id": "chatcmpl-93wIW4A2r0YjlDvx7PKvHV0VxbprP",
-        "choices": [
-            {
-                "finish_reason": "stop",
-                "index": 0,
-                "logprobs": None,
-                "message": {
-                    "content": "This is a test, this is a test, this is a test.",
-                    "role": "assistant",
-                    "function_call": None,
-                    "tool_calls": None
-                }
-            }
-        ],
-        "created": 1710726108,
-        "model": "gpt-4-0613",
-        "object": "chat.completion",
-        "system_fingerprint": None,
-        "usage": {
-            "completion_tokens": 15,
-            "prompt_tokens": 14,
-            "total_tokens": 29
-        }
-    }
+        "content" : [MagicMock(text="Some text", type="text")],
+        "system_fingerprint" : "None",
+        "usage" : MagicMock(input_tokens=23, output_tokens=44),
+        "chunks" : [MagicMock(delta="Some text", message="text")]}
 
-    def setUp(self):
-        self.openai_mock, self.tracer, self.span = common_setup(self.data, 'openai.chat.completions.create')
 
+    def setUp(self):
+        
+        # Mock the original method
+        self.anthropic_mock, self.tracer, self.span = common_setup(self.data, None)
 
     def tearDown(self):
-        self.openai_mock.stop()
+        pass
 
-    def test_chat_completions_create_non_streaming(self):
+    def test_anthropic(self):
         # Arrange
-        version = importlib.metadata.version('openai')
-        llm_model_value = 'gpt-4'
-        messages_value = [{'role': 'user', 'content': 'Say this is a test three times'}]
-
+        version = importlib.metadata.version('anthropic')        
         kwargs = {
-            'model': llm_model_value,
-            'messages': messages_value,
-            'stream': False,
-        }
+            "model": "claude-3-opus-20240229",
+            "messages" : [{"role": "user", "content": "How are you today?"}],
+            "stream": False
+        }   
 
         # Act
-        wrapped_function = chat_completions_create(openai.chat.completions.create, version, self.tracer)
-        result = wrapped_function(MagicMock(), MagicMock(), (), kwargs)
+        wrapped_function = messages_create("anthropic.messages.create", version, self.tracer)
+        result = wrapped_function(self.anthropic_mock, MagicMock(), (), kwargs)
+        
 
         # Assert
-        self.assertTrue(self.tracer.start_as_current_span.called_once_with("openai.chat.completions.create", kind=SpanKind.CLIENT))
-
+        self.assertTrue(self.tracer.start_as_current_span.called_once_with("anthropic.messages.create", kind=SpanKind.CLIENT))
+        self.assertTrue(self.span.set_status.has_calls([call(Status(StatusCode.OK))]))
+        
         expected_attributes = {
-            "langtrace.service.name": "OpenAI",
+            "langtrace.sdk.name": "langtrace-python-sdk",
+            "langtrace.service.name": "Anthropic",
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
-            "url.full": "chat/completions/create",
-            "llm.api": APIS["CHAT_COMPLETION"]["ENDPOINT"],
-            "llm.model": kwargs.get('model'),
-            "llm.prompts": json.dumps(kwargs.get('messages', [])),
-            "llm.stream": kwargs.get('stream'),
+            "url.full": "/v1/messages",
+            "llm.api": APIS["MESSAGES_CREATE"]["ENDPOINT"],
+            "llm.model": kwargs.get("model"),
+            "llm.prompts": json.dumps(kwargs.get("messages", [])),
+            "llm.stream": kwargs.get("stream"),
         }
+
         self.assertTrue(
             self.span.set_attribute.has_calls(
                 [call(key, value) for key, value in expected_attributes.items()], any_order=True
             )
         )
+       
+        expected_result_data = {"system_fingerprint": "None"  }   
 
-        self.assertEqual(self.span.set_status.call_count, 1)
-        self.assertTrue(self.span.set_status.has_calls([call(Status(StatusCode.OK))]))
+        self.assertEqual(result.system_fingerprint, expected_result_data["system_fingerprint"])
 
-        expected_result = ['id', 'choices', 'created', 'model', 'system_fingerprint', 'object', 'usage']
-        result_keys = json.loads(result).keys()
-        self.assertSetEqual(set(expected_result), set(result_keys), "Keys mismatch")
-
-        expected_content = "This is a test, this is a test, this is a test."
-        self.assertEqual(
-            json.loads(result).get('choices')[0].get('message').get('content'), expected_content, "Content mismatch"
-        )
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `langtrace_python_sdk-1.2.9/src/tests/openai/test_image_generation.py` & `langtrace_python_sdk-1.3.1/src/tests/openai/test_image_generation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,70 @@
 import unittest
 from unittest.mock import MagicMock, Mock, patch, call
 from langtrace_python_sdk.instrumentation.openai.patch import images_generate
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace import get_tracer
+from opentelemetry import baggage
 import importlib.metadata
 import openai
 from langtrace_python_sdk.constants.instrumentation.openai import APIS
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 import json
 from tests.utils import common_setup
 
+
 class TestImageGeneration(unittest.TestCase):
     data = {
         "created": 1710983755,
         "data": [
             {
                 "b64_json": "null",
                 "revised_prompt": "A charming and adorable baby sea otter. This small, fluffy creature is floating gracefully on its back, with its tiny webbed paws folded cutely over its fuzzy belly. It has big, round, innocent eyes that are brimming with youthful curiosity. As it blissfully floats on the calm, sparkling ocean surface under the glow of the golden sunset, it playfully tosses a shiny seashell from one paw to another, showcasing its playful and distinctively otter-like behavior.",
                 "url": "https://images.openai.com/sea-otter.jpg"
             }
         ]
     }
 
     def setUp(self):
-        self.openai_mock, self.tracer, self.span = common_setup(self.data, 'openai.images.generate')
+        self.openai_mock, self.tracer, self.span = common_setup(self.data, "openai.images.generate")
 
 
     def tearDown(self):
         self.openai_mock.stop()
 
     def test_image_generation(self):
         # Arrange
         version = importlib.metadata.version('openai')
         llm_model_value = 'dall-e-3'
         prompt_value = "A cute baby sea otter"
         kwargs = {
             'model': llm_model_value,
             'prompt': prompt_value,
-            'stream': False        }
+            'stream': False } 
+
 
         # Act
         wrapped_function = images_generate(openai.images.generate, version, self.tracer)
         result = wrapped_function(MagicMock(), MagicMock(), (), kwargs)
 
         # Assert
         self.assertTrue(self.tracer.start_as_current_span.called_once_with("openai.images.generate", kind=SpanKind.CLIENT))
 
         expected_attributes = {
-            "langtrace.service.name": 'OpenAI',
+            'langtrace.sdk.name': 'langtrace-python-sdk',
+            "langtrace.service.name": "OpenAI",
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": 'https://api.openai.com/v1/',
             "llm.api": "images_generation_endpoint",  
             "llm.model": kwargs.get('model'),
             "llm.stream": kwargs.get('stream'),  
-            "llm.prompts": json.dumps([kwargs.get('prompt', [])])
+            "llm.prompts": json.dumps([kwargs.get('prompt', [])]),
         }
         self.assertTrue(self.span.set_attribute.has_calls([call(key, value) for key, value in expected_attributes.items()], any_order=True))
         self.assertTrue(self.span.set_status.called_once_with(Status(StatusCode.OK)))
 
         expected_result = ['created', 'data']
         result_keys = json.loads(result).keys()
         self.assertSetEqual(set(expected_result), set(result_keys), "Keys mismatch")
```

### Comparing `langtrace_python_sdk-1.2.9/src/tests/pinecone/test_pinecone.py` & `langtrace_python_sdk-1.3.1/src/tests/pinecone/test_pinecone.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,26 +38,33 @@
         result = wrapped_function(MagicMock(), MagicMock(), (vectors,), {})
 
         # Assert
         self.assertTrue(self.tracer.start_as_current_span.called_once_with("pinecone.data.index", kind=SpanKind.CLIENT))
         api = APIS[method]
         service_provider = SERVICE_PROVIDERS["PINECONE"]
         expected_attributes = {
+            'langtrace.sdk.name': 'langtrace-python-sdk',
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "vectordb",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "db.system": "pinecone",
             "db.operation": api["OPERATION"],
         }
         self.assertTrue(
             self.span.set_attribute.has_calls(
                 [call(key, value) for key, value in expected_attributes.items()], any_order=True
             )
         )      
+
+        actual_calls = self.span.set_attribute.call_args_list
+
+        for key, value in expected_attributes.items():
+            self.assertIn(call(key, value), actual_calls)
+            
         self.assertEqual(self.span.set_status.call_count, 1)
         self.assertTrue(self.span.set_status.has_calls([call(Status(StatusCode.OK))]))
 
         expected_result = ['status', 'message', 'upserted_ids']
         result_keys = json.loads(result).keys()
         self.assertSetEqual(set(expected_result), set(result_keys), "Keys mismatch")
```

### Comparing `langtrace_python_sdk-1.2.9/.gitignore` & `langtrace_python_sdk-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/LICENSE` & `langtrace_python_sdk-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.9/pyproject.toml` & `langtrace_python_sdk-1.3.1/pyproject.toml`

 * *Files identical despite different names*

