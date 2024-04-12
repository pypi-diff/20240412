# Comparing `tmp/pymemgpt_nightly-0.3.9.dev20240411025350.tar.gz` & `tmp/pymemgpt_nightly-0.3.9.dev20240411103902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemgpt_nightly-0.3.9.dev20240411025350.tar", max compression
+gzip compressed data, was "pymemgpt_nightly-0.3.9.dev20240411103902.tar", max compression
```

## Comparing `pymemgpt_nightly-0.3.9.dev20240411025350.tar` & `pymemgpt_nightly-0.3.9.dev20240411103902.tar`

### file list

```diff
@@ -1,171 +1,171 @@
--rw-r--r--   0        0        0    10760 2024-04-11 02:53:42.943613 pymemgpt_nightly-0.3.9.dev20240411025350/LICENSE
--rw-r--r--   0        0        0     8441 2024-04-11 02:53:42.943613 pymemgpt_nightly-0.3.9.dev20240411025350/README.md
--rw-r--r--   0        0        0      108 2024-04-11 02:53:50.131612 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/__init__.py
--rw-r--r--   0        0        0       29 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/__main__.py
--rw-r--r--   0        0        0    55434 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent.py
--rw-r--r--   0        0        0    10728 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/chroma.py
--rw-r--r--   0        0        0    25552 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/db.py
--rw-r--r--   0        0        0     5288 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/lancedb.py
--rw-r--r--   0        0        0     6390 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/storage.py
--rw-r--r--   0        0        0      169 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/README.md
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/__init__.py
--rw-r--r--   0        0        0     7088 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/agent_autoreply.py
--rw-r--r--   0        0        0     6813 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/agent_docs.py
--rw-r--r--   0        0        0     7929 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/agent_groupchat.py
--rw-r--r--   0        0        0     7375 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/memgpt_coder_autogen.ipynb
--rw-r--r--   0        0        0     9346 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/interface.py
--rw-r--r--   0        0        0    20931 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/memgpt_agent.py
--rw-r--r--   0        0        0     3644 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/benchmark/benchmark.py
--rw-r--r--   0        0        0      536 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/benchmark/constants.py
--rw-r--r--   0        0        0    34724 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/cli/cli.py
--rw-r--r--   0        0        0    45520 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/cli/cli_config.py
--rw-r--r--   0        0        0    10453 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/cli/cli_load.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/client/__init__.py
--rw-r--r--   0        0        0     3239 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/client/admin.py
--rw-r--r--   0        0        0    26894 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/client/client.py
--rw-r--r--   0        0        0    18729 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/config.py
--rw-r--r--   0        0        0      390 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/configs/memgpt_hosted.json
--rw-r--r--   0        0        0      373 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/configs/openai.json
--rw-r--r--   0        0        0     5606 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/constants.py
--rw-r--r--   0        0        0     5390 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/credentials.py
--rw-r--r--   0        0        0     9529 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/data_sources/connectors.py
--rw-r--r--   0        0        0    28513 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/data_types.py
--rw-r--r--   0        0        0     7601 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/embeddings.py
--rw-r--r--   0        0        0      820 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/errors.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/__init__.py
--rw-r--r--   0        0        0     7343 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/function_sets/base.py
--rw-r--r--   0        0        0     4775 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/function_sets/extras.py
--rw-r--r--   0        0        0     7403 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/functions.py
--rw-r--r--   0        0        0     5433 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/schema_generator.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/humans/__init__.py
--rw-r--r--   0        0        0       17 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/humans/examples/basic.txt
--rw-r--r--   0        0        0      305 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/humans/examples/cs_phd.txt
--rw-r--r--   0        0        0    12994 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/interface.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/llm_api/__init__.py
--rw-r--r--   0        0        0     6816 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/llm_api/azure_openai.py
--rw-r--r--   0        0        0    19315 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/llm_api/google_ai.py
--rw-r--r--   0        0        0    10622 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/llm_api/llm_api_tools.py
--rw-r--r--   0        0        0     5972 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/llm_api/openai.py
--rw-r--r--   0        0        0      175 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/README.md
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/__init__.py
--rw-r--r--   0        0        0    13519 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/chat_completion_proxy.py
--rw-r--r--   0        0        0     1032 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/constants.py
--rw-r--r--   0        0        0     2788 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/function_parser.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/grammars/__init__.py
--rw-r--r--   0        0        0    56322 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/grammars/gbnf_grammar_generator.py
--rw-r--r--   0        0        0      667 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/grammars/json.gbnf
--rw-r--r--   0        0        0     3255 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf
--rw-r--r--   0        0        0     3562 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/groq/api.py
--rw-r--r--   0        0        0     7793 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/json_parser.py
--rw-r--r--   0        0        0     2586 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/koboldcpp/api.py
--rw-r--r--   0        0        0      557 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/koboldcpp/settings.py
--rw-r--r--   0        0        0     2492 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llamacpp/api.py
--rw-r--r--   0        0        0      548 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llamacpp/settings.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/__init__.py
--rw-r--r--   0        0        0    19913 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py
--rw-r--r--   0        0        0    21457 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py
--rw-r--r--   0        0        0    19975 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py
--rw-r--r--   0        0        0    10300 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py
--rw-r--r--   0        0        0     6144 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py
--rw-r--r--   0        0        0      419 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/wrapper_base.py
--rw-r--r--   0        0        0    14956 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py
--rw-r--r--   0        0        0     4630 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/lmstudio/api.py
--rw-r--r--   0        0        0      857 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/lmstudio/settings.py
--rw-r--r--   0        0        0     3660 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/ollama/api.py
--rw-r--r--   0        0        0      894 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/ollama/settings.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/settings/__init__.py
--rw-r--r--   0        0        0     1222 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/settings/deterministic_mirostat.py
--rw-r--r--   0        0        0     3058 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/settings/settings.py
--rw-r--r--   0        0        0      719 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/settings/simple.py
--rw-r--r--   0        0        0     4846 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/utils.py
--rw-r--r--   0        0        0     2612 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/vllm/api.py
--rw-r--r--   0        0        0     2658 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/api.py
--rw-r--r--   0        0        0     2354 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/legacy_api.py
--rw-r--r--   0        0        0      579 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/legacy_settings.py
--rw-r--r--   0        0        0      593 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/settings.py
--rw-r--r--   0        0        0     1211 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/log.py
--rw-r--r--   0        0        0    20047 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/main.py
--rw-r--r--   0        0        0    20376 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/memory.py
--rw-r--r--   0        0        0    29420 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/metadata.py
--rw-r--r--   0        0        0    31537 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/migrate.py
--rw-r--r--   0        0        0     3295 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/chat_completion_request.py
--rw-r--r--   0        0        0     1562 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/chat_completion_response.py
--rw-r--r--   0        0        0      356 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/embedding_response.py
--rw-r--r--   0        0        0     7977 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/openai.py
--rw-r--r--   0        0        0     8957 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/pydantic_models.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/openai_backcompat/__init__.py
--rw-r--r--   0        0        0    13692 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/openai_backcompat/openai_object.py
--rw-r--r--   0        0        0     5882 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/persistence_manager.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/__init__.py
--rw-r--r--   0        0        0     1849 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/anna_pa.txt
--rw-r--r--   0        0        0     1196 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/google_search_persona.txt
--rw-r--r--   0        0        0      431 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/memgpt_doc.txt
--rw-r--r--   0        0        0      164 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/memgpt_starter.txt
--rw-r--r--   0        0        0     1236 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sam.txt
--rw-r--r--   0        0        0     1171 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sam_pov.txt
--rw-r--r--   0        0        0     1053 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sam_simple_pov_gpt35.txt
--rw-r--r--   0        0        0     8192 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sqldb/test.db
--rw-r--r--   0        0        0      248 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/presets/examples/memgpt_chat.yaml
--rw-r--r--   0        0        0      247 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/presets/examples/memgpt_docs.yaml
--rw-r--r--   0        0        0      374 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/presets/examples/memgpt_extras.yaml
--rw-r--r--   0        0        0     7575 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/presets/presets.py
--rw-r--r--   0        0        0     2789 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/presets/utils.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/__init__.py
--rw-r--r--   0        0        0    12907 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/gpt_functions.py
--rw-r--r--   0        0        0     1139 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/gpt_summarize.py
--rw-r--r--   0        0        0     1045 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/gpt_system.py
--rw-r--r--   0        0        0     4758 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_base.txt
--rw-r--r--   0        0        0     5479 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_chat.txt
--rw-r--r--   0        0        0     1057 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_chat_compressed.txt
--rw-r--r--   0        0        0     4819 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_doc.txt
--rw-r--r--   0        0        0     5047 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_gpt35_extralong.txt
--rw-r--r--   0        0        0     2967 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_intuitive_knowledge.txt
--rw-r--r--   0        0        0     4663 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_modified_chat.txt
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/__init__.py
--rw-r--r--   0        0        0       92 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/constants.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/admin/__init__.py
--rw-r--r--   0        0        0     6130 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/admin/users.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/__init__.py
--rw-r--r--   0        0        0     1757 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/command.py
--rw-r--r--   0        0        0     6138 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/config.py
--rw-r--r--   0        0        0     5114 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/index.py
--rw-r--r--   0        0        0     7640 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/memory.py
--rw-r--r--   0        0        0     8583 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/message.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/auth/__init__.py
--rw-r--r--   0        0        0     1303 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/auth/index.py
--rw-r--r--   0        0        0      775 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/auth_token.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/config/__init__.py
--rw-r--r--   0        0        0     1136 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/config/index.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/humans/__init__.py
--rw-r--r--   0        0        0     1732 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/humans/index.py
--rw-r--r--   0        0        0     5482 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/interface.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/models/__init__.py
--rw-r--r--   0        0        0     1401 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/models/index.py
--rw-r--r--   0        0        0    23956 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/openai_assistants/assistants.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/personas/__init__.py
--rw-r--r--   0        0        0     1795 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/personas/index.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/presets/__init__.py
--rw-r--r--   0        0        0     5014 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/presets/index.py
--rw-r--r--   0        0        0     9580 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/server.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/sources/__init__.py
--rw-r--r--   0        0        0     8218 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/sources/index.py
--rw-r--r--   0        0        0      914 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/static_files.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/tools/__init__.py
--rw-r--r--   0        0        0     2560 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/tools/index.py
--rw-r--r--   0        0        0    63646 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/server.py
--rw-r--r--   0        0        0    43424 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/assets/index-0c5d3001.css
--rw-r--r--   0        0        0   725155 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/assets/index-bf421135.js
--rw-r--r--   0        0        0    28783 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/favicon.ico
--rw-r--r--   0        0        0     1199 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/index.html
--rw-r--r--   0        0        0    85383 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/memgpt_logo_transparent.png
--rw-r--r--   0        0        0     1667 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/utils.py
--rw-r--r--   0        0        0        0 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/__init__.py
--rw-r--r--   0        0        0     4264 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/example_client.py
--rw-r--r--   0        0        0     4124 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/interface.py
--rw-r--r--   0        0        0     2257 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/protocol.py
--rw-r--r--   0        0        0     6122 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/server.py
--rw-r--r--   0        0        0     7281 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/system.py
--rw-r--r--   0        0        0    31426 2024-04-11 02:53:42.967613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/utils.py
--rw-r--r--   0        0        0     2285 2024-04-11 02:53:50.131612 pymemgpt_nightly-0.3.9.dev20240411025350/pyproject.toml
--rw-r--r--   0        0        0    11046 1970-01-01 00:00:00.000000 pymemgpt_nightly-0.3.9.dev20240411025350/PKG-INFO
+-rw-r--r--   0        0        0    10760 2024-04-11 10:38:55.455901 pymemgpt_nightly-0.3.9.dev20240411103902/LICENSE
+-rw-r--r--   0        0        0     8441 2024-04-11 10:38:55.455901 pymemgpt_nightly-0.3.9.dev20240411103902/README.md
+-rw-r--r--   0        0        0      108 2024-04-11 10:39:02.663830 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/__init__.py
+-rw-r--r--   0        0        0       29 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/__main__.py
+-rw-r--r--   0        0        0    55434 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent.py
+-rw-r--r--   0        0        0    10728 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/chroma.py
+-rw-r--r--   0        0        0    25552 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/db.py
+-rw-r--r--   0        0        0     5288 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/lancedb.py
+-rw-r--r--   0        0        0     6390 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/storage.py
+-rw-r--r--   0        0        0      169 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/__init__.py
+-rw-r--r--   0        0        0     7088 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/agent_autoreply.py
+-rw-r--r--   0        0        0     6813 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/agent_docs.py
+-rw-r--r--   0        0        0     7929 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/agent_groupchat.py
+-rw-r--r--   0        0        0     7375 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/memgpt_coder_autogen.ipynb
+-rw-r--r--   0        0        0     9346 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/interface.py
+-rw-r--r--   0        0        0    20931 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/memgpt_agent.py
+-rw-r--r--   0        0        0     3644 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/benchmark/benchmark.py
+-rw-r--r--   0        0        0      536 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/benchmark/constants.py
+-rw-r--r--   0        0        0    34724 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/cli/cli.py
+-rw-r--r--   0        0        0    45520 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/cli/cli_config.py
+-rw-r--r--   0        0        0    10453 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/cli/cli_load.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/client/__init__.py
+-rw-r--r--   0        0        0     3239 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/client/admin.py
+-rw-r--r--   0        0        0    26894 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/client/client.py
+-rw-r--r--   0        0        0    18729 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/config.py
+-rw-r--r--   0        0        0      390 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/configs/memgpt_hosted.json
+-rw-r--r--   0        0        0      373 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/configs/openai.json
+-rw-r--r--   0        0        0     5606 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/constants.py
+-rw-r--r--   0        0        0     5390 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/credentials.py
+-rw-r--r--   0        0        0     9529 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/data_sources/connectors.py
+-rw-r--r--   0        0        0    28513 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/data_types.py
+-rw-r--r--   0        0        0     7601 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/embeddings.py
+-rw-r--r--   0        0        0      820 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/errors.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/__init__.py
+-rw-r--r--   0        0        0     7343 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/function_sets/base.py
+-rw-r--r--   0        0        0     4775 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/function_sets/extras.py
+-rw-r--r--   0        0        0     7403 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/functions.py
+-rw-r--r--   0        0        0     5433 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/schema_generator.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/humans/__init__.py
+-rw-r--r--   0        0        0       17 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/humans/examples/basic.txt
+-rw-r--r--   0        0        0      305 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/humans/examples/cs_phd.txt
+-rw-r--r--   0        0        0    12994 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/interface.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/__init__.py
+-rw-r--r--   0        0        0     6816 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/azure_openai.py
+-rw-r--r--   0        0        0    19315 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/google_ai.py
+-rw-r--r--   0        0        0    10622 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/llm_api_tools.py
+-rw-r--r--   0        0        0     5972 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/openai.py
+-rw-r--r--   0        0        0      175 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/__init__.py
+-rw-r--r--   0        0        0    13519 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/chat_completion_proxy.py
+-rw-r--r--   0        0        0     1032 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/constants.py
+-rw-r--r--   0        0        0     2788 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/function_parser.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/grammars/__init__.py
+-rw-r--r--   0        0        0    56322 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/grammars/gbnf_grammar_generator.py
+-rw-r--r--   0        0        0      667 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/grammars/json.gbnf
+-rw-r--r--   0        0        0     3255 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf
+-rw-r--r--   0        0        0     3562 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/groq/api.py
+-rw-r--r--   0        0        0     7793 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/json_parser.py
+-rw-r--r--   0        0        0     2586 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/koboldcpp/api.py
+-rw-r--r--   0        0        0      557 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/koboldcpp/settings.py
+-rw-r--r--   0        0        0     2492 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llamacpp/api.py
+-rw-r--r--   0        0        0      548 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llamacpp/settings.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/__init__.py
+-rw-r--r--   0        0        0    19913 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py
+-rw-r--r--   0        0        0    21457 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py
+-rw-r--r--   0        0        0    19975 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py
+-rw-r--r--   0        0        0    10300 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py
+-rw-r--r--   0        0        0     6144 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py
+-rw-r--r--   0        0        0      419 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/wrapper_base.py
+-rw-r--r--   0        0        0    14956 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py
+-rw-r--r--   0        0        0     4630 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/lmstudio/api.py
+-rw-r--r--   0        0        0      857 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/lmstudio/settings.py
+-rw-r--r--   0        0        0     3660 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/ollama/api.py
+-rw-r--r--   0        0        0      894 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/ollama/settings.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/settings/__init__.py
+-rw-r--r--   0        0        0     1222 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/settings/deterministic_mirostat.py
+-rw-r--r--   0        0        0     3058 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/settings/settings.py
+-rw-r--r--   0        0        0      719 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/settings/simple.py
+-rw-r--r--   0        0        0     4846 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/utils.py
+-rw-r--r--   0        0        0     2612 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/vllm/api.py
+-rw-r--r--   0        0        0     2658 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/api.py
+-rw-r--r--   0        0        0     2354 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/legacy_api.py
+-rw-r--r--   0        0        0      579 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/legacy_settings.py
+-rw-r--r--   0        0        0      593 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/settings.py
+-rw-r--r--   0        0        0     1211 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/log.py
+-rw-r--r--   0        0        0    20047 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/main.py
+-rw-r--r--   0        0        0    20376 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/memory.py
+-rw-r--r--   0        0        0    29420 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/metadata.py
+-rw-r--r--   0        0        0    31537 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/migrate.py
+-rw-r--r--   0        0        0     3295 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/chat_completion_request.py
+-rw-r--r--   0        0        0     1562 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/chat_completion_response.py
+-rw-r--r--   0        0        0      356 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/embedding_response.py
+-rw-r--r--   0        0        0     7977 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/openai.py
+-rw-r--r--   0        0        0     8957 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/pydantic_models.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/openai_backcompat/__init__.py
+-rw-r--r--   0        0        0    13692 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/openai_backcompat/openai_object.py
+-rw-r--r--   0        0        0     5882 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/persistence_manager.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/__init__.py
+-rw-r--r--   0        0        0     1849 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/anna_pa.txt
+-rw-r--r--   0        0        0     1196 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/google_search_persona.txt
+-rw-r--r--   0        0        0      431 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/memgpt_doc.txt
+-rw-r--r--   0        0        0      164 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/memgpt_starter.txt
+-rw-r--r--   0        0        0     1236 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sam.txt
+-rw-r--r--   0        0        0     1171 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sam_pov.txt
+-rw-r--r--   0        0        0     1053 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sam_simple_pov_gpt35.txt
+-rw-r--r--   0        0        0     8192 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sqldb/test.db
+-rw-r--r--   0        0        0      248 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/presets/examples/memgpt_chat.yaml
+-rw-r--r--   0        0        0      247 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/presets/examples/memgpt_docs.yaml
+-rw-r--r--   0        0        0      374 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/presets/examples/memgpt_extras.yaml
+-rw-r--r--   0        0        0     7575 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/presets/presets.py
+-rw-r--r--   0        0        0     2789 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/presets/utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/__init__.py
+-rw-r--r--   0        0        0    12907 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/gpt_functions.py
+-rw-r--r--   0        0        0     1139 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/gpt_summarize.py
+-rw-r--r--   0        0        0     1045 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/gpt_system.py
+-rw-r--r--   0        0        0     4758 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_base.txt
+-rw-r--r--   0        0        0     5479 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_chat.txt
+-rw-r--r--   0        0        0     1057 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_chat_compressed.txt
+-rw-r--r--   0        0        0     4819 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_doc.txt
+-rw-r--r--   0        0        0     5047 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_gpt35_extralong.txt
+-rw-r--r--   0        0        0     2967 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_intuitive_knowledge.txt
+-rw-r--r--   0        0        0     4663 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_modified_chat.txt
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/constants.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/admin/__init__.py
+-rw-r--r--   0        0        0     6130 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/admin/users.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/__init__.py
+-rw-r--r--   0        0        0     1757 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/command.py
+-rw-r--r--   0        0        0     6138 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/config.py
+-rw-r--r--   0        0        0     5114 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/index.py
+-rw-r--r--   0        0        0     7640 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/memory.py
+-rw-r--r--   0        0        0     8583 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/message.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/auth/__init__.py
+-rw-r--r--   0        0        0     1303 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/auth/index.py
+-rw-r--r--   0        0        0      775 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/auth_token.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/config/__init__.py
+-rw-r--r--   0        0        0     1136 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/config/index.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/humans/__init__.py
+-rw-r--r--   0        0        0     1732 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/humans/index.py
+-rw-r--r--   0        0        0     5482 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/interface.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/models/__init__.py
+-rw-r--r--   0        0        0     1401 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/models/index.py
+-rw-r--r--   0        0        0    23956 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/openai_assistants/assistants.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/personas/__init__.py
+-rw-r--r--   0        0        0     1795 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/personas/index.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/presets/__init__.py
+-rw-r--r--   0        0        0     5014 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/presets/index.py
+-rw-r--r--   0        0        0     9580 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/server.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/sources/__init__.py
+-rw-r--r--   0        0        0     8218 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/sources/index.py
+-rw-r--r--   0        0        0      914 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/static_files.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/tools/__init__.py
+-rw-r--r--   0        0        0     2560 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/tools/index.py
+-rw-r--r--   0        0        0    63646 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/server.py
+-rw-r--r--   0        0        0    43424 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/assets/index-0c5d3001.css
+-rw-r--r--   0        0        0   725155 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/assets/index-bf421135.js
+-rw-r--r--   0        0        0    28783 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/favicon.ico
+-rw-r--r--   0        0        0     1199 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/index.html
+-rw-r--r--   0        0        0    85383 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/memgpt_logo_transparent.png
+-rw-r--r--   0        0        0     1667 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/__init__.py
+-rw-r--r--   0        0        0     4264 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/example_client.py
+-rw-r--r--   0        0        0     4124 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/interface.py
+-rw-r--r--   0        0        0     2257 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/protocol.py
+-rw-r--r--   0        0        0     6122 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/server.py
+-rw-r--r--   0        0        0     7281 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/system.py
+-rw-r--r--   0        0        0    31426 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/utils.py
+-rw-r--r--   0        0        0     2285 2024-04-11 10:39:02.663830 pymemgpt_nightly-0.3.9.dev20240411103902/pyproject.toml
+-rw-r--r--   0        0        0    11046 1970-01-01 00:00:00.000000 pymemgpt_nightly-0.3.9.dev20240411103902/PKG-INFO
```

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/LICENSE` & `pymemgpt_nightly-0.3.9.dev20240411103902/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/README.md` & `pymemgpt_nightly-0.3.9.dev20240411103902/README.md`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/chroma.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/chroma.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/db.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/db.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/lancedb.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/lancedb.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/storage.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/storage.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/agent_autoreply.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/agent_autoreply.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/agent_docs.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/agent_docs.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/agent_groupchat.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/agent_groupchat.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/memgpt_coder_autogen.ipynb` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/memgpt_coder_autogen.ipynb`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/interface.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/memgpt_agent.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/memgpt_agent.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/benchmark/benchmark.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/benchmark/constants.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/benchmark/constants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/cli/cli.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/cli/cli_config.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/cli/cli_load.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/cli/cli_load.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/client/admin.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/client/admin.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/client/client.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/client/client.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/config.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/config.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/constants.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/constants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/credentials.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/credentials.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/data_sources/connectors.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/data_sources/connectors.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/data_types.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/data_types.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/embeddings.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/embeddings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/errors.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/errors.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/function_sets/base.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/function_sets/base.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/function_sets/extras.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/function_sets/extras.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/functions.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/functions.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/schema_generator.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/schema_generator.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/interface.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/llm_api/azure_openai.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/llm_api/google_ai.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/google_ai.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/llm_api/llm_api_tools.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/llm_api_tools.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/llm_api/openai.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/openai.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/chat_completion_proxy.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/chat_completion_proxy.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/constants.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/constants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/function_parser.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/function_parser.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/grammars/gbnf_grammar_generator.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/grammars/gbnf_grammar_generator.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/grammars/json.gbnf` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/grammars/json.gbnf`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/groq/api.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/groq/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/json_parser.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/json_parser.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/koboldcpp/api.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/koboldcpp/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/koboldcpp/settings.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/koboldcpp/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llamacpp/api.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llamacpp/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llamacpp/settings.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llamacpp/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/lmstudio/api.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/lmstudio/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/lmstudio/settings.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/lmstudio/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/ollama/api.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/ollama/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/ollama/settings.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/ollama/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/settings/deterministic_mirostat.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/settings/deterministic_mirostat.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/settings/settings.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/settings/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/settings/simple.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/settings/simple.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/utils.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/vllm/api.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/vllm/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/api.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/legacy_api.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/legacy_api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/legacy_settings.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/legacy_settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/settings.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/log.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/log.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/main.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/main.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/memory.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/memory.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/metadata.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/metadata.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/migrate.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/migrate.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/chat_completion_request.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/chat_completion_request.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/chat_completion_response.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/openai.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/openai.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/pydantic_models.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/openai_backcompat/openai_object.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/openai_backcompat/openai_object.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/persistence_manager.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/persistence_manager.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/anna_pa.txt` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/anna_pa.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/google_search_persona.txt` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/google_search_persona.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sam.txt` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sam.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sam_pov.txt` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sam_pov.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sam_simple_pov_gpt35.txt` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sam_simple_pov_gpt35.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sqldb/test.db` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sqldb/test.db`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/presets/presets.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/presets/presets.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/presets/utils.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/presets/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/gpt_functions.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/gpt_functions.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/gpt_summarize.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/gpt_summarize.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/gpt_system.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/gpt_system.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_base.txt` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_base.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_chat.txt` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_chat.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_chat_compressed.txt` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_chat_compressed.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_doc.txt` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_doc.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_gpt35_extralong.txt` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_gpt35_extralong.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_intuitive_knowledge.txt` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_intuitive_knowledge.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_modified_chat.txt` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_modified_chat.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/admin/users.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/admin/users.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/command.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/command.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/config.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/config.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/index.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/memory.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/memory.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/message.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/message.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/auth/index.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/auth/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/auth_token.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/auth_token.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/config/index.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/config/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/humans/index.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/humans/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/interface.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/models/index.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/models/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/openai_assistants/assistants.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/openai_assistants/assistants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/personas/index.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/personas/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/presets/index.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/presets/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/server.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/server.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/sources/index.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/sources/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/static_files.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/static_files.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/tools/index.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/tools/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/server.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/server.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/assets/index-0c5d3001.css` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/assets/index-0c5d3001.css`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/assets/index-bf421135.js` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/assets/index-bf421135.js`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/favicon.ico` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/favicon.ico`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/index.html` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/index.html`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/memgpt_logo_transparent.png` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/memgpt_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/utils.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/example_client.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/example_client.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/interface.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/protocol.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/protocol.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/server.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/server.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/system.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/system.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/utils.py` & `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/pyproject.toml` & `pymemgpt_nightly-0.3.9.dev20240411103902/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymemgpt-nightly"
-version = "0.3.9.dev20240411025350"
+version = "0.3.9.dev20240411103902"
 packages = [
     {include = "memgpt"}
 ]
 description = "Teaching LLMs memory management for unbounded context"
 authors = [
     "MemGPT Team <hi@memgpt.ai>",
 ]
```

### Comparing `pymemgpt_nightly-0.3.9.dev20240411025350/PKG-INFO` & `pymemgpt_nightly-0.3.9.dev20240411103902/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemgpt-nightly
-Version: 0.3.9.dev20240411025350
+Version: 0.3.9.dev20240411103902
 Summary: Teaching LLMs memory management for unbounded context
 License: Apache License
 Author: MemGPT Team
 Author-email: hi@memgpt.ai
 Requires-Python: >=3.10,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymemgpt-nightly Version: 0.3.9.dev20240411025350
+Metadata-Version: 2.1 Name: pymemgpt-nightly Version: 0.3.9.dev20240411103902
 Summary: Teaching LLMs memory management for unbounded context License: Apache
 License Author: MemGPT Team Author-email: hi@memgpt.ai Requires-Python:
 >=3.10,<3.13 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Provides-Extra: autogen Provides-Extra:
 dev Provides-Extra: local Provides-Extra: postgres Provides-Extra: server
```

