# Comparing `tmp/agent_os_py-0.1.0.tar.gz` & `tmp/agent_os_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent_os_py-0.1.0.tar", max compression
+gzip compressed data, was "agent_os_py-0.1.1.tar", max compression
```

## Comparing `agent_os_py-0.1.0.tar` & `agent_os_py-0.1.1.tar`

### file list

```diff
@@ -1,68 +1,74 @@
--rw-r--r--   0        0        0     1073 2023-07-24 02:56:14.252362 agent_os_py-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     4683 2023-09-19 15:31:31.152782 agent_os_py-0.1.0/README.md
--rw-r--r--   0        0        0     3508 2023-09-08 12:28:38.033624 agent_os_py-0.1.0/agents/jetpack/chat/chat_completions.py
--rw-r--r--   0        0        0     2462 2023-09-17 12:35:58.217922 agent_os_py-0.1.0/agents/jetpack/chat/chat_queries.py
--rw-r--r--   0        0        0    11904 2023-09-17 11:29:05.716719 agent_os_py-0.1.0/agents/jetpack/chat/chat_wit.py
--rw-r--r--   0        0        0    17270 2023-09-15 16:26:28.741162 agent_os_py-0.1.0/agents/jetpack/coder/coder_completions.py
--rw-r--r--   0        0        0    11940 2023-09-17 11:53:25.994817 agent_os_py-0.1.0/agents/jetpack/coder/coder_wit.py
--rw-r--r--   0        0        0     3473 2023-09-17 14:03:16.943325 agent_os_py-0.1.0/agents/jetpack/coder/retriever_completions.py
--rw-r--r--   0        0        0     7333 2023-09-17 09:13:20.259473 agent_os_py-0.1.0/agents/jetpack/coder/retriever_wit.py
--rw-r--r--   0        0        0    15428 2023-09-17 08:58:06.590136 agent_os_py-0.1.0/agents/jetpack/design.html
--rw-r--r--   0        0        0     1482 2023-09-09 07:36:54.276651 agent_os_py-0.1.0/agents/jetpack/frontend/frontend_queries.py
--rw-r--r--   0        0        0     1443 2023-09-15 16:32:03.805099 agent_os_py-0.1.0/agents/jetpack/frontend/frontend_wit.py
--rw-r--r--   0        0        0       58 2023-09-07 07:15:44.282515 agent_os_py-0.1.0/agents/jetpack/messages/__init__.py
--rw-r--r--   0        0        0     2046 2023-09-07 07:15:44.282515 agent_os_py-0.1.0/agents/jetpack/messages/messages_chat.py
--rw-r--r--   0        0        0     1009 2023-09-17 11:26:19.078508 agent_os_py-0.1.0/agents/jetpack/messages/messages_coder.py
--rw-r--r--   0        0        0      312 2023-09-14 11:53:46.869729 agent_os_py-0.1.0/agents/jetpack/sync.toml
--rw-r--r--   0        0        0        0 2023-09-08 09:19:16.095178 agent_os_py-0.1.0/agents/jetpack/tailwind.config.js
--rw-r--r--   0        0        0      442 2023-09-17 12:33:09.456384 agent_os_py-0.1.0/agents/jetpack/templates/artifacts.html
--rw-r--r--   0        0        0     2097 2023-09-08 10:31:46.143315 agent_os_py-0.1.0/agents/jetpack/templates/chat_messages.html
--rw-r--r--   0        0        0    10703 2023-09-17 14:14:21.687009 agent_os_py-0.1.0/agents/jetpack/templates/index.html
--rw-r--r--   0        0        0      280 2023-09-07 07:12:39.325064 agent_os_py-0.1.0/agents/lib/completions/__init__.py
--rw-r--r--   0        0        0     3107 2023-09-07 07:12:39.325064 agent_os_py-0.1.0/agents/lib/completions/completion_helpers.py
--rw-r--r--   0        0        0     1524 2023-09-07 07:12:39.325064 agent_os_py-0.1.0/agents/lib/completions/function_builder.py
--rw-r--r--   0        0        0     2477 2023-09-07 07:12:39.325064 agent_os_py-0.1.0/agents/lib/completions/prompt_builder.py
--rw-r--r--   0        0        0       75 2023-09-07 07:12:39.335897 agent_os_py-0.1.0/agents/lib/tools/__init__.py
--rw-r--r--   0        0        0     1627 2023-09-15 16:40:18.898934 agent_os_py-0.1.0/agents/lib/tools/data_parser.py
--rw-r--r--   0        0        0     1603 2023-09-07 10:10:02.498040 agent_os_py-0.1.0/agents/lib/tools/store_wrapper.py
--rw-r--r--   0        0        0     1615 2023-09-19 15:32:19.502751 agent_os_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    11061 2023-09-16 06:21:25.151871 agent_os_py-0.1.0/src/cli/aos.py
--rw-r--r--   0        0        0      431 2023-09-13 10:42:44.572481 agent_os_py-0.1.0/src/grit/__init__.py
--rw-r--r--   0        0        0     1008 2023-07-23 22:03:29.554456 agent_os_py-0.1.0/src/grit/object_model.py
--rw-r--r--   0        0        0     8765 2023-08-17 13:54:58.419032 agent_os_py-0.1.0/src/grit/object_serialization.py
--rw-r--r--   0        0        0      635 2023-07-23 21:59:13.216163 agent_os_py-0.1.0/src/grit/object_store.py
--rw-r--r--   0        0        0     1174 2023-09-13 10:42:29.072481 agent_os_py-0.1.0/src/grit/references.py
--rw-r--r--   0        0        0        0 2023-05-23 15:39:40.100000 agent_os_py-0.1.0/src/grit/stores/__init__.py
--rw-r--r--   0        0        0      140 2023-05-23 15:39:02.170000 agent_os_py-0.1.0/src/grit/stores/file/__init__.py
--rw-r--r--   0        0        0     3699 2023-08-17 13:57:20.140641 agent_os_py-0.1.0/src/grit/stores/file/file_object_store.py
--rw-r--r--   0        0        0     2507 2023-09-18 21:52:36.467422 agent_os_py-0.1.0/src/grit/stores/file/file_references.py
--rw-r--r--   0        0        0      204 2023-07-10 14:28:44.720369 agent_os_py-0.1.0/src/grit/stores/lmdb/__init__.py
--rw-r--r--   0        0        0     2092 2023-09-15 16:42:33.568011 agent_os_py-0.1.0/src/grit/stores/lmdb/lmdb_object_store.py
--rw-r--r--   0        0        0     2099 2023-09-15 16:55:01.576704 agent_os_py-0.1.0/src/grit/stores/lmdb/lmdb_references.py
--rw-r--r--   0        0        0     2286 2023-09-15 16:42:30.870513 agent_os_py-0.1.0/src/grit/stores/lmdb/shared_env.py
--rw-r--r--   0        0        0      152 2023-05-23 16:19:52.210000 agent_os_py-0.1.0/src/grit/stores/memory/__init__.py
--rw-r--r--   0        0        0      958 2023-08-17 13:54:21.423215 agent_os_py-0.1.0/src/grit/stores/memory/memory_object_store.py
--rw-r--r--   0        0        0      848 2023-07-09 10:18:07.306013 agent_os_py-0.1.0/src/grit/stores/memory/memory_references.py
--rw-r--r--   0        0        0     9755 2023-09-15 16:41:15.134730 agent_os_py-0.1.0/src/grit/tree_helpers.py
--rw-r--r--   0        0        0       99 2023-09-13 11:04:33.162418 agent_os_py-0.1.0/src/runtime/__init__.py
--rw-r--r--   0        0        0    18682 2023-09-17 19:05:50.205922 agent_os_py-0.1.0/src/runtime/actor_executor.py
--rw-r--r--   0        0        0    10397 2023-07-17 19:20:00.604606 agent_os_py-0.1.0/src/runtime/core_loader.py
--rw-r--r--   0        0        0     2470 2023-08-17 14:02:01.623022 agent_os_py-0.1.0/src/runtime/query_executor.py
--rw-r--r--   0        0        0    10328 2023-08-17 13:54:21.423215 agent_os_py-0.1.0/src/runtime/resolvers.py
--rw-r--r--   0        0        0    13169 2023-09-15 16:54:37.353387 agent_os_py-0.1.0/src/runtime/runtime.py
--rw-r--r--   0        0        0     9856 2023-09-15 16:48:18.392800 agent_os_py-0.1.0/src/runtime/runtime_executor.py
--rw-r--r--   0        0        0       79 2023-06-25 16:36:59.685475 agent_os_py-0.1.0/src/sync/__init__.py
--rw-r--r--   0        0        0    13030 2023-09-15 16:51:34.096838 agent_os_py-0.1.0/src/sync/actor_push.py
--rw-r--r--   0        0        0     8830 2023-09-18 21:52:36.467422 agent_os_py-0.1.0/src/sync/sync_file.py
--rw-r--r--   0        0        0     7363 2023-09-18 21:52:36.467422 agent_os_py-0.1.0/src/sync/sync_item.py
--rw-r--r--   0        0        0       34 2023-06-14 07:36:53.400000 agent_os_py-0.1.0/src/web/__init__.py
--rw-r--r--   0        0        0    22703 2023-09-15 16:50:39.821873 agent_os_py-0.1.0/src/web/web_server.py
--rw-r--r--   0        0        0      155 2023-07-17 14:18:33.775229 agent_os_py-0.1.0/src/wit/__init__.py
--rw-r--r--   0        0        0    46234 2023-09-18 21:52:36.467422 agent_os_py-0.1.0/src/wit/data_model.py
--rw-r--r--   0        0        0     5013 2023-07-23 22:06:09.400263 agent_os_py-0.1.0/src/wit/data_model_utils.py
--rw-r--r--   0        0        0      271 2023-07-14 13:46:52.352417 agent_os_py-0.1.0/src/wit/errors.py
--rw-r--r--   0        0        0     3373 2023-07-23 22:19:41.401797 agent_os_py-0.1.0/src/wit/wit_api.py
--rw-r--r--   0        0        0    29824 2023-09-17 18:54:52.753072 agent_os_py-0.1.0/src/wit/wit_routers.py
--rw-r--r--   0        0        0     2865 2023-09-15 16:55:01.576704 agent_os_py-0.1.0/src/wit/wit_state.py
--rw-r--r--   0        0        0     2502 2023-08-17 13:54:21.423215 agent_os_py-0.1.0/src/wit/wut.py
--rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 agent_os_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-24 02:56:14.252362 agent_os_py-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     4853 2024-04-12 09:20:00.299726 agent_os_py-0.1.1/README.md
+-rw-r--r--   0        0        0      343 2023-11-15 09:54:13.770144 agent_os_py-0.1.1/agents/jetpack/chat/artifacts.html
+-rw-r--r--   0        0        0     3666 2023-10-23 08:23:54.081039 agent_os_py-0.1.1/agents/jetpack/chat/chat_completions.py
+-rw-r--r--   0        0        0      374 2023-11-15 09:54:13.770144 agent_os_py-0.1.1/agents/jetpack/chat/chat_messages.html
+-rw-r--r--   0        0        0     2462 2023-09-17 12:35:58.217922 agent_os_py-0.1.1/agents/jetpack/chat/chat_queries.py
+-rw-r--r--   0        0        0    11166 2023-11-15 09:54:13.770144 agent_os_py-0.1.1/agents/jetpack/chat/chat_wit.py
+-rw-r--r--   0        0        0    17352 2023-10-23 08:23:54.081039 agent_os_py-0.1.1/agents/jetpack/coder/coder_completions.py
+-rw-r--r--   0        0        0    11274 2023-11-15 09:54:13.770144 agent_os_py-0.1.1/agents/jetpack/coder/coder_wit.py
+-rw-r--r--   0        0        0     3473 2023-10-21 00:28:19.152059 agent_os_py-0.1.1/agents/jetpack/coder/retriever_completions.py
+-rw-r--r--   0        0        0     6746 2023-11-15 09:54:13.770144 agent_os_py-0.1.1/agents/jetpack/coder/retriever_wit.py
+-rw-r--r--   0        0        0   217144 2023-10-23 08:23:54.091039 agent_os_py-0.1.1/agents/jetpack/design/design.css
+-rw-r--r--   0        0        0    13567 2023-10-23 08:23:54.091039 agent_os_py-0.1.1/agents/jetpack/design/design.html
+-rw-r--r--   0        0        0     1545 2023-10-23 08:23:54.091039 agent_os_py-0.1.1/agents/jetpack/frontend/frontend_queries.py
+-rw-r--r--   0        0        0     1164 2023-11-15 09:54:13.770144 agent_os_py-0.1.1/agents/jetpack/frontend/frontend_wit.py
+-rw-r--r--   0        0        0   228701 2023-11-15 09:54:13.770144 agent_os_py-0.1.1/agents/jetpack/frontend/index.html
+-rw-r--r--   0        0        0       58 2023-09-07 07:15:44.282515 agent_os_py-0.1.1/agents/jetpack/messages/__init__.py
+-rw-r--r--   0        0        0     2046 2023-09-07 07:15:44.282515 agent_os_py-0.1.1/agents/jetpack/messages/messages_chat.py
+-rw-r--r--   0        0        0     1009 2023-09-17 11:26:19.078508 agent_os_py-0.1.1/agents/jetpack/messages/messages_coder.py
+-rw-r--r--   0        0        0      703 2023-11-15 09:54:13.770144 agent_os_py-0.1.1/agents/jetpack/sync.toml
+-rw-r--r--   0        0        0        0 2023-09-08 09:19:16.095178 agent_os_py-0.1.1/agents/jetpack/tailwind.config.js
+-rw-r--r--   0        0        0      280 2023-09-07 07:12:39.325064 agent_os_py-0.1.1/agents/lib/completions/__init__.py
+-rw-r--r--   0        0        0     3107 2023-09-07 07:12:39.325064 agent_os_py-0.1.1/agents/lib/completions/completion_helpers.py
+-rw-r--r--   0        0        0     1524 2023-09-07 07:12:39.325064 agent_os_py-0.1.1/agents/lib/completions/function_builder.py
+-rw-r--r--   0        0        0     2477 2023-09-07 07:12:39.325064 agent_os_py-0.1.1/agents/lib/completions/prompt_builder.py
+-rw-r--r--   0        0        0       75 2023-09-07 07:12:39.335897 agent_os_py-0.1.1/agents/lib/tools/__init__.py
+-rw-r--r--   0        0        0     1627 2023-09-15 16:40:18.898934 agent_os_py-0.1.1/agents/lib/tools/data_parser.py
+-rw-r--r--   0        0        0     1603 2023-09-07 10:10:02.498040 agent_os_py-0.1.1/agents/lib/tools/store_wrapper.py
+-rw-r--r--   0        0        0     1909 2024-04-12 09:21:14.569703 agent_os_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11061 2023-09-16 06:21:25.151871 agent_os_py-0.1.1/src/cli/aos.py
+-rw-r--r--   0        0        0      451 2023-11-15 09:54:13.780144 agent_os_py-0.1.1/src/grit/__init__.py
+-rw-r--r--   0        0        0     1008 2023-07-23 22:03:29.554456 agent_os_py-0.1.1/src/grit/object_model.py
+-rw-r--r--   0        0        0     1655 2024-03-06 16:39:31.495577 agent_os_py-0.1.1/src/grit/object_model_v2.py
+-rw-r--r--   0        0        0     8765 2023-08-17 13:54:58.419032 agent_os_py-0.1.1/src/grit/object_serialization.py
+-rw-r--r--   0        0        0      635 2023-07-23 21:59:13.216163 agent_os_py-0.1.1/src/grit/object_store.py
+-rw-r--r--   0        0        0     1276 2023-11-15 09:54:13.780144 agent_os_py-0.1.1/src/grit/references.py
+-rw-r--r--   0        0        0        0 2023-05-23 15:39:40.100000 agent_os_py-0.1.1/src/grit/stores/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-23 15:39:02.170000 agent_os_py-0.1.1/src/grit/stores/file/__init__.py
+-rw-r--r--   0        0        0     3699 2023-08-17 13:57:20.140641 agent_os_py-0.1.1/src/grit/stores/file/file_object_store.py
+-rw-r--r--   0        0        0     2507 2023-09-18 21:52:36.467422 agent_os_py-0.1.1/src/grit/stores/file/file_references.py
+-rw-r--r--   0        0        0      204 2023-07-10 14:28:44.720369 agent_os_py-0.1.1/src/grit/stores/lmdb/__init__.py
+-rw-r--r--   0        0        0     2092 2023-09-15 16:42:33.568011 agent_os_py-0.1.1/src/grit/stores/lmdb/lmdb_object_store.py
+-rw-r--r--   0        0        0     2099 2023-09-15 16:55:01.576704 agent_os_py-0.1.1/src/grit/stores/lmdb/lmdb_references.py
+-rw-r--r--   0        0        0     2286 2023-09-15 16:42:30.870513 agent_os_py-0.1.1/src/grit/stores/lmdb/shared_env.py
+-rw-r--r--   0        0        0      152 2023-05-23 16:19:52.210000 agent_os_py-0.1.1/src/grit/stores/memory/__init__.py
+-rw-r--r--   0        0        0      958 2023-08-17 13:54:21.423215 agent_os_py-0.1.1/src/grit/stores/memory/memory_object_store.py
+-rw-r--r--   0        0        0      848 2023-07-09 10:18:07.306013 agent_os_py-0.1.1/src/grit/stores/memory/memory_references.py
+-rw-r--r--   0        0        0     9755 2023-09-15 16:41:15.134730 agent_os_py-0.1.1/src/grit/tree_helpers.py
+-rw-r--r--   0        0        0       99 2023-09-13 11:04:33.162418 agent_os_py-0.1.1/src/runtime/__init__.py
+-rw-r--r--   0        0        0    18950 2023-12-06 09:01:35.957563 agent_os_py-0.1.1/src/runtime/actor_executor.py
+-rw-r--r--   0        0        0    10397 2023-07-17 19:20:00.604606 agent_os_py-0.1.1/src/runtime/core_loader.py
+-rw-r--r--   0        0        0     2531 2023-12-06 09:01:35.957563 agent_os_py-0.1.1/src/runtime/query_executor.py
+-rw-r--r--   0        0        0     2353 2023-11-15 09:54:13.790144 agent_os_py-0.1.1/src/runtime/request_response_executor.py
+-rw-r--r--   0        0        0    10328 2023-08-17 13:54:21.423215 agent_os_py-0.1.1/src/runtime/resolvers.py
+-rw-r--r--   0        0        0    13785 2023-12-06 09:01:35.957563 agent_os_py-0.1.1/src/runtime/runtime.py
+-rw-r--r--   0        0        0     9856 2023-09-15 16:48:18.392800 agent_os_py-0.1.1/src/runtime/runtime_executor.py
+-rw-r--r--   0        0        0       79 2023-06-25 16:36:59.685475 agent_os_py-0.1.1/src/sync/__init__.py
+-rw-r--r--   0        0        0    12347 2023-11-15 09:54:13.790144 agent_os_py-0.1.1/src/sync/actor_push.py
+-rw-r--r--   0        0        0     8074 2023-11-15 09:54:13.790144 agent_os_py-0.1.1/src/sync/sync_file.py
+-rw-r--r--   0        0        0     7371 2024-04-12 09:08:39.789925 agent_os_py-0.1.1/src/sync/sync_item.py
+-rw-r--r--   0        0        0       34 2023-06-14 07:36:53.400000 agent_os_py-0.1.1/src/web/__init__.py
+-rw-r--r--   0        0        0    22703 2023-09-15 16:50:39.821873 agent_os_py-0.1.1/src/web/web_server.py
+-rw-r--r--   0        0        0      469 2023-12-06 09:01:35.957563 agent_os_py-0.1.1/src/wit/__init__.py
+-rw-r--r--   0        0        0    46491 2023-11-15 09:54:13.790144 agent_os_py-0.1.1/src/wit/data_model.py
+-rw-r--r--   0        0        0     5013 2023-07-23 22:06:09.400263 agent_os_py-0.1.1/src/wit/data_model_utils.py
+-rw-r--r--   0        0        0      271 2023-07-14 13:46:52.352417 agent_os_py-0.1.1/src/wit/errors.py
+-rw-r--r--   0        0        0     7378 2024-04-12 08:56:53.760125 agent_os_py-0.1.1/src/wit/prototype.py
+-rw-r--r--   0        0        0      264 2023-12-06 09:01:35.957563 agent_os_py-0.1.1/src/wit/query.py
+-rw-r--r--   0        0        0      295 2023-11-15 09:54:13.800144 agent_os_py-0.1.1/src/wit/request_response.py
+-rw-r--r--   0        0        0     3369 2023-10-01 09:29:45.760711 agent_os_py-0.1.1/src/wit/wit_api.py
+-rw-r--r--   0        0        0    30355 2023-12-06 09:01:35.957563 agent_os_py-0.1.1/src/wit/wit_routers.py
+-rw-r--r--   0        0        0     3303 2023-11-15 09:54:13.800144 agent_os_py-0.1.1/src/wit/wit_state.py
+-rw-r--r--   0        0        0     2502 2023-08-17 13:54:21.423215 agent_os_py-0.1.1/src/wit/wut.py
+-rw-r--r--   0        0        0     5978 1970-01-01 00:00:00.000000 agent_os_py-0.1.1/PKG-INFO
```

### Comparing `agent_os_py-0.1.0/LICENSE.txt` & `agent_os_py-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/README.md` & `agent_os_py-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   - The framework plays well with other AI libraries such as LangChain or LlamaIndex.
   - The system is designed for "[local-first](https://www.inkandswitch.com/local-first/)" agents that run on your machine, but it should also be possible to run parts of an agent in the cloud.
   - The data layer is made for longevity. We introduce a novel data structure that is inspired by Git. It's a content addressable storage that maintains your agent's history and memory and makes sure you never lose data.
   - An agent's primary purpose is not to run large language models on your machine (although that's possible too), but to provide a place to execute the code and functions that are generated by these models. It then composes these functions into larger features and routes events and data to them.
   - To demonstrate the power of the Agent OS, this project comes with a demo agent called ["Jetpack"](agents/README.md#jetpack) that can chat with you and write self-executing programs.
 
 
-<p><a href="https://www.youtube.com/embed/V8QpNic7b24" target="_blank"><img src="docs/images/agents-fig-1-jetpack-demo.png" alt="Jetpack Demo Video" width="700" /></a>
+<p><a href="https://www.youtube.com/watch?v=7HJXUMCDFks" target="_blank"><img src="docs/images/screenshot.png" alt="Jetpack Demo Video" width="700" /></a>
 <br>
 <small>Click the the image to watch a short demo on YouTube.</small>
 </p>
 
 
 ## Getting Started
 As long as the project is still in alpha, the best way to get started is to clone this repository.
@@ -41,14 +41,20 @@
 ```
 
 ## Test Drive an Agent 🤖 
 To run your first agent, put an `.env` file in the project root that contains an OpenAI API key. (It also works without an `.env` file or key if you just want to give the project a quick spin.)
 ```
 OPENAI_API_KEY=sk-myspecialkey
 ```
+### Agent Dependencies
+Some of the dependencies for the demo agents are optional and not part of the core Agent OS source. To install them, run:
+```
+poetry install --with agents
+```
+
 ### Jetpack Agent
 The ["Jetpack" agent](agents/README.md) demonstrates what the Agent OS can do and is geared towards end-to-end code generation and execution. It's a conversational agent that can accomplish various tasks for you. To run it, execute the following commands:
 ```
 poetry run aos -d agents/jetpack/ push
 poetry run aos -d agents/jetpack/ run
 ```
```

#### html2text {}

```diff
@@ -34,28 +34,30 @@
 (https://python-poetry.org/). Works on Linux, macOS, and Windows. Once cloned,
 `cd` into the repository and run: ``` poetry install ``` The project comes with
 a CLI that can be used to initiate and run agents. To see the available
 commands run: ``` poetry run aos --help ``` ## Test Drive an Agent ð¤ To run
 your first agent, put an `.env` file in the project root that contains an
 OpenAI API key. (It also works without an `.env` file or key if you just want
 to give the project a quick spin.) ``` OPENAI_API_KEY=sk-myspecialkey ``` ###
-Jetpack Agent The ["Jetpack" agent](agents/README.md) demonstrates what the
-Agent OS can do and is geared towards end-to-end code generation and execution.
-It's a conversational agent that can accomplish various tasks for you. To run
-it, execute the following commands: ``` poetry run aos -d agents/jetpack/ push
-poetry run aos -d agents/jetpack/ run ``` Jetpack comes with a web interface,
-and the Agent OS hosts a web server. To access the interface, browse to http://
-127.0.0.1:5000/ag/jetpack/wit/actors/frontend/query/web ## Project Structure *
-`agents/`: examples of agent implementations. [See the folder](agents/) for
-more details. * `jetpack/`: the flagship agent demo, geared towards
-conversational task completion through code generation. * `src/`: contains all
-relevant modules that are part of the Agent OS. * `grit/`: object store,
-inspired by Git. * `wit/`: libraries to help write "wit" state transition
-functions * `runtime/`: the Agent OS runtime: actor executor, custom python
-module loader, and wit function resolver. * `sync/`: modules to push and pull
-data into grit from the developer's file system. * `web/`: the web server that
-provides the web interface. * `cli/`: the "aos" (agent OS) CLI. * `tests/`:
-extensive unit tests that cover most of the `/src` packages and modules. *
-`docs/`: documentation, intended to be rendered as a GitBook. ## Running the
-Tests If you want to hack on the code, it is helpful to run the tests. The
-project uses `pytest` and has almost 100 unit tests. ``` poetry run pytest
-tests/ ```
+Agent Dependencies Some of the dependencies for the demo agents are optional
+and not part of the core Agent OS source. To install them, run: ``` poetry
+install --with agents ``` ### Jetpack Agent The ["Jetpack" agent](agents/
+README.md) demonstrates what the Agent OS can do and is geared towards end-to-
+end code generation and execution. It's a conversational agent that can
+accomplish various tasks for you. To run it, execute the following commands:
+``` poetry run aos -d agents/jetpack/ push poetry run aos -d agents/jetpack/
+run ``` Jetpack comes with a web interface, and the Agent OS hosts a web
+server. To access the interface, browse to http://127.0.0.1:5000/ag/jetpack/
+wit/actors/frontend/query/web ## Project Structure * `agents/`: examples of
+agent implementations. [See the folder](agents/) for more details. * `jetpack/
+`: the flagship agent demo, geared towards conversational task completion
+through code generation. * `src/`: contains all relevant modules that are part
+of the Agent OS. * `grit/`: object store, inspired by Git. * `wit/`: libraries
+to help write "wit" state transition functions * `runtime/`: the Agent OS
+runtime: actor executor, custom python module loader, and wit function
+resolver. * `sync/`: modules to push and pull data into grit from the
+developer's file system. * `web/`: the web server that provides the web
+interface. * `cli/`: the "aos" (agent OS) CLI. * `tests/`: extensive unit tests
+that cover most of the `/src` packages and modules. * `docs/`: documentation,
+intended to be rendered as a GitBook. ## Running the Tests If you want to hack
+on the code, it is helpful to run the tests. The project uses `pytest` and has
+almost 100 unit tests. ``` poetry run pytest tests/ ```
```

### Comparing `agent_os_py-0.1.0/agents/jetpack/chat/chat_completions.py` & `agent_os_py-0.1.1/agents/jetpack/chat/chat_completions.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         So, if the function is changing data, retrieving data, or generating content, you can expect it to return not the actual data but just an id to the result.
 
         Since we are generating code, it is also necessary to have an example of how to call the function. 
         For example, if the function is called "download_image", then you should ask the user to give an example of a real URL to use for testing.
 
         You can access the web, internal URLs, the file system, and so on, because you can write and execute code.
 
+        When the request is to retreive some data, do not ask for the structure of the data, assume it will be determiend later by the coder system.
+        
         Once the code is written, either request changes (code_request) to the code because the user mentioned changes, or call the code because the user asked for a code execution (code_exec).
 
         Whenever the user asks you modify or call a function make the actual function call--do not just copy previous output.
         """)
     
     for msg in messages:
         prompt.append_msg(msg.content, msg.from_name, clean_whitespace=False)
```

### Comparing `agent_os_py-0.1.0/agents/jetpack/chat/chat_queries.py` & `agent_os_py-0.1.1/agents/jetpack/chat/chat_queries.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/agents/jetpack/chat/chat_wit.py` & `agent_os_py-0.1.1/agents/jetpack/chat/chat_wit.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,35 @@
 from grit import *
 from wit import *
 from jetpack.messages import *
 from jetpack.coder.coder_wit import create_coder_actor
 from jetpack.coder.retriever_wit import create_retriever_actor
 from jetpack.chat.chat_completions import chat_completion
 
+
+#========================================================================================
+# Setup & State
+#
+# A "chat" limits a conversation to a single topic and goal. 
+# Each chat corresponds to a single chat window in Jetpack.
+#========================================================================================
 logger = logging.getLogger(__name__)
 
-# A "chat" limits a conversation to a single topic and goal. Each chat corresponds to a single chat window in Jetpack.
+async def create_chat_actor(
+        ctx:MessageContext,
+        name:str="Main"
+        ) -> ActorId:
+    state = ChatState()
+    state.name = name
+    return await create_actor_from_prototype_with_state(
+        ctx.prototype_actors["chat"], 
+        state, 
+        ctx.request_response, 
+        ctx.store)
+
 
 class ChatState(WitState):
     name:str="Main"
 
     retriever:ActorId|None = None
     coder:ActorId|None = None
 
@@ -20,69 +38,31 @@
     code_plan:CodePlanned|None = None
     code_spec:CodeSpec|None = None
     code_deploy:CodeDeployed|None = None
     code_fail:CodeFailed|None = None
     current_execution:CodeExecution|None = None
     last_result:CodeExecuted|None = None
 
-async def create_chat_actor(
-        store:ObjectStore, 
-        name:str="Main", #allows the differentiation of multiple scopes
-        templates:TreeId=None,
-        wit_ref:str|None=None,
-        wit_query_ref:str|None=None,
-        ) -> OutboxMessage:
-    #TODO: how to know if this should be external or loaded from a core?
-    if wit_ref is not None:
-        core = Core.from_external_wit_ref(store, wit_ref=wit_ref)
-    else:
-        core = Core.from_external_wit_ref(store, "chat_wit:app")
-    if wit_query_ref is not None:
-        core.makeb("wit_query").set_as_str("external:"+wit_query_ref)
-    else:
-        core.makeb("wit_query").set_as_str("external:chat_queries:app")
-
-    args = core.maket('args')
-    if name is not None:
-        args.makeb('name').set_as_str(name)
-    #add the templates to the core
-    if templates is not None:
-        core.add("templates", templates)
-
-    genesis_msg = await OutboxMessage.from_genesis(store, core)
-    return genesis_msg
-
-
+#========================================================================================
+# Wit
+#========================================================================================
 app = Wit()
 
-
 @app.genesis_message
 async def on_genesis(msg:InboxMessage, ctx:MessageContext, state:ChatState) -> None:
     logger.info("received genesis")
     
-    args:TreeObject = await ctx.core.get('args')
-    if args is not None:
-        logger.info("loading args")
-        if 'name' in args:
-            state.name = (await args.getb('name')).get_as_str()
-            logger.info(f"'{state.name}': new chat actor created")
-
-    if state.name is None:
-        state.name = "Main"
-
     #create the downstream actors
-    coder_msg = await create_coder_actor(ctx.store, name=f"{state.name} Coder")
-    state.coder = coder_msg.recipient_id
-    ctx.outbox.add(coder_msg)
-    logger.info(f"'{state.name}': created coder actor %s", coder_msg.recipient_id.hex())
-
-    retriever_msg = await create_retriever_actor(ctx.store, forward_to=state.coder)
-    state.retriever = retriever_msg.recipient_id
-    ctx.outbox.add(retriever_msg)
-    logger.info(f"'{state.name}': created retriever actor %s", retriever_msg.recipient_id.hex())
+    coder_id = await create_coder_actor(ctx, name=f"{state.name} Coder")
+    state.coder = coder_id
+    logger.info(f"'{state.name}': created coder actor {coder_id.hex()}")
+
+    retriever_id = await create_retriever_actor(ctx, forward_to=state.coder)
+    state.retriever = retriever_id
+    logger.info(f"'{state.name}': created retriever actor {retriever_id.hex()}")
 
 
 @app.message("web")
 async def on_message_web(content:str, ctx:MessageContext, state:ChatState) -> None:
     logger.info(f"'{state.name}': received message from user")
     # save in the core
     msgt = await ctx.core.gett("messages")
@@ -194,16 +174,16 @@
         ctx.outbox.add_new_msg(ctx.agent_id, "artifact", mt="artifact")
 
 @app.message("code_deployed")
 async def on_message_code_deployed(code:CodeDeployed, ctx:MessageContext, state:ChatState) -> None:
     logger.info(f"'{state.name}': received callback: code_deployed")
     state.code_deploy = code
     if state.code_deploy.code is not None:
-        # render the code and notify frontend
-        chat_message = ChatMessage.from_actor(f"Here is the function and code I generated:\n```\n{code.code}\n```\n", ctx.actor_id)
+        # notify frontend
+        chat_message = ChatMessage.from_actor("**Igenerated the function and deployed it.**  \nYou can view it in the artifacts on the right.", ctx.actor_id)
         messages_tree = await ctx.core.gett("messages")
         messages_tree.makeb(str(chat_message.id), True).set_as_json(chat_message)
         ctx.outbox.add_new_msg(ctx.agent_id, str(chat_message.id), mt="receipt")
         ctx.outbox.add_new_msg(ctx.agent_id, "artifact", mt="artifact")
 
 @app.message("code_executed")
 async def on_message_code_executed(exec:CodeExecuted, ctx:MessageContext, state:ChatState) -> None:
```

### Comparing `agent_os_py-0.1.0/agents/jetpack/coder/coder_completions.py` & `agent_os_py-0.1.1/agents/jetpack/coder/coder_completions.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,14 +156,17 @@
         "openai", 
         "pandas", 
         "requests", 
         "PIL",
         "scipy",
         "numpy",
         "sklearn",
+        "yfinance",
+        "matplotlib",
+        "openpyxl",
         ]
     prompt.append_to_prev(", ".join(third_party_modules))
 
     if data_examples is not None:
         for data_location, data_example in data_examples.items():
             prompt.append_msg("Here is an example of data at location: "+data_location)
             prompt.append_to_prev_code(data_example, codetype="")
@@ -324,14 +327,15 @@
         "openai", 
         "pandas", 
         "requests", 
         "PIL",
         "scipy",
         "numpy",
         "sklearn",
+        "openpyxl",
         ]
     prompt.append_to_prev(", ".join(third_party_modules))
     #end copied
 
     prompt.append_msg("Here is the task that the Python module needs to accomplish: " + task_description)
 
     prompt.append_msg("Let's describe the desired input and output of the entry function.")
```

### Comparing `agent_os_py-0.1.0/agents/jetpack/coder/coder_wit.py` & `agent_os_py-0.1.1/agents/jetpack/coder/coder_wit.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,96 +3,72 @@
 from wit import *
 from wit.wit_routers import _Wrapper
 from runtime import CoreResolver
 from tools import StoreWrapper
 from jetpack.messages import *
 from jetpack.coder.coder_completions import *
 
+#========================================================================================
+# Setup & State
+#========================================================================================
 logger = logging.getLogger(__name__)
 
+async def create_coder_actor(
+        ctx:MessageContext,
+        name:str="coder",
+        spec:CodeSpec|None=None,
+        job_execution:CodeExecution|None=None,
+        ) -> ActorId:
+    state = CoderState()
+    state.name = name
+    state.code_spec = spec
+    state.job_execution = job_execution
+    state.notify.add(ctx.actor_id)
+    return await create_actor_from_prototype_with_state(
+        ctx.prototype_actors["coder"], 
+        state, 
+        ctx.request_response, 
+        ctx.store)
+
+
 class CoderState(WitState):
     name:str = "coder"
     notify:set[ActorId] = set()
 
     code_spec:CodeSpec|None = None
     code_plan:str|None = None
     code_tries_max:int = 3
     code_tries:int = 0
     code_errors:str|None = None
     job_execution:CodeExecution|None = None
 
-def reset_code(state:CoderState):
-    state.code_plan = None
-    state.code_tries = 0
-    state.code_tries_max = 3
-    state.code_errors = None
-
-
-def notify_all(state:CoderState, outbox:Outbox, msg:any, mt:str|None=None):
-    for actor_id in state.notify:
-        outbox.add_new_msg(actor_id, msg, mt=mt)
-
-async def create_coder_actor(
-        store:ObjectStore, 
-        name:str="coder", #allows the differentiation of multiple coders
-        spec:CodeSpec|None=None,
-        job_execution:CodeExecution|None=None,
-        wit_ref:str|None=None,
-        ) -> OutboxMessage:
-    #TODO: how to know if this should be external or loaded from a core?
-    if wit_ref is not None:
-        core = Core.from_external_wit_ref(store, wit_ref=wit_ref)
-    else:
-        core = Core.from_external_wit_ref(store, "coder_wit:app")
-
-    args = core.maket('args')
-    if name is not None:
-        args.makeb('name').set_as_str(name)
-    if spec is not None:
-        args.makeb('code_spec').set_as_json(spec)
-    if job_execution is not None:
-        args.makeb('job_execution').set_as_json(job_execution)
-    
-    genesis_msg = await OutboxMessage.from_genesis(store, core)
-    return genesis_msg
-
-
+#========================================================================================
+# Wit
+#========================================================================================
 app = Wit()
 
 @app.genesis_message
-async def on_genesis_message(msg:InboxMessage, core:Core, state:CoderState, outbox:Outbox, actor_id:ActorId):
+async def on_genesis_message(msg:InboxMessage, state:CoderState, ctx:MessageContext,):
     logger.info("on_genesis_message")
-    #copy args into state
-    args:TreeObject = await core.get('args')
-    if args is not None:
-        logger.info("loading args")
-        if 'name' in args:
-            state.name = (await args.getb('name')).get_as_str()
-        if 'code_spec' in args:
-            state.code_spec = (await args.getb('code_spec')).get_as_model(CodeSpec)
-        if 'job_execution' in args:
-            state.job_execution = (await args.getb('job_execution')).get_as_model(CodeExecution)
-        # add the sender to the notify list
-        # only if args are provided, because we can assume the sender is another actor
-        state.notify.add(msg.sender_id)
     logger.info("is job: %s", state.job_execution is not None)
     # if code specs were provided, move right to the spec state
     # and send message to move on to the plan state 
     if state.code_spec is not None:
         reset_code(state)
-        outbox.add_new_msg(actor_id, "plan", mt="plan")
+        ctx.outbox.add_new_msg(ctx.actor_id, "plan", mt="plan")
+
 
 @app.message("spec")
-async def on_spec_message(spec:CodeSpec, msg:InboxMessage, state:CoderState, outbox:Outbox, actor_id:ActorId):
+async def on_spec_message(spec:CodeSpec, state:CoderState, ctx:MessageContext):
     logger.info("on_spec_message")
     state.code_spec = spec
     reset_code(state)
-    state.notify.add(msg.sender_id)
-    outbox.add_new_msg(actor_id, "plan", mt="plan")
-    notify_all(state, outbox, spec, mt="code_speced")
+    state.notify.add(ctx.message.sender_id)
+    ctx.outbox.add_new_msg(ctx.actor_id, "plan", mt="plan")
+    notify_all(state, ctx.outbox, spec, mt="code_speced")
 
 
 @app.message("plan")
 async def on_plan_message(msg:InboxMessage, state:CoderState, ctx:MessageContext):
     logger.info("on_plan_message")
     if state.code_spec.input_spec is None or state.code_spec.output_spec is None:
         logger.info("generating input and/or output specs")
@@ -267,7 +243,18 @@
         return
 
 @app.message("fail")
 async def on_fail_message(msg:InboxMessage, state:CoderState, ctx:MessageContext):
     logger.info("on_fail_message")
     notify_all(state, ctx.outbox, CodeFailed(errors=state.code_errors), mt="code_failed")
 
+
+
+def reset_code(state:CoderState):
+    state.code_plan = None
+    state.code_tries = 0
+    state.code_tries_max = 3
+    state.code_errors = None
+
+def notify_all(state:CoderState, outbox:Outbox, msg:any, mt:str|None=None):
+    for actor_id in state.notify:
+        outbox.add_new_msg(actor_id, msg, mt=mt)
```

### Comparing `agent_os_py-0.1.0/agents/jetpack/coder/retriever_completions.py` & `agent_os_py-0.1.1/agents/jetpack/coder/retriever_completions.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/agents/jetpack/coder/retriever_wit.py` & `agent_os_py-0.1.1/agents/jetpack/coder/retriever_wit.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,50 @@
 import logging
 from grit import *
 from wit import *
 from jetpack.messages import *
 from jetpack.coder.retriever_completions import *
 from jetpack.coder.coder_wit import create_coder_actor
 
+#========================================================================================
+# Setup & State
+#========================================================================================
 logger = logging.getLogger(__name__)
 
+async def create_retriever_actor(
+        ctx:MessageContext,
+        request:CodeRequest|None=None,
+        forward_to:ActorId|None=None,
+        ) -> ActorId:
+    state = RetrieverState()
+    state.code_request = request
+    state.forward_to = forward_to
+    state.notify.add(ctx.actor_id)
+    return await create_actor_from_prototype_with_state(
+        ctx.prototype_actors["retriever"], 
+        state, 
+        ctx.request_response, 
+        ctx.store)
+
 class RetrieverState(WitState):
     code_request:CodeRequest|None = None
     locations:list[str]|None = None
     retrieval_coders:dict[ActorId,str]|None = None
     retrieved_data:dict[str,str]|None = None
     notify:set[ActorId] = set()
     forward_to:ActorId|None = None
 
-    def __init__(self):
-        super().__init__()
-
-def notify_all(state:RetrieverState, outbox:Outbox, msg:any, mt:str|None=None):
-    for actor_id in state.notify:
-        outbox.add_new_msg(actor_id, msg, mt=mt)
-
-async def create_retriever_actor(
-        store:ObjectStore, 
-        request:CodeRequest|None=None,
-        forward_to:ActorId|None=None,
-        wit_ref:str|None=None,
-        ) -> OutboxMessage:
-    #TODO: how to know if this should be external or loaded from a core?
-    if wit_ref is not None:
-        core = Core.from_external_wit_ref(store, wit_ref=wit_ref)
-    else:
-        core = Core.from_external_wit_ref(store, "retriever_wit:app")
-
-    args = core.maket('args')
-    if request is not None:
-        args.makeb('code_request').set_as_json(request)
-    if forward_to is not None:
-        args.makeb('forward_to').set_as_bytes(forward_to)
-    
-    genesis_msg = await OutboxMessage.from_genesis(store, core)
-    return genesis_msg
-
-
+#========================================================================================
+# Wit
+#========================================================================================
 app = Wit()
 
 @app.genesis_message
 async def on_genesis_message(msg:InboxMessage, core:Core, state:RetrieverState, outbox:Outbox, actor_id:ActorId):
     logger.info("on_genesis_message")
-    #copy args into state
-    args:TreeObject = await core.get('args')
-    if args is not None:
-        logger.info("loading args")
-        if 'code_request' in args:
-            state.code_request = (await args.getb('code_request')).get_as_model(CodeRequest)
-        if 'forward_to' in args:
-            forward_to = (await args.getb('forward_to')).get_as_bytes()
-            logger.info("forward_to: %s", forward_to.hex())
-            state.forward_to = forward_to
-        # add the sender to the notify list
-        # only if args are provided, because we can assume the sender is another actor
-        state.notify.add(msg.sender_id)
     # if code specs were provided, move right to the plan
     # and send message to move on to the plan state 
     if state.code_request is not None:
         outbox.add_new_msg(actor_id, "plan", mt="plan")
 
 @app.message("request")
 async def on_request_message(request:CodeRequest, msg:InboxMessage, state:RetrieverState, outbox:Outbox, actor_id:ActorId):
@@ -92,15 +71,15 @@
     else:
         logger.info("no retrievals needed")
         state.locations = None
         state.retrieved_data = None
         ctx.outbox.add_new_msg(ctx.actor_id, "complete", mt="complete")
 
 @app.message("retrieve")
-async def on_retrieve_message(msg:InboxMessage, state:RetrieverState, outbox:Outbox, actor_id:ActorId, store:ObjectStore):
+async def on_retrieve_message(msg:InboxMessage, state:RetrieverState, ctx:MessageContext):
     logger.info("on_retrieve_message")
     state.retrieval_coders = {}
     if state.retrieved_data is None:
         state.retrieved_data = {}
     for location in state.locations:
         #check if the data was already retrieved
         if location in state.retrieved_data:
@@ -113,38 +92,38 @@
         ```
         However, before we can write the code, we need to understand what the structure of the data is at the following location:
         ```
         {location}
         ```
         Whatever the format of the data at that location, we need to retrieve it and return it as a string (`contents`).
         Do not take any inputs to the function, just use the location as a variable inside the code.
+        To retrieve the schema, do not use the openpyxl library, just use requests.
         """
 
         retrieve_spec = CodeSpec(
             task_description=task_description,
             input_spec=CodeSpec.empty_inputoutput_spec(),
             output_spec=json.loads('{"properties": {"contents": {"title": "Contents of Location", "type": "string"}}, "required": ["contents"], "type": "object"}'),
             input_examples=[json.dumps(CodeSpec.empty_inputoutput_spec())]
             )
         retrieve_job = CodeExecution(
             input_arguments=json.loads('{"type": "object", "properties": {}}'),
             input_description=None,
         )
-        retrieve_msg = await create_coder_actor(
-            store, 
+        coder_id = await create_coder_actor(
+            ctx, 
             f"retrieve: {location}",
             retrieve_spec,
             retrieve_job)
-        outbox.add(retrieve_msg)
-        state.retrieval_coders[retrieve_msg.recipient_id] = location
+        state.retrieval_coders[coder_id] = location
         state.retrieved_data[location] = None
     
     #if no retrievals coders were needed, move on to the completed state
     if len(state.retrieval_coders) == 0:
-        outbox.add_new_msg(actor_id, "complete", mt="complete")
+        ctx.outbox.add_new_msg(ctx.actor_id, "complete", mt="complete")
 
 @app.message("complete")
 async def on_complete_message(msg:InboxMessage, state:RetrieverState, outbox:Outbox, actor_id:ActorId):
     logger.info("on_complete_message")
     if state.forward_to is not None:
         spec = CodeSpec(
             task_description=state.code_request.task_description,
@@ -170,7 +149,12 @@
         location = state.retrieval_coders[ctx.message.sender_id]
         state.retrieved_data[location] = exec.output['contents']
         logger.info("retrieved data for location:", location, state.retrieved_data[location])
         state.retrieval_coders.pop(ctx.message.sender_id)
         if len(state.retrieval_coders) == 0:
             ctx.outbox.add_new_msg(ctx.actor_id, "complete", mt="complete")
 
+
+
+def notify_all(state:RetrieverState, outbox:Outbox, msg:any, mt:str|None=None):
+    for actor_id in state.notify:
+        outbox.add_new_msg(actor_id, msg, mt=mt)
```

### Comparing `agent_os_py-0.1.0/agents/jetpack/frontend/frontend_queries.py` & `agent_os_py-0.1.1/agents/jetpack/frontend/frontend_queries.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     template_kwargs = {
         'agent_id': ctx.agent_id.hex(),
         'frontend_id': ctx.actor_id.hex(),
         'chat_actors': {k:v.hex() for k,v in state.chat_actors.items()},
         'chat_titles': state.chat_titles,
         'current_chat': current_chat,
         'current_chat_id': state.chat_actors[current_chat].hex(),
+        'current_chat_title': state.chat_titles[current_chat],
         }
     return await render_template(ctx.core, "/templates/index.html", **template_kwargs)
 
 env = Environment(autoescape=select_autoescape())
 async def render_template(core:Core, template_path, **kwargs) -> BlobObject:
     template_blob = await core.get_path(template_path)
     if(template_blob is None):
```

### Comparing `agent_os_py-0.1.0/agents/jetpack/frontend/frontend_wit.py` & `agent_os_py-0.1.1/agents/jetpack/frontend/frontend_wit.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,27 +22,18 @@
 @app.message('create-chat')
 async def on_create_chat(chat:dict, ctx:MessageContext, state:FrontendState) -> None:
     logger.info("received create chat")
     title = chat['name']
     slug = await create_chat(title, ctx, state)
     ctx.outbox.add_reply_msg(ctx.message, slug, mt="new-chat")
 
-
 async def create_chat(title:str, ctx:MessageContext, state:FrontendState):
-    #find the templates to pass to the new chat
-    templ = await ctx.core.get("templates")
-    if templ is None:
-        raise Exception("templates not found")
-    templ_id = templ.get_as_object_id()
-
     #create the chat
     slug = slugify(title)
-    genesis_msg = await create_chat_actor(ctx.store, name=slug, templates=templ_id)
-    ctx.outbox.add(genesis_msg)
-    state.chat_actors[slug] = genesis_msg.recipient_id
+    chat_id = await create_chat_actor(ctx, name=slug)
+    state.chat_actors[slug] = chat_id
     state.chat_titles[slug] = title
     return slug
 
-
-def slugify(text):
+def slugify(text:str):
     text = text.lower()
     return re.sub(r'[\W_]+', '-', text)
```

### Comparing `agent_os_py-0.1.0/agents/jetpack/messages/messages_chat.py` & `agent_os_py-0.1.1/agents/jetpack/messages/messages_chat.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/agents/jetpack/messages/messages_coder.py` & `agent_os_py-0.1.1/agents/jetpack/messages/messages_coder.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/agents/lib/completions/completion_helpers.py` & `agent_os_py-0.1.1/agents/lib/completions/completion_helpers.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/agents/lib/completions/function_builder.py` & `agent_os_py-0.1.1/agents/lib/completions/function_builder.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/agents/lib/completions/prompt_builder.py` & `agent_os_py-0.1.1/agents/lib/completions/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/agents/lib/tools/data_parser.py` & `agent_os_py-0.1.1/agents/lib/tools/data_parser.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/agents/lib/tools/store_wrapper.py` & `agent_os_py-0.1.1/agents/lib/tools/store_wrapper.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/pyproject.toml` & `agent_os_py-0.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agent-os-py"
-version = "0.1.0"
+version = "0.1.1"
 description = "A library and runtime to build autonomous AI agents."
 authors = []
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "grit", from = "src"}, 
     {include = "wit", from = "src"}, 
@@ -22,36 +22,52 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 python-dotenv = "^1.0.0"
 pydantic = "^2.0.1"
 aiofiles = "^23.1.0"
 async-lru = "^2.0.2"
-pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 tomlkit = "^0.11.8"
 lmdb = "^1.4.1"
 watchfiles = "^0.19.0"
 starlette = "^0.28.0"
 sse-starlette = "^1.6.1"
 uvicorn = "^0.22.0"
-httpx = "^0.24.1"
-httpx-sse = ">=0.3.0,<0.4.0"
-jinja2 = "^3.1.2"
 click = "^8.1.5"
-openai = "^0.27.8"
-pandas = "^1.5.3"
+filetype = "^1.2.0"
+
+[tool.poetry.group.test.dependencies]
+pytest = "^8.1.1"
+httpx = "^0.27.0"
+httpx-sse = "^0.4.0"
+
+
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.3.7"
+
+
+# to install run poetry install --with agents
+[tool.poetry.group.agents]
+optional = true
+
+[tool.poetry.group.agents.dependencies]
+jinja2 = "^3.1.3"
+openai = "^1.17.0"
+pandas = "^2.2.2"
 requests = "^2.31.0"
-pillow = "^10.0.0"
-scikit-learn = "^1.3.0"
+pillow = "^10.3.0"
+scikit-learn = "^1.4.2"
 transitions = "^0.9.0"
-beautifulsoup4 = "^4.12.2"
-mistune = "^3.0.1"
-filetype = "^1.2.0"
-ruff = "^0.0.285"
+beautifulsoup4 = "^4.12.3"
+mistune = "^3.0.2"
+yfinance = "^0.2.37"
+matplotlib = "^3.8.4"
+openpyxl = "^3.1.2"
+jsonschema = "^4.21.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
@@ -59,12 +75,12 @@
 [tool.poetry.scripts]
 aos = "cli.aos:cli"
 perf = "tests.perf.perf:main"
 gen = "examples.coder.generator.gen_workbench:main"
 
 [tool.ruff]
 select = ["E", "F", "B"]
-ignore = ["F403", "F405"]
+ignore = ["F403", "F405", "E501"]
 line-length = 150
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401", "E402"]
```

### Comparing `agent_os_py-0.1.0/src/cli/aos.py` & `agent_os_py-0.1.1/src/cli/aos.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/grit/object_model.py` & `agent_os_py-0.1.1/src/grit/object_model.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/grit/object_serialization.py` & `agent_os_py-0.1.1/src/grit/object_serialization.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/grit/object_store.py` & `agent_os_py-0.1.1/src/grit/object_store.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/grit/references.py` & `agent_os_py-0.1.1/src/grit/references.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,12 +32,15 @@
     if(isinstance(actor_id, ActorId)):
         actor_id = actor_id.hex()
     return f"heads/{actor_id}"
 
 def ref_actor_name(actor_name_ref:str) -> str:
     return f"actors/{actor_name_ref}"
 
+def ref_prototype_name(prototype_name_ref:str) -> str:
+    return f"prototypes/{prototype_name_ref}"
+
 def ref_runtime_actor_name(actor_name_ref:str) -> str:
     return f"runtime/{actor_name_ref}"
 
 def ref_runtime_agent() -> str:
     return "runtime/agent"
```

### Comparing `agent_os_py-0.1.0/src/grit/stores/file/file_object_store.py` & `agent_os_py-0.1.1/src/grit/stores/file/file_object_store.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/grit/stores/file/file_references.py` & `agent_os_py-0.1.1/src/grit/stores/file/file_references.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/grit/stores/lmdb/lmdb_object_store.py` & `agent_os_py-0.1.1/src/grit/stores/lmdb/lmdb_object_store.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/grit/stores/lmdb/lmdb_references.py` & `agent_os_py-0.1.1/src/grit/stores/lmdb/lmdb_references.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/grit/stores/lmdb/shared_env.py` & `agent_os_py-0.1.1/src/grit/stores/lmdb/shared_env.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/grit/stores/memory/memory_object_store.py` & `agent_os_py-0.1.1/src/grit/stores/memory/memory_object_store.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/grit/stores/memory/memory_references.py` & `agent_os_py-0.1.1/src/grit/stores/memory/memory_references.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/grit/tree_helpers.py` & `agent_os_py-0.1.1/src/grit/tree_helpers.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/runtime/actor_executor.py` & `agent_os_py-0.1.1/src/runtime/actor_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,51 +2,54 @@
 import logging
 import asyncio
 import inspect
 from typing import Awaitable, Callable
 from grit import *
 from wit import *
 from .resolvers import Resolver
-from .query_executor import QueryExecutor
 
 MailboxUpdate = tuple[ActorId, ActorId, MessageId] # sender_id, recipient_id, message_id
 MailboxUpdateCallback = Callable[[set[MailboxUpdate]], Awaitable[None]]
 
 class GenesisMessageNotReadyError(Exception):
     pass
 
 class ExecutionContext:
     store:ObjectStore
     references:References
     resolver:Resolver
-    query_executor:QueryExecutor
     agent_name:str
     agent_id:ActorId
     async_semaphore:asyncio.Semaphore|None
     sync_semaphore:asyncio.Semaphore|None
+    named_actors:dict[str,ActorId]
+    prototype_actors:dict[str,ActorId]
+    query:Query
+    request_response:RequestResponse
 
     def __init__(self):
         self.store = None
         self.references = None
         self.resolver = None
-        self.query_executor = None
         self.agent_name = None
         self.agent_id = None
         self.async_semaphore = None
         self.sync_semaphore = None
+        self.named_actors = {}
+        self.prototype_actors = {}
+        self.query = None
+        self.request_response = None
 
     @classmethod
     def from_store(cls, store:ObjectStore, references:References, resolver:Resolver, agent_id:ActorId) -> ExecutionContext:
         ctx = cls()
         ctx.store = store
         ctx.references = references
         ctx.resolver = resolver
         ctx.agent_id = agent_id
-        ctx.query_executor = None
-        ctx.agent_name = None
         return ctx
     
 class ActorExecutor:
     '''Runs an actor's steps whenever new inbox messages arrive. Use factory methods to create an instance.'''
     ctx:ExecutionContext
     actor_id:ActorId
     
@@ -341,14 +344,18 @@
         args = (self.last_step_id, self.new_inbox)
         kwargs = {
             'agent_id': ctx.agent_id,
             'actor_id': self.actor_id,
             'object_store': ctx.store,
             'store': ctx.store,
             'cancel_event': self.cancel_event,
+            'named_actors': ctx.named_actors,
+            'prototype_actors': ctx.prototype_actors,
+            'query': ctx.query,
+            'request_response': ctx.request_response,
         }
         task_name = f'wit_function_{self.actor_id}'
         if(self.is_async):
             #if there is a semaphore that limits how many async wits can execute in parallel, use it
             if ctx.async_semaphore is not None:
                 async with ctx.async_semaphore:
                     self.run_task = asyncio.create_task(self.func(*args, **kwargs), name=task_name)
```

### Comparing `agent_os_py-0.1.0/src/runtime/core_loader.py` & `agent_os_py-0.1.1/src/runtime/core_loader.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/runtime/query_executor.py` & `agent_os_py-0.1.1/src/runtime/query_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 from grit import *
 from wit.errors import QueryError
+from wit.query import Query
 from .resolvers import Resolver
 
-class QueryExecutor:
+class QueryExecutor(Query):
     """Executes wit queries against an actor's head step."""
     loader:ObjectLoader
     references:References
     resolver:Resolver
     agent_id:ActorId
     
     def __init__(self, 
@@ -44,14 +45,15 @@
             raise QueryError(f"Actor '{actor_id_str}' has no query function.")
         args = (current_step_id, query_name, context)
         kwargs ={
             'loader': self.loader,
             'object_loader': self.loader,
             'actor_id': actor_id,
             'agent_id': self.agent_id,
+            'query': self
         } 
         try:
             result = await query_func(*args, **kwargs)
             return result
         except Exception as e:
             raise QueryError(f"Query '{query_name}' to '{actor_id_str}', with step '{current_step_id_str}', failed with an exception: {e}") from e
```

### Comparing `agent_os_py-0.1.0/src/runtime/resolvers.py` & `agent_os_py-0.1.1/src/runtime/resolvers.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/runtime/runtime.py` & `agent_os_py-0.1.1/src/runtime/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import asyncio
 from grit import *
 from wit import *
 from .resolvers import *
 from .query_executor import QueryExecutor
 from .actor_executor import ExecutionContext, ActorExecutor, MailboxUpdate
 from .runtime_executor import RuntimeExecutor, agent_id_from_name
+from .request_response_executor import RequestResponseExecutor
 
 logger = logging.getLogger(__name__)
 
 class Runtime:
     """The main runtime API to run an agent."""
 
     ctx:ExecutionContext
@@ -45,15 +46,15 @@
             self.ctx.resolver = MetaResover.with_all(store)
 
         #if no agent_name was provided, it will be loaded later, in __init_agent_executor 
         if agent_name is not None:
             self.ctx.agent_name = agent_name
             self.ctx.agent_id = agent_id_from_name(agent_name)
 
-        self.ctx.query_executor = QueryExecutor(self.ctx.store, self.ctx.references, self.ctx.resolver, self.ctx.agent_id)
+        self.ctx.query = QueryExecutor(self.ctx.store, self.ctx.references, self.ctx.resolver, self.ctx.agent_id)
 
         self.__cancel_event = asyncio.Event()
         self.__running_event = asyncio.Event()
         self.__executors = {}
         self.__runtime_executor = None
         self.__outbox_queue = asyncio.Queue()
         self.__executor_lock = asyncio.Lock()
@@ -73,15 +74,15 @@
     def references(self) -> References:
         return self.ctx.references
     @property
     def resolver(self) -> Resolver:
         return self.ctx.resolver
     @property
     def query_executor(self) -> QueryExecutor:
-        return self.ctx.query_executor
+        return self.ctx.query
 
     #todo: add lock around __executors
     def get_actors(self) -> list[ActorId]:
         return list(self.__executors.keys())
     
     def actor_exists(self, actor_id:ActorId) -> bool:
         return actor_id in self.__executors
@@ -125,27 +126,31 @@
             if(self.__runtime_executor is not None):
                 return
             #TODO: support loading the agent even if no name was provided, from the refs and core
             self.__runtime_executor = await RuntimeExecutor.from_agent_name(self.ctx, self.agent_name)
             if(self.agent_id != self.__runtime_executor.agent_id):
                 raise Exception(f"Agent name {self.agent_name} with id '{self.agent_id.hex()}' does not match the agent executor id "+
                                 f"'{self.__runtime_executor.agent_id.hex()}'. Did you use the right name?")
-    
+            # the request-response executor can only be created now that the runtime executor exists
+            # but we might want to consider to move the construction of such "user-space" dependencies somewhere else
+            self.ctx.request_response = RequestResponseExecutor(self.ctx.store, self.__runtime_executor)
+
     def wait_until_running(self) -> asyncio.Future:
         return self.__running_event.wait()
 
     def stop(self):
         self.__cancel_event.set()
 
     async def start(self):
         await self.__init_runtime_executor()
         refs = await self.references.get_all()
-        actor_heads:dict[ActorId, StepId] = (
-            {bytes.fromhex(ref.removeprefix('heads/')):step_id for ref,step_id in refs.items() if ref.startswith('heads/')}
-            )
+        actor_heads:dict[ActorId, StepId] = {bytes.fromhex(ref.removeprefix('heads/')):step_id for ref,step_id in refs.items() if ref.startswith('heads/')}
+
+        self.ctx.named_actors = {ref.removeprefix('actors/'):actor_id for ref,actor_id in refs.items() if ref.startswith('actors/')}
+        self.ctx.prototype_actors = {ref.removeprefix('prototypes/'):actor_id for ref,actor_id in refs.items() if ref.startswith('prototypes/')}
 
         async with self.__executor_lock:
             self.__executors:dict[ActorId, ActorExecutor] = {}
             for actor_id, step_id in actor_heads.items():
                 if(actor_id != self.__runtime_executor.agent_id): # exclude the agent actor, which is managed separately
                     self.__executors[actor_id] = await ActorExecutor.from_last_step(self.ctx, actor_id, step_id)
             gather_executors = self.__executors.copy()
```

### Comparing `agent_os_py-0.1.0/src/runtime/runtime_executor.py` & `agent_os_py-0.1.1/src/runtime/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/sync/actor_push.py` & `agent_os_py-0.1.1/src/sync/actor_push.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import mimetypes  
 from collections import OrderedDict
 from typing import Iterable
 from grit.object_serialization import blob_to_bytes
 from grit import *
 from wit import *
 from runtime.runtime_executor import add_offline_message_to_runtime_outbox, remove_offline_message_from_runtime_outbox
+from wit.prototype import wrap_in_prototype
 from . sync_item import SyncItem, sync_from_push_path, sync_from_push_value
 
 logger = logging.Logger(__name__)
 
 # Utility class to push external data to a specific actor
 
 class ActorPush():
@@ -20,50 +21,56 @@
     
     If the actor doesnt exist yet, it will create a genesis message.
     It the actor already exists it will generate an update messsage."""
     _actor_id:ActorId
     _is_genesis:bool
     _sync_items:OrderedDict[str, SyncItem]
     actor_name:str
+    is_prototype:bool
     wit:str
     wit_query:str
     wit_update:str
     runtime:str
-    notify:set[str]
 
     def __init__(self, is_genesis:bool, actor_id:ActorId|None=None):
         self._is_genesis = is_genesis
         self._actor_id = actor_id
         if(not is_genesis and actor_id is None):
             raise ValueError("Cannot create a non-genesis actor push without an actor id.")
         self._sync_items = OrderedDict()
         self.actor_name = None
+        self.is_prototype = False
         self.wit = None
         self.wit_query = None
         self.wit_update = None
         self.runtime = None
-        self.notify = set()
 
     @classmethod
-    async def from_actor_name(cls, references:References, actor_name:str) -> ActorPush:
+    async def from_actor_name(cls, references:References, actor_name:str, is_prototype:bool=False) -> ActorPush:
         # check if the actor already exists
-        actor_id = await references.get(ref_actor_name(actor_name))
-        if(actor_id is not None):
+        if is_prototype:
+            actor_ref = ref_prototype_name(actor_name)
+        else:
+            actor_ref = ref_actor_name(actor_name)
+
+        actor_id = await references.get(actor_ref)
+        if actor_id is not None:
             # the actor ref is a just helper reference, to make sure the actor 
             # actually exists (i.e. the genesis step has run) also check if there 
             # is a step head for this actor
             step_id = await references.get(ref_step_head(actor_id))
         else:
             step_id = None
         #now, either create a genesis push, or an update push
-        if(step_id is None):
+        if step_id is None:
             obj = cls(is_genesis=True, actor_id=None)
         else:
             obj = cls(is_genesis=False, actor_id=actor_id)
         obj.actor_name = actor_name
+        obj.is_prototype = is_prototype
         return obj
 
     @property
     def is_genesis(self) -> bool:
         return self._is_genesis
     
     @property
@@ -128,14 +135,17 @@
             sync_item:SyncItem
             for sync_item in sync_items:
                 if(sync_item.has_item_value):
                     blob_obj = _blob_from_value(sync_item.item_value)
                 else:
                     blob_obj = _blob_from_file(os.path.join(sync_item.dir_path, sync_item.file_name))
                 node.add(sync_item.item_name, blob_obj)
+        #check if the core needs to be wrapped as a prototype
+        if(self.is_prototype):
+            core = wrap_in_prototype(core)
         return core
     
     async def diff_core_with_actor(self, store:ObjectStore, references:References) -> AsyncIterator[tuple[str, str]]:
         if(self._is_genesis):
             push_core = self.to_core()
             async for path, _trees, blobs in push_core.walk():
                 for blob in blobs:
@@ -166,34 +176,35 @@
                     except Exception as ex:
                         yield push_blob_path, f"error retrieving path: {ex}"
 
     async def create_and_inject_messages(self, store:ObjectStore, references:References, agent_name:str) -> StepId:
         # While pushing the first genesis core to actors, the initial wit can fail (not be found, code error, etc). 
         # If this is the case the developer will iterate on the push files and values and as a consequnce change the 
         # actor id of the target actor each time.
-        # So, if this is a genesis push, look if there is already an agent ref for this actor, and if so, remove it.
+        # So, if this is a genesis push, look if there is already an actor ref for this actor, and if so, remove it.
+        if self.is_prototype:
+            actor_ref = ref_prototype_name(self.actor_name)
+        else:
+            actor_ref = ref_actor_name(self.actor_name)
+
         if(self._is_genesis):
-            previous_genesis_actor_id = await references.get(ref_actor_name(self.actor_name))
+            previous_genesis_actor_id = await references.get(actor_ref)
             if(previous_genesis_actor_id is not None):
                 await remove_offline_message_from_runtime_outbox(store, references, agent_name, previous_genesis_actor_id)
         # Now, create the message
         msg = await self.create_actor_message(store)
         # Don't set previous, so that this message can be pushed multiple times, 
         # resulting in an override of the current message in the outbox.
         # With set_previous=False, the message is treated like a signal, and only the last message will apply.
         step_id = await add_offline_message_to_runtime_outbox(store, references, agent_name, msg, set_previous=False)
-        # If this the gnesis step, also create an agen ref
+        # If this the genesis step, also create an actor ref
         if(self._is_genesis and self.actor_name is not None):
             # This may override the actor ref, if the genesis step changes over multiple initial pushes, 
             # but once the runtime runs, the actor ref needs to be fix
-            await references.set(ref_actor_name(self.actor_name), msg.recipient_id)
-        #notify other actors about the creation of this one
-        notify_msgs = await self.create_notification_messages(references, msg.recipient_id)
-        for notify_msg in notify_msgs:
-            await add_offline_message_to_runtime_outbox(store, references, agent_name, notify_msg, set_previous=True)
+            await references.set(actor_ref, msg.recipient_id)
         return step_id
         
     async def create_actor_message(self, store:ObjectStore) -> OutboxMessage:
         if(self._is_genesis):
             return await self.__create_genesis_message(store)
         else:
             return self.__create_update_message()
@@ -208,31 +219,14 @@
     def __create_update_message(self) -> OutboxMessage:
         core = self.to_core()
         if(self._actor_id is None):
             raise Exception("Cannot create update message without actor_id.")
         update_msg = OutboxMessage.from_update(self.actor_id, core)
         return update_msg
     
-    async def create_notification_messages(self, references:References, actor_id:ActorId) -> list[OutboxMessage]:
-        if(not self._is_genesis):
-            return []
-        if(len(self.notify) == 0):
-            return []
-        notify_msgs = []
-        for actor_to_notify in self.notify:
-            actor_to_notify_id = await references.get(ref_actor_name(actor_to_notify))
-            if(actor_to_notify_id is None):
-                raise Exception(
-                    f"Cannot notify actor {actor_to_notify} because no actor id was found in references '{ref_actor_name(actor_to_notify)}'."
-                    )
-            notify_msg = OutboxMessage.from_new(actor_to_notify_id, {'actor_name': self.actor_name, 'actor_id': actor_id.hex()})
-            notify_msg.mt = "notify_genesis"
-            notify_msgs.append(notify_msg)
-        return notify_msgs
-    
 
 def _blob_from_value(value:any) -> BlobObject:
     if isinstance(value, str):
         return BlobObject.from_str(value)
     elif isinstance(value, bytes):
         return BlobObject.from_bytes(value)
     elif isinstance(value, dict) or isinstance(value, list) or isinstance(value, tuple) or isinstance(value, Iterable):
```

### Comparing `agent_os_py-0.1.0/src/sync/sync_file.py` & `agent_os_py-0.1.1/src/sync/sync_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,15 +100,16 @@
     for actor_table in actors:
         actor_push = await _actor_push_from_toml_table(references, actor_table, all)
         actor_pushes.append(actor_push)
     return actor_pushes
 
 async def _actor_push_from_toml_table(references:References, actor_table:Container, all:Container|None=None) -> ActorPush:        
     actor_name = actor_table['name']
-    actor_push = await ActorPush.from_actor_name(references, actor_name)
+    is_prototype = actor_table.get('is_prototype', False)
+    actor_push = await ActorPush.from_actor_name(references, actor_name, is_prototype)
     if all is not None:
         _add_table_to_actor_push(actor_push, all)
     _add_table_to_actor_push(actor_push, actor_table)
     return actor_push
 
 def _add_table_to_actor_push(actor_push:ActorPush, table:Container):
     def try_add_path(path_key:str):
@@ -137,22 +138,14 @@
             try_add_values(key)
     if "wit" in table:
         actor_push.wit = table["wit"]
     if "wit_query" in table:
         actor_push.wit_query = table["wit_query"]
     if "wit_update" in table and not actor_push.is_genesis:
         actor_push.wit_update = table["wit_update"]
-    if "name" in table:
-        actor_push.actor_name = table["name"]
-    if "notify" in table:
-        notify = table['notify']
-        if(isinstance(notify, str)):
-            notify = [notify]
-        for actor_to_notify in notify:
-            actor_push.notify.add(actor_to_notify)
 
 def _read_toml_file(file_path) -> TOMLDocument:
     file_path = _convert_posix_to_win(file_path)
     with open(file_path, 'r') as f:
         return _read_toml_string(f.read())
 
 def _read_toml_string(toml_string) -> TOMLDocument:
@@ -187,32 +180,25 @@
             for key in actor.keys():
                 if key not in valid_keys:
                     raise ValueError(f"Invalid actor key '{key}'. Valid keys are '{valid_keys}'.")
             if 'name' not in actor:
                 raise ValueError("Actor name is required. Use 'name' to define an actor reference name.")
             else:
                 actor_names.append(actor['name'])
-            #check that the actors that need to be notified about this actor have been defined *before* this actor
-            if 'notify' in actor:
-                notify = actor['notify']
-                if(isinstance(notify, str)):
-                    notify = [notify]
-                if(not isinstance(notify, list)):
-                    raise ValueError(f"Actor to notify must be a string or list of strings, but was {type(notify)}.")
-                for actor_to_notify in notify:
-                    if(actor_to_notify not in actor_names):
-                        raise ValueError(f"Actor to notify '{actor_to_notify}' has not been defined before this one '{actor['name']}'. "+
-                                         f"Define the actor '{actor_to_notify}' above this one.")
+            
+            if 'is_prototype' in actor:
+                if(not isinstance(actor['is_prototype'], bool)):
+                    raise ValueError(f"Actor is_prototype must be a boolean, but was {type(actor['is_prototype'])}.")
 
     if('agent' in doc):
         validate_agent(doc['agent'])
     valid_all_keys = ['push', 'pull', 'sync', 'push_value', 'push_on_genesis', 'push_value_on_genesis', 'runtime', 'external_paths']
     if('all' in doc):
         validate_all(doc['all'], valid_all_keys)
-    valid_actor_keys = ['name', 'wit', 'wit_query', 'notify'] + valid_all_keys
+    valid_actor_keys = ['name', 'wit', 'wit_query', 'is_prototype'] + valid_all_keys
     if 'actors' in doc:
         #raise ValueError('No actors table array (aka heading) is defined. Use [[actors]] to define one or more actors.')
         validate_actors(doc['actors'], valid_actor_keys)
 
 def _convert_posix_to_win(path:str) -> str:
     if os.name == "nt" and "/" in path:
         return path.replace("/", os.sep)
```

### Comparing `agent_os_py-0.1.0/src/sync/sync_item.py` & `agent_os_py-0.1.1/src/sync/sync_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
+from dataclasses import dataclass
 import os
 import posixpath
 from pathlib import PureWindowsPath, PurePosixPath
-from attr import dataclass
+
 from grit import *
 
 @dataclass
 class SyncItem:
     """An item to sync between the the external world, usually the file system, and Grit."""
     dir_path:str
     file_name:str
```

### Comparing `agent_os_py-0.1.0/src/web/web_server.py` & `agent_os_py-0.1.1/src/web/web_server.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/wit/data_model.py` & `agent_os_py-0.1.1/src/wit/data_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -533,26 +533,26 @@
             if(self.__loader is not None and isinstance(self.__loader, ObjectStore)):
                 store = self.__loader
             else:
                 raise Exception("Cannot persist tree, no ObjectStore instance provided, "+
                                 "tried to see if the loader is an ObjectStore instance, but it is not.")
         tree_to_store = {}
         for(key, value) in self.__tree.items():
-            if(isinstance(value, ObjectId)):
+            if isinstance(value, ObjectId):
                 tree_to_store[key] = value
-            elif(isinstance(value, TreeObject)):
+            elif isinstance(value, TreeObject) or isinstance(value, Core) or type(value).__name__ == 'TreeObject' or type(value).__name__ == 'Core':
                 #only persist non-empty trees
                 if(not value.is_empty()):
                     tree_to_store[key] = await value.persist(store)
-            elif(isinstance(value, BlobObject)):
+            elif isinstance(value, BlobObject):
                 #only persist non-empty blobs
                 if(not value.is_empty()):
                     tree_to_store[key] = await value.persist(store)
             else:
-                raise TypeError(f"Cannot persist tree, invalid type for key '{key}'")
+                raise TypeError(f"Cannot persist tree, invalid type for key '{key}', is '{type(value)}'.")
         self.__tree_id = await store.store(tree_to_store)
         self.__dirty = False
         return self.__tree_id
 
     #==========================================
     # Util APIs
     #==========================================
@@ -646,15 +646,15 @@
     
     async def get_path(self, path: str) -> TreeObject | BlobObject | None:
         '''TreeObject only allows relative paths, since this is the root, absolute paths are allowed.'''
         if(len(path) > 0 and path[0] == '/'):
             path = path[1:]
         return await super().get_path(path)
     
-    async def merge(self, new_core:Core):
+    async def merge(self, new_core:Core|TreeObject):
         '''Merges the new_core into the current core. The current core will be modified.'''
         # walk the new_core and see if the current core is different
         async for _path, _trees, blobs in new_core.walk():
             for blob in blobs:
                 new_blob_path = blob.path()
                 try:
                     target_blob:BlobObject = await self.get_path(new_blob_path)
@@ -908,15 +908,15 @@
         gen_content_id = await core.persist(store)
         msg = cls(gen_content_id, is_signal=False)
         msg.content = gen_content_id
         msg.headers["mt"] = "genesis"
         return msg
     
     @classmethod
-    def from_update(cls, recipient_id:ActorId, core:TreeObject) -> OutboxMessage:
+    def from_update(cls, recipient_id:ActorId, core:TreeObject|TreeId) -> OutboxMessage:
         msg = cls(recipient_id, is_signal=False)
         msg.content = _ensure_content(core)
         msg.headers["mt"] = "update"
         return msg
 
     @classmethod
     def from_new(cls, recipient_id:ActorId, content:ValidMessageContent, is_signal:bool=False, mt:str|None=None) -> OutboxMessage:
@@ -942,15 +942,15 @@
         return content
     elif(isinstance(content, str)):
         return BlobObject.from_str(content)
     elif(isinstance(content, bytes)):
         return BlobObject.from_bytes(content)
     elif(isinstance(content, dict)):
         return BlobObject.from_json(content)
-    elif(isinstance(content, BlobObject) or isinstance(content, TreeObject)):
+    elif(isinstance(content, BlobObject) or isinstance(content, TreeObject)) or type(content).__name__ == 'BlobObject' or type(content).__name__ == 'TreeObject' or type(content).__name__ == 'Core':
         return content
     elif(isinstance(content, BaseModel)):
         return BlobObject.from_json(content)
     else:
         raise Exception("Invalid content type")
 
 class Outbox:
```

### Comparing `agent_os_py-0.1.0/src/wit/data_model_utils.py` & `agent_os_py-0.1.1/src/wit/data_model_utils.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/src/wit/wit_api.py` & `agent_os_py-0.1.1/src/wit/wit_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,8 +59,7 @@
     def query(self, /, query_name:str, *, more_struff:str=None) -> Callable[[DecoratedCallable], DecoratedCallable]:
         def decorator(func:DecoratedCallable) -> DecoratedCallable:
             return self._wit_query_router.register_query_handler(query_name, func)
         return decorator
     
     def wut_query(self, func, /) -> Callable[[], DecoratedCallable]:
         return self._wit_query_router.register_query_handler("wut", func)
-
```

### Comparing `agent_os_py-0.1.0/src/wit/wit_routers.py` & `agent_os_py-0.1.1/src/wit/wit_routers.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from itertools import islice
 from pydantic import BaseModel
 from grit import *
 from .data_model import *
 from .data_model_utils import *
 from .errors import InvalidWitException, InvalidMessageException, QueryError
 from .wit_state import WitState
+from .query import Query
+from .request_response import RequestResponse
 
 # The classes are mostly used internally to wrap user defined functions and route wit messages to the
 # correct message handler.
 
 DecoratedCallable = TypeVar("DecoratedCallable", bound=Callable[..., Any])
 
 #===================================================================================================
@@ -26,27 +28,32 @@
     inbox:Inbox
     outbox:Outbox
     core:Core
     step_id:StepId
     actor_id:ActorId
     agent_id:ActorId
     store:ObjectStore
+    named_actors:dict[str,ActorId]
+    prototype_actors:dict[str,ActorId]
+    query:Query
+    request_response:RequestResponse
 
 @dataclass(frozen=True)
 class QueryContext():
     query_name:str
     query_args:Blob|None
     query_args_json:dict|None
     inbox:Inbox
     outbox:Outbox
     core:Core
     step_id:StepId
     actor_id:ActorId
     agent_id:ActorId
     loader:ObjectLoader
+    query:Query
 
 #===================================================================================================
 # Function Wrapper Util
 #===================================================================================================
 class _Wrapper():
     """Wraps a user defined function and analizes the signature to determine how to call it."""
     def __init__(self, func:Callable) -> None:
@@ -331,14 +338,18 @@
                 step_id=step_id,
                 inbox=inbox,
                 outbox=outbox,
                 core=core,
                 store=store,
                 actor_id=kwargs.get('actor_id'),
                 agent_id=kwargs.get('agent_id'),
+                named_actors=kwargs.get('named_actors', {}),
+                prototype_actors=kwargs.get('prototype_actors', {}),
+                query=kwargs.get('query', None),
+                request_response=kwargs.get('request_response', None),
             )
             kwargs[wrapper.context_param.name] = ctx
         return kwargs
 
 #===================================================================================================
 # Query Routing & Handling
 #
@@ -529,15 +540,17 @@
                 query_args_json=query_args_json,
                 step_id=step_id,
                 inbox=inbox,
                 outbox=outbox,
                 core=core,
                 loader=loader,
                 actor_id=kwargs['actor_id'],
-                agent_id=kwargs['agent_id'])
+                agent_id=kwargs['agent_id'],
+                query=kwargs.get('query', None),
+                )
         
         #finally, add the json args to the kwargs, so they can be accessed direcly by name
         if(isinstance(query_args_json, dict)):
             for key, value in query_args_json.items():
                 # do not allow json keys to override any of the existing kwargs
                 if(key not in kwargs):
                     kwargs[key] = value
```

### Comparing `agent_os_py-0.1.0/src/wit/wit_state.py` & `agent_os_py-0.1.1/src/wit/wit_state.py`

 * *Files 21% similar despite different names*

```diff
@@ -51,17 +51,22 @@
                 #print(f'loading {attr_key}')
                 #try to find the blob
                 property_data = await state.get(attr_key)
                 if property_data is not None:
                     if(not isinstance(property_data, BlobObject)): #we expect this to be a blob object
                         raise Exception(f'Expected property {attr_key} to be a BlobObject, but got {type(property_data)}')
                     try:
-                        self.__setattr__(attr_key, pickle.loads(property_data.get_as_bytes()))
+                        attr_bytes = property_data.get_as_bytes()
+                        if attr_bytes is not None:
+                            attr_value = pickle.loads(attr_bytes)
+                            self.__setattr__(attr_key, attr_value)
+                        else:
+                            self.__setattr__(attr_key, None)
                     except Exception as e:
-                        logger.exception(f'Error loading {attr_key}')
+                        logger.exception(f'Error loading {attr_key}: {e}')
         self._after_load()
 
     async def _persist_to_core(self, core:Core):
         self._before_persist()
         attributes = dir(self)
         state = core.maket_path(self._core_path, exist_ok=True)
         for attr_key in attributes:
@@ -70,7 +75,12 @@
                 attr_value = self.__getattribute__(attr_key)
                 if(attr_value is not None):
                     #print(f'persisting {attr_key}')
                     property_data.set_as_bytes(pickle.dumps(attr_value))
                 else:
                     property_data.set_empty()
         self._after_persist()
+
+    async def _persist_to_tree_id(self, store:ObjectStore):
+        tmp_core = Core(store, {}, None)
+        await self._persist_to_core(tmp_core)
+        return await tmp_core.persist()
```

### Comparing `agent_os_py-0.1.0/src/wit/wut.py` & `agent_os_py-0.1.1/src/wit/wut.py`

 * *Files identical despite different names*

### Comparing `agent_os_py-0.1.0/PKG-INFO` & `agent_os_py-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,30 @@
 Metadata-Version: 2.1
 Name: agent-os-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library and runtime to build autonomous AI agents.
 Home-page: https://github.com/lukebuehler/agent-os
 License: MIT
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: async-lru (>=2.0.2,<3.0.0)
-Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: click (>=8.1.5,<9.0.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
-Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: httpx-sse (>=0.3.0,<0.4.0)
-Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: lmdb (>=1.4.1,<2.0.0)
-Requires-Dist: mistune (>=3.0.1,<4.0.0)
-Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: pydantic (>=2.0.1,<3.0.0)
-Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: ruff (>=0.0.285,<0.0.286)
-Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
 Requires-Dist: sse-starlette (>=1.6.1,<2.0.0)
 Requires-Dist: starlette (>=0.28.0,<0.29.0)
 Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
-Requires-Dist: transitions (>=0.9.0,<0.10.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: watchfiles (>=0.19.0,<0.20.0)
 Project-URL: Repository, https://github.com/lukebuehler/agent-os
 Description-Content-Type: text/markdown
 
 # Agent OS 
 🌞 Build autonomous AI agents!
@@ -55,15 +43,15 @@
   - The framework plays well with other AI libraries such as LangChain or LlamaIndex.
   - The system is designed for "[local-first](https://www.inkandswitch.com/local-first/)" agents that run on your machine, but it should also be possible to run parts of an agent in the cloud.
   - The data layer is made for longevity. We introduce a novel data structure that is inspired by Git. It's a content addressable storage that maintains your agent's history and memory and makes sure you never lose data.
   - An agent's primary purpose is not to run large language models on your machine (although that's possible too), but to provide a place to execute the code and functions that are generated by these models. It then composes these functions into larger features and routes events and data to them.
   - To demonstrate the power of the Agent OS, this project comes with a demo agent called ["Jetpack"](agents/README.md#jetpack) that can chat with you and write self-executing programs.
 
 
-<p><a href="https://www.youtube.com/embed/V8QpNic7b24" target="_blank"><img src="docs/images/agents-fig-1-jetpack-demo.png" alt="Jetpack Demo Video" width="700" /></a>
+<p><a href="https://www.youtube.com/watch?v=7HJXUMCDFks" target="_blank"><img src="docs/images/screenshot.png" alt="Jetpack Demo Video" width="700" /></a>
 <br>
 <small>Click the the image to watch a short demo on YouTube.</small>
 </p>
 
 
 ## Getting Started
 As long as the project is still in alpha, the best way to get started is to clone this repository.
@@ -81,14 +69,20 @@
 ```
 
 ## Test Drive an Agent 🤖 
 To run your first agent, put an `.env` file in the project root that contains an OpenAI API key. (It also works without an `.env` file or key if you just want to give the project a quick spin.)
 ```
 OPENAI_API_KEY=sk-myspecialkey
 ```
+### Agent Dependencies
+Some of the dependencies for the demo agents are optional and not part of the core Agent OS source. To install them, run:
+```
+poetry install --with agents
+```
+
 ### Jetpack Agent
 The ["Jetpack" agent](agents/README.md) demonstrates what the Agent OS can do and is geared towards end-to-end code generation and execution. It's a conversational agent that can accomplish various tasks for you. To run it, execute the following commands:
 ```
 poetry run aos -d agents/jetpack/ push
 poetry run aos -d agents/jetpack/ run
 ```
```

#### html2text {}

```diff
@@ -1,28 +1,21 @@
-Metadata-Version: 2.1 Name: agent-os-py Version: 0.1.0 Summary: A library and
+Metadata-Version: 2.1 Name: agent-os-py Version: 0.1.1 Summary: A library and
 runtime to build autonomous AI agents. Home-page: https://github.com/
 lukebuehler/agent-os License: MIT Requires-Python: >=3.10,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: aiofiles
-(>=23.1.0,<24.0.0) Requires-Dist: async-lru (>=2.0.2,<3.0.0) Requires-Dist:
-beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist: click (>=8.1.5,<9.0.0)
-Requires-Dist: filetype (>=1.2.0,<2.0.0) Requires-Dist: httpx
-(>=0.24.1,<0.25.0) Requires-Dist: httpx-sse (>=0.3.0,<0.4.0) Requires-Dist:
-jinja2 (>=3.1.2,<4.0.0) Requires-Dist: lmdb (>=1.4.1,<2.0.0) Requires-Dist:
-mistune (>=3.0.1,<4.0.0) Requires-Dist: openai (>=0.27.8,<0.28.0) Requires-
-Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist: pillow (>=10.0.0,<11.0.0)
-Requires-Dist: pydantic (>=2.0.1,<3.0.0) Requires-Dist: pytest (>=7.3.1,<8.0.0)
-Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0) Requires-Dist: python-dotenv
-(>=1.0.0,<2.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: ruff
-(>=0.0.285,<0.0.286) Requires-Dist: scikit-learn (>=1.3.0,<2.0.0) Requires-
-Dist: sse-starlette (>=1.6.1,<2.0.0) Requires-Dist: starlette
-(>=0.28.0,<0.29.0) Requires-Dist: tomlkit (>=0.11.8,<0.12.0) Requires-Dist:
-transitions (>=0.9.0,<0.10.0) Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
-Requires-Dist: watchfiles (>=0.19.0,<0.20.0) Project-URL: Repository, https://
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Requires-Dist: aiofiles (>=23.1.0,<24.0.0) Requires-Dist: async-
+lru (>=2.0.2,<3.0.0) Requires-Dist: click (>=8.1.5,<9.0.0) Requires-Dist:
+filetype (>=1.2.0,<2.0.0) Requires-Dist: lmdb (>=1.4.1,<2.0.0) Requires-Dist:
+pydantic (>=2.0.1,<3.0.0) Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0) Requires-Dist: sse-starlette
+(>=1.6.1,<2.0.0) Requires-Dist: starlette (>=0.28.0,<0.29.0) Requires-Dist:
+tomlkit (>=0.11.8,<0.12.0) Requires-Dist: uvicorn (>=0.22.0,<0.23.0) Requires-
+Dist: watchfiles (>=0.19.0,<0.20.0) Project-URL: Repository, https://
 github.com/lukebuehler/agent-os Description-Content-Type: text/markdown # Agent
 OS ð Build autonomous AI agents! ð ï¸The Agent OS is an experimental
 framework and runtime to build sophisticated, long running, and self-coding AI
 agents. We believe that the most important super-power of AI agents is to write
 and execute their own code to interact with the world. But for that to work,
 they need to run in a suitable environmentâa place designed to be inhabited
 by agents. The Agent OS is designed from the ground up to function as a long-
@@ -55,28 +48,30 @@
 (https://python-poetry.org/). Works on Linux, macOS, and Windows. Once cloned,
 `cd` into the repository and run: ``` poetry install ``` The project comes with
 a CLI that can be used to initiate and run agents. To see the available
 commands run: ``` poetry run aos --help ``` ## Test Drive an Agent ð¤ To run
 your first agent, put an `.env` file in the project root that contains an
 OpenAI API key. (It also works without an `.env` file or key if you just want
 to give the project a quick spin.) ``` OPENAI_API_KEY=sk-myspecialkey ``` ###
-Jetpack Agent The ["Jetpack" agent](agents/README.md) demonstrates what the
-Agent OS can do and is geared towards end-to-end code generation and execution.
-It's a conversational agent that can accomplish various tasks for you. To run
-it, execute the following commands: ``` poetry run aos -d agents/jetpack/ push
-poetry run aos -d agents/jetpack/ run ``` Jetpack comes with a web interface,
-and the Agent OS hosts a web server. To access the interface, browse to http://
-127.0.0.1:5000/ag/jetpack/wit/actors/frontend/query/web ## Project Structure *
-`agents/`: examples of agent implementations. [See the folder](agents/) for
-more details. * `jetpack/`: the flagship agent demo, geared towards
-conversational task completion through code generation. * `src/`: contains all
-relevant modules that are part of the Agent OS. * `grit/`: object store,
-inspired by Git. * `wit/`: libraries to help write "wit" state transition
-functions * `runtime/`: the Agent OS runtime: actor executor, custom python
-module loader, and wit function resolver. * `sync/`: modules to push and pull
-data into grit from the developer's file system. * `web/`: the web server that
-provides the web interface. * `cli/`: the "aos" (agent OS) CLI. * `tests/`:
-extensive unit tests that cover most of the `/src` packages and modules. *
-`docs/`: documentation, intended to be rendered as a GitBook. ## Running the
-Tests If you want to hack on the code, it is helpful to run the tests. The
-project uses `pytest` and has almost 100 unit tests. ``` poetry run pytest
-tests/ ```
+Agent Dependencies Some of the dependencies for the demo agents are optional
+and not part of the core Agent OS source. To install them, run: ``` poetry
+install --with agents ``` ### Jetpack Agent The ["Jetpack" agent](agents/
+README.md) demonstrates what the Agent OS can do and is geared towards end-to-
+end code generation and execution. It's a conversational agent that can
+accomplish various tasks for you. To run it, execute the following commands:
+``` poetry run aos -d agents/jetpack/ push poetry run aos -d agents/jetpack/
+run ``` Jetpack comes with a web interface, and the Agent OS hosts a web
+server. To access the interface, browse to http://127.0.0.1:5000/ag/jetpack/
+wit/actors/frontend/query/web ## Project Structure * `agents/`: examples of
+agent implementations. [See the folder](agents/) for more details. * `jetpack/
+`: the flagship agent demo, geared towards conversational task completion
+through code generation. * `src/`: contains all relevant modules that are part
+of the Agent OS. * `grit/`: object store, inspired by Git. * `wit/`: libraries
+to help write "wit" state transition functions * `runtime/`: the Agent OS
+runtime: actor executor, custom python module loader, and wit function
+resolver. * `sync/`: modules to push and pull data into grit from the
+developer's file system. * `web/`: the web server that provides the web
+interface. * `cli/`: the "aos" (agent OS) CLI. * `tests/`: extensive unit tests
+that cover most of the `/src` packages and modules. * `docs/`: documentation,
+intended to be rendered as a GitBook. ## Running the Tests If you want to hack
+on the code, it is helpful to run the tests. The project uses `pytest` and has
+almost 100 unit tests. ``` poetry run pytest tests/ ```
```

