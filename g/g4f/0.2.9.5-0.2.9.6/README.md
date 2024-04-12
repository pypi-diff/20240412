# Comparing `tmp/g4f-0.2.9.5.tar.gz` & `tmp/g4f-0.2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.2.9.5.tar", last modified: Fri Apr 12 16:03:41 2024, max compression
+gzip compressed data, was "g4f-0.2.9.6.tar", last modified: Fri Apr 12 19:03:40 2024, max compression
```

## Comparing `g4f-0.2.9.5.tar` & `g4f-0.2.9.6.tar`

### file list

```diff
@@ -1,236 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.427513 g4f-0.2.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-12 16:03:37.000000 g4f-0.2.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 16:03:37.000000 g4f-0.2.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    49179 2024-04-12 16:03:41.427513 g4f-0.2.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    45983 2024-04-12 16:03:37.000000 g4f-0.2.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.387513 g4f-0.2.9.5/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.395513 g4f-0.2.9.5/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    20730 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/Llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.395513 g4f-0.2.9.5/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.403513 g4f-0.2.9.5/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.403513 g4f-0.2.9.5/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.403513 g4f-0.2.9.5/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    31603 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.407513 g4f-0.2.9.5/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.407513 g4f-0.2.9.5/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.407513 g4f-0.2.9.5/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.407513 g4f-0.2.9.5/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.407513 g4f-0.2.9.5/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/openai/har_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.411513 g4f-0.2.9.5/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.411513 g4f-0.2.9.5/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/unfinished/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.411513 g4f-0.2.9.5/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.411513 g4f-0.2.9.5/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.415513 g4f-0.2.9.5/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.415513 g4f-0.2.9.5/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.415513 g4f-0.2.9.5/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.383514 g4f-0.2.9.5/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.415513 g4f-0.2.9.5/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    22498 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.415513 g4f-0.2.9.5/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.419513 g4f-0.2.9.5/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    45840 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.419513 g4f-0.2.9.5/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.419513 g4f-0.2.9.5/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.419513 g4f-0.2.9.5/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.423513 g4f-0.2.9.5/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.423513 g4f-0.2.9.5/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9438 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.423513 g4f-0.2.9.5/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-12 16:03:37.000000 g4f-0.2.9.5/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:41.423513 g4f-0.2.9.5/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    49179 2024-04-12 16:03:41.000000 g4f-0.2.9.5/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-04-12 16:03:41.000000 g4f-0.2.9.5/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:03:41.000000 g4f-0.2.9.5/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 16:03:41.000000 g4f-0.2.9.5/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-12 16:03:41.000000 g4f-0.2.9.5/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 16:03:41.000000 g4f-0.2.9.5/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:03:41.427513 g4f-0.2.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-12 16:03:37.000000 g4f-0.2.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.139410 g4f-0.2.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-12 19:03:36.000000 g4f-0.2.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 19:03:36.000000 g4f-0.2.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    49179 2024-04-12 19:03:40.139410 g4f-0.2.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    45983 2024-04-12 19:03:36.000000 g4f-0.2.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.099410 g4f-0.2.9.6/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.107410 g4f-0.2.9.6/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/Llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.111410 g4f-0.2.9.6/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.115410 g4f-0.2.9.6/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.115410 g4f-0.2.9.6/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.119410 g4f-0.2.9.6/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31632 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.119410 g4f-0.2.9.6/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.119410 g4f-0.2.9.6/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.119410 g4f-0.2.9.6/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.123410 g4f-0.2.9.6/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.123410 g4f-0.2.9.6/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/openai/har_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.123410 g4f-0.2.9.6/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.123410 g4f-0.2.9.6/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/unfinished/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.123410 g4f-0.2.9.6/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.127410 g4f-0.2.9.6/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.127410 g4f-0.2.9.6/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.127410 g4f-0.2.9.6/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.127410 g4f-0.2.9.6/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.095410 g4f-0.2.9.6/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.127410 g4f-0.2.9.6/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    22498 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.127410 g4f-0.2.9.6/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.131410 g4f-0.2.9.6/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    45880 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.131410 g4f-0.2.9.6/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.131410 g4f-0.2.9.6/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.131410 g4f-0.2.9.6/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.135410 g4f-0.2.9.6/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.135410 g4f-0.2.9.6/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9438 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.135410 g4f-0.2.9.6/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-12 19:03:36.000000 g4f-0.2.9.6/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:03:40.135410 g4f-0.2.9.6/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49179 2024-04-12 19:03:40.000000 g4f-0.2.9.6/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-12 19:03:40.000000 g4f-0.2.9.6/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:03:40.000000 g4f-0.2.9.6/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 19:03:40.000000 g4f-0.2.9.6/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-12 19:03:40.000000 g4f-0.2.9.6/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 19:03:40.000000 g4f-0.2.9.6/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:03:40.139410 g4f-0.2.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-12 19:03:36.000000 g4f-0.2.9.6/setup.py
```

### Comparing `g4f-0.2.9.5/LICENSE` & `g4f-0.2.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/PKG-INFO` & `g4f-0.2.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.2.9.5
+Version: 0.2.9.6
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.2.9.5 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.2.9.6 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.2.9.5/README.md` & `g4f-0.2.9.6/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/Aura.py` & `g4f-0.2.9.6/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/Bing.py` & `g4f-0.2.9.6/g4f/Provider/Bing.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import random
 import json
 import uuid
 import time
 import asyncio
 from urllib import parse
