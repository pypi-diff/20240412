# Comparing `tmp/livekit-agents-0.5.dev1.tar.gz` & `tmp/livekit-agents-0.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-agents-0.5.dev1.tar", last modified: Thu Apr 11 21:57:21 2024, max compression
+gzip compressed data, was "livekit-agents-0.5.dev2.tar", last modified: Thu Apr 11 23:22:34 2024, max compression
```

## Comparing `livekit-agents-0.5.dev1.tar` & `livekit-agents-0.5.dev2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.306522 livekit-agents-0.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-11 21:57:21.306522 livekit-agents-0.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.294522 livekit-agents-0.5.dev1/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.298522 livekit-agents-0.5.dev1/livekit/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.298522 livekit-agents-0.5.dev1/livekit/agents/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/aio/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/aio/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/aio/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/aio/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/aio/sleep.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/aio/wait_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/apipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit/agents/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/cli/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/cli/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/cli/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit/agents/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/codecs/mp3.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/http_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit/agents/ipc/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/ipc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/ipc/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/ipc/job_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/ipc/job_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/ipc/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/ipc_enc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/job_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/job_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit/agents/llm/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/llm/function_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/llm/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit/agents/stt/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/stt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/stt/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/stt/stt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit/agents/tokenize/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/tokenize/sentence_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit/agents/tts/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/tts/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/tts/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/vad.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/voice_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)    15451 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/livekit/agents/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:57:21.302522 livekit-agents-0.5.dev1/livekit_agents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-11 21:57:21.000000 livekit-agents-0.5.dev1/livekit_agents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-11 21:57:21.000000 livekit-agents-0.5.dev1/livekit_agents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:57:21.000000 livekit-agents-0.5.dev1/livekit_agents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-11 21:57:21.000000 livekit-agents-0.5.dev1/livekit_agents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 21:57:21.000000 livekit-agents-0.5.dev1/livekit_agents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 21:57:21.306522 livekit-agents-0.5.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-11 21:57:17.000000 livekit-agents-0.5.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:22:34.952476 livekit-agents-0.5.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-11 23:22:34.952476 livekit-agents-0.5.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:22:34.940476 livekit-agents-0.5.dev2/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:22:34.944476 livekit-agents-0.5.dev2/livekit/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:22:34.944476 livekit-agents-0.5.dev2/livekit/agents/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/aio/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/aio/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/aio/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/aio/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/aio/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/aio/wait_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/apipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:22:34.948476 livekit-agents-0.5.dev2/livekit/agents/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/cli/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/cli/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/cli/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:22:34.948476 livekit-agents-0.5.dev2/livekit/agents/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/codecs/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/http_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:22:34.948476 livekit-agents-0.5.dev2/livekit/agents/ipc/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/ipc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/ipc/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/ipc/job_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/ipc/job_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/ipc/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/ipc_enc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/job_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/job_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:22:34.948476 livekit-agents-0.5.dev2/livekit/agents/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/llm/function_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/llm/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:22:34.948476 livekit-agents-0.5.dev2/livekit/agents/stt/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/stt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/stt/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/stt/stt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:22:34.948476 livekit-agents-0.5.dev2/livekit/agents/tokenize/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/tokenize/sentence_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:22:34.948476 livekit-agents-0.5.dev2/livekit/agents/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/tts/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/tts/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/voice_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15451 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/livekit/agents/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:22:34.952476 livekit-agents-0.5.dev2/livekit_agents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-11 23:22:34.000000 livekit-agents-0.5.dev2/livekit_agents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-11 23:22:34.000000 livekit-agents-0.5.dev2/livekit_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:22:34.000000 livekit-agents-0.5.dev2/livekit_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-11 23:22:34.000000 livekit-agents-0.5.dev2/livekit_agents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 23:22:34.000000 livekit-agents-0.5.dev2/livekit_agents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 23:22:34.952476 livekit-agents-0.5.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-11 23:22:30.000000 livekit-agents-0.5.dev2/setup.py
```

### Comparing `livekit-agents-0.5.dev1/PKG-INFO` & `livekit-agents-0.5.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.5.dev1
+Version: 0.5.dev2
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
```

### Comparing `livekit-agents-0.5.dev1/livekit/agents/__init__.py` & `livekit-agents-0.5.dev2/livekit/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/aio/channel.py` & `livekit-agents-0.5.dev2/livekit/agents/aio/channel.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/aio/debug.py` & `livekit-agents-0.5.dev2/livekit/agents/aio/debug.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/aio/interval.py` & `livekit-agents-0.5.dev2/livekit/agents/aio/interval.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/aio/select.py` & `livekit-agents-0.5.dev2/livekit/agents/aio/select.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/aio/sleep.py` & `livekit-agents-0.5.dev2/livekit/agents/aio/sleep.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/aio/wait_group.py` & `livekit-agents-0.5.dev2/livekit/agents/aio/wait_group.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/apipe.py` & `livekit-agents-0.5.dev2/livekit/agents/apipe.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/cli/cli.py` & `livekit-agents-0.5.dev2/livekit/agents/cli/cli.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/cli/log.py` & `livekit-agents-0.5.dev2/livekit/agents/cli/log.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/cli/protocol.py` & `livekit-agents-0.5.dev2/livekit/agents/cli/protocol.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/cli/watcher.py` & `livekit-agents-0.5.dev2/livekit/agents/cli/watcher.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/codecs/__init__.py` & `livekit-agents-0.5.dev2/livekit/agents/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/codecs/mp3.py` & `livekit-agents-0.5.dev2/livekit/agents/codecs/mp3.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/http_server.py` & `livekit-agents-0.5.dev2/livekit/agents/http_server.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/ipc/job_main.py` & `livekit-agents-0.5.dev2/livekit/agents/ipc/job_process.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,141 +1,147 @@
-from __future__ import annotations
-
 import asyncio
 import contextlib
