# Comparing `tmp/livekit-agents-0.5.dev0.tar.gz` & `tmp/livekit-agents-0.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-agents-0.5.dev0.tar", last modified: Thu Apr 11 21:51:27 2024, max compression
+gzip compressed data, was "livekit-agents-0.5.dev1.tar", last modified: Thu Apr 11 21:57:21 2024, max compression
```

## Comparing `livekit-agents-0.5.dev0.tar` & `livekit-agents-0.5.dev1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.391691 livekit-agents-0.5.dev0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.399691 livekit-agents-0.5.dev0/livekit/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.399691 livekit-agents-0.5.dev0/livekit/agents/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/aio/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/aio/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/aio/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/aio/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/aio/sleep.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/aio/wait_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/apipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.399691 livekit-agents-0.5.dev0/livekit/agents/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/cli/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/cli/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/cli/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.399691 livekit-agents-0.5.dev0/livekit/agents/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/codecs/mp3.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/http_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.399691 livekit-agents-0.5.dev0/livekit/agents/ipc/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/ipc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/ipc/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/ipc/job_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/ipc/job_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/ipc/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/ipc_enc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/job_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/job_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/livekit/agents/llm/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/llm/function_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/llm/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/livekit/agents/stt/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/stt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/stt/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/stt/stt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/livekit/agents/tokenize/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/tokenize/sentence_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/livekit/agents/tts/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/tts/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/tts/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/vad.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/voice_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)    15451 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/livekit/agents/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/livekit_agents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-11 21:51:27.000000 livekit-agents-0.5.dev0/livekit_agents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-11 21:51:27.000000 livekit-agents-0.5.dev0/livekit_agents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:51:27.000000 livekit-agents-0.5.dev0/livekit_agents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-11 21:51:27.000000 livekit-agents-0.5.dev0/livekit_agents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 21:51:27.000000 livekit-agents-0.5.dev0/livekit_agents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 21:51:27.403691 livekit-agents-0.5.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-11 21:51:22.000000 livekit-agents-0.5.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.306522 livekit-agents-0.5.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-11 21:57:21.306522 livekit-agents-0.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.294522 livekit-agents-0.5.dev1/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.298522 livekit-agents-0.5.dev1/livekit/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.298522 livekit-agents-0.5.dev1/livekit/agents/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/aio/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/aio/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/aio/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/aio/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/aio/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/aio/wait_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/apipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit/agents/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/cli/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/cli/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/cli/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit/agents/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/codecs/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/http_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit/agents/ipc/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/ipc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/ipc/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/ipc/job_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/ipc/job_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/ipc/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/ipc_enc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/job_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/job_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit/agents/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/llm/function_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/llm/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit/agents/stt/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/stt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/stt/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/stt/stt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit/agents/tokenize/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/tokenize/sentence_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit/agents/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/tts/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/tts/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/voice_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15451 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit_agents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-11 21:57:21.000000 livekit-agents-0.5.dev1/livekit_agents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-11 21:57:21.000000 livekit-agents-0.5.dev1/livekit_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:57:21.000000 livekit-agents-0.5.dev1/livekit_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-11 21:57:21.000000 livekit-agents-0.5.dev1/livekit_agents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 21:57:21.000000 livekit-agents-0.5.dev1/livekit_agents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 21:57:21.306522 livekit-agents-0.5.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/setup.py
```

### Comparing `livekit-agents-0.5.dev0/PKG-INFO` & `livekit-agents-0.5.dev1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.5.dev0
+Version: 0.5.dev1
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
@@ -25,13 +25,14 @@
 Requires-Dist: livekit-protocol~=0.4
 Requires-Dist: protobuf>=3
 Requires-Dist: types-protobuf<5,>=4
 Requires-Dist: python-json-logger~=2.0
 Requires-Dist: attrs~=23.0
 Requires-Dist: watchfiles~=0.21
 Requires-Dist: colorlog~=6.0
+Requires-Dist: psutil~=5.9
 Provides-Extra: codecs
 Requires-Dist: av>=11.0.0; extra == "codecs"
 
 # LiveKit Agents
 
 The core LiveKit Agents Framework. See top-level README for more information.
