# Comparing `tmp/eidolon_ai_sdk-0.1.24.tar.gz` & `tmp/eidolon_ai_sdk-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_sdk-0.1.24.tar", max compression
+gzip compressed data, was "eidolon_ai_sdk-0.1.25.tar", max compression
```

## Comparing `eidolon_ai_sdk-0.1.24.tar` & `eidolon_ai_sdk-0.1.25.tar`

### file list

```diff
@@ -1,136 +1,136 @@
--rw-r--r--   0        0        0     2569 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/README.md
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/__init__.py
--rw-r--r--   0        0        0     2415 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/agent.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/__init__.py
--rw-r--r--   0        0        0     4645 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/document_manager.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
--rw-r--r--   0        0        0      971 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
--rw-r--r--   0        0        0     3405 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
--rw-r--r--   0        0        0     4173 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
--rw-r--r--   0        0        0     2805 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
--rw-r--r--   0        0        0     4510 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
--rw-r--r--   0        0        0      448 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
--rw-r--r--   0        0        0     3699 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
--rw-r--r--   0        0        0     2053 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
--rw-r--r--   0        0        0     3212 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
--rw-r--r--   0        0        0     1647 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
--rw-r--r--   0        0        0     1328 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
--rw-r--r--   0        0        0     3356 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
--rw-r--r--   0        0        0     1400 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
--rw-r--r--   0        0        0     1398 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
--rw-r--r--   0        0        0     4786 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
--rw-r--r--   0        0        0    43465 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
--rw-r--r--   0        0        0     5516 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/generic_agent.py
--rw-r--r--   0        0        0     1998 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/openai_whisper_agent.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/__init__.py
--rw-r--r--   0        0        0     2078 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
--rw-r--r--   0        0        0     1444 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
--rw-r--r--   0        0        0     2339 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
--rw-r--r--   0        0        0      559 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
--rw-r--r--   0        0        0     2939 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/retriever.py
--rw-r--r--   0        0        0     3640 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
--rw-r--r--   0        0        0    11421 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/simple_agent.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/__init__.py
--rw-r--r--   0        0        0     1825 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/checker.py
--rw-r--r--   0        0        0     2468 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/controller.py
--rw-r--r--   0        0        0     1503 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/memory.py
--rw-r--r--   0        0        0     1423 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/prompts.py
--rw-r--r--   0        0        0      364 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/thought.py
--rw-r--r--   0        0        0     4951 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
--rw-r--r--   0        0        0     7614 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
--rw-r--r--   0        0        0     4446 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent_os.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/bin/__init__.py
--rwxr-xr-x   0        0        0     9444 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/bin/agent_creator.py
--rw-r--r--   0        0        0     7578 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/bin/agent_http_server.py
--rwxr-xr-x   0        0        0     3789 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/bin/replay.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/__init__.py
--rw-r--r--   0        0        0     8297 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/code_builtins.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/components/__init__.py
--rw-r--r--   0        0        0     2223 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/components/opentelemetry.py
--rw-r--r--   0        0        0     4256 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/components/usage.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/logic_units/__init__.py
--rw-r--r--   0        0        0     5662 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/logic_units/web_search.py
--rw-r--r--   0        0        0      239 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
--rw-r--r--   0        0        0      236 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
--rw-r--r--   0        0        0      242 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
--rw-r--r--   0        0        0      181 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/machine.yaml
--rw-r--r--   0        0        0      231 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
--rw-r--r--   0        0        0      257 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
--rw-r--r--   0        0        0      231 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
--rw-r--r--   0        0        0      235 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/openai_35.yaml
--rw-r--r--   0        0        0      234 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/resources/openai_4.yaml
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/__init__.py
--rw-r--r--   0        0        0     1843 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agent_call_history.py
--rw-r--r--   0        0        0     4293 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agent_cpu.py
--rw-r--r--   0        0        0     2956 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agent_io.py
--rw-r--r--   0        0        0     7916 2024-04-05 21:02:16.976908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agents_logic_unit.py
--rw-r--r--   0        0        0      292 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/call_context.py
--rw-r--r--   0        0        0     2833 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/conversation_memory_unit.py
--rw-r--r--   0        0        0     8231 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/conversational_agent_cpu.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/__init__.py
--rw-r--r--   0        0        0    10036 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
--rw-r--r--   0        0        0    12148 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
--rw-r--r--   0        0        0    12773 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
--rw-r--r--   0        0        0     3119 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
--rw-r--r--   0        0        0     1679 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm_message.py
--rw-r--r--   0        0        0     1910 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm_unit.py
--rw-r--r--   0        0        0     4199 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/logic_unit.py
--rw-r--r--   0        0        0     3541 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/memory_unit.py
--rw-r--r--   0        0        0      825 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/processing_unit.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/io/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/__init__.py
--rw-r--r--   0        0        0     1157 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/agent_memory.py
--rw-r--r--   0        0        0     5309 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/chroma_vector_store.py
--rw-r--r--   0        0        0      641 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/document.py
--rw-r--r--   0        0        0     2620 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/embeddings.py
--rw-r--r--   0        0        0     2517 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/file_memory.py
--rw-r--r--   0        0        0     4220 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/file_system_vector_store.py
--rw-r--r--   0        0        0     3912 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/in_memory_file_memory.py
--rw-r--r--   0        0        0     5780 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/local_file_memory.py
--rw-r--r--   0        0        0     4837 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/local_symbolic_memory.py
--rw-r--r--   0        0        0     4067 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
--rw-r--r--   0        0        0      996 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/noop_memory.py
--rw-r--r--   0        0        0     1976 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/s3_file_memory.py
--rw-r--r--   0        0        0     5453 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/semantic_memory.py
--rw-r--r--   0        0        0      869 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/similarity_memory.py
--rw-r--r--   0        0        0     1516 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/vector_store.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/__init__.py
--rw-r--r--   0        0        0      771 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/authentication_processor.py
--rw-r--r--   0        0        0     2091 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/azure_authorizer.py
--rw-r--r--   0        0        0     1231 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/functional_authorizer.py
--rw-r--r--   0        0        0     2001 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/google_auth.py
--rw-r--r--   0        0        0     1867 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/jwt_processor.py
--rw-r--r--   0        0        0      484 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/okta_authorizor.py
--rw-r--r--   0        0        0     1076 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/permissions.py
--rw-r--r--   0        0        0     2462 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/process_authorizer.py
--rw-r--r--   0        0        0     1780 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/security_manager.py
--rw-r--r--   0        0        0     1052 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/security_middleware.py
--rw-r--r--   0        0        0      428 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/user.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/__init__.py
--rw-r--r--   0        0        0     1377 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/agent_contract.py
--rw-r--r--   0        0        0    20899 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/agent_controller.py
--rw-r--r--   0        0        0    13397 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/agent_machine.py
--rw-r--r--   0        0        0     1149 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/dynamic_middleware.py
--rw-r--r--   0        0        0     3432 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/fn_handler.py
--rw-r--r--   0        0        0     3911 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/process_file_system.py
--rw-r--r--   0        0        0     4275 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/processes.py
--rw-r--r--   0        0        0     6895 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/reference_model.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/resources/__init__.py
--rw-r--r--   0        0        0      314 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/resources/agent_resource.py
--rw-r--r--   0        0        0      414 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/resources/machine_resource.py
--rw-r--r--   0        0        0      684 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/resources/reference_resource.py
--rw-r--r--   0        0        0     1663 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/resources/resources_base.py
--rw-r--r--   0        0        0        0 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/__init__.py
--rw-r--r--   0        0        0      509 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/async_wrapper.py
--rw-r--r--   0        0        0     2806 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/class_utils.py
--rw-r--r--   0        0        0     3812 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/replay.py
--rw-r--r--   0        0        0     6483 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/schema_to_model.py
--rw-r--r--   0        0        0      900 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/str_utils.py
--rw-r--r--   0        0        0     3445 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/stream_collector.py
--rw-r--r--   0        0        0      565 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/logging.conf
--rw-r--r--   0        0        0     2003 2024-04-05 21:02:16.980908 eidolon_ai_sdk-0.1.24/pyproject.toml
--rw-r--r--   0        0        0     4759 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.24/PKG-INFO
+-rw-r--r--   0        0        0     2569 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/__init__.py
+-rw-r--r--   0        0        0     2415 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/agent.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/__init__.py
+-rw-r--r--   0        0        0     4645 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/document_manager.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
+-rw-r--r--   0        0        0      971 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
+-rw-r--r--   0        0        0     3405 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
+-rw-r--r--   0        0        0     4173 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
+-rw-r--r--   0        0        0     2805 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
+-rw-r--r--   0        0        0     4510 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
+-rw-r--r--   0        0        0      448 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
+-rw-r--r--   0        0        0     3699 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
+-rw-r--r--   0        0        0     2053 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
+-rw-r--r--   0        0        0     3212 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
+-rw-r--r--   0        0        0     1647 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
+-rw-r--r--   0        0        0     1328 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
+-rw-r--r--   0        0        0     3356 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
+-rw-r--r--   0        0        0     1400 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
+-rw-r--r--   0        0        0     1398 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
+-rw-r--r--   0        0        0     4786 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
+-rw-r--r--   0        0        0    43465 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
+-rw-r--r--   0        0        0     5516 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/generic_agent.py
+-rw-r--r--   0        0        0     1998 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/openai_whisper_agent.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/__init__.py
+-rw-r--r--   0        0        0     2078 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
+-rw-r--r--   0        0        0     1444 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
+-rw-r--r--   0        0        0     2339 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
+-rw-r--r--   0        0        0      559 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
+-rw-r--r--   0        0        0     2939 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/retriever.py
+-rw-r--r--   0        0        0     3640 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
+-rw-r--r--   0        0        0    11421 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/simple_agent.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/__init__.py
+-rw-r--r--   0        0        0     1825 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/checker.py
+-rw-r--r--   0        0        0     2468 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/controller.py
+-rw-r--r--   0        0        0     1503 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/memory.py
+-rw-r--r--   0        0        0     1423 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/prompts.py
+-rw-r--r--   0        0        0      364 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/thought.py
+-rw-r--r--   0        0        0     4951 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
+-rw-r--r--   0        0        0     7614 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
+-rw-r--r--   0        0        0     4446 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent_os.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/bin/__init__.py
+-rwxr-xr-x   0        0        0     9444 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/bin/agent_creator.py
+-rw-r--r--   0        0        0     7578 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/bin/agent_http_server.py
+-rwxr-xr-x   0        0        0     3789 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/bin/replay.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/__init__.py
+-rw-r--r--   0        0        0     8297 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/code_builtins.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/components/__init__.py
+-rw-r--r--   0        0        0     2223 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/components/opentelemetry.py
+-rw-r--r--   0        0        0     4256 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/components/usage.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/logic_units/__init__.py
+-rw-r--r--   0        0        0     5662 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/logic_units/web_search.py
+-rw-r--r--   0        0        0      239 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
+-rw-r--r--   0        0        0      236 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
+-rw-r--r--   0        0        0      242 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
+-rw-r--r--   0        0        0      181 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/machine.yaml
+-rw-r--r--   0        0        0      231 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
+-rw-r--r--   0        0        0      257 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
+-rw-r--r--   0        0        0      231 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
+-rw-r--r--   0        0        0      235 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/openai_35.yaml
+-rw-r--r--   0        0        0      234 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/openai_4.yaml
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/__init__.py
+-rw-r--r--   0        0        0     1843 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agent_call_history.py
+-rw-r--r--   0        0        0     4293 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agent_cpu.py
+-rw-r--r--   0        0        0     2956 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agent_io.py
+-rw-r--r--   0        0        0     7916 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agents_logic_unit.py
+-rw-r--r--   0        0        0      292 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/call_context.py
+-rw-r--r--   0        0        0     2833 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/conversation_memory_unit.py
+-rw-r--r--   0        0        0     8231 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/conversational_agent_cpu.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/__init__.py
+-rw-r--r--   0        0        0    10036 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
+-rw-r--r--   0        0        0    12148 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
+-rw-r--r--   0        0        0    12773 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
+-rw-r--r--   0        0        0     3119 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
+-rw-r--r--   0        0        0     1679 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm_message.py
+-rw-r--r--   0        0        0     1910 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm_unit.py
+-rw-r--r--   0        0        0     4199 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/logic_unit.py
+-rw-r--r--   0        0        0     3541 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/memory_unit.py
+-rw-r--r--   0        0        0      825 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/processing_unit.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/io/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/__init__.py
+-rw-r--r--   0        0        0     1157 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/agent_memory.py
+-rw-r--r--   0        0        0     5309 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/chroma_vector_store.py
+-rw-r--r--   0        0        0      641 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/document.py
+-rw-r--r--   0        0        0     2620 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/embeddings.py
+-rw-r--r--   0        0        0     2517 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/file_memory.py
+-rw-r--r--   0        0        0     4220 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/file_system_vector_store.py
+-rw-r--r--   0        0        0     3912 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/in_memory_file_memory.py
+-rw-r--r--   0        0        0     5780 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/local_file_memory.py
+-rw-r--r--   0        0        0     4837 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/local_symbolic_memory.py
+-rw-r--r--   0        0        0     3762 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
+-rw-r--r--   0        0        0      996 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/noop_memory.py
+-rw-r--r--   0        0        0     1976 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/s3_file_memory.py
+-rw-r--r--   0        0        0     5413 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/semantic_memory.py
+-rw-r--r--   0        0        0      869 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/similarity_memory.py
+-rw-r--r--   0        0        0     1516 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/vector_store.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/authentication_processor.py
+-rw-r--r--   0        0        0     2091 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/azure_authorizer.py
+-rw-r--r--   0        0        0     1231 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/functional_authorizer.py
+-rw-r--r--   0        0        0     2001 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/google_auth.py
+-rw-r--r--   0        0        0     1867 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/jwt_processor.py
+-rw-r--r--   0        0        0      484 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/okta_authorizor.py
+-rw-r--r--   0        0        0     1076 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/permissions.py
+-rw-r--r--   0        0        0     2462 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/process_authorizer.py
+-rw-r--r--   0        0        0     1780 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/security_manager.py
+-rw-r--r--   0        0        0     1052 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/security_middleware.py
+-rw-r--r--   0        0        0      428 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/user.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/__init__.py
+-rw-r--r--   0        0        0     1377 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/agent_contract.py
+-rw-r--r--   0        0        0    20899 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/agent_controller.py
+-rw-r--r--   0        0        0    13397 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/agent_machine.py
+-rw-r--r--   0        0        0     1149 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/dynamic_middleware.py
+-rw-r--r--   0        0        0     3432 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/fn_handler.py
+-rw-r--r--   0        0        0     3911 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/process_file_system.py
+-rw-r--r--   0        0        0     4275 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/processes.py
+-rw-r--r--   0        0        0     6895 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/reference_model.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/resources/__init__.py
+-rw-r--r--   0        0        0      314 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/resources/agent_resource.py
+-rw-r--r--   0        0        0      414 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/resources/machine_resource.py
+-rw-r--r--   0        0        0      684 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/resources/reference_resource.py
+-rw-r--r--   0        0        0     1663 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/resources/resources_base.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/__init__.py
+-rw-r--r--   0        0        0      509 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/async_wrapper.py
+-rw-r--r--   0        0        0     2806 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/class_utils.py
+-rw-r--r--   0        0        0     3812 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/replay.py
+-rw-r--r--   0        0        0     6483 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/schema_to_model.py
+-rw-r--r--   0        0        0      900 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/str_utils.py
+-rw-r--r--   0        0        0     3445 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/stream_collector.py
+-rw-r--r--   0        0        0      565 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/logging.conf
+-rw-r--r--   0        0        0     2003 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/pyproject.toml
+-rw-r--r--   0        0        0     4759 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.25/PKG-INFO
```

### Comparing `eidolon_ai_sdk-0.1.24/README.md` & `eidolon_ai_sdk-0.1.25/README.md`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/agent.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/document_manager.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/document_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/generic_agent.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/generic_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/openai_whisper_agent.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/openai_whisper_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/retriever.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/retriever.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/simple_agent.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/simple_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/checker.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/checker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/controller.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/memory.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/prompts.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/thought_generators.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/thought_generators.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent/tot_agent/tot_agent.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/tot_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/agent_os.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent_os.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/bin/agent_creator.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/bin/agent_creator.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/bin/agent_http_server.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/bin/agent_http_server.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/bin/replay.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/bin/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/code_builtins.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/code_builtins.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/components/opentelemetry.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/components/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/components/usage.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/components/usage.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/builtins/logic_units/web_search.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/logic_units/web_search.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agent_call_history.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agent_call_history.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agent_cpu.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agent_cpu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agent_io.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agent_io.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/agents_logic_unit.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agents_logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/conversation_memory_unit.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/conversation_memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/conversational_agent_cpu.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/conversational_agent_cpu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm/open_ai_speech.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/open_ai_speech.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm_message.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm_message.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/llm_unit.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/logic_unit.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/memory_unit.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/cpu/processing_unit.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/processing_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/agent_memory.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/agent_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/chroma_vector_store.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/chroma_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/document.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/document.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/embeddings.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/file_memory.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/file_system_vector_store.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/file_system_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/in_memory_file_memory.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/in_memory_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/local_file_memory.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/local_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/local_symbolic_memory.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/local_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/mongo_symbolic_memory.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/mongo_symbolic_memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from pydantic import Field, BaseModel
 
 from eidolon_ai_sdk.memory.semantic_memory import SymbolicMemory
 from eidolon_ai_sdk.system.reference_model import Specable
 
 
 class MongoSymbolicMemoryConfig(BaseModel):
-    mongo_connection_string: Optional[str] = Field(
-        default=None, description="The connection string to the MongoDB instance."
+    mongo_connection_string: str = Field(
+        default=os.environ.get("MONGO_CONNECTION_STR", "mongodb://localhost:27017/?directConnection=true"), description="The connection string to the MongoDB instance."
     )
-    mongo_database_name: str = Field(default="eidolon", description="The name of the MongoDB database to use.")
+    mongo_database_name: str = Field(default=os.environ.get("MONGO_DATABASE_NAME", "eidolon"), description="The name of the MongoDB database to use.")
 
 
 class MongoSymbolicMemory(SymbolicMemory, Specable[MongoSymbolicMemoryConfig]):
     mongo_connection_string: Optional[str]
     mongo_database_name: str
     _database: Optional[ContextVar]
 
@@ -79,24 +79,14 @@
 
     async def upsert_one(self, symbol_collection: str, document: dict[str, Any], query: dict[str, Any]) -> None:
         return await self.database[symbol_collection].update_one(query, {"$set": document}, upsert=True)
 
     async def delete(self, symbol_collection, query):
         return await self.database[symbol_collection].delete_many(query)
 
-    async def start(self):
-        """
-        Starts the memory implementation. Noop for this implementation.
-        """
-        if self.database is None:
-            if self.mongo_connection_string is None:
-                self.mongo_connection_string = os.getenv("MONGO_CONNECTION_STRING")
-            if self.mongo_database_name is None:
-                self.mongo_database_name = os.getenv("MONGO_DATABASE_NAME")
-
     async def stop(self):
         """
         Stops the memory implementation. Noop for this implementation.
         """
         if self.database is not None:
             self.database.client.close()
             self._database = None
```

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/noop_memory.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/noop_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/s3_file_memory.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/s3_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/semantic_memory.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/semantic_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,21 @@
 
     This class defines the contract for symbolic memory operations such as starting
     and stopping the memory service, and CRUD (Create, Read, Update, Delete) operations
     on symbolic data. Implementations of this class are expected to manage collections
     of symbols, providing a high-level interface to store and retrieve symbolic information.
     """
 
-    @abstractmethod
     async def start(self):
         """
         Prepares the symbolic memory for operation, which may include tasks like
         allocating resources or initializing connections to databases.
         """
         pass
 
-    @abstractmethod
     async def stop(self):
         """
         Properly shuts down the symbolic memory, ensuring that any resources are released
         or any established connections are terminated.
         """
         pass
```

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/similarity_memory.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/similarity_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/memory/vector_store.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/authentication_processor.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/authentication_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/azure_authorizer.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/azure_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/functional_authorizer.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/functional_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/google_auth.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/google_auth.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/jwt_processor.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/jwt_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/permissions.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/permissions.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/process_authorizer.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/process_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/security_manager.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/security_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/security/security_middleware.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/security_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/agent_contract.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/agent_contract.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/agent_controller.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/agent_controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/agent_machine.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/agent_machine.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/dynamic_middleware.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/dynamic_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/fn_handler.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/fn_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/process_file_system.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/process_file_system.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/processes.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/processes.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/reference_model.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/reference_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/resources/reference_resource.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/resources/reference_resource.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/system/resources/resources_base.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/resources/resources_base.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/class_utils.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/class_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/replay.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/schema_to_model.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/schema_to_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/str_utils.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/str_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/eidolon_ai_sdk/util/stream_collector.py` & `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/stream_collector.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/logging.conf` & `eidolon_ai_sdk-0.1.25/logging.conf`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.24/pyproject.toml` & `eidolon_ai_sdk-0.1.25/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eidolon-ai-sdk"
-version = "0.1.24"
+version = "0.1.25"
 description = "An Open Source Agent Services Framework"
 authors = ["Luke Lalor <lukehlalor@gmail.com>"]
 readme = "README.md"
 include = ["logging.conf"]
 
 [tool.poetry.urls]
 Github = "https://github.com/eidolon-ai/eidolon"
```

### Comparing `eidolon_ai_sdk-0.1.24/PKG-INFO` & `eidolon_ai_sdk-0.1.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eidolon-ai-sdk
-Version: 0.1.24
+Version: 0.1.25
 Summary: An Open Source Agent Services Framework
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
```