-from datetime import datetime
+from datetime import datetime, date
 from aiohttp import ClientSession, ClientTimeout, BaseConnector, WSMsgType
 
 from ..typing import AsyncResult, Messages, ImageType, Cookies
 from ..image import ImageRequest
 from ..errors import ResponseStatusError, RateLimitError
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
 from .helper import get_connector, get_random_hex
@@ -28,14 +28,15 @@
     precise = "Precise"
     copilot = "Copilot"
 
 class Bing(AsyncGeneratorProvider, ProviderModelMixin):
     """
     Bing provider for generating responses using the Bing API.
     """
+    label = "Microsoft Copilot in Bing"
     url = "https://bing.com/chat"
     working = True
     supports_message_history = True
     supports_gpt_4 = True
     default_model = "Balanced"
     models = [getattr(Tones, key) for key in Tones.__dict__ if not key.startswith("__")]
         
@@ -43,15 +44,15 @@
     def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
         timeout: int = 900,
         api_key: str = None,
-        cookies: Cookies = {},
+        cookies: Cookies = None,
         connector: BaseConnector = None,
         tone: str = None,
         image: ImageType = None,
         web_search: bool = False,
         context: str = None,
         **kwargs
     ) -> AsyncResult:
@@ -65,25 +66,23 @@
         :param cookies: Cookies for the session.
         :param tone: The tone of the response.
         :param image: The image type to be used.
         :param web_search: Flag to enable or disable web search.
         :return: An asynchronous result object.
         """
         prompt = messages[-1]["content"]
-        if api_key is not None:
-            cookies["_U"] = api_key
         if context is None:
             context = create_context(messages[:-1]) if len(messages) > 1 else None
         if tone is None:
             tone = tone if model.startswith("gpt-4") else model
         tone = cls.get_model("" if tone is None else tone)
         gpt4_turbo = True if model.startswith("gpt-4-turbo") else False
 
         return stream_generate(
-            prompt, tone, image, context, cookies,
+            prompt, tone, image, context, api_key, cookies,
             get_connector(connector, proxy, True),
             proxy, web_search, gpt4_turbo, timeout,
             **kwargs
         )
 
 def create_context(messages: Messages) -> str:
     """
@@ -106,19 +105,23 @@
     return {
         'SRCHD'         : 'AF=NOFORM',
         'PPLState'      : '1',
         'KievRPSSecAuth': '',
         'SUID'          : '',
         'SRCHUSR'       : '',
         'SRCHHPGUSR'    : f'HV={int(time.time())}',
+        'BCP'           : 'AD=1&AL=1&SM=1',
+        '_Rwho'         : f'u=d&ts={date.today().isoformat()}',
     }
 
-def create_headers(cookies: Cookies = None) -> dict:
+def create_headers(cookies: Cookies = None, api_key: str = None) -> dict:
     if cookies is None:
         cookies = get_default_cookies()