-import logging
-import os
-
-from livekit import rtc
-
-from .. import aio, apipe, ipc_enc
-from ..job_context import JobContext
-from ..job_request import AutoSubscribe
+import multiprocessing
+import sys
+import threading
+
+from livekit.protocol import agent
+
+from .. import aio, apipe
+from ..job_request import AcceptData
+from ..log import logger
 from ..utils import time_ms
-from . import protocol
+from . import consts, protocol
+from .job_main import _run_job
 
 
-class LogHandler(logging.Handler):
-    """Log handler forwarding logs to the worker process"""
-
-    def __init__(self, writer: ipc_enc.ProcessPipeWriter) -> None:
-        super().__init__(logging.NOTSET)
-        self._writer = writer
-
-    def emit(self, record: logging.LogRecord) -> None:
-        try:
-            ipc_enc.write_msg(
-                self._writer,
-                protocol.Log(level=record.levelno, message=record.getMessage()),
-            )
-        except Exception as e:
-            print(f"failed to write log: {e}")
-
-
-async def _start(
-    pipe: apipe.AsyncPipe, args: protocol.JobMainArgs, room: rtc.Room
-) -> None:
-    close_tx, close_rx = aio.channel()  # used by the JobContext to signal shutdown
-
-    auto_subscribe = args.accept_data.auto_subscribe
-    opts = rtc.RoomOptions(auto_subscribe=True)
-    if auto_subscribe != AutoSubscribe.SUBSCRIBE_ALL:
-        opts.auto_subscribe = False
-
-        def on_track_published(pub: rtc.RemoteTrackPublication, *_):
-            if (
-                pub.kind == rtc.TrackKind.KIND_AUDIO
-                and auto_subscribe == AutoSubscribe.AUDIO_ONLY
-            ):
-                pub.set_subscribed(True)
-            elif (
-                pub.kind == rtc.TrackKind.KIND_VIDEO
-                and auto_subscribe == AutoSubscribe.VIDEO_ONLY
-            ):
-                pub.set_subscribed(True)
-
-        if auto_subscribe != AutoSubscribe.SUBSCRIBE_NONE:
-            room.on("track_published", on_track_published)
-
-    cnt = room.connect(args.url, args.token, options=opts)
-    start_req: protocol.StartJobRequest | None = None
-    usertask: asyncio.Task | None = None
-    shutting_down = False
-
-    async def _start_if_valid():
-        nonlocal usertask
-        if start_req and room.isconnected():
-            # start the job
-            await pipe.write(protocol.StartJobResponse())
-
-            ctx = JobContext(
-                close_tx,
-                start_req.job,
-                room,
-            )
-            usertask = asyncio.create_task(args.accept_data.target(ctx))
-
-    async with contextlib.aclosing(aio.select([pipe, cnt, close_rx])) as select:
-        while True:
-            s = await select()
-            if s.selected is cnt:
-                if s.exc:
-                    await pipe.write(protocol.StartJobResponse(exc=s.exc))
-                    break  # failed to connect, break and exit the process
-                await _start_if_valid()
-
-            if s.selected is close_rx:
-                await pipe.write(protocol.UserExit())
-                break
-
-            msg = s.result()
-            if isinstance(msg, protocol.ShutdownRequest):
-                shutting_down = True
-                break
-            if isinstance(msg, protocol.StartJobRequest):
-                start_req = msg
-                await _start_if_valid()
-            if isinstance(msg, protocol.Ping):
-                last_timestamp = msg.timestamp
-                await pipe.write(
-                    protocol.Pong(last_timestamp=last_timestamp, timestamp=time_ms())
+class JobProcess:
+    def __init__(
+        self,
+        job: agent.Job,
+        url: str,
+        token: str,
+        accept_data: AcceptData,
+        loop: asyncio.AbstractEventLoop | None = None,
+    ) -> None:
+        self._loop = loop or asyncio.get_event_loop()
+        self._job = job
+        pch, cch = multiprocessing.Pipe(duplex=True)
+        asyncio_debug = self._loop.get_debug()
+        args = (
+            cch,
+            protocol.JobMainArgs(job.id, url, token, accept_data, asyncio_debug),
+        )
+        self._process = multiprocessing.Process(
+            target=_run_job, args=args, daemon=True
+        )  # daemon=True to avoid unresponsive process in production
+        self._pipe = apipe.AsyncPipe(
+            pch, loop=self._loop, messages=protocol.IPC_MESSAGES
+        )
+        self._close_future = asyncio.Future()
+
+    async def run(self) -> None:
+        self._process.start()
+
+        start_timeout = asyncio.sleep(consts.START_TIMEOUT)
+        ping_interval = aio.interval(consts.PING_INTERVAL)
+        pong_timeout = aio.sleep(consts.PING_TIMEOUT)
+
+        start_res: protocol.StartJobResponse | None = None
+
+        await self._pipe.write(protocol.StartJobRequest(job=self._job))
+        async with contextlib.aclosing(
+            aio.select([self._pipe, start_timeout, ping_interval, pong_timeout])
+        ) as select:
+            while True:
+                s = await select()
+                if s.selected is start_timeout and start_res is None:
+                    logger.error(
+                        "process start timed out, killing job",
+                        extra=self.logging_extra(),
+                    )
+                    self._sig_kill()
+                    break
+
+                if s.selected is pong_timeout:
+                    logger.error(
+                        "job ping timeout, killing job",
+                        extra=self.logging_extra(),
+                    )
+                    self._sig_kill()
+                    break
+
+                if s.selected is ping_interval:
+                    ping = protocol.Ping(timestamp=time_ms())
+                    await self._pipe.write(ping)  # send ping each consts.PING_INTERVAL
+                    continue
+
+                try:
+                    res = s.result()
+                except aio.ChanClosed:
+                    logger.error(
+                        "pipe closed, exiting job",
+                        extra=self.logging_extra(),
+                    )
+                    break
+
+                if isinstance(res, protocol.StartJobResponse):
+                    start_res = res
+                if isinstance(res, protocol.Log):
+                    logger.log(res.level, res.message, extra=self.logging_extra())
+                if isinstance(res, protocol.Pong):
+                    delay = time_ms() - res.timestamp
+                    if delay > consts.HIGH_PING_THRESHOLD * 1000:
+                        logger.warning(
+                            "job is unresponsive",
+                            extra={"delay": delay, **self.logging_extra()},
+                        )
+
+                    with contextlib.suppress(aio.SleepFinished):
+                        pong_timeout.reset()
+
+                if isinstance(res, protocol.UserExit) or isinstance(
+                    res, protocol.ShutdownResponse
+                ):
+                    logger.info("job exiting", extra=self.logging_extra())
+                    break
+
+        def _join_process():
+            try:
+                self._process.join()
+            except Exception as e:
+                logger.error(
+                    "error joining job process",
+                    exc_info=e,
+                    extra=self.logging_extra(),
                 )
 
-    logging.debug("disconnecting from room")
-    await room.disconnect()
+            self._loop.call_soon_threadsafe(self._close_future.set_result, None)
+
+        join_t = threading.Thread(target=_join_process, daemon=True)
+        join_t.start()
+        await self._close_future
+
+        logger.info("job process closed", extra=self.logging_extra())
+
+    def _sig_kill(self) -> None:
+        if not self._process.is_alive():
+            return
+
+        logger.info("killing job process", extra=self.logging_extra())
+        if sys.platform == "win32":
+            self._process.terminate()
+        else:
+            self._process.kill()
+
+    async def aclose(self) -> None:
+        logger.info("closing job process", extra=self.logging_extra())
+        await self._pipe.write(protocol.ShutdownRequest())
+        await self._close_future
+        self._pipe.close()
+
+    @property
+    def job(self) -> agent.Job:
+        return self._job
 
-    if usertask is not None:
-        with contextlib.suppress(asyncio.CancelledError):
-            await usertask  # type: ignore
-
-    if shutting_down:
-        await pipe.write(protocol.ShutdownResponse())
-
-
-def _run_job(cch: ipc_enc.ProcessPipe, args: protocol.JobMainArgs) -> None:
-    """Entry point for a job process"""
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-
-    logging.root.setLevel(logging.NOTSET)
-    # logging.root.propagate = False
-    logging.root.addHandler(LogHandler(cch))
-
-    # current process pid
-    pid = os.getpid()
-    logging.debug(
-        "process started", extra={"job_id": args.job_id, "url": args.url, "pid": pid}
-    )
-
-    pipe = apipe.AsyncPipe(cch, loop, protocol.IPC_MESSAGES)
-    loop.slow_callback_duration = 0.02  # 20ms
-    aio.debug.hook_slow_callbacks(0.75)
-    loop.set_debug(args.asyncio_debug)
-
-    room = rtc.Room(loop=loop)
-    main_task = loop.create_task(_start(pipe, args, room))
-
-    try:
-        loop.run_until_complete(main_task)
-    except KeyboardInterrupt:
-        # ignore
-        loop.run_until_complete(main_task)
+    def logging_extra(self) -> dict:
+        return {"job_id": self._job.id, "pid": self._process.pid}
```

### Comparing `livekit-agents-0.5.dev1/livekit/agents/ipc/protocol.py` & `livekit-agents-0.5.dev2/livekit/agents/ipc/protocol.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/ipc_enc.py` & `livekit-agents-0.5.dev2/livekit/agents/ipc_enc.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/job_context.py` & `livekit-agents-0.5.dev2/livekit/agents/job_context.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/job_request.py` & `livekit-agents-0.5.dev2/livekit/agents/job_request.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/llm/__init__.py` & `livekit-agents-0.5.dev2/livekit/agents/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/llm/function_context.py` & `livekit-agents-0.5.dev2/livekit/agents/llm/function_context.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/llm/llm.py` & `livekit-agents-0.5.dev2/livekit/agents/llm/llm.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/plugin.py` & `livekit-agents-0.5.dev2/livekit/agents/plugin.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/stt/stream_adapter.py` & `livekit-agents-0.5.dev2/livekit/agents/stt/stream_adapter.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/stt/stt.py` & `livekit-agents-0.5.dev2/livekit/agents/stt/stt.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/tokenize/sentence_tokenizer.py` & `livekit-agents-0.5.dev2/livekit/agents/tokenize/sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/tts/stream_adapter.py` & `livekit-agents-0.5.dev2/livekit/agents/tts/stream_adapter.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/tts/tts.py` & `livekit-agents-0.5.dev2/livekit/agents/tts/tts.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/utils.py` & `livekit-agents-0.5.dev2/livekit/agents/utils.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/vad.py` & `livekit-agents-0.5.dev2/livekit/agents/vad.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/version.py` & `livekit-agents-0.5.dev2/livekit/agents/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.5.dev1"
+__version__ = "0.5.dev2"
```

### Comparing `livekit-agents-0.5.dev1/livekit/agents/voice_assistant.py` & `livekit-agents-0.5.dev2/livekit/agents/voice_assistant.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit/agents/worker.py` & `livekit-agents-0.5.dev2/livekit/agents/worker.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/livekit_agents.egg-info/PKG-INFO` & `livekit-agents-0.5.dev2/livekit_agents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.5.dev1
+Version: 0.5.dev2
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
```

### Comparing `livekit-agents-0.5.dev1/livekit_agents.egg-info/SOURCES.txt` & `livekit-agents-0.5.dev2/livekit_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev1/setup.py` & `livekit-agents-0.5.dev2/setup.py`

 * *Files identical despite different names*

