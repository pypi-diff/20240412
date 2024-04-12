# Comparing `tmp/generate_core-0.4.2.tar.gz` & `tmp/generate_core-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate_core-0.4.2.tar", max compression
+gzip compressed data, was "generate_core-0.4.3.tar", max compression
```

## Comparing `generate_core-0.4.2.tar` & `generate_core-0.4.3.tar`

### file list

```diff
@@ -1,78 +1,80 @@
--rw-r--r--   0        0        0     1067 2024-03-11 03:11:33.337919 generate_core-0.4.2/LICENSE
--rw-r--r--   0        0        0     8989 2024-03-11 03:11:33.337919 generate_core-0.4.2/README.md
--rw-r--r--   0        0        0     4275 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/__init__.py
--rw-r--r--   0        0        0      994 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/access_token_manager.py
--rw-r--r--   0        0        0     3750 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/__init__.py
--rw-r--r--   0        0        0     5864 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/base.py
--rw-r--r--   0        0        0      920 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/cost_caculator.py
--rw-r--r--   0        0        0     1071 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/message/__init__.py
--rw-r--r--   0        0        0     2274 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/message/core.py
--rw-r--r--   0        0        0      666 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/message/exception.py
--rw-r--r--   0        0        0     1603 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/message/utils.py
--rw-r--r--   0        0        0      669 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/model_output.py
--rw-r--r--   0        0        0     2387 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/__init__.py
--rw-r--r--   0        0        0     8434 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/anthropic.py
--rw-r--r--   0        0        0     3604 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/azure.py
--rw-r--r--   0        0        0     7067 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/baichuan.py
--rw-r--r--   0        0        0     8648 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/bailian.py
--rw-r--r--   0        0        0     6688 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/dashscope.py
--rw-r--r--   0        0        0     9178 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/dashscope_multimodal.py
--rw-r--r--   0        0        0     2967 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/deepseek.py
--rw-r--r--   0        0        0     8135 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/hunyuan.py
--rw-r--r--   0        0        0     5535 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/minimax.py
--rw-r--r--   0        0        0     7992 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/minimax_legacy.py
--rw-r--r--   0        0        0    15084 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/minimax_pro.py
--rw-r--r--   0        0        0     2609 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/moonshot.py
--rw-r--r--   0        0        0     4424 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/openai.py
--rw-r--r--   0        0        0    13922 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/openai_like.py
--rw-r--r--   0        0        0     3226 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/test.py
--rw-r--r--   0        0        0     9678 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/wenxin.py
--rw-r--r--   0        0        0     2465 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/yi.py
--rw-r--r--   0        0        0    20581 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/models/zhipu.py
--rw-r--r--   0        0        0     2362 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/printer.py
--rw-r--r--   0        0        0     2271 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/stream_manager.py
--rw-r--r--   0        0        0     3225 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/chat_completion/tool.py
--rw-r--r--   0        0        0     3004 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/highlevel.py
--rw-r--r--   0        0        0    10242 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/http.py
--rw-r--r--   0        0        0     1475 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/image_generation/__init__.py
--rw-r--r--   0        0        0     1223 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/image_generation/base.py
--rw-r--r--   0        0        0      710 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/image_generation/models/__init__.py
--rw-r--r--   0        0        0     7542 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/image_generation/models/baidu.py
--rw-r--r--   0        0        0     7064 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/image_generation/models/openai.py
--rw-r--r--   0        0        0     4404 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/image_generation/models/qianfan.py
--rw-r--r--   0        0        0     3093 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/image_generation/models/zhipu.py
--rw-r--r--   0        0        0     3400 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/model.py
--rw-r--r--   0        0        0        0 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/modifiers/__init__.py
--rw-r--r--   0        0        0     9232 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/modifiers/agent.py
--rw-r--r--   0        0        0     5110 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/modifiers/hook.py
--rw-r--r--   0        0        0     3935 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/modifiers/limit.py
--rw-r--r--   0        0        0     2720 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/modifiers/session.py
--rw-r--r--   0        0        0     8155 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/modifiers/structure.py
--rw-r--r--   0        0        0     1147 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/platforms/__init__.py
--rw-r--r--   0        0        0      440 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/platforms/anthropic.py
--rw-r--r--   0        0        0      487 2024-03-11 03:11:33.337919 generate_core-0.4.2/generate/platforms/azure.py
--rw-r--r--   0        0        0      444 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/platforms/baichuan.py
--rw-r--r--   0        0        0     3278 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/platforms/baidu.py
--rw-r--r--   0        0        0     1434 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/platforms/bailian.py
--rw-r--r--   0        0        0      997 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/platforms/base.py
--rw-r--r--   0        0        0      423 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/platforms/dashscope.py
--rw-r--r--   0        0        0      419 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/platforms/deepseek.py
--rw-r--r--   0        0        0      575 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/platforms/hunyuan.py
--rw-r--r--   0        0        0      452 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/platforms/minimax.py
--rw-r--r--   0        0        0      417 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/platforms/moonshot.py
--rw-r--r--   0        0        0      411 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/platforms/openai.py
--rw-r--r--   0        0        0      198 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/platforms/openai_like.py
--rw-r--r--   0        0        0      431 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/platforms/yi.py
--rw-r--r--   0        0        0     1217 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/platforms/zhipu.py
--rw-r--r--   0        0        0     1398 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/test.py
--rw-r--r--   0        0        0     1019 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/text_to_speech/__init__.py
--rw-r--r--   0        0        0     1099 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/text_to_speech/base.py
--rw-r--r--   0        0        0      419 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/text_to_speech/models/__init__.py
--rw-r--r--   0        0        0     8043 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/text_to_speech/models/minimax.py
--rw-r--r--   0        0        0     3690 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/text_to_speech/models/openai.py
--rw-r--r--   0        0        0      450 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/types.py
--rw-r--r--   0        0        0     6918 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/ui.py
--rw-r--r--   0        0        0     1540 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/utils.py
--rw-r--r--   0        0        0       22 2024-03-11 03:11:33.341919 generate_core-0.4.2/generate/version.py
--rw-r--r--   0        0        0     1908 2024-03-11 03:11:33.341919 generate_core-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    10205 1970-01-01 00:00:00.000000 generate_core-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-12 03:10:53.501705 generate_core-0.4.3/LICENSE
+-rw-r--r--   0        0        0    10107 2024-04-12 03:10:53.501705 generate_core-0.4.3/README.md
+-rw-r--r--   0        0        0     4411 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/__init__.py
+-rw-r--r--   0        0        0      994 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/access_token_manager.py
+-rw-r--r--   0        0        0     3884 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/__init__.py
+-rw-r--r--   0        0        0     5765 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/base.py
+-rw-r--r--   0        0        0      920 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/cost_caculator.py
+-rw-r--r--   0        0        0     1071 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/message/__init__.py
+-rw-r--r--   0        0        0     2731 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/message/core.py
+-rw-r--r--   0        0        0      666 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/message/exception.py
+-rw-r--r--   0        0        0     1603 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/message/utils.py
+-rw-r--r--   0        0        0      669 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/model_output.py
+-rw-r--r--   0        0        0     2522 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/__init__.py
+-rw-r--r--   0        0        0     8612 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/anthropic.py
+-rw-r--r--   0        0        0     3604 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/azure.py
+-rw-r--r--   0        0        0     7067 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/baichuan.py
+-rw-r--r--   0        0        0     8648 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/bailian.py
+-rw-r--r--   0        0        0     6688 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/dashscope.py
+-rw-r--r--   0        0        0     9178 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/dashscope_multimodal.py
+-rw-r--r--   0        0        0     2967 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/deepseek.py
+-rw-r--r--   0        0        0     8135 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/hunyuan.py
+-rw-r--r--   0        0        0     5535 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/minimax.py
+-rw-r--r--   0        0        0     7992 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/minimax_legacy.py
+-rw-r--r--   0        0        0    15084 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/minimax_pro.py
+-rw-r--r--   0        0        0     2609 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/moonshot.py
+-rw-r--r--   0        0        0     4424 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/openai.py
+-rw-r--r--   0        0        0    13949 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/openai_like.py
+-rw-r--r--   0        0        0     2893 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/stepfun.py
+-rw-r--r--   0        0        0     3226 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/test.py
+-rw-r--r--   0        0        0     9678 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/wenxin.py
+-rw-r--r--   0        0        0     2489 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/yi.py
+-rw-r--r--   0        0        0    20581 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/zhipu.py
+-rw-r--r--   0        0        0     2362 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/printer.py
+-rw-r--r--   0        0        0     2271 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/stream_manager.py
+-rw-r--r--   0        0        0     3225 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/chat_completion/tool.py
+-rw-r--r--   0        0        0     3040 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/highlevel.py
+-rw-r--r--   0        0        0    10242 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/http.py
+-rw-r--r--   0        0        0     1475 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/image_generation/__init__.py
+-rw-r--r--   0        0        0     1223 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/image_generation/base.py
+-rw-r--r--   0        0        0      710 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/image_generation/models/__init__.py
+-rw-r--r--   0        0        0     7538 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/image_generation/models/baidu.py
+-rw-r--r--   0        0        0     7064 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/image_generation/models/openai.py
+-rw-r--r--   0        0        0     4404 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/image_generation/models/qianfan.py
+-rw-r--r--   0        0        0     3093 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/image_generation/models/zhipu.py
+-rw-r--r--   0        0        0     3400 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/model.py
+-rw-r--r--   0        0        0        0 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/modifiers/__init__.py
+-rw-r--r--   0        0        0     9232 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/modifiers/agent.py
+-rw-r--r--   0        0        0     5110 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/modifiers/hook.py
+-rw-r--r--   0        0        0     3935 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/modifiers/limit.py
+-rw-r--r--   0        0        0     2854 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/modifiers/session.py
+-rw-r--r--   0        0        0     8333 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/modifiers/structure.py
+-rw-r--r--   0        0        0     1225 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/__init__.py
+-rw-r--r--   0        0        0      440 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/anthropic.py
+-rw-r--r--   0        0        0      487 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/azure.py
+-rw-r--r--   0        0        0      444 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/baichuan.py
+-rw-r--r--   0        0        0     3278 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/baidu.py
+-rw-r--r--   0        0        0     1434 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/bailian.py
+-rw-r--r--   0        0        0      997 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/base.py
+-rw-r--r--   0        0        0      423 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/dashscope.py
+-rw-r--r--   0        0        0      419 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/deepseek.py
+-rw-r--r--   0        0        0      575 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/hunyuan.py
+-rw-r--r--   0        0        0      452 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/minimax.py
+-rw-r--r--   0        0        0      417 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/moonshot.py
+-rw-r--r--   0        0        0      411 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/openai.py
+-rw-r--r--   0        0        0      198 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/openai_like.py
+-rw-r--r--   0        0        0      411 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/stepfun.py
+-rw-r--r--   0        0        0      431 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/yi.py
+-rw-r--r--   0        0        0     1216 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/zhipu.py
+-rw-r--r--   0        0        0     1398 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/test.py
+-rw-r--r--   0        0        0     1019 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/text_to_speech/__init__.py
+-rw-r--r--   0        0        0     1099 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/text_to_speech/base.py
+-rw-r--r--   0        0        0      419 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/text_to_speech/models/__init__.py
+-rw-r--r--   0        0        0     8043 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/text_to_speech/models/minimax.py
+-rw-r--r--   0        0        0     3690 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/text_to_speech/models/openai.py
+-rw-r--r--   0        0        0      450 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/types.py
+-rw-r--r--   0        0        0     7200 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/ui.py
+-rw-r--r--   0        0        0     2242 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/utils.py
+-rw-r--r--   0        0        0       22 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/version.py
+-rw-r--r--   0        0        0     2119 2024-04-12 03:10:53.505705 generate_core-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    11300 1970-01-01 00:00:00.000000 generate_core-0.4.3/PKG-INFO
```

### Comparing `generate_core-0.4.2/LICENSE` & `generate_core-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/README.md` & `generate_core-0.4.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,65 @@
-# Generate
+<div align="center">
+  <img src="logo/logo.png" alt="Generate Logo" width="200"/>
+</div>
+
+<div align="center">
+    <h1>Generate</h1>
+    <p>
+        A Python Package to Access World-Class Generative Models.
+    </p>
+    <p>
+        <a href="https://wangyuxinwhy.github.io/generate/">中文文档</a>
+        ｜
+        <a href="https://colab.research.google.com/github/wangyuxinwhy/generate/blob/main/examples/tutorial.ipynb">交互式教程</a>
+    </p>
+
+[![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)](#)
+[![CI Status](https://github.com/wangyuxinwhy/generate/actions/workflows/ci.yml/badge.svg)](https://github.com/wangyuxinwhy/generate/actions/workflows/ci.yml)
+[![CD Status](https://github.com/wangyuxinwhy/generate/actions/workflows/cd.yml/badge.svg)](https://github.com/wangyuxinwhy/generate/actions/workflows/cd.yml)
+[![License](https://img.shields.io/github/license/wangyuxinwhy/generate)](https://github.com/wangyuxinwhy/generate/blob/main/LICENSE)
+[![Documentation](https://img.shields.io/badge/docs-latest-brightgreen.svg)](https://wangyuxinwhy.github.io/generate/)
+[![Made with Love](https://img.shields.io/badge/made%20with-love-red.svg)](#)
+
+</div>
+<br>
+<br>
 
-[文档](https://wangyuxinwhy.github.io/generate/)
+# 简介
 
-> A Python Package to Access World-Class Generative Models.
 
-## 简介
 
 Generate 允许用户通过统一的 api 访问多平台的生成式模型，当前支持：
 
-| 平台 🤖       | 同步 🔄 | 异步 ⏳ | 流式 🌊 | Vision 👀 | Tools 🛠️ |
-|----------------|---------|---------|---------|-----------|-----------|
-| OpenAI         | ✅       | ✅       | ✅       | ✅         | ✅         |
-| Azure         | ✅       | ✅       | ❌       | ✅         | ✅         |
-| Anthropic         | ✅       | ✅       | ✅       | ✅         | ❌         |
-| 文心 Wenxin | ✅       | ✅       | ✅       | ❌         | ✅         |
-| 百炼 Bailian | ✅       | ✅       | ✅       | ❌         | ❌         |
-| 灵积 DashScope | ✅       | ✅       | ✅       | ✅         | ❌         |
-| 百川智能 Baichuan | ✅       | ✅       | ✅       | ❌         | ❌         |
-| Minimax        | ✅       | ✅       | ✅       | ❌         | ✅         |
-| 混元 Hunyuan        | ✅       | ✅       | ✅       | ❌         | ✅         |
-| 智谱 Zhipu    | ✅       | ✅       | ✅       | ✅         | ✅         |
-| 月之暗面 Moonshot| ✅       | ✅       | ✅       | ❌         | ❌         |
-| DeepSeek       | ✅       | ✅       | ✅       | ❌         | ❌         |
-| 零一万物 Yi       | ✅       | ✅       | ✅       | ❌         | ❌         |
+| 平台 🤖           | 同步 🔄 | 异步 ⏳ | 流式 🌊 | Vision 👀 | Tools 🛠️ |
+| ----------------- | ------- | ------- | ------- | --------- | -------- |
+| OpenAI            | ✅      | ✅      | ✅      | ✅        | ✅       |
+| Azure             | ✅      | ✅      | ❌      | ✅        | ✅       |
+| Anthropic         | ✅      | ✅      | ✅      | ✅        | ❌       |
+| 文心 Wenxin       | ✅      | ✅      | ✅      | ❌        | ✅       |
+| 百炼 Bailian      | ✅      | ✅      | ✅      | ❌        | ❌       |
+| 灵积 DashScope    | ✅      | ✅      | ✅      | ✅        | ❌       |
+| 百川智能 Baichuan | ✅      | ✅      | ✅      | ❌        | ❌       |
+| Minimax           | ✅      | ✅      | ✅      | ❌        | ✅       |
+| 混元 Hunyuan      | ✅      | ✅      | ✅      | ❌        | ❌       |
+| 智谱 Zhipu        | ✅      | ✅      | ✅      | ✅        | ✅       |
+| 月之暗面 Moonshot | ✅      | ✅      | ✅      | ❌        | ❌       |
+| DeepSeek          | ✅      | ✅      | ✅      | ❌        | ❌       |
+| 零一万物 Yi       | ✅      | ✅      | ✅      | ✅        | ❌       |
+| 阶跃星辰 StepFun  | ✅      | ✅      | ✅      | ✅        | ❌       |
 
 ## Features
 
-* **多模态**，支持文本生成，多模态文本生成，结构体生成，图像生成，语音生成...
-* **跨平台**，支持 OpenAI，Azure，Minimax，智谱，月之暗面，文心一言 在内的国内外 10+ 平台
-* **One API**，统一了不同平台的消息格式，推理参数，接口封装，返回解析，让用户无需关心不同平台的差异
-* **异步，流式和并发**，提供流式调用，非流式调用，同步调用，异步调用，异步批量并发调用，适配不同的应用场景
-* **自带电池**，提供 chainlit UI，输入检查，参数检查，计费，速率控制，*Agent*, *Tool call* 等
-* **轻量**，最小化依赖，不同平台的请求和鉴权逻辑均为原生内置功能
-* **高质量代码**，100% typehints，pylance strict, ruff lint & format,  test coverage > 85% ...
+- **多模态**，支持文本生成，多模态文本生成，结构体生成，图像生成，语音生成...
+- **跨平台**，支持 OpenAI，Azure，Minimax，智谱，月之暗面，文心一言 在内的国内外 10+ 平台
+- **One API**，统一了不同平台的消息格式，推理参数，接口封装，返回解析，让用户无需关心不同平台的差异
+- **异步，流式和并发**，提供流式调用，非流式调用，同步调用，异步调用，异步批量并发调用，适配不同的应用场景
+- **自带电池**，提供 chainlit UI，输入检查，参数检查，计费，速率控制，_Agent_, _Tool call_ 等
+- **轻量**，最小化依赖，不同平台的请求和鉴权逻辑均为原生内置功能
+- **高质量代码**，100% typehints，pylance strict, ruff lint & format, test coverage > 85% ...
 
 ## 基础使用
 
 <a target="_blank" href="https://colab.research.google.com/github/wangyuxinwhy/generate/blob/main/examples/tutorial.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
@@ -69,14 +92,15 @@
 DashScopeMultiModalChat
 MoonshotChat
 DeepSeekChat
 YiChat
 ```
 
 ### 配置模型 API
+
 ```python
 from generate import WenxinChat
 
 # 获取如何配置文心一言，其他模型同理
 print(WenxinChat.how_to_settings())
 
 # ----- Output -----
@@ -173,14 +197,15 @@
     cost=0.000693,
     extra={'usage': {'prompt_tokens': 75, 'completion_tokens': 12, 'total_tokens': 87}},
     structure=Country(name='France', capital='Paris')
 )
 ```
 
 #### 速率限制
+
 ```python
 import time
 from generate import OpenAIChat
 
 # 限制速率，每 10 秒最多 4 次请求
 limit_model = OpenAIChat().limit(max_generates_per_time_window=2, num_seconds_in_time_window=10)
 start_time = time.time()
@@ -196,26 +221,28 @@
 3
 elapsed time: 11.47 seconds
 4
 elapsed time: 12.15 seconds
 ```
 
 #### 对话历史保持
+
 ```python
 from generate import OpenAIChat
 
 session_model = OpenAIChat().session()
 session_model.generate('i am bob')
 print(session_model.generate('What is my name?').reply)
 
 # ----- Output -----
 Your name is Bob.
 ```
 
 #### 工具调用
+
 ```python
 from generate import OpenAIChat, tool
 
 @tool
 def get_weather(location: str) -> str:
     return f'{location}, 27°C, Sunny'
 
@@ -238,17 +265,17 @@
 ImageGenerationOutput(
     model_info=ModelInfo(task='image_generation', type='openai', name='dall-e-3'),
     cost=0.56,
     extra={},
     images=[
         GeneratedImage(
             url='https://oaidalleapiprodscus.blob.core.windows.net/...',
-            prompt='Visualize an astronomical illustration featuring a black hole at its core. The black hole 
-should be portrayed with strong gravitational lensing effect that distorts the light around it. Include a 
-surrounding accretion disk, glowing brightly with blue and white hues, streaked with shades of red and orange, 
+            prompt='Visualize an astronomical illustration featuring a black hole at its core. The black hole
+should be portrayed with strong gravitational lensing effect that distorts the light around it. Include a
+surrounding accretion disk, glowing brightly with blue and white hues, streaked with shades of red and orange,
 indicating heat and intense energy. The cosmos in the background should be filled with distant stars, galaxies, and
 nebulas, illuminating the vast, infinite space with specks of light.',
             image_format='png',
             content=b'<image bytes>'
         )
     ]
 )
@@ -268,16 +295,16 @@
     cost=0.01,
     extra={},
     audio=b'<audio bytes>',
     audio_format='mp3'
 )
 ```
 
-
 ### 多种调用方式
+
 ```python
 from generate import OpenAIChat
 
 model = OpenAIChat()
 for stream_output in model.stream_generate('介绍一下唐朝'):
     print(stream_output.stream.delta, end='', flush=True)
 
@@ -291,8 +318,8 @@
 
 ### 启动 chainlit UI
 
 ```bash
 python -m generate.ui
 # help
 # python -m generate.ui --help
-```
+```
```

### Comparing `generate_core-0.4.2/generate/__init__.py` & `generate_core-0.4.3/generate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     MinimaxProChatParameters,
     MoonshotChat,
     MoonshotChatParameters,
     OpenAIChat,
     OpenAIChatParameters,
     Prompt,
     RemoteChatCompletionModel,
+    StepFunChat,
+    StepFunChatParameters,
     WenxinChat,
     WenxinChatParameters,
     YiChat,
     YiChatParameters,
     ZhipuCharacterChat,
     ZhipuCharacterChatParameters,
     ZhipuChat,
@@ -69,14 +71,15 @@
     DashScopeSettings,
     DeepSeekSettings,
     HunyuanSettings,
     MinimaxSettings,
     MoonshotSettings,
     OpenAISettings,
     QianfanSettings,
+    StepFunSettings,
     YiSettings,
     ZhipuSettings,
 )
 from generate.text_to_speech import (
     MinimaxProSpeech,
     MinimaxProSpeechParameters,
     MinimaxSpeech,
@@ -101,14 +104,17 @@
     'MinimaxProChatParameters',
     'MinimaxLegacyChat',
     'MinimaxLegacyChatParameters',
     'ZhipuChat',
     'ZhipuChatParameters',
     'ZhipuCharacterChat',
     'ZhipuCharacterChatParameters',
+    'StepFunChat',
+    'StepFunChatParameters',
+    'StepFunSettings',
     'WenxinChat',
     'WenxinChatParameters',
     'HunyuanChat',
     'HunyuanChatParameters',
     'BaichuanChat',
     'BaichuanChatParameters',
     'BailianChat',
```

### Comparing `generate_core-0.4.2/generate/access_token_manager.py` & `generate_core-0.4.3/generate/access_token_manager.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/__init__.py` & `generate_core-0.4.3/generate/chat_completion/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     MinimaxLegacyChatParameters,
     MinimaxProChat,
     MinimaxProChatParameters,
     MoonshotChat,
     MoonshotChatParameters,
     OpenAIChat,
     OpenAIChatParameters,
+    StepFunChat,
+    StepFunChatParameters,
     WenxinChat,
     WenxinChatParameters,
     YiChat,
     YiChatParameters,
     ZhipuCharacterChat,
     ZhipuCharacterChatParameters,
     ZhipuChat,
@@ -66,14 +68,15 @@
     (HunyuanChat, HunyuanChatParameters),
     (BaichuanChat, BaichuanChatParameters),
     (BailianChat, BailianChatParameters),
     (DashScopeChat, DashScopeChatParameters),
     (DashScopeMultiModalChat, DashScopeMultiModalChatParameters),
     (MoonshotChat, MoonshotChatParameters),
     (DeepSeekChat, DashScopeChatParameters),
+    (StepFunChat, StepFunChatParameters),
     (YiChat, YiChatParameters),
 ]
 
 ChatModelRegistry: dict[str, tuple[Type[ChatCompletionModel], Type[ModelParameters]]] = {
     model_cls.model_type: (model_cls, parameter_cls) for model_cls, parameter_cls in ChatModels
 }
 
@@ -103,14 +106,16 @@
     'HunyuanChatParameters',
     'BaichuanChat',
     'BaichuanChatParameters',
     'BailianChat',
     'BailianChatParameters',
     'YiChat',
     'YiChatParameters',
+    'StepFunChat',
+    'StepFunChatParameters',
     'AnthropicChat',
     'AnthropicChatParameters',
     'DashScopeChat',
     'DashScopeChatParameters',
     'DashScopeMultiModalChat',
     'DashScopeMultiModalChatParameters',
     'MoonshotChat',
```

### Comparing `generate_core-0.4.2/generate/chat_completion/base.py` & `generate_core-0.4.3/generate/chat_completion/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,31 +25,29 @@
 
 
 logger = logging.getLogger(__name__)
 
 
 class ChatCompletionModel(GenerateModel[Prompt, ChatCompletionOutput], ABC):
     model_task: ClassVar[str] = 'chat_completion'
-    model_type: ClassVar[str]
 
     @abstractmethod
     def async_stream_generate(self, prompt: Prompt, **kwargs: Any) -> AsyncIterator[ChatCompletionStreamOutput]:
         ...
 
     def stream_generate(self, prompt: Prompt, **kwargs: Any) -> Iterator[ChatCompletionStreamOutput]:
         return sync_aiter(self.async_stream_generate(prompt, **kwargs))
 
     def structure(
-        self, output_structure_type: Type[O], instruction: str | None = None, **kwargs: Unpack['StructureModelKwargs']
+        self, output_structure_type: Type[O], **kwargs: Unpack['StructureModelKwargs']
     ) -> 'StructureGenerateModel[Self, O]':
         from generate.modifiers.structure import StructureGenerateModel
 
         return StructureGenerateModel(
             self,
-            instruction=instruction,
             output_structure_type=output_structure_type,
             **kwargs,
         )
 
     def session(self) -> 'SessionChatCompletionModel':
         from generate.modifiers.session import SessionChatCompletionModel
```

### Comparing `generate_core-0.4.2/generate/chat_completion/cost_caculator.py` & `generate_core-0.4.3/generate/chat_completion/cost_caculator.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/message/__init__.py` & `generate_core-0.4.3/generate/chat_completion/message/__init__.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/message/core.py` & `generate_core-0.4.3/generate/chat_completion/message/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from __future__ import annotations
 
+import mimetypes
+from pathlib import Path
 from typing import Any, Dict, List, Literal, Optional, Sequence, Union
 
 from pydantic import BaseModel, TypeAdapter
+from typing_extensions import Self
+
+from generate.utils import fetch_data
 
 
 class Message(BaseModel):
     role: str
     name: Optional[str] = None
     content: Any
 
@@ -34,14 +39,21 @@
     image_url: ImageUrl
 
 
 class ImagePart(BaseModel):
     image: bytes
     image_format: Optional[str] = None
 
+    @classmethod
+    def from_url_or_path(cls, url_or_path: str | Path) -> Self:
+        image_data = fetch_data(str(url_or_path))
+        mimetype = mimetypes.guess_type(url=str(url_or_path))[0]
+        image_format = mimetype.split('/')[1] if mimetype is not None else None
+        return cls(image=image_data, image_format=image_format)
+
 
 class UserMultiPartMessage(Message):
     role: Literal['user'] = 'user'
     content: List[Union[TextPart, ImageUrlPart, ImagePart]]
 
 
 class FunctionMessage(Message):
```

### Comparing `generate_core-0.4.2/generate/chat_completion/message/exception.py` & `generate_core-0.4.3/generate/chat_completion/message/exception.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/message/utils.py` & `generate_core-0.4.3/generate/chat_completion/message/utils.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/model_output.py` & `generate_core-0.4.3/generate/chat_completion/model_output.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/models/__init__.py` & `generate_core-0.4.3/generate/chat_completion/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from generate.chat_completion.models.deepseek import DeepSeekChat, DeepSeekChatParameters
 from generate.chat_completion.models.hunyuan import HunyuanChat, HunyuanChatParameters
 from generate.chat_completion.models.minimax import MinimaxChat, MinimaxChatParameters
 from generate.chat_completion.models.minimax_legacy import MinimaxLegacyChat, MinimaxLegacyChatParameters
 from generate.chat_completion.models.minimax_pro import MinimaxProChat, MinimaxProChatParameters
 from generate.chat_completion.models.moonshot import MoonshotChat, MoonshotChatParameters
 from generate.chat_completion.models.openai import OpenAIChat, OpenAIChatParameters
+from generate.chat_completion.models.stepfun import StepFunChat, StepFunChatParameters
 from generate.chat_completion.models.wenxin import WenxinChat, WenxinChatParameters
 from generate.chat_completion.models.yi import YiChat, YiChatParameters
 from generate.chat_completion.models.zhipu import (
     ZhipuCharacterChat,
     ZhipuCharacterChatParameters,
     ZhipuChat,
     ZhipuChatParameters,
@@ -45,14 +46,16 @@
     'MinimaxProChatParameters',
     'MinimaxChat',
     'MinimaxChatParameters',
     'OpenAIChat',
     'OpenAIChatParameters',
     'WenxinChat',
     'WenxinChatParameters',
+    'StepFunChat',
+    'StepFunChatParameters',
     'YiChat',
     'YiChatParameters',
     'ZhipuChat',
     'ZhipuChatParameters',
     'ZhipuCharacterChat',
     'ZhipuCharacterChatParameters',
     'DashScopeChat',
```

### Comparing `generate_core-0.4.2/generate/chat_completion/models/anthropic.py` & `generate_core-0.4.3/generate/chat_completion/models/anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,22 @@
     temperature: Optional[Temperature]
     top_p: Optional[Probability]
     top_k: Optional[PositiveInt]
 
 
 class AnthropicChat(RemoteChatCompletionModel):
     model_type: ClassVar[str] = 'anthropic'
-    available_models: ClassVar[List[str]] = ['claude-2.1', 'claude-2.0', 'claude-instant-1.2']
+    available_models: ClassVar[List[str]] = [
+        'claude-2.1',
+        'claude-2.0',
+        'claude-instant-1.2',
+        'claude-3-opus-20240229',
+        'claude-3-sonnet-20240229',
+        'claude-3-haiku-20240307',
+    ]
 
     parameters: AnthropicChatParameters
     settings: AnthropicSettings
 
     def __init__(
         self,
         model: str = 'claude-2.1',
@@ -103,15 +110,15 @@
             message_dict = {'role': 'user', 'content': []}
             for part in message.content:
                 if isinstance(part, TextPart):
                     message_dict['content'].append({'type': 'text', 'text': part.text})
 
                 if isinstance(part, ImagePart):
                     data = base64.b64encode(part.image).decode()
-                    media_type = part.image_format or 'image/jpeg'
+                    media_type = 'image/jpeg' if part.image_format is None else f'image/{part.image_format}'
                     message_dict['content'].append(
                         {'type': 'image', 'source': {'type': 'base64', 'media_type': media_type, 'data': data}}
                     )
 
                 if isinstance(part, ImageUrlPart):
                     response = self.http_client.get({'url': part.image_url.url})
                     data = base64.b64encode(response.content).decode()
```

### Comparing `generate_core-0.4.2/generate/chat_completion/models/azure.py` & `generate_core-0.4.3/generate/chat_completion/models/azure.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/models/baichuan.py` & `generate_core-0.4.3/generate/chat_completion/models/baichuan.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/models/bailian.py` & `generate_core-0.4.3/generate/chat_completion/models/bailian.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/models/dashscope.py` & `generate_core-0.4.3/generate/chat_completion/models/dashscope.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/models/dashscope_multimodal.py` & `generate_core-0.4.3/generate/chat_completion/models/dashscope_multimodal.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/models/deepseek.py` & `generate_core-0.4.3/generate/chat_completion/models/deepseek.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/models/hunyuan.py` & `generate_core-0.4.3/generate/chat_completion/models/hunyuan.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/models/minimax.py` & `generate_core-0.4.3/generate/chat_completion/models/minimax.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/models/minimax_legacy.py` & `generate_core-0.4.3/generate/chat_completion/models/minimax_legacy.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/models/minimax_pro.py` & `generate_core-0.4.3/generate/chat_completion/models/minimax_pro.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/models/moonshot.py` & `generate_core-0.4.3/generate/chat_completion/models/moonshot.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/models/openai.py` & `generate_core-0.4.3/generate/chat_completion/models/openai.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/models/openai_like.py` & `generate_core-0.4.3/generate/chat_completion/models/openai_like.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,10 +366,11 @@
             model_name=response['model'],
             input_tokens=input_tokens,
             output_tokens=output_tokens,
         )
 
     def _determine_finish_reason(self, response: ResponseValue) -> str | None:
         choice = response['choices'][0]
-        if (finish_reason := choice.get('finish_reason')) is None:
+        finish_reason = choice.get('finish_reason') or None
+        if finish_reason is None:
             finish_reason: str | None = finish_details['type'] if (finish_details := choice.get('finish_details')) else None
         return finish_reason
```

### Comparing `generate_core-0.4.2/generate/chat_completion/models/test.py` & `generate_core-0.4.3/generate/chat_completion/models/test.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/models/wenxin.py` & `generate_core-0.4.3/generate/chat_completion/models/wenxin.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/models/yi.py` & `generate_core-0.4.3/generate/chat_completion/models/yi.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 class YiParametersDict(RemoteModelParametersDict, total=False):
     temperature: Optional[Annotated[float, Field(ge=0, lt=2)]]
     max_tokens: Optional[PositiveInt]
 
 
 class YiChat(OpenAILikeChat):
     model_type: ClassVar[str] = 'yi'
-    available_models: ClassVar[List[str]] = ['yi-34b-chat', 'Yi-34B-Chat-200K']
+    available_models: ClassVar[List[str]] = ['yi-34b-chat-0205', 'yi-34b-chat-200k', 'yi-vl-plus']
 
     parameters: YiChatParameters
     settings: YiSettings
 
     def __init__(
         self,
-        model: str = 'yi-34b-chat',
+        model: str = 'yi-34b-chat-0205',
         parameters: YiChatParameters | None = None,
         settings: YiSettings | None = None,
         http_client: HttpClient | None = None,
     ) -> None:
         parameters = parameters or YiChatParameters()
         settings = settings or YiSettings()  # type: ignore
         http_client = http_client or HttpClient()
```

### Comparing `generate_core-0.4.2/generate/chat_completion/models/zhipu.py` & `generate_core-0.4.3/generate/chat_completion/models/zhipu.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/printer.py` & `generate_core-0.4.3/generate/chat_completion/printer.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/stream_manager.py` & `generate_core-0.4.3/generate/chat_completion/stream_manager.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/chat_completion/tool.py` & `generate_core-0.4.3/generate/chat_completion/tool.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/highlevel.py` & `generate_core-0.4.3/generate/highlevel.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,33 +23,33 @@
 )
 
 
 def load_chat_model(model_id: str) -> ChatCompletionModel:
     if '/' not in model_id:
         model_type = model_id
         return ChatModelRegistry[model_type][0]()
-    model_type, name = model_id.split('/')
+    model_type, name = model_id.split('/', maxsplit=1)
     model_cls = ChatModelRegistry[model_type][0]
     return model_cls.from_name(name)
 
 
 def load_speech_model(model_id: str) -> TextToSpeechModel:
     if '/' not in model_id:
         model_type = model_id
         return SpeechModelRegistry[model_type][0]()
-    model_type, name = model_id.split('/')
+    model_type, name = model_id.split('/', maxsplit=1)
     model_cls = SpeechModelRegistry[model_type][0]
     return model_cls.from_name(name)
 
 
 def load_image_generation_model(model_id: str) -> ImageGenerationModel:
     if '/' not in model_id:
         model_type = model_id
         return ImageGenerationModelRegistry[model_type][0]()
-    model_type, name = model_id.split('/')
+    model_type, name = model_id.split('/', maxsplit=1)
     model_cls = ImageGenerationModelRegistry[model_type][0]
     return model_cls.from_name(name)
 
 
 def generate_text(prompt: Prompt, model_id: str = 'openai', **kwargs: Any) -> ChatCompletionOutput:
     model = load_chat_model(model_id)
     return model.generate(prompt, **kwargs)
```

### Comparing `generate_core-0.4.2/generate/http.py` & `generate_core-0.4.3/generate/http.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/image_generation/__init__.py` & `generate_core-0.4.3/generate/image_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/image_generation/base.py` & `generate_core-0.4.3/generate/image_generation/base.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/image_generation/models/__init__.py` & `generate_core-0.4.3/generate/image_generation/models/__init__.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/image_generation/models/baidu.py` & `generate_core-0.4.3/generate/image_generation/models/baidu.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         output_data = {}
         width, height = self.size.split('x')
         output_data['width'] = int(width)
         output_data['height'] = int(height)
         n = self.n or 1
         output_data['image_num'] = n
         if self.reference_image:
-            if isinstance(self.reference_image, HttpUrl):
+            if isinstance(self.reference_image, str):
                 output_data['url'] = self.reference_image
             else:
                 output_data['image'] = self.reference_image
         if self.change_degree:
             output_data['change_degree'] = self.change_degree
         return output_data
```

### Comparing `generate_core-0.4.2/generate/image_generation/models/openai.py` & `generate_core-0.4.3/generate/image_generation/models/openai.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/image_generation/models/qianfan.py` & `generate_core-0.4.3/generate/image_generation/models/qianfan.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/image_generation/models/zhipu.py` & `generate_core-0.4.3/generate/image_generation/models/zhipu.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/model.py` & `generate_core-0.4.3/generate/model.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/modifiers/agent.py` & `generate_core-0.4.3/generate/modifiers/agent.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/modifiers/hook.py` & `generate_core-0.4.3/generate/modifiers/hook.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/modifiers/limit.py` & `generate_core-0.4.3/generate/modifiers/limit.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/modifiers/session.py` & `generate_core-0.4.3/generate/modifiers/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,28 +43,32 @@
         self.history.append(model_output.message)
         return model_output
 
     @override
     def stream_generate(self, prompt: Prompt, **kwargs: Any) -> Iterator[ChatCompletionStreamOutput]:
         messages = ensure_messages(prompt)
         self.history.extend(messages)
+        finished = False
         for stream_output in self.model.stream_generate(self.history, **kwargs):
-            yield stream_output
+            if not finished:
+                yield stream_output
             if stream_output.is_finish:
+                finished = True
                 self.history.append(stream_output.message)
-                return
 
     @override
     async def async_stream_generate(self, prompt: Prompt, **kwargs: Any) -> AsyncIterator[ChatCompletionStreamOutput]:
         messages = ensure_messages(prompt)
         self.history.extend(messages)
+        finished = False
         async for stream_output in self.model.async_stream_generate(self.history, **kwargs):
-            yield stream_output
+            if not finished:
+                yield stream_output
             if stream_output.is_finish:
+                finished = True
                 self.history.append(stream_output.message)
-                return
 
     async def async_batch_generate(self, prompts: Iterable[Prompt], **kwargs: Any) -> NoReturn:
         raise RuntimeError('Async Batch generation is not supported for session model')
 
     def reset(self) -> None:
         self.history.clear()
```

### Comparing `generate_core-0.4.2/generate/modifiers/structure.py` & `generate_core-0.4.3/generate/modifiers/structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,37 +108,41 @@
 
 
 class StructureModelOutput(ModelOutput, Generic[O]):
     structure: O
 
 
 class StructureModelKwargs(TypedDict, Generic[O], total=False):
+    instruction: Optional[str]
     examples: Optional[Iterable[Example[O]]]
     system_template: str
     max_num_reask: int
+    output_exclude_none: bool
 
 
 class StructureGenerateModel(GenerateModel[str, StructureModelOutput[O]], Generic[M, O]):
     model_task: ClassVar[str] = 'text_to_structure'
 
     def __init__(
         self,
         model: M,
         output_structure_type: Type[O],
         instruction: str | None = None,
         examples: Optional[Iterable[Example[O]]] = None,
         system_template: str = system_template,
+        output_exclude_none: bool = True,
         max_num_reask: int = 2,
     ) -> None:
         self.model = model
         self.instruction = instruction or f'Extract {output_structure_type.__name__}'
         self.output_structure_type = output_structure_type
         self.examples = examples or []
         self.system_template = system_template
         self.max_num_reask = max_num_reask
+        self.output_exclude_none = output_exclude_none
 
         self.model_type = self.model.model_type  # type: ignore
 
     @property
     def name(self) -> str:
         return self.model.name
 
@@ -148,15 +152,15 @@
 
     @property
     def messages(self) -> List[UnionMessage]:
         messages = []
         messages.append(self.system_message)
         for example in self.examples:
             messages.extend(ensure_messages(example.prompt))
-            messages.append(AssistantMessage(content=example.output.model_dump_json(exclude_none=True)))
+            messages.append(AssistantMessage(content=example.output.model_dump_json(exclude_none=self.output_exclude_none)))
         return messages
 
     @property
     def _output_format_description(self) -> str:
         json_schema = self.output_structure_type.model_json_schema()
         have_ref = '$defs' in json_schema
         if have_ref:
```

### Comparing `generate_core-0.4.2/generate/platforms/__init__.py` & `generate_core-0.4.3/generate/platforms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from generate.platforms.base import PlatformSettings
 from generate.platforms.dashscope import DashScopeSettings
 from generate.platforms.deepseek import DeepSeekSettings
 from generate.platforms.hunyuan import HunyuanSettings
 from generate.platforms.minimax import MinimaxSettings
 from generate.platforms.moonshot import MoonshotSettings
 from generate.platforms.openai import OpenAISettings
+from generate.platforms.stepfun import StepFunSettings
 from generate.platforms.yi import YiSettings
 from generate.platforms.zhipu import ZhipuSettings
 
 __all__ = [
     'AzureSettings',
     'AnthropicSettings',
     'BaichuanSettings',
@@ -25,8 +26,9 @@
     'BailianSettings',
     'HunyuanSettings',
     'DashScopeSettings',
     'MoonshotSettings',
     'DeepSeekSettings',
     'YiSettings',
     'PlatformSettings',
+    'StepFunSettings',
 ]
```

### Comparing `generate_core-0.4.2/generate/platforms/baidu.py` & `generate_core-0.4.3/generate/platforms/baidu.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/platforms/bailian.py` & `generate_core-0.4.3/generate/platforms/bailian.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/platforms/base.py` & `generate_core-0.4.3/generate/platforms/base.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/platforms/hunyuan.py` & `generate_core-0.4.3/generate/platforms/hunyuan.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/platforms/zhipu.py` & `generate_core-0.4.3/generate/platforms/zhipu.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class ZhipuSettings(PlatformSettings):
     model_config = SettingsConfigDict(extra='ignore', env_prefix='zhipu_', env_file='.env')
 
     api_key: SecretStr
     v3_api_base: str = 'https://open.bigmodel.cn/api/paas/v3/model-api'
-    v4_api_base: str = 'https://open.bigmodel.cn/api/paas/v4/'
+    v4_api_base: str = 'https://open.bigmodel.cn/api/paas/v4'
     platform_url: str = 'https://open.bigmodel.cn/dev/howuse/introduction'
 
 
 @cachetools.func.ttl_cache(ttl=CACHE_TTL_SECONDS)
 def generate_zhipu_token(api_key: str) -> str:
     try:
         api_key, secret = api_key.split('.')
```

### Comparing `generate_core-0.4.2/generate/test.py` & `generate_core-0.4.3/generate/test.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/text_to_speech/__init__.py` & `generate_core-0.4.3/generate/text_to_speech/__init__.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/text_to_speech/base.py` & `generate_core-0.4.3/generate/text_to_speech/base.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/text_to_speech/models/minimax.py` & `generate_core-0.4.3/generate/text_to_speech/models/minimax.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/text_to_speech/models/openai.py` & `generate_core-0.4.3/generate/text_to_speech/models/openai.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.2/generate/ui.py` & `generate_core-0.4.3/generate/ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 
-from typing import Any, List, Optional, cast
+from typing import Any, List, Optional, Type, cast
 
 from pydantic import BaseModel
 
+from generate.chat_completion.base import RemoteChatCompletionModel
 from generate.chat_completion.models.dashscope_multimodal import DashScopeMultiModalChat
+from generate.model import ModelInfo
 
 try:
     import chainlit as cl
     import typer
     from chainlit.element import Avatar
     from chainlit.input_widget import Select, Slider, TextInput
 except ImportError as e:
     raise ImportError('Please install chainlit with "pip install chainlit typer"') from e
 
-from generate import ChatCompletionModel, load_chat_model
+from generate import ChatCompletionModel, ChatModelRegistry, load_chat_model
 from generate.chat_completion.message import (
     ImagePart,
     ImageUrl,
     ImageUrlPart,
     Messages,
     SystemMessage,
     TextPart,
@@ -60,34 +62,32 @@
         'moonshot': 'https://yuxin-wang.oss-cn-beijing.aliyuncs.com/uPic/hc2Ygt.png',
         'deepseek': 'https://yuxin-wang.oss-cn-beijing.aliyuncs.com/uPic/SgdohV.png',
     }
     return [Avatar(name=k, url=v) for k, v in avatar_map.items()]
 
 
 def get_generate_settings() -> List[Any]:
+    available_model_ids = []
+    for model_cls, _ in ChatModelRegistry.values():
+        model_cls = cast(Type[RemoteChatCompletionModel], model_cls)
+        for model_name in model_cls.available_models:
+            model_info = ModelInfo(
+                task=model_cls.model_task,
+                type=model_cls.model_type,
+                name=model_name,
+            )
+            available_model_ids.append(model_info.model_id)
     model_select = Select(
         id='Model',
         label='Model',
-        values=[
-            'openai',
-            'openai/gpt-4-vision-preview',
-            'dashscope',
-            'dashscope_multimodal',
-            'zhipu',
-            'zhipu/glm-4v',
-            'wenxin',
-            'baichuan',
-            'minimax_pro',
-            'moonshot',
-            'deepseek',
-        ],
+        values=available_model_ids,
     )
     model_id = TextInput(
         id='ModelId',
-        label='Model ID',
+        label='Custom Model ID',
         initial='',
         description='如 openai/gpt-4-turbo-preview，此设置会覆盖 Model 选项。',
     )
     system_message_input = TextInput(
         id='SystemMessage',
         label='System Message',
         initial='',
```

### Comparing `generate_core-0.4.2/pyproject.toml` & `generate_core-0.4.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,78 +1,81 @@
 [tool.poetry]
 name = "generate-core"
-version = "0.4.2"
+version = "0.4.3"
 description = "文本生成，图像生成，语音生成"
 authors = ["wangyuxin <wangyuxin@mokahr.com>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "generate"}]
+packages = [{ include = "generate" }]
 repository = "https://github.com/wangyuxinwhy/generate"
 keywords = ["openai", "text generation", "image generation", "text to speech"]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 asyncer = "0.0.2"
 typing-extensions = "^4.6.2"
 httpx = "^0.24.1"
 tenacity = "^8.2.2"
 pyjwt = "^2.8.0"
 cachetools = "^5.3.1"
 tqdm = "^4.66.1"
 pydantic = "^2.0"
 docstring-parser = "^0.15"
-anyio = "<4.0.0"
-httpx-sse = "0.3.1"
+httpx-sse = "^0.4.0"
 pydantic-settings = "^2.1.0"
 
 [tool.ruff]
 line-length = 128
-select = [
-    "E",  # pycodestyle errors
-    "W",  # pycodestyle warnings
-    "F",  # pyflakes
-    "I",  # isort
-    "C",  # flake8-comprehensions
-    "B",  # flake8-bugbear
+lint.select = [
+    "E",    # pycodestyle errors
+    "W",    # pycodestyle warnings
+    "F",    # pyflakes
+    "I",    # isort
+    "C",    # flake8-comprehensions
+    "B",    # flake8-bugbear
     "N",
     "SIM",
     "ANN",
     "A",
     "T",
     "PT",
     "RET",
     "TRY",
     "PERF",
 ]
-ignore = [
-    "E501",  # line too long, handled by black
-    "B008",  # do not perform function calls in argument defaults
-    "B905",  # zip strict
-    "C901",  # too complex
-    "A003",  # shadow builtin 
-    "ANN1",  # self and cls
-    "ANN401", # Dynamically typed expressions (typing.Any) are disallowed in
-    "TRY003", # Avoid specifying long messages outside the exception class
+lint.ignore = [
+    "E501",    # line too long, handled by black
+    "B008",    # do not perform function calls in argument defaults
+    "B905",    # zip strict
+    "C901",    # too complex
+    "A003",    # shadow builtin 
+    "ANN1",    # self and cls
+    "ANN401",  # Dynamically typed expressions (typing.Any) are disallowed in
+    "TRY003",  # Avoid specifying long messages outside the exception class
     "PLC0414", # reimport
 ]
 exclude = ["playground", "api_docs"]
 target-version = "py38"
-
-[tool.ruff.format]
-quote-style = "single"
+format.quote-style = "single"
+# [tool.ruff.format]
+# quote-style = "single"
 
 [tool.pyright]
-reportMissingTypeStubs=false
+reportMissingTypeStubs = false
+# TODO: remove this when all errors are fixed
+reportIncompatibleVariableOverride = false
+reportIncompatibleMethodOverride = false
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pyright = "^1.1.310"
 ruff = "^0.1.4"
 coverage = "^7.3.2"
 mkdocs-material = "^9.5.12"
+pytest-mock = "^3.12.0"
 
 [tool.poetry.group.bailian.dependencies]
 broadscope-bailian = "^1.1.8"
 
 
 [tool.poetry.group.ui.dependencies]
 chainlit = "^1.0.200"
```

### Comparing `generate_core-0.4.2/PKG-INFO` & `generate_core-0.4.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,73 +1,95 @@
 Metadata-Version: 2.1
 Name: generate-core
-Version: 0.4.2
+Version: 0.4.3
 Summary: 文本生成，图像生成，语音生成
 Home-page: https://github.com/wangyuxinwhy/generate
 License: MIT
 Keywords: openai,text generation,image generation,text to speech
 Author: wangyuxin
 Author-email: wangyuxin@mokahr.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: anyio (<4.0.0)
 Requires-Dist: asyncer (==0.0.2)
 Requires-Dist: cachetools (>=5.3.1,<6.0.0)
 Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: httpx-sse (==0.3.1)
+Requires-Dist: httpx-sse (>=0.4.0,<0.5.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Requires-Dist: typing-extensions (>=4.6.2,<5.0.0)
 Project-URL: Repository, https://github.com/wangyuxinwhy/generate
 Description-Content-Type: text/markdown
 
-# Generate
+<div align="center">
+  <img src="logo/logo.png" alt="Generate Logo" width="200"/>
+</div>
+
+<div align="center">
+    <h1>Generate</h1>
+    <p>
+        A Python Package to Access World-Class Generative Models.
+    </p>
+    <p>
+        <a href="https://wangyuxinwhy.github.io/generate/">中文文档</a>
+        ｜
+        <a href="https://colab.research.google.com/github/wangyuxinwhy/generate/blob/main/examples/tutorial.ipynb">交互式教程</a>
+    </p>
+
+[![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)](#)
+[![CI Status](https://github.com/wangyuxinwhy/generate/actions/workflows/ci.yml/badge.svg)](https://github.com/wangyuxinwhy/generate/actions/workflows/ci.yml)
+[![CD Status](https://github.com/wangyuxinwhy/generate/actions/workflows/cd.yml/badge.svg)](https://github.com/wangyuxinwhy/generate/actions/workflows/cd.yml)
+[![License](https://img.shields.io/github/license/wangyuxinwhy/generate)](https://github.com/wangyuxinwhy/generate/blob/main/LICENSE)
+[![Documentation](https://img.shields.io/badge/docs-latest-brightgreen.svg)](https://wangyuxinwhy.github.io/generate/)
+[![Made with Love](https://img.shields.io/badge/made%20with-love-red.svg)](#)
+
+</div>
+<br>
+<br>
 
-[文档](https://wangyuxinwhy.github.io/generate/)
+# 简介
 
-> A Python Package to Access World-Class Generative Models.
 
-## 简介
 
 Generate 允许用户通过统一的 api 访问多平台的生成式模型，当前支持：
 
-| 平台 🤖       | 同步 🔄 | 异步 ⏳ | 流式 🌊 | Vision 👀 | Tools 🛠️ |
-|----------------|---------|---------|---------|-----------|-----------|
-| OpenAI         | ✅       | ✅       | ✅       | ✅         | ✅         |
-| Azure         | ✅       | ✅       | ❌       | ✅         | ✅         |
-| Anthropic         | ✅       | ✅       | ✅       | ✅         | ❌         |
-| 文心 Wenxin | ✅       | ✅       | ✅       | ❌         | ✅         |
-| 百炼 Bailian | ✅       | ✅       | ✅       | ❌         | ❌         |
-| 灵积 DashScope | ✅       | ✅       | ✅       | ✅         | ❌         |
-| 百川智能 Baichuan | ✅       | ✅       | ✅       | ❌         | ❌         |
-| Minimax        | ✅       | ✅       | ✅       | ❌         | ✅         |
-| 混元 Hunyuan        | ✅       | ✅       | ✅       | ❌         | ✅         |
-| 智谱 Zhipu    | ✅       | ✅       | ✅       | ✅         | ✅         |
-| 月之暗面 Moonshot| ✅       | ✅       | ✅       | ❌         | ❌         |
-| DeepSeek       | ✅       | ✅       | ✅       | ❌         | ❌         |
-| 零一万物 Yi       | ✅       | ✅       | ✅       | ❌         | ❌         |
+| 平台 🤖           | 同步 🔄 | 异步 ⏳ | 流式 🌊 | Vision 👀 | Tools 🛠️ |
+| ----------------- | ------- | ------- | ------- | --------- | -------- |
+| OpenAI            | ✅      | ✅      | ✅      | ✅        | ✅       |
+| Azure             | ✅      | ✅      | ❌      | ✅        | ✅       |
+| Anthropic         | ✅      | ✅      | ✅      | ✅        | ❌       |
+| 文心 Wenxin       | ✅      | ✅      | ✅      | ❌        | ✅       |
+| 百炼 Bailian      | ✅      | ✅      | ✅      | ❌        | ❌       |
+| 灵积 DashScope    | ✅      | ✅      | ✅      | ✅        | ❌       |
+| 百川智能 Baichuan | ✅      | ✅      | ✅      | ❌        | ❌       |
+| Minimax           | ✅      | ✅      | ✅      | ❌        | ✅       |
+| 混元 Hunyuan      | ✅      | ✅      | ✅      | ❌        | ❌       |
+| 智谱 Zhipu        | ✅      | ✅      | ✅      | ✅        | ✅       |
+| 月之暗面 Moonshot | ✅      | ✅      | ✅      | ❌        | ❌       |
+| DeepSeek          | ✅      | ✅      | ✅      | ❌        | ❌       |
+| 零一万物 Yi       | ✅      | ✅      | ✅      | ✅        | ❌       |
+| 阶跃星辰 StepFun  | ✅      | ✅      | ✅      | ✅        | ❌       |
 
 ## Features
 
-* **多模态**，支持文本生成，多模态文本生成，结构体生成，图像生成，语音生成...
-* **跨平台**，支持 OpenAI，Azure，Minimax，智谱，月之暗面，文心一言 在内的国内外 10+ 平台
-* **One API**，统一了不同平台的消息格式，推理参数，接口封装，返回解析，让用户无需关心不同平台的差异
-* **异步，流式和并发**，提供流式调用，非流式调用，同步调用，异步调用，异步批量并发调用，适配不同的应用场景
-* **自带电池**，提供 chainlit UI，输入检查，参数检查，计费，速率控制，*Agent*, *Tool call* 等
-* **轻量**，最小化依赖，不同平台的请求和鉴权逻辑均为原生内置功能
-* **高质量代码**，100% typehints，pylance strict, ruff lint & format,  test coverage > 85% ...
+- **多模态**，支持文本生成，多模态文本生成，结构体生成，图像生成，语音生成...
+- **跨平台**，支持 OpenAI，Azure，Minimax，智谱，月之暗面，文心一言 在内的国内外 10+ 平台
+- **One API**，统一了不同平台的消息格式，推理参数，接口封装，返回解析，让用户无需关心不同平台的差异
+- **异步，流式和并发**，提供流式调用，非流式调用，同步调用，异步调用，异步批量并发调用，适配不同的应用场景
+- **自带电池**，提供 chainlit UI，输入检查，参数检查，计费，速率控制，_Agent_, _Tool call_ 等
+- **轻量**，最小化依赖，不同平台的请求和鉴权逻辑均为原生内置功能
+- **高质量代码**，100% typehints，pylance strict, ruff lint & format, test coverage > 85% ...
 
 ## 基础使用
 
 <a target="_blank" href="https://colab.research.google.com/github/wangyuxinwhy/generate/blob/main/examples/tutorial.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
@@ -100,14 +122,15 @@
 DashScopeMultiModalChat
 MoonshotChat
 DeepSeekChat
 YiChat
 ```
 
 ### 配置模型 API
+
 ```python
 from generate import WenxinChat
 
 # 获取如何配置文心一言，其他模型同理
 print(WenxinChat.how_to_settings())
 
 # ----- Output -----
@@ -204,14 +227,15 @@
     cost=0.000693,
     extra={'usage': {'prompt_tokens': 75, 'completion_tokens': 12, 'total_tokens': 87}},
     structure=Country(name='France', capital='Paris')
 )
 ```
 
 #### 速率限制
+
 ```python
 import time
 from generate import OpenAIChat
 
 # 限制速率，每 10 秒最多 4 次请求
 limit_model = OpenAIChat().limit(max_generates_per_time_window=2, num_seconds_in_time_window=10)
 start_time = time.time()
@@ -227,26 +251,28 @@
 3
 elapsed time: 11.47 seconds
 4
 elapsed time: 12.15 seconds
 ```
 
 #### 对话历史保持
+
 ```python
 from generate import OpenAIChat
 
 session_model = OpenAIChat().session()
 session_model.generate('i am bob')
 print(session_model.generate('What is my name?').reply)
 
 # ----- Output -----
 Your name is Bob.
 ```
 
 #### 工具调用
+
 ```python
 from generate import OpenAIChat, tool
 
 @tool
 def get_weather(location: str) -> str:
     return f'{location}, 27°C, Sunny'
 
@@ -269,17 +295,17 @@
 ImageGenerationOutput(
     model_info=ModelInfo(task='image_generation', type='openai', name='dall-e-3'),
     cost=0.56,
     extra={},
     images=[
         GeneratedImage(
             url='https://oaidalleapiprodscus.blob.core.windows.net/...',
-            prompt='Visualize an astronomical illustration featuring a black hole at its core. The black hole 
-should be portrayed with strong gravitational lensing effect that distorts the light around it. Include a 
-surrounding accretion disk, glowing brightly with blue and white hues, streaked with shades of red and orange, 
+            prompt='Visualize an astronomical illustration featuring a black hole at its core. The black hole
+should be portrayed with strong gravitational lensing effect that distorts the light around it. Include a
+surrounding accretion disk, glowing brightly with blue and white hues, streaked with shades of red and orange,
 indicating heat and intense energy. The cosmos in the background should be filled with distant stars, galaxies, and
 nebulas, illuminating the vast, infinite space with specks of light.',
             image_format='png',
             content=b'<image bytes>'
         )
     ]
 )
@@ -299,16 +325,16 @@
     cost=0.01,
     extra={},
     audio=b'<audio bytes>',
     audio_format='mp3'
 )
 ```
 
-
 ### 多种调用方式
+
 ```python
 from generate import OpenAIChat
 
 model = OpenAIChat()
 for stream_output in model.stream_generate('介绍一下唐朝'):
     print(stream_output.stream.delta, end='', flush=True)
 
@@ -323,7 +349,8 @@
 ### 启动 chainlit UI
 
 ```bash
 python -m generate.ui
 # help
 # python -m generate.ui --help
 ```
+
```