+    if api_key is not None:
+        cookies["_U"] = api_key
     headers = Defaults.headers.copy()
     headers["cookie"] = "; ".join(f"{k}={v}" for k, v in cookies.items())
     headers["x-forwarded-for"] = get_ip_address()
     return headers
 
 class Defaults:
     """
@@ -360,14 +363,15 @@
 
 async def stream_generate(
     prompt: str,
     tone: str,
     image: ImageType = None,
     context: str = None,
     cookies: dict = None,
+    api_key: str = None,
     connector: BaseConnector = None,
     proxy: str = None,
     web_search: bool = False,
     gpt4_turbo: bool = False,
     timeout: int = 900,
     conversation: Conversation = None,
     return_conversation: bool = False,
@@ -385,15 +389,15 @@
     :param context: Additional context for the prompt.
     :param cookies: Cookies for the session.
     :param web_search: Flag to enable web search.
     :param gpt4_turbo: Flag to enable GPT-4 Turbo.
     :param timeout: Timeout for the request.
     :return: An asynchronous generator yielding responses.
     """
-    headers = create_headers(cookies)
+    headers = create_headers(cookies, api_key)
     new_conversation = conversation is None
     max_retries = (5 if new_conversation else 0) if max_retries is None else max_retries
     async with ClientSession(
         timeout=ClientTimeout(total=timeout), connector=connector
     ) as session:
         first = True
         while first or conversation is None:
```

### Comparing `g4f-0.2.9.5/g4f/Provider/BingCreateImages.py` & `g4f-0.2.9.6/g4f/Provider/BingCreateImages.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from ..image import ImageResponse
 from ..errors import MissingRequirementsError, MissingAuthError
 from ..typing import AsyncResult, Messages, Cookies
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
 from .bing.create_images import create_images, create_session, get_cookies_from_browser
 
 class BingCreateImages(AsyncGeneratorProvider, ProviderModelMixin):
+    label = "Microsoft Designer"
     url = "https://www.bing.com/images/create"
     working = True
 
     def __init__(self, cookies: Cookies = None, proxy: str = None) -> None:
         self.cookies: Cookies = cookies
         self.proxy: str = proxy
```

### Comparing `g4f-0.2.9.5/g4f/Provider/ChatForAi.py` & `g4f-0.2.9.6/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/Chatgpt4Online.py` & `g4f-0.2.9.6/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/ChatgptAi.py` & `g4f-0.2.9.6/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/ChatgptFree.py` & `g4f-0.2.9.6/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/ChatgptNext.py` & `g4f-0.2.9.6/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/ChatgptX.py` & `g4f-0.2.9.6/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/DeepInfra.py` & `g4f-0.2.9.6/g4f/Provider/DeepInfra.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import requests
 from ..typing import AsyncResult, Messages
 from .needs_auth.Openai import Openai
 
 class DeepInfra(Openai):
+    label = "DeepInfra"
     url = "https://deepinfra.com"
     working = True
     needs_auth = False
     supports_stream = True
     supports_message_history = True
     default_model = 'meta-llama/Llama-2-70b-chat-hf'