```

### Comparing `livekit-agents-0.5.dev0/livekit/agents/__init__.py` & `livekit-agents-0.5.dev1/livekit/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/aio/channel.py` & `livekit-agents-0.5.dev1/livekit/agents/aio/channel.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/aio/debug.py` & `livekit-agents-0.5.dev1/livekit/agents/aio/debug.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/aio/interval.py` & `livekit-agents-0.5.dev1/livekit/agents/aio/interval.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/aio/select.py` & `livekit-agents-0.5.dev1/livekit/agents/aio/select.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/aio/sleep.py` & `livekit-agents-0.5.dev1/livekit/agents/aio/sleep.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/aio/wait_group.py` & `livekit-agents-0.5.dev1/livekit/agents/aio/wait_group.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/apipe.py` & `livekit-agents-0.5.dev1/livekit/agents/apipe.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/cli/cli.py` & `livekit-agents-0.5.dev1/livekit/agents/cli/cli.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/cli/log.py` & `livekit-agents-0.5.dev1/livekit/agents/cli/log.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/cli/protocol.py` & `livekit-agents-0.5.dev1/livekit/agents/cli/protocol.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/cli/watcher.py` & `livekit-agents-0.5.dev1/livekit/agents/cli/watcher.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/codecs/__init__.py` & `livekit-agents-0.5.dev1/livekit/agents/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/codecs/mp3.py` & `livekit-agents-0.5.dev1/livekit/agents/codecs/mp3.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/http_server.py` & `livekit-agents-0.5.dev1/livekit/agents/http_server.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/ipc/job_main.py` & `livekit-agents-0.5.dev1/livekit/agents/ipc/job_main.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/ipc/job_process.py` & `livekit-agents-0.5.dev1/livekit/agents/ipc/job_process.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/ipc/protocol.py` & `livekit-agents-0.5.dev1/livekit/agents/ipc/protocol.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/ipc_enc.py` & `livekit-agents-0.5.dev1/livekit/agents/ipc_enc.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/job_context.py` & `livekit-agents-0.5.dev1/livekit/agents/job_context.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/job_request.py` & `livekit-agents-0.5.dev1/livekit/agents/job_request.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/llm/__init__.py` & `livekit-agents-0.5.dev1/livekit/agents/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/llm/function_context.py` & `livekit-agents-0.5.dev1/livekit/agents/llm/function_context.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/llm/llm.py` & `livekit-agents-0.5.dev1/livekit/agents/llm/llm.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/plugin.py` & `livekit-agents-0.5.dev1/livekit/agents/plugin.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/stt/stream_adapter.py` & `livekit-agents-0.5.dev1/livekit/agents/stt/stream_adapter.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/stt/stt.py` & `livekit-agents-0.5.dev1/livekit/agents/stt/stt.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/tokenize/sentence_tokenizer.py` & `livekit-agents-0.5.dev1/livekit/agents/tokenize/sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/tts/stream_adapter.py` & `livekit-agents-0.5.dev1/livekit/agents/tts/stream_adapter.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/tts/tts.py` & `livekit-agents-0.5.dev1/livekit/agents/tts/tts.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/utils.py` & `livekit-agents-0.5.dev1/livekit/agents/utils.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/vad.py` & `livekit-agents-0.5.dev1/livekit/agents/vad.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/version.py` & `livekit-agents-0.5.dev1/livekit/agents/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.5.dev0"
+__version__ = "0.5.dev1"
```

### Comparing `livekit-agents-0.5.dev0/livekit/agents/voice_assistant.py` & `livekit-agents-0.5.dev1/livekit/agents/voice_assistant.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit/agents/worker.py` & `livekit-agents-0.5.dev1/livekit/agents/worker.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/livekit_agents.egg-info/PKG-INFO` & `livekit-agents-0.5.dev1/livekit_agents.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.5.dev0
+Version: 0.5.dev1
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
@@ -25,13 +25,14 @@
 Requires-Dist: livekit-protocol~=0.4
 Requires-Dist: protobuf>=3
 Requires-Dist: types-protobuf<5,>=4
 Requires-Dist: python-json-logger~=2.0
 Requires-Dist: attrs~=23.0
 Requires-Dist: watchfiles~=0.21
 Requires-Dist: colorlog~=6.0
+Requires-Dist: psutil~=5.9
 Provides-Extra: codecs
 Requires-Dist: av>=11.0.0; extra == "codecs"
 
 # LiveKit Agents
 
 The core LiveKit Agents Framework. See top-level README for more information.
```

### Comparing `livekit-agents-0.5.dev0/livekit_agents.egg-info/SOURCES.txt` & `livekit-agents-0.5.dev1/livekit_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev0/setup.py` & `livekit-agents-0.5.dev1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         "livekit-protocol~=0.4",
         "protobuf>=3",
         "types-protobuf>=4,<5",
         "python-json-logger~=2.0",
         "attrs~=23.0",
         "watchfiles~=0.21",
         "colorlog~=6.0",
+        "psutil~=5.9",
     ],
     extras_require={
         "codecs": ["av>=11.0.0"],
     },
     package_data={
         "livekit.agents": ["py.typed"],
     },
```