```

### Comparing `g4f-0.2.9.5/g4f/Provider/DeepInfraImage.py` & `g4f-0.2.9.6/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/DuckDuckGo.py` & `g4f-0.2.9.6/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/FlowGpt.py` & `g4f-0.2.9.6/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/FreeChatgpt.py` & `g4f-0.2.9.6/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/FreeGpt.py` & `g4f-0.2.9.6/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/GeminiPro.py` & `g4f-0.2.9.6/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/GeminiProChat.py` & `g4f-0.2.9.6/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/GigaChat.py` & `g4f-0.2.9.6/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/GptTalkRu.py` & `g4f-0.2.9.6/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/HuggingChat.py` & `g4f-0.2.9.6/g4f/Provider/HuggingChat.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..requests.raise_for_status import raise_for_status
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
 from .helper import format_prompt, get_connector
 
 class HuggingChat(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://huggingface.co/chat"
     working = True
-    default_model = "meta-llama/Llama-2-70b-chat-hf"
+    default_model = "mistralai/Mixtral-8x7B-Instruct-v0.1"
     models = [
         "mistralai/Mixtral-8x7B-Instruct-v0.1",
         "google/gemma-7b-it",
         "meta-llama/Llama-2-70b-chat-hf",
         "NousResearch/Nous-Hermes-2-Mixtral-8x7B-DPO",
         "codellama/CodeLlama-34b-Instruct-hf",
         "mistralai/Mistral-7B-Instruct-v0.2",
```

### Comparing `g4f-0.2.9.5/g4f/Provider/HuggingFace.py` & `g4f-0.2.9.6/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/Koala.py` & `g4f-0.2.9.6/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/Liaobots.py` & `g4f-0.2.9.6/g4f/Provider/Liaobots.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
                     cls._cookie_jar = session.cookie_jar
 
             data = {
                 "conversationId": str(uuid.uuid4()),
                 "model": models[cls.get_model(model)],
                 "messages": messages,
                 "key": "",
-                "prompt": kwargs.get("system_message", "You are ChatGPT, a large language model trained by OpenAI. Follow the user's instructions carefully."),
+                "prompt": kwargs.get("system_message", "You are a helpful assistant."),
             }
             async with session.post(
                 "https://liaobots.work/api/chat",
                 json=data,
                 headers={"x-auth-code": cls._auth_code},
                 verify_ssl=False
             ) as response:
```

### Comparing `g4f-0.2.9.5/g4f/Provider/Llama2.py` & `g4f-0.2.9.6/g4f/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/Local.py` & `g4f-0.2.9.6/g4f/Provider/Local.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     has_requirements = False
 
 from ..typing import Messages, CreateResult
 from ..providers.base_provider import AbstractProvider, ProviderModelMixin
 from ..errors import MissingRequirementsError
 
 class Local(AbstractProvider, ProviderModelMixin):
+    label = "gpt4all"
     working = True
     supports_message_history = True
     supports_system_message = True
     supports_stream = True
 
     @classmethod
     def get_models(cls):
```

### Comparing `g4f-0.2.9.5/g4f/Provider/PerplexityLabs.py` & `g4f-0.2.9.6/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/Pi.py` & `g4f-0.2.9.6/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/ReplicateImage.py` & `g4f-0.2.9.6/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/Vercel.py` & `g4f-0.2.9.6/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.2.9.6/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/You.py` & `g4f-0.2.9.6/g4f/Provider/You.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/__init__.py` & `g4f-0.2.9.6/g4f/Provider/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,30 @@
 
 from .deprecated      import *
 from .not_working     import *
 from .selenium        import *
 from .needs_auth      import *
 from .unfinished      import *
 
+from .Aichatos         import Aichatos
 from .Aura             import Aura
 from .Bing             import Bing
 from .BingCreateImages import BingCreateImages
+from .Blackbox         import Blackbox
 from .ChatForAi        import ChatForAi
 from .Chatgpt4Online   import Chatgpt4Online
 from .ChatgptAi        import ChatgptAi
 from .ChatgptFree      import ChatgptFree
 from .ChatgptNext      import ChatgptNext
 from .ChatgptX         import ChatgptX
+from .Cnote            import Cnote
 from .DeepInfra        import DeepInfra
 from .DeepInfraImage   import DeepInfraImage
 from .DuckDuckGo       import DuckDuckGo
+from .Feedough         import Feedough
 from .FlowGpt          import FlowGpt
 from .FreeChatgpt      import FreeChatgpt
 from .FreeGpt          import FreeGpt
 from .GigaChat         import GigaChat
 from .GeminiPro        import GeminiPro
 from .GeminiProChat    import GeminiProChat
 from .GptTalkRu        import GptTalkRu
@@ -58,8 +62,8 @@
     provider.__name__ for provider in __providers__
 ]
 __map__: dict[str, ProviderType] = dict([
     (provider.__name__, provider) for provider in __providers__
 ])
 
 class ProviderUtils:
-    convert: dict[str, ProviderType] = __map__
+    convert: dict[str, ProviderType] = __map__
```

### Comparing `g4f-0.2.9.5/g4f/Provider/bing/conversation.py` & `g4f-0.2.9.6/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/bing/create_images.py` & `g4f-0.2.9.6/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/bing/upload_image.py` & `g4f-0.2.9.6/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/AiService.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Aibn.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Aichat.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Ails.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Berlin.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Equing.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Forefront.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/H2o.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Myshell.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Phind.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/V50.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Vercel.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/deprecated/__init__.py` & `g4f-0.2.9.6/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.2.9.6/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.2.9.6/g4f/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/needs_auth/Groq.py` & `g4f-0.2.9.6/g4f/Provider/needs_auth/Groq.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from .Openai import Openai
 from ...typing import AsyncResult, Messages
 
 class Groq(Openai):
+    lebel = "Groq"
     url = "https://console.groq.com/playground"
     working = True
     default_model = "mixtral-8x7b-32768"
     models = ["mixtral-8x7b-32768", "llama2-70b-4096", "gemma-7b-it"]
     model_aliases = {"mixtral-8x7b": "mixtral-8x7b-32768", "llama2-70b": "llama2-70b-4096"}
 
     @classmethod
```

### Comparing `g4f-0.2.9.5/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.2.9.6/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import requests
 
 from .Openai import Openai
 from ...typing import AsyncResult, Messages
 
 class OpenRouter(Openai):
+    label = "OpenRouter"
     url = "https://openrouter.ai"
     working = True
     default_model = "openrouter/auto"
 
     @classmethod
     def get_models(cls):
         if not cls.models:
```

### Comparing `g4f-0.2.9.5/g4f/Provider/needs_auth/Openai.py` & `g4f-0.2.9.6/g4f/Provider/needs_auth/Openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from ..helper import filter_none
 from ..base_provider import AsyncGeneratorProvider, ProviderModelMixin, FinishReason
 from ...typing import Union, Optional, AsyncResult, Messages
 from ...requests import StreamSession, raise_for_status
 from ...errors import MissingAuthError, ResponseError
 
 class Openai(AsyncGeneratorProvider, ProviderModelMixin):
+    label = "OpenAI API"
     url = "https://openai.com"
     working = True
     needs_auth = True
     supports_message_history = True
     supports_system_message = True
 
     @classmethod
```

### Comparing `g4f-0.2.9.5/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.2.9.6/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from ...providers.conversation import BaseConversation
 from ..openai.har_file import getArkoseAndAccessToken, NoValidHarFileError
 from ... import debug
 
 class OpenaiChat(AsyncGeneratorProvider, ProviderModelMixin):
     """A class for creating and managing conversations with OpenAI chat service"""
 
+    lebel = "OpenAI ChatGPT"
     url = "https://chat.openai.com"
     working = True
     supports_gpt_35_turbo = True
     supports_gpt_4 = True
     supports_message_history = True
     supports_system_message = True
     default_model = None
```

### Comparing `g4f-0.2.9.5/g4f/Provider/needs_auth/Poe.py` & `g4f-0.2.9.6/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.2.9.6/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/needs_auth/Theb.py` & `g4f-0.2.9.6/g4f/Provider/needs_auth/Theb.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     "code-llama-7b": "Code Llama 7B",
     "code-llama-13b": "Code Llama 13B",
     "code-llama-34b": "Code Llama 34B",
     "qwen-7b-chat": "Qwen 7B"
 }
 
 class Theb(AbstractProvider):
+    label = "TheB.AI"
     url = "https://beta.theb.ai"
     working = True
     supports_gpt_35_turbo = True
     supports_gpt_4 = True
     supports_stream = True
 
     @classmethod
```

### Comparing `g4f-0.2.9.5/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.2.9.6/g4f/Provider/needs_auth/ThebApi.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "code-llama-7b": "Code Llama 7B",
     "code-llama-13b": "Code Llama 13B",
     "code-llama-34b": "Code Llama 34B",
     "qwen-7b-chat": "Qwen 7B"
 }
 
 class ThebApi(Openai):
+    label = "TheB.AI API"
     url = "https://theb.ai"
     working = True
     needs_auth = True
     default_model = "gpt-3.5-turbo"
     models = list(models)
 
     @classmethod
```

### Comparing `g4f-0.2.9.5/g4f/Provider/not_working/AItianhu.py` & `g4f-0.2.9.6/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/not_working/Bestim.py` & `g4f-0.2.9.6/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/not_working/ChatBase.py` & `g4f-0.2.9.6/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.2.9.6/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.2.9.6/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.2.9.6/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.2.9.6/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/not_working/Gpt6.py` & `g4f-0.2.9.6/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/not_working/GptChatly.py` & `g4f-0.2.9.6/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/not_working/GptForLove.py` & `g4f-0.2.9.6/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/not_working/GptGo.py` & `g4f-0.2.9.6/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/not_working/GptGod.py` & `g4f-0.2.9.6/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.2.9.6/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.2.9.6/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.2.9.6/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/npm/package-lock.json` & `g4f-0.2.9.6/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/openai/crypt.py` & `g4f-0.2.9.6/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/openai/har_file.py` & `g4f-0.2.9.6/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.2.9.6/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/selenium/Bard.py` & `g4f-0.2.9.6/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/selenium/MyShell.py` & `g4f-0.2.9.6/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.2.9.6/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/selenium/Phind.py` & `g4f-0.2.9.6/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/selenium/TalkAi.py` & `g4f-0.2.9.6/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.2.9.6/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.2.9.6/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/unfinished/Komo.py` & `g4f-0.2.9.6/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.2.9.6/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/unfinished/Replicate.py` & `g4f-0.2.9.6/g4f/Provider/unfinished/Replicate.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/Provider/you/har_file.py` & `g4f-0.2.9.6/g4f/Provider/you/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/__init__.py` & `g4f-0.2.9.6/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/api/__init__.py` & `g4f-0.2.9.6/g4f/api/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/api/_logging.py` & `g4f-0.2.9.6/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/cli.py` & `g4f-0.2.9.6/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/client/async_client.py` & `g4f-0.2.9.6/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/client/client.py` & `g4f-0.2.9.6/g4f/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,15 @@
             model,
             self.provider if provider is None else provider,
             stream,
             ignored,
             ignore_working,
             ignore_stream,
         )
+        
         stop = [stop] if isinstance(stop, str) else stop
         response = provider.create_completion(
             model, messages,
             stream=stream,            
             **filter_none(
                 proxy=self.client.get_proxy() if proxy is None else proxy,
                 max_tokens=max_tokens,
```

### Comparing `g4f-0.2.9.5/g4f/client/helper.py` & `g4f-0.2.9.6/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/client/image_models.py` & `g4f-0.2.9.6/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/client/service.py` & `g4f-0.2.9.6/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/client/stubs.py` & `g4f-0.2.9.6/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/client/types.py` & `g4f-0.2.9.6/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/cookies.py` & `g4f-0.2.9.6/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/errors.py` & `g4f-0.2.9.6/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/__init__.py` & `g4f-0.2.9.6/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/client/index.html` & `g4f-0.2.9.6/g4f/gui/client/index.html`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/client/static/css/style.css` & `g4f-0.2.9.6/g4f/gui/client/static/css/style.css`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.2.9.6/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.2.9.6/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.2.9.6/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.2.9.6/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/client/static/img/gpt.png` & `g4f-0.2.9.6/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/client/static/img/user.png` & `g4f-0.2.9.6/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.2.9.6/g4f/gui/client/static/js/chat.v1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1033,17 +1033,18 @@
     models.forEach((model) => {
         let option = document.createElement("option");
         option.value = option.text = model;
         modelSelect.appendChild(option);
     });
 
     providers = await api("providers")
-    providers.forEach((provider) => {
+    Object.entries(providers).forEach(([provider, label]) => {
         let option = document.createElement("option");
-        option.value = option.text = provider;
+        option.value = provider;
+        option.text = label;
         providerSelect.appendChild(option);
     })
 
     await load_provider_models(appStorage.getItem("provider"));
     await load_settings_storage()
 
     const hide_systemPrompt = document.getElementById("hide-systemPrompt")
```

### Comparing `g4f-0.2.9.5/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.2.9.6/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.2.9.6/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/client/static/js/icons.js` & `g4f-0.2.9.6/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.2.9.6/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.2.9.6/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.2.9.6/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/server/android_gallery.py` & `g4f-0.2.9.6/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/server/api.py` & `g4f-0.2.9.6/g4f/gui/server/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,24 @@
             else:
                 return [];
 
     def get_providers(self) -> list[str]:
         """
         Return a list of all working providers.
         """
-        return [provider.__name__ for provider in __providers__ if provider.working]
+        return {
+            provider.__name__: (provider.label
+                if hasattr(provider, "label")
+                else provider.__name__) +
+                (" (WebDriver)"
+                if "webdriver" in provider.get_parameters()
+                else "")
+            for provider in __providers__
+            if provider.working
+        }
 
     def get_version(self):
         """
         Returns the current and latest version of the application.
 
         Returns:
             dict: A dictionary containing the current and latest version.
```

### Comparing `g4f-0.2.9.5/g4f/gui/server/backend.py` & `g4f-0.2.9.6/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/server/config.py` & `g4f-0.2.9.6/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/server/internet.py` & `g4f-0.2.9.6/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/server/js_api.py` & `g4f-0.2.9.6/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/server/website.py` & `g4f-0.2.9.6/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/gui/webview.py` & `g4f-0.2.9.6/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/image.py` & `g4f-0.2.9.6/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/local/__init__.py` & `g4f-0.2.9.6/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/locals/models.py` & `g4f-0.2.9.6/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/locals/provider.py` & `g4f-0.2.9.6/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/models.py` & `g4f-0.2.9.6/g4f/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__  import annotations
 
 from dataclasses import dataclass
 
 from .Provider import RetryProvider, ProviderType
-from .Provider   import (
+from .Provider import (
     Chatgpt4Online,
     PerplexityLabs,
     GeminiProChat,
     ChatgptNext,
     HuggingChat,
     HuggingFace,
     OpenaiChat,
@@ -15,14 +15,15 @@
     DeepInfra,
     GigaChat,
     Liaobots,
     FreeGpt,
     Llama2,
     Vercel,
     Gemini,
+    Koala,
     Bing,
     You,
     Pi,
 )
 
 @dataclass(unsafe_hash=True)
 class Model:
@@ -67,15 +68,20 @@
     ])
 )
 
 # GPT-3.5 / GPT-4
 gpt_35_turbo = Model(
     name          = 'gpt-3.5-turbo',
     base_provider = 'openai',
-    best_provider = OpenaiChat
+    best_provider = RetryProvider([
+        FreeGpt,
+        You,
+        ChatgptNext,
+        Koala,
+    ])
 )
 
 gpt_4 = Model(
     name          = 'gpt-4',
     base_provider = 'openai',
     best_provider = RetryProvider([
         Bing, Liaobots,
```

### Comparing `g4f-0.2.9.5/g4f/providers/base_provider.py` & `g4f-0.2.9.6/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/providers/create_images.py` & `g4f-0.2.9.6/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/providers/helper.py` & `g4f-0.2.9.6/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/providers/retry_provider.py` & `g4f-0.2.9.6/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/providers/types.py` & `g4f-0.2.9.6/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/requests/__init__.py` & `g4f-0.2.9.6/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/requests/aiohttp.py` & `g4f-0.2.9.6/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/requests/curl_cffi.py` & `g4f-0.2.9.6/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/requests/defaults.py` & `g4f-0.2.9.6/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/requests/raise_for_status.py` & `g4f-0.2.9.6/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/stubs.py` & `g4f-0.2.9.6/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/typing.py` & `g4f-0.2.9.6/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/version.py` & `g4f-0.2.9.6/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f/webdriver.py` & `g4f-0.2.9.6/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/g4f.egg-info/PKG-INFO` & `g4f-0.2.9.6/g4f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.2.9.5
+Version: 0.2.9.6
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.2.9.5 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.2.9.6 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.2.9.5/g4f.egg-info/SOURCES.txt` & `g4f-0.2.9.6/g4f.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,26 +15,30 @@
 g4f/webdriver.py
 g4f.egg-info/PKG-INFO
 g4f.egg-info/SOURCES.txt
 g4f.egg-info/dependency_links.txt
 g4f.egg-info/entry_points.txt
 g4f.egg-info/requires.txt
 g4f.egg-info/top_level.txt
+g4f/Provider/Aichatos.py
 g4f/Provider/Aura.py
 g4f/Provider/Bing.py
 g4f/Provider/BingCreateImages.py
+g4f/Provider/Blackbox.py
 g4f/Provider/ChatForAi.py
 g4f/Provider/Chatgpt4Online.py
 g4f/Provider/ChatgptAi.py
 g4f/Provider/ChatgptFree.py
 g4f/Provider/ChatgptNext.py
 g4f/Provider/ChatgptX.py
+g4f/Provider/Cnote.py
 g4f/Provider/DeepInfra.py
 g4f/Provider/DeepInfraImage.py
 g4f/Provider/DuckDuckGo.py
+g4f/Provider/Feedough.py
 g4f/Provider/FlowGpt.py
 g4f/Provider/FreeChatgpt.py
 g4f/Provider/FreeGpt.py
 g4f/Provider/GeminiPro.py
 g4f/Provider/GeminiProChat.py
 g4f/Provider/GigaChat.py
 g4f/Provider/GptTalkRu.py
```

### Comparing `g4f-0.2.9.5/g4f.egg-info/requires.txt` & `g4f-0.2.9.6/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.9.5/setup.py` & `g4f-0.2.9.6/setup.py`

 * *Files identical despite different names*

