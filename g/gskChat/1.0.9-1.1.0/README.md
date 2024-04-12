# Comparing `tmp/gskChat-1.0.9.tar.gz` & `tmp/gskChat-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gskChat-1.0.9.tar", last modified: Sun Apr  7 13:59:21 2024, max compression
+gzip compressed data, was "gskChat-1.1.0.tar", last modified: Fri Apr 12 14:00:37 2024, max compression
```

## Comparing `gskChat-1.0.9.tar` & `gskChat-1.1.0.tar`

### file list

```diff
@@ -1,393 +1,393 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.048525 gskChat-1.0.9/
--rw-rw-rw-   0        0        0      224 2024-03-24 15:15:13.000000 gskChat-1.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2874 2024-04-07 13:59:21.048525 gskChat-1.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.490163 gskChat-1.0.9/gskChat/
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.530545 gskChat-1.0.9/gskChat/Provider/
--rw-rw-rw-   0        0        0     1607 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Aura.py
--rw-rw-rw-   0        0        0    20640 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Bing.py
--rw-rw-rw-   0        0        0     2193 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/BingCreateImages.py
--rw-rw-rw-   0        0        0     2508 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/ChatForAi.py
--rw-rw-rw-   0        0        0     2653 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Chatgpt4Online.py
--rw-rw-rw-   0        0        0     3608 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/ChatgptAi.py
--rw-rw-rw-   0        0        0     2855 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/ChatgptFree.py
--rw-rw-rw-   0        0        0     2503 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/ChatgptNext.py
--rw-rw-rw-   0        0        0     4278 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/ChatgptX.py
--rw-rw-rw-   0        0        0     3526 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/DeepInfra.py
--rw-rw-rw-   0        0        0     3196 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/FlowGpt.py
--rw-rw-rw-   0        0        0     2530 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/FreeChatgpt.py
--rw-rw-rw-   0        0        0     1791 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/FreeGpt.py
--rw-rw-rw-   0        0        0     3937 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/GeminiPro.py
--rw-rw-rw-   0        0        0     2557 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/GeminiProChat.py
--rw-rw-rw-   0        0        0     3926 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/GigaChat.py
--rw-rw-rw-   0        0        0     2321 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/GptTalkRu.py
--rw-rw-rw-   0        0        0     3615 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/HuggingChat.py
--rw-rw-rw-   0        0        0     2940 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/HuggingFace.py
--rw-rw-rw-   0        0        0     2485 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Koala.py
--rw-rw-rw-   0        0        0     5099 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Liaobots.py
--rw-rw-rw-   0        0        0     3105 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Llama2.py
--rw-rw-rw-   0        0        0     3951 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/PerplexityLabs.py
--rw-rw-rw-   0        0        0     2355 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Pi.py
--rw-rw-rw-   0        0        0     4027 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Vercel.py
--rw-rw-rw-   0        0        0     7243 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/You.py
--rw-rw-rw-   0        0        0     2047 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.563444 gskChat-1.0.9/gskChat/Provider/__pycache__/
--rw-rw-rw-   0        0        0     2618 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Aura.cpython-312.pyc
--rw-rw-rw-   0        0        0    20847 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Bing.cpython-312.pyc
--rw-rw-rw-   0        0        0     3577 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/BingCreateImages.cpython-312.pyc
--rw-rw-rw-   0        0        0     3774 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/ChatForAi.cpython-312.pyc
--rw-rw-rw-   0        0        0     3889 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Chatgpt4Online.cpython-312.pyc
--rw-rw-rw-   0        0        0     4740 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptAi.cpython-312.pyc
--rw-rw-rw-   0        0        0     3951 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptFree.cpython-312.pyc
--rw-rw-rw-   0        0        0     3325 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptNext.cpython-312.pyc
--rw-rw-rw-   0        0        0     5386 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptX.cpython-312.pyc
--rw-rw-rw-   0        0        0     4547 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/DeepInfra.cpython-312.pyc
--rw-rw-rw-   0        0        0     3912 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/FlowGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     3552 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/FreeChatgpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     3089 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/FreeGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     5017 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/GeminiPro.cpython-312.pyc
--rw-rw-rw-   0        0        0     3887 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/GeminiProChat.cpython-312.pyc
--rw-rw-rw-   0        0        0     5557 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/GigaChat.cpython-312.pyc
--rw-rw-rw-   0        0        0     4066 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/GptTalkRu.cpython-312.pyc
--rw-rw-rw-   0        0        0     5345 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/HuggingChat.cpython-312.pyc
--rw-rw-rw-   0        0        0     4428 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/HuggingFace.cpython-312.pyc
--rw-rw-rw-   0        0        0     3521 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Koala.cpython-312.pyc
--rw-rw-rw-   0        0        0     5673 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Liaobots.cpython-312.pyc
--rw-rw-rw-   0        0        0     4082 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Llama2.cpython-312.pyc
--rw-rw-rw-   0        0        0     5769 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/PerplexityLabs.cpython-312.pyc
--rw-rw-rw-   0        0        0     3523 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Pi.cpython-312.pyc
--rw-rw-rw-   0        0        0     5112 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Vercel.cpython-312.pyc
--rw-rw-rw-   0        0        0     9701 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/You.cpython-312.pyc
--rw-rw-rw-   0        0        0     2677 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0      323 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/base_provider.cpython-312.pyc
--rw-rw-rw-   0        0        0      333 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/helper.cpython-312.pyc
--rw-rw-rw-   0        0        0       86 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/base_provider.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.566436 gskChat-1.0.9/gskChat/Provider/bing/
--rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/bing/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.570474 gskChat-1.0.9/gskChat/Provider/bing/__pycache__/
--rw-rw-rw-   0        0        0      203 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/bing/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     5088 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/bing/__pycache__/conversation.cpython-312.pyc
--rw-rw-rw-   0        0        0    10876 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/bing/__pycache__/create_images.cpython-312.pyc
--rw-rw-rw-   0        0        0     6076 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/bing/__pycache__/upload_image.cpython-312.pyc
--rw-rw-rw-   0        0        0     3468 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/bing/conversation.py
--rw-rw-rw-   0        0        0     7597 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/bing/create_images.py
--rw-rw-rw-   0        0        0     4746 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/bing/upload_image.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.602300 gskChat-1.0.9/gskChat/Provider/deprecated/
--rw-rw-rw-   0        0        0     1397 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Acytoo.py
--rw-rw-rw-   0        0        0     1669 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/AiAsk.py
--rw-rw-rw-   0        0        0     2196 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/AiChatOnline.py
--rw-rw-rw-   0        0        0     1148 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/AiService.py
--rw-rw-rw-   0        0        0     1396 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Aibn.py
--rw-rw-rw-   0        0        0     2517 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Aichat.py
--rw-rw-rw-   0        0        0     3358 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Ails.py
--rw-rw-rw-   0        0        0     2952 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Aivvm.py
--rw-rw-rw-   0        0        0     2807 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Berlin.py
--rw-rw-rw-   0        0        0     1934 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/ChatAnywhere.py
--rw-rw-rw-   0        0        0     1303 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/ChatgptDuo.py
--rw-rw-rw-   0        0        0     1873 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/CodeLinkAva.py
--rw-rw-rw-   0        0        0     1356 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Cromicle.py
--rw-rw-rw-   0        0        0     2498 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/DfeHub.py
--rw-rw-rw-   0        0        0     3398 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/EasyChat.py
--rw-rw-rw-   0        0        0     2755 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Equing.py
--rw-rw-rw-   0        0        0     4018 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/FakeGpt.py
--rw-rw-rw-   0        0        0     2929 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/FastGpt.py
--rw-rw-rw-   0        0        0     1282 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Forefront.py
--rw-rw-rw-   0        0        0     3552 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/GPTalk.py
--rw-rw-rw-   0        0        0     2658 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/GeekGpt.py
--rw-rw-rw-   0        0        0     2515 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/GetGpt.py
--rw-rw-rw-   0        0        0     2925 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/H2o.py
--rw-rw-rw-   0        0        0     2674 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Hashnode.py
--rw-rw-rw-   0        0        0     1700 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Lockchat.py
--rw-rw-rw-   0        0        0     5050 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Myshell.py
--rw-rw-rw-   0        0        0     2500 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/NoowAi.py
--rw-rw-rw-   0        0        0     2287 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Opchatgpts.py
--rw-rw-rw-   0        0        0     5353 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Phind.py
--rw-rw-rw-   0        0        0     2077 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/V50.py
--rw-rw-rw-   0        0        0    12167 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Vercel.py
--rw-rw-rw-   0        0        0     1964 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Vitalentum.py
--rw-rw-rw-   0        0        0     3415 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/VoiGpt.py
--rw-rw-rw-   0        0        0     2464 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Wewordle.py
--rw-rw-rw-   0        0        0     2020 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Wuguokai.py
--rw-rw-rw-   0        0        0     1976 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Ylokh.py
--rw-rw-rw-   0        0        0     1922 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Yqcloud.py
--rw-rw-rw-   0        0        0     1194 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.644472 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/
--rw-rw-rw-   0        0        0     2523 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Acytoo.cpython-312.pyc
--rw-rw-rw-   0        0        0     2705 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/AiAsk.cpython-312.pyc
--rw-rw-rw-   0        0        0     3107 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/AiChatOnline.cpython-312.pyc
--rw-rw-rw-   0        0        0     1976 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/AiService.cpython-312.pyc
--rw-rw-rw-   0        0        0     2702 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Aibn.cpython-312.pyc
--rw-rw-rw-   0        0        0     3337 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Aichat.cpython-312.pyc
--rw-rw-rw-   0        0        0     4946 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Ails.cpython-312.pyc
--rw-rw-rw-   0        0        0     3266 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Aivvm.cpython-312.pyc
--rw-rw-rw-   0        0        0     3969 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Berlin.cpython-312.pyc
--rw-rw-rw-   0        0        0     2911 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/ChatAnywhere.cpython-312.pyc
--rw-rw-rw-   0        0        0     2243 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/ChatgptDuo.cpython-312.pyc
--rw-rw-rw-   0        0        0     2831 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/CodeLinkAva.cpython-312.pyc
--rw-rw-rw-   0        0        0     2812 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Cromicle.cpython-312.pyc
--rw-rw-rw-   0        0        0     3098 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/DfeHub.cpython-312.pyc
--rw-rw-rw-   0        0        0     4043 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/EasyChat.cpython-312.pyc
--rw-rw-rw-   0        0        0     3381 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Equing.cpython-312.pyc
--rw-rw-rw-   0        0        0     5651 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/FakeGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     3377 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/FastGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     1953 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Forefront.cpython-312.pyc
--rw-rw-rw-   0        0        0     5271 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/GPTalk.cpython-312.pyc
--rw-rw-rw-   0        0        0     3197 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/GeekGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     2831 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/GetGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     4367 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/H2o.cpython-312.pyc
--rw-rw-rw-   0        0        0     4072 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Hashnode.cpython-312.pyc
--rw-rw-rw-   0        0        0     2331 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Lockchat.cpython-312.pyc
--rw-rw-rw-   0        0        0     7947 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Myshell.cpython-312.pyc
--rw-rw-rw-   0        0        0     3339 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/NoowAi.cpython-312.pyc
--rw-rw-rw-   0        0        0     3166 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Opchatgpts.cpython-312.pyc
--rw-rw-rw-   0        0        0     7793 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Phind.cpython-312.pyc
--rw-rw-rw-   0        0        0     2607 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/V50.cpython-312.pyc
--rw-rw-rw-   0        0        0     8348 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Vercel.cpython-312.pyc
--rw-rw-rw-   0        0        0     3117 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Vitalentum.cpython-312.pyc
--rw-rw-rw-   0        0        0     3644 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/VoiGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     3606 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Wewordle.cpython-312.pyc
--rw-rw-rw-   0        0        0     2702 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Wuguokai.cpython-312.pyc
--rw-rw-rw-   0        0        0     3036 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Ylokh.cpython-312.pyc
--rw-rw-rw-   0        0        0     3066 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Yqcloud.cpython-312.pyc
--rw-rw-rw-   0        0        0     1269 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.650520 gskChat-1.0.9/gskChat/Provider/gigachat_crt/
--rw-rw-rw-   0        0        0     2056 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-rw-rw-   0        0        0      111 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/helper.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.657503 gskChat-1.0.9/gskChat/Provider/needs_auth/
--rw-rw-rw-   0        0        0     8145 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/Gemini.py
--rw-rw-rw-   0        0        0     3309 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/OpenAssistant.py
--rw-rw-rw-   0        0        0    30868 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/OpenaiChat.py
--rw-rw-rw-   0        0        0     4289 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/Poe.py
--rw-rw-rw-   0        0        0     1897 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/Raycast.py
--rw-rw-rw-   0        0        0     5465 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/Theb.py
--rw-rw-rw-   0        0        0     2655 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/ThebApi.py
--rw-rw-rw-   0        0        0      245 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.666530 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/
--rw-rw-rw-   0        0        0    12063 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Gemini.cpython-312.pyc
--rw-rw-rw-   0        0        0     4902 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/OpenAssistant.cpython-312.pyc
--rw-rw-rw-   0        0        0    39633 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/OpenaiChat.cpython-312.pyc
--rw-rw-rw-   0        0        0     5188 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Poe.cpython-312.pyc
--rw-rw-rw-   0        0        0     2349 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Raycast.cpython-312.pyc
--rw-rw-rw-   0        0        0     6707 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Theb.cpython-312.pyc
--rw-rw-rw-   0        0        0     3305 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/ThebApi.cpython-312.pyc
--rw-rw-rw-   0        0        0      429 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.677914 gskChat-1.0.9/gskChat/Provider/not_working/
--rw-rw-rw-   0        0        0     3106 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/AItianhu.py
--rw-rw-rw-   0        0        0     1432 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/Bestim.py
--rw-rw-rw-   0        0        0     4546 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/ChatBase.py
--rw-rw-rw-   0        0        0     2863 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/ChatgptDemo.py
--rw-rw-rw-   0        0        0     2062 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/ChatgptDemoAi.py
--rw-rw-rw-   0        0        0     3056 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/ChatgptLogin.py
--rw-rw-rw-   0        0        0     2245 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/Chatxyz.py
--rw-rw-rw-   0        0        0     2243 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/Gpt6.py
--rw-rw-rw-   0        0        0     1033 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/GptChatly.py
--rw-rw-rw-   0        0        0     3529 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/GptForLove.py
--rw-rw-rw-   0        0        0     2480 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/GptGo.py
--rw-rw-rw-   0        0        0     2061 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/GptGod.py
--rw-rw-rw-   0        0        0     2093 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/OnlineGpt.py
--rw-rw-rw-   0        0        0      498 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.694478 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/
--rw-rw-rw-   0        0        0     3828 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/AItianhu.cpython-312.pyc
--rw-rw-rw-   0        0        0     2150 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/Bestim.cpython-312.pyc
--rw-rw-rw-   0        0        0     5577 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatBase.cpython-312.pyc
--rw-rw-rw-   0        0        0     4629 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatgptDemo.cpython-312.pyc
--rw-rw-rw-   0        0        0     3031 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatgptDemoAi.cpython-312.pyc
--rw-rw-rw-   0        0        0     4835 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatgptLogin.cpython-312.pyc
--rw-rw-rw-   0        0        0     3079 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/Chatxyz.cpython-312.pyc
--rw-rw-rw-   0        0        0     3251 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/Gpt6.cpython-312.pyc
--rw-rw-rw-   0        0        0     1724 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptChatly.cpython-312.pyc
--rw-rw-rw-   0        0        0     4841 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptForLove.cpython-312.pyc
--rw-rw-rw-   0        0        0     3729 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptGo.cpython-312.pyc
--rw-rw-rw-   0        0        0     3028 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptGod.cpython-312.pyc
--rw-rw-rw-   0        0        0     3024 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/OnlineGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0      632 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.703535 gskChat-1.0.9/gskChat/Provider/npm/
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.707525 gskChat-1.0.9/gskChat/Provider/npm/node_modules/
--rw-rw-rw-   0        0        0      346 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/npm/node_modules/.package-lock.json
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.741010 gskChat-1.0.9/gskChat/Provider/npm/node_modules/crypto-js/
--rw-rw-rw-   0        0        0     6449 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/npm/node_modules/crypto-js/README.md
--rw-rw-rw-   0        0        0   219092 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-rw-rw-   0        0        0      698 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/npm/package-lock.json
--rw-rw-rw-   0        0        0       54 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/npm/package.json
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.746996 gskChat-1.0.9/gskChat/Provider/selenium/
--rw-rw-rw-   0        0        0     3839 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/selenium/AItianhuSpace.py
--rw-rw-rw-   0        0        0     2859 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/selenium/Bard.py
--rw-rw-rw-   0        0        0     2250 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/selenium/MyShell.py
--rw-rw-rw-   0        0        0     3681 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/selenium/PerplexityAi.py
--rw-rw-rw-   0        0        0     3655 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/selenium/Phind.py
--rw-rw-rw-   0        0        0     2678 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/selenium/TalkAi.py
--rw-rw-rw-   0        0        0      183 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.754918 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/
--rw-rw-rw-   0        0        0     4847 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/AItianhuSpace.cpython-312.pyc
--rw-rw-rw-   0        0        0     3759 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/Bard.cpython-312.pyc
--rw-rw-rw-   0        0        0     2914 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/MyShell.cpython-312.pyc
--rw-rw-rw-   0        0        0     4525 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/PerplexityAi.cpython-312.pyc
--rw-rw-rw-   0        0        0     4649 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/Phind.cpython-312.pyc
--rw-rw-rw-   0        0        0     3407 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/TalkAi.cpython-312.pyc
--rw-rw-rw-   0        0        0      400 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.757910 gskChat-1.0.9/gskChat/Provider/unfinished/
--rw-rw-rw-   0        0        0     2260 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/unfinished/AiChatting.py
--rw-rw-rw-   0        0        0     2441 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/unfinished/ChatAiGpt.py
--rw-rw-rw-   0        0        0     1450 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/unfinished/Komo.py
--rw-rw-rw-   0        0        0     3298 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/unfinished/MikuChat.py
--rw-rw-rw-   0        0        0      142 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/unfinished/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.764894 gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/
--rw-rw-rw-   0        0        0     3349 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/AiChatting.cpython-312.pyc
--rw-rw-rw-   0        0        0     3656 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/ChatAiGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     2378 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/Komo.cpython-312.pyc
--rw-rw-rw-   0        0        0     5497 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/MikuChat.cpython-312.pyc
--rw-rw-rw-   0        0        0      338 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0    10959 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.779386 gskChat-1.0.9/gskChat/__pycache__/
--rw-rw-rw-   0        0        0    12330 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     2461 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/cli.cpython-312.pyc
--rw-rw-rw-   0        0        0    11637 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/client.cpython-312.pyc
--rw-rw-rw-   0        0        0     4537 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/cookies.cpython-312.pyc
--rw-rw-rw-   0        0        0      478 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/debug.cpython-312.pyc
--rw-rw-rw-   0        0        0     2492 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/errors.cpython-312.pyc
--rw-rw-rw-   0        0        0    11732 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/image.cpython-312.pyc
--rw-rw-rw-   0        0        0     6305 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/models.cpython-312.pyc
--rw-rw-rw-   0        0        0     5533 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/stubs.cpython-312.pyc
--rw-rw-rw-   0        0        0     1152 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/typing.cpython-312.pyc
--rw-rw-rw-   0        0        0     5221 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/version.cpython-312.pyc
--rw-rw-rw-   0        0        0    12909 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/webdriver.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.782488 gskChat-1.0.9/gskChat/api/
--rw-rw-rw-   0        0        0     5168 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.787474 gskChat-1.0.9/gskChat/api/__pycache__/
--rw-rw-rw-   0        0        0     9054 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/api/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     2317 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/api/__pycache__/_logging.cpython-312.pyc
--rw-rw-rw-   0        0        0      195 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/api/__pycache__/_tokenizer.cpython-312.pyc
--rw-rw-rw-   0        0        0      639 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/api/__pycache__/run.cpython-312.pyc
--rw-rw-rw-   0        0        0      893 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/api/_logging.py
--rw-rw-rw-   0        0        0      286 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/api/_tokenizer.py
--rw-rw-rw-   0        0        0      201 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/api/run.py
--rw-rw-rw-   0        0        0     1318 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/cli.py
--rw-rw-rw-   0        0        0     8568 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/client.py
--rw-rw-rw-   0        0        0     3406 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/cookies.py
--rw-rw-rw-   0        0        0      169 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/debug.py
--rw-rw-rw-   0        0        0      712 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/errors.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.789470 gskChat-1.0.9/gskChat/gui/
--rw-rw-rw-   0        0        0     1567 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.792540 gskChat-1.0.9/gskChat/gui/__pycache__/
--rw-rw-rw-   0        0        0     2290 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     1249 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/__pycache__/run.cpython-312.pyc
--rw-rw-rw-   0        0        0     2080 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/__pycache__/webview.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.860189 gskChat-1.0.9/gskChat/gui/client/
--rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.861547 gskChat-1.0.9/gskChat/gui/client/__pycache__/
--rw-rw-rw-   0        0        0      200 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/client/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0    25804 2024-04-07 13:04:16.000000 gskChat-1.0.9/gskChat/gui/client/index.html
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.861547 gskChat-1.0.9/gskChat/gui/client/static/
--rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.862546 gskChat-1.0.9/gskChat/gui/client/static/__pycache__/
--rw-rw-rw-   0        0        0      207 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/client/static/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.864542 gskChat-1.0.9/gskChat/gui/client/static/css/
--rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/css/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.865539 gskChat-1.0.9/gskChat/gui/client/static/css/__pycache__/
--rw-rw-rw-   0        0        0      211 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/client/static/css/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0    26730 2024-04-07 13:57:33.000000 gskChat-1.0.9/gskChat/gui/client/static/css/style.css
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.957429 gskChat-1.0.9/gskChat/gui/client/static/img/
--rw-rw-rw-   0        0        0     4286 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/1.png
--rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.958425 gskChat-1.0.9/gskChat/gui/client/static/img/__pycache__/
--rw-rw-rw-   0        0        0      211 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/client/static/img/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     8908 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/android-chrome-192x192.png
--rw-rw-rw-   0        0        0    17626 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/android-chrome-512x512.png
--rw-rw-rw-   0        0        0     7984 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/apple-touch-icon.png
--rw-rw-rw-   0        0        0     2258 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/content.png
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.959422 gskChat-1.0.9/gskChat/gui/client/static/img/cursor/
--rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/cursor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.959422 gskChat-1.0.9/gskChat/gui/client/static/img/cursor/__pycache__/
--rw-rw-rw-   0        0        0      218 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/client/static/img/cursor/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0      721 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/favicon-16x16.png
--rw-rw-rw-   0        0        0      499 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/favicon-16x162.png
--rw-rw-rw-   0        0        0     4286 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/favicon-32x32.png
--rw-rw-rw-   0        0        0   501120 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/gpt.png
--rw-rw-rw-   0        0        0     2885 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/gpt1.png
--rw-rw-rw-   0        0        0     2551 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/graphic-designer.png
--rw-rw-rw-   0        0        0  2853419 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/loading-1.gif
--rw-rw-rw-   0        0        0   251420 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/loading-101.gif
--rw-rw-rw-   0        0        0   162448 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/programmer.jpg
--rw-rw-rw-   0        0        0     1783 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/programmer.png
--rw-rw-rw-   0        0        0      447 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/site.webmanifest
--rw-rw-rw-   0        0        0   200333 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/teacher.jpg
--rw-rw-rw-   0        0        0    23088 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/telegram.png
--rw-rw-rw-   0        0        0   175178 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/user.png
--rw-rw-rw-   0        0        0   117644 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/write.jpg
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.005483 gskChat-1.0.9/gskChat/gui/client/static/js/
--rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/js/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.006481 gskChat-1.0.9/gskChat/gui/client/static/js/__pycache__/
--rw-rw-rw-   0        0        0      210 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/client/static/js/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0    33901 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/js/chat.v1.js
--rw-rw-rw-   0        0        0   118841 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/js/highlight.min.js
--rw-rw-rw-   0        0        0     1083 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/js/highlightjs-copy.min.js
--rw-rw-rw-   0        0        0    10865 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/js/icons.js
--rw-rw-rw-   0        0        0      410 2024-04-07 13:22:40.000000 gskChat-1.0.9/gskChat/gui/client/test.html
--rw-rw-rw-   0        0        0      615 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/run.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.011516 gskChat-1.0.9/gskChat/gui/server/
--rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.020713 gskChat-1.0.9/gskChat/gui/server/__pycache__/
--rw-rw-rw-   0        0        0      200 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     3366 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/android_gallery.cpython-312.pyc
--rw-rw-rw-   0        0        0    12282 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/api.cpython-312.pyc
--rw-rw-rw-   0        0        0      577 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/app.cpython-312.pyc
--rw-rw-rw-   0        0        0     4568 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/backend.cpython-312.pyc
--rw-rw-rw-   0        0        0    14765 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/config.cpython-312.pyc
--rw-rw-rw-   0        0        0     7883 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/internet.cpython-312.pyc
--rw-rw-rw-   0        0        0     1513 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/website.cpython-312.pyc
--rw-rw-rw-   0        0        0     2470 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/android_gallery.py
--rw-rw-rw-   0        0        0     9422 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/api.py
--rw-rw-rw-   0        0        0      271 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/app.py
--rw-rw-rw-   0        0        0     3681 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/backend.py
--rw-rw-rw-   0        0        0    15354 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/config.py
--rw-rw-rw-   0        0        0     4918 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/internet.py
--rw-rw-rw-   0        0        0      839 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/website.py
--rw-rw-rw-   0        0        0     1200 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/webview.py
--rw-rw-rw-   0        0        0     8399 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/image.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.021710 gskChat-1.0.9/gskChat/local/
--rw-rw-rw-   0        0        0     1405 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/local/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.024702 gskChat-1.0.9/gskChat/local/__pycache__/
--rw-rw-rw-   0        0        0     2679 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/local/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     3047 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/local/__pycache__/_engine.cpython-312.pyc
--rw-rw-rw-   0        0        0     2179 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/local/__pycache__/_models.cpython-312.pyc
--rw-rw-rw-   0        0        0     1832 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/local/_engine.py
--rw-rw-rw-   0        0        0     2959 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/local/_models.py
--rw-rw-rw-   0        0        0     7633 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/models.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.029490 gskChat-1.0.9/gskChat/providers/
--rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/providers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.035504 gskChat-1.0.9/gskChat/providers/__pycache__/
--rw-rw-rw-   0        0        0      199 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/providers/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0    13248 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/providers/__pycache__/base_provider.cpython-312.pyc
--rw-rw-rw-   0        0        0     7555 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/providers/__pycache__/create_images.cpython-312.pyc
--rw-rw-rw-   0        0        0     2745 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/providers/__pycache__/helper.cpython-312.pyc
--rw-rw-rw-   0        0        0     9044 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/providers/__pycache__/retry_provider.cpython-312.pyc
--rw-rw-rw-   0        0        0     4203 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/providers/__pycache__/types.cpython-312.pyc
--rw-rw-rw-   0        0        0     9260 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/providers/base_provider.py
--rw-rw-rw-   0        0        0     6594 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/providers/create_images.py
--rw-rw-rw-   0        0        0     1528 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/providers/helper.py
--rw-rw-rw-   0        0        0     6869 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/providers/retry_provider.py
--rw-rw-rw-   0        0        0     3083 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/providers/types.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.038497 gskChat-1.0.9/gskChat/requests/
--rw-rw-rw-   0        0        0     3959 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/requests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.044537 gskChat-1.0.9/gskChat/requests/__pycache__/
--rw-rw-rw-   0        0        0     4981 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/requests/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     3226 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/requests/__pycache__/aiohttp.cpython-312.pyc
--rw-rw-rw-   0        0        0     5284 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/requests/__pycache__/curl_cffi.cpython-312.pyc
--rw-rw-rw-   0        0        0     1415 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/requests/__pycache__/defaults.cpython-312.pyc
--rw-rw-rw-   0        0        0     2638 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/requests/__pycache__/raise_for_status.cpython-312.pyc
--rw-rw-rw-   0        0        0     1775 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/requests/aiohttp.py
--rw-rw-rw-   0        0        0     3016 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/requests/curl_cffi.py
--rw-rw-rw-   0        0        0     1091 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/requests/defaults.py
--rw-rw-rw-   0        0        0     1625 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/requests/raise_for_status.py
--rw-rw-rw-   0        0        0     2938 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/stubs.py
--rw-rw-rw-   0        0        0      875 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/typing.py
--rw-rw-rw-   0        0        0     3821 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/version.py
--rw-rw-rw-   0        0        0     9953 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.045534 gskChat-1.0.9/gskChat.egg-info/
--rw-rw-rw-   0        0        0     2874 2024-04-07 13:59:20.000000 gskChat-1.0.9/gskChat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    15760 2024-04-07 13:59:20.000000 gskChat-1.0.9/gskChat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 13:59:20.000000 gskChat-1.0.9/gskChat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-07 13:59:20.000000 gskChat-1.0.9/gskChat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      621 2024-04-07 13:59:20.000000 gskChat-1.0.9/gskChat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-07 13:59:20.000000 gskChat-1.0.9/gskChat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 13:59:21.050769 gskChat-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     3200 2024-04-07 13:59:12.000000 gskChat-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.237611 gskChat-1.1.0/
+-rw-rw-rw-   0        0        0      224 2024-03-24 15:15:13.000000 gskChat-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2874 2024-04-12 14:00:37.236614 gskChat-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.708273 gskChat-1.1.0/gskChat/
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.748370 gskChat-1.1.0/gskChat/Provider/
+-rw-rw-rw-   0        0        0     1607 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/Aura.py
+-rw-rw-rw-   0        0        0    20640 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/Bing.py
+-rw-rw-rw-   0        0        0     2193 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/BingCreateImages.py
+-rw-rw-rw-   0        0        0     2508 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/ChatForAi.py
+-rw-rw-rw-   0        0        0     2653 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/Chatgpt4Online.py
+-rw-rw-rw-   0        0        0     3608 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/ChatgptAi.py
+-rw-rw-rw-   0        0        0     2855 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/ChatgptFree.py
+-rw-rw-rw-   0        0        0     2503 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/ChatgptNext.py
+-rw-rw-rw-   0        0        0     4278 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/ChatgptX.py
+-rw-rw-rw-   0        0        0     3526 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/DeepInfra.py
+-rw-rw-rw-   0        0        0     3196 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/FlowGpt.py
+-rw-rw-rw-   0        0        0     2530 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/FreeChatgpt.py
+-rw-rw-rw-   0        0        0     1791 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/FreeGpt.py
+-rw-rw-rw-   0        0        0     3937 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/GeminiPro.py
+-rw-rw-rw-   0        0        0     2557 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/GeminiProChat.py
+-rw-rw-rw-   0        0        0     3926 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/GigaChat.py
+-rw-rw-rw-   0        0        0     2321 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/GptTalkRu.py
+-rw-rw-rw-   0        0        0     3615 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/HuggingChat.py
+-rw-rw-rw-   0        0        0     2940 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/HuggingFace.py
+-rw-rw-rw-   0        0        0     2485 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/Koala.py
+-rw-rw-rw-   0        0        0     5099 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/Liaobots.py
+-rw-rw-rw-   0        0        0     3105 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/Llama2.py
+-rw-rw-rw-   0        0        0     3951 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/PerplexityLabs.py
+-rw-rw-rw-   0        0        0     2355 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/Pi.py
+-rw-rw-rw-   0        0        0     4027 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/Vercel.py
+-rw-rw-rw-   0        0        0     7243 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/You.py
+-rw-rw-rw-   0        0        0     2047 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.777392 gskChat-1.1.0/gskChat/Provider/__pycache__/
+-rw-rw-rw-   0        0        0     2618 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/Aura.cpython-312.pyc
+-rw-rw-rw-   0        0        0    20847 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/Bing.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3577 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/BingCreateImages.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3774 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/ChatForAi.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3889 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/Chatgpt4Online.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4740 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/ChatgptAi.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3951 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/ChatgptFree.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3325 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/ChatgptNext.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5386 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/ChatgptX.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4547 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/DeepInfra.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3912 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/FlowGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3552 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/FreeChatgpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3089 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/FreeGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5017 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/GeminiPro.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3887 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/GeminiProChat.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5557 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/GigaChat.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4066 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/GptTalkRu.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5345 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/HuggingChat.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4428 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/HuggingFace.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3521 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/Koala.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5673 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/Liaobots.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4082 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/Llama2.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5769 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/PerplexityLabs.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3523 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/Pi.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5112 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/Vercel.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9701 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/You.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2677 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0      323 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/base_provider.cpython-312.pyc
+-rw-rw-rw-   0        0        0      333 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/__pycache__/helper.cpython-312.pyc
+-rw-rw-rw-   0        0        0       86 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/base_provider.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.780387 gskChat-1.1.0/gskChat/Provider/bing/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/bing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.784375 gskChat-1.1.0/gskChat/Provider/bing/__pycache__/
+-rw-rw-rw-   0        0        0      203 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/bing/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5088 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/bing/__pycache__/conversation.cpython-312.pyc
+-rw-rw-rw-   0        0        0    10876 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/bing/__pycache__/create_images.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6076 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/bing/__pycache__/upload_image.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3468 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/bing/conversation.py
+-rw-rw-rw-   0        0        0     7597 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/bing/create_images.py
+-rw-rw-rw-   0        0        0     4746 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/bing/upload_image.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.811582 gskChat-1.1.0/gskChat/Provider/deprecated/
+-rw-rw-rw-   0        0        0     1397 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Acytoo.py
+-rw-rw-rw-   0        0        0     1669 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/AiAsk.py
+-rw-rw-rw-   0        0        0     2196 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/AiChatOnline.py
+-rw-rw-rw-   0        0        0     1148 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/AiService.py
+-rw-rw-rw-   0        0        0     1396 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Aibn.py
+-rw-rw-rw-   0        0        0     2517 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Aichat.py
+-rw-rw-rw-   0        0        0     3358 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Ails.py
+-rw-rw-rw-   0        0        0     2952 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Aivvm.py
+-rw-rw-rw-   0        0        0     2807 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Berlin.py
+-rw-rw-rw-   0        0        0     1934 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/ChatAnywhere.py
+-rw-rw-rw-   0        0        0     1303 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/ChatgptDuo.py
+-rw-rw-rw-   0        0        0     1873 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/CodeLinkAva.py
+-rw-rw-rw-   0        0        0     1356 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Cromicle.py
+-rw-rw-rw-   0        0        0     2498 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/DfeHub.py
+-rw-rw-rw-   0        0        0     3398 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/EasyChat.py
+-rw-rw-rw-   0        0        0     2755 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Equing.py
+-rw-rw-rw-   0        0        0     4018 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/FakeGpt.py
+-rw-rw-rw-   0        0        0     2929 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/FastGpt.py
+-rw-rw-rw-   0        0        0     1282 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Forefront.py
+-rw-rw-rw-   0        0        0     3552 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/GPTalk.py
+-rw-rw-rw-   0        0        0     2658 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/GeekGpt.py
+-rw-rw-rw-   0        0        0     2515 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/GetGpt.py
+-rw-rw-rw-   0        0        0     2925 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/H2o.py
+-rw-rw-rw-   0        0        0     2674 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Hashnode.py
+-rw-rw-rw-   0        0        0     1700 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Lockchat.py
+-rw-rw-rw-   0        0        0     5050 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Myshell.py
+-rw-rw-rw-   0        0        0     2500 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/NoowAi.py
+-rw-rw-rw-   0        0        0     2287 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Opchatgpts.py
+-rw-rw-rw-   0        0        0     5353 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Phind.py
+-rw-rw-rw-   0        0        0     2077 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/V50.py
+-rw-rw-rw-   0        0        0    12167 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Vercel.py
+-rw-rw-rw-   0        0        0     1964 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Vitalentum.py
+-rw-rw-rw-   0        0        0     3415 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/VoiGpt.py
+-rw-rw-rw-   0        0        0     2464 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Wewordle.py
+-rw-rw-rw-   0        0        0     2020 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Wuguokai.py
+-rw-rw-rw-   0        0        0     1976 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Ylokh.py
+-rw-rw-rw-   0        0        0     1922 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/Yqcloud.py
+-rw-rw-rw-   0        0        0     1194 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.848395 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/
+-rw-rw-rw-   0        0        0     2523 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Acytoo.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2705 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/AiAsk.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3107 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/AiChatOnline.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1976 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/AiService.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2702 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Aibn.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3337 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Aichat.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4946 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Ails.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3266 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Aivvm.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3969 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Berlin.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2911 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/ChatAnywhere.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2243 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/ChatgptDuo.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2831 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/CodeLinkAva.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2812 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Cromicle.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3098 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/DfeHub.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4043 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/EasyChat.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3381 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Equing.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5651 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/FakeGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3377 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/FastGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1953 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Forefront.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5271 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/GPTalk.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3197 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/GeekGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2831 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/GetGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4367 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/H2o.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4072 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Hashnode.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2331 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Lockchat.cpython-312.pyc
+-rw-rw-rw-   0        0        0     7947 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Myshell.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3339 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/NoowAi.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3166 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Opchatgpts.cpython-312.pyc
+-rw-rw-rw-   0        0        0     7793 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Phind.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2607 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/V50.cpython-312.pyc
+-rw-rw-rw-   0        0        0     8348 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Vercel.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3117 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Vitalentum.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3644 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/VoiGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3606 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Wewordle.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2702 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Wuguokai.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3036 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Ylokh.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3066 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Yqcloud.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1269 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.852385 gskChat-1.1.0/gskChat/Provider/gigachat_crt/
+-rw-rw-rw-   0        0        0     2056 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-rw-rw-   0        0        0      111 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/helper.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.858848 gskChat-1.1.0/gskChat/Provider/needs_auth/
+-rw-rw-rw-   0        0        0     8145 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/Gemini.py
+-rw-rw-rw-   0        0        0     3309 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/OpenAssistant.py
+-rw-rw-rw-   0        0        0    30868 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/OpenaiChat.py
+-rw-rw-rw-   0        0        0     4289 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/Poe.py
+-rw-rw-rw-   0        0        0     1897 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/Raycast.py
+-rw-rw-rw-   0        0        0     5465 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/Theb.py
+-rw-rw-rw-   0        0        0     2655 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/ThebApi.py
+-rw-rw-rw-   0        0        0      245 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.865362 gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/
+-rw-rw-rw-   0        0        0    12063 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/Gemini.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4902 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/OpenAssistant.cpython-312.pyc
+-rw-rw-rw-   0        0        0    39633 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/OpenaiChat.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5188 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/Poe.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2349 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/Raycast.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6707 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/Theb.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3305 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/ThebApi.cpython-312.pyc
+-rw-rw-rw-   0        0        0      429 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.875856 gskChat-1.1.0/gskChat/Provider/not_working/
+-rw-rw-rw-   0        0        0     3106 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/not_working/AItianhu.py
+-rw-rw-rw-   0        0        0     1432 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/not_working/Bestim.py
+-rw-rw-rw-   0        0        0     4546 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/not_working/ChatBase.py
+-rw-rw-rw-   0        0        0     2863 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/not_working/ChatgptDemo.py
+-rw-rw-rw-   0        0        0     2062 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/not_working/ChatgptDemoAi.py
+-rw-rw-rw-   0        0        0     3056 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/not_working/ChatgptLogin.py
+-rw-rw-rw-   0        0        0     2245 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/not_working/Chatxyz.py
+-rw-rw-rw-   0        0        0     2243 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/not_working/Gpt6.py
+-rw-rw-rw-   0        0        0     1033 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/not_working/GptChatly.py
+-rw-rw-rw-   0        0        0     3529 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/not_working/GptForLove.py
+-rw-rw-rw-   0        0        0     2480 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/not_working/GptGo.py
+-rw-rw-rw-   0        0        0     2061 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/not_working/GptGod.py
+-rw-rw-rw-   0        0        0     2093 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/not_working/OnlineGpt.py
+-rw-rw-rw-   0        0        0      498 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/not_working/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.888766 gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/
+-rw-rw-rw-   0        0        0     3828 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/AItianhu.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2150 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/Bestim.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5577 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/ChatBase.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4629 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/ChatgptDemo.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3031 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/ChatgptDemoAi.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4835 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/ChatgptLogin.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3079 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/Chatxyz.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3251 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/Gpt6.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1724 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/GptChatly.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4841 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/GptForLove.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3729 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/GptGo.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3028 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/GptGod.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3024 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/OnlineGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0      632 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.896407 gskChat-1.1.0/gskChat/Provider/npm/
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.901394 gskChat-1.1.0/gskChat/Provider/npm/node_modules/
+-rw-rw-rw-   0        0        0      346 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/npm/node_modules/.package-lock.json
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.932460 gskChat-1.1.0/gskChat/Provider/npm/node_modules/crypto-js/
+-rw-rw-rw-   0        0        0     6449 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/npm/node_modules/crypto-js/README.md
+-rw-rw-rw-   0        0        0   219092 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-rw-rw-   0        0        0      698 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/npm/package-lock.json
+-rw-rw-rw-   0        0        0       54 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/npm/package.json
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.938135 gskChat-1.1.0/gskChat/Provider/selenium/
+-rw-rw-rw-   0        0        0     3839 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/selenium/AItianhuSpace.py
+-rw-rw-rw-   0        0        0     2859 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/selenium/Bard.py
+-rw-rw-rw-   0        0        0     2250 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/selenium/MyShell.py
+-rw-rw-rw-   0        0        0     3681 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/selenium/PerplexityAi.py
+-rw-rw-rw-   0        0        0     3655 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/selenium/Phind.py
+-rw-rw-rw-   0        0        0     2678 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/selenium/TalkAi.py
+-rw-rw-rw-   0        0        0      183 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.945205 gskChat-1.1.0/gskChat/Provider/selenium/__pycache__/
+-rw-rw-rw-   0        0        0     4847 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/selenium/__pycache__/AItianhuSpace.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3759 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/selenium/__pycache__/Bard.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2914 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/selenium/__pycache__/MyShell.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4525 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/selenium/__pycache__/PerplexityAi.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4649 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/selenium/__pycache__/Phind.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3407 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/selenium/__pycache__/TalkAi.cpython-312.pyc
+-rw-rw-rw-   0        0        0      400 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/selenium/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.948511 gskChat-1.1.0/gskChat/Provider/unfinished/
+-rw-rw-rw-   0        0        0     2260 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/unfinished/AiChatting.py
+-rw-rw-rw-   0        0        0     2441 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/unfinished/ChatAiGpt.py
+-rw-rw-rw-   0        0        0     1450 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/unfinished/Komo.py
+-rw-rw-rw-   0        0        0     3298 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/unfinished/MikuChat.py
+-rw-rw-rw-   0        0        0      142 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/Provider/unfinished/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.954495 gskChat-1.1.0/gskChat/Provider/unfinished/__pycache__/
+-rw-rw-rw-   0        0        0     3349 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/unfinished/__pycache__/AiChatting.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3656 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/unfinished/__pycache__/ChatAiGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2378 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/unfinished/__pycache__/Komo.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5497 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/unfinished/__pycache__/MikuChat.cpython-312.pyc
+-rw-rw-rw-   0        0        0      338 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/Provider/unfinished/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0    10959 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.967540 gskChat-1.1.0/gskChat/__pycache__/
+-rw-rw-rw-   0        0        0    12330 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2461 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/__pycache__/cli.cpython-312.pyc
+-rw-rw-rw-   0        0        0    11637 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/__pycache__/client.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4537 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/__pycache__/cookies.cpython-312.pyc
+-rw-rw-rw-   0        0        0      478 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/__pycache__/debug.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2492 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/__pycache__/errors.cpython-312.pyc
+-rw-rw-rw-   0        0        0    11732 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/__pycache__/image.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6305 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/__pycache__/models.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5533 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/__pycache__/stubs.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1152 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/__pycache__/typing.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5221 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/__pycache__/version.cpython-312.pyc
+-rw-rw-rw-   0        0        0    12909 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/__pycache__/webdriver.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.973055 gskChat-1.1.0/gskChat/api/
+-rw-rw-rw-   0        0        0     5168 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.978570 gskChat-1.1.0/gskChat/api/__pycache__/
+-rw-rw-rw-   0        0        0     9054 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/api/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2317 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/api/__pycache__/_logging.cpython-312.pyc
+-rw-rw-rw-   0        0        0      195 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/api/__pycache__/_tokenizer.cpython-312.pyc
+-rw-rw-rw-   0        0        0      639 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/api/__pycache__/run.cpython-312.pyc
+-rw-rw-rw-   0        0        0      893 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/api/_logging.py
+-rw-rw-rw-   0        0        0      286 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/api/_tokenizer.py
+-rw-rw-rw-   0        0        0      201 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/api/run.py
+-rw-rw-rw-   0        0        0     1318 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/cli.py
+-rw-rw-rw-   0        0        0     8568 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/client.py
+-rw-rw-rw-   0        0        0     3406 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/cookies.py
+-rw-rw-rw-   0        0        0      169 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/debug.py
+-rw-rw-rw-   0        0        0      712 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.981564 gskChat-1.1.0/gskChat/gui/
+-rw-rw-rw-   0        0        0     1567 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:36.984067 gskChat-1.1.0/gskChat/gui/__pycache__/
+-rw-rw-rw-   0        0        0     2290 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1249 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/__pycache__/run.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2080 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/__pycache__/webview.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.053188 gskChat-1.1.0/gskChat/gui/client/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.054186 gskChat-1.1.0/gskChat/gui/client/__pycache__/
+-rw-rw-rw-   0        0        0      200 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/client/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0    26769 2024-04-12 13:35:55.000000 gskChat-1.1.0/gskChat/gui/client/index.html
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.055233 gskChat-1.1.0/gskChat/gui/client/static/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.055233 gskChat-1.1.0/gskChat/gui/client/static/__pycache__/
+-rw-rw-rw-   0        0        0      207 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/client/static/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.057305 gskChat-1.1.0/gskChat/gui/client/static/css/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/css/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.058303 gskChat-1.1.0/gskChat/gui/client/static/css/__pycache__/
+-rw-rw-rw-   0        0        0      211 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/client/static/css/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0    27455 2024-04-12 13:58:16.000000 gskChat-1.1.0/gskChat/gui/client/static/css/style.css
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.138381 gskChat-1.1.0/gskChat/gui/client/static/img/
+-rw-rw-rw-   0        0        0     4286 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/1.png
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.139369 gskChat-1.1.0/gskChat/gui/client/static/img/__pycache__/
+-rw-rw-rw-   0        0        0      211 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/client/static/img/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     8908 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/android-chrome-192x192.png
+-rw-rw-rw-   0        0        0    17626 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/android-chrome-512x512.png
+-rw-rw-rw-   0        0        0     7984 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/apple-touch-icon.png
+-rw-rw-rw-   0        0        0     2258 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/content.png
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.140365 gskChat-1.1.0/gskChat/gui/client/static/img/cursor/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/cursor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.141363 gskChat-1.1.0/gskChat/gui/client/static/img/cursor/__pycache__/
+-rw-rw-rw-   0        0        0      218 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/client/static/img/cursor/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0      721 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/favicon-16x16.png
+-rw-rw-rw-   0        0        0      499 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/favicon-16x162.png
+-rw-rw-rw-   0        0        0     4286 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/favicon-32x32.png
+-rw-rw-rw-   0        0        0   501120 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/gpt.png
+-rw-rw-rw-   0        0        0     2885 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/gpt1.png
+-rw-rw-rw-   0        0        0     2551 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/graphic-designer.png
+-rw-rw-rw-   0        0        0  2853419 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/loading-1.gif
+-rw-rw-rw-   0        0        0   251420 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/loading-101.gif
+-rw-rw-rw-   0        0        0   162448 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/programmer.jpg
+-rw-rw-rw-   0        0        0     1783 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/programmer.png
+-rw-rw-rw-   0        0        0      447 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/site.webmanifest
+-rw-rw-rw-   0        0        0   200333 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/teacher.jpg
+-rw-rw-rw-   0        0        0    23088 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/telegram.png
+-rw-rw-rw-   0        0        0   175178 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/user.png
+-rw-rw-rw-   0        0        0   117644 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/img/write.jpg
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.186333 gskChat-1.1.0/gskChat/gui/client/static/js/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/js/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.187330 gskChat-1.1.0/gskChat/gui/client/static/js/__pycache__/
+-rw-rw-rw-   0        0        0      210 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/client/static/js/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0    33901 2024-04-12 13:27:16.000000 gskChat-1.1.0/gskChat/gui/client/static/js/chat.v1.js
+-rw-rw-rw-   0        0        0   118841 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/js/highlight.min.js
+-rw-rw-rw-   0        0        0     1083 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/js/highlightjs-copy.min.js
+-rw-rw-rw-   0        0        0    10865 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/client/static/js/icons.js
+-rw-rw-rw-   0        0        0      410 2024-04-07 13:22:40.000000 gskChat-1.1.0/gskChat/gui/client/test.html
+-rw-rw-rw-   0        0        0      615 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/run.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.193314 gskChat-1.1.0/gskChat/gui/server/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/server/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.201456 gskChat-1.1.0/gskChat/gui/server/__pycache__/
+-rw-rw-rw-   0        0        0      200 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/server/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3366 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/server/__pycache__/android_gallery.cpython-312.pyc
+-rw-rw-rw-   0        0        0    12282 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/server/__pycache__/api.cpython-312.pyc
+-rw-rw-rw-   0        0        0      577 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/server/__pycache__/app.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4568 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/server/__pycache__/backend.cpython-312.pyc
+-rw-rw-rw-   0        0        0    14765 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/server/__pycache__/config.cpython-312.pyc
+-rw-rw-rw-   0        0        0     7883 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/server/__pycache__/internet.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1513 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/gui/server/__pycache__/website.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2470 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/server/android_gallery.py
+-rw-rw-rw-   0        0        0     9422 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/server/api.py
+-rw-rw-rw-   0        0        0      271 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/server/app.py
+-rw-rw-rw-   0        0        0     3681 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/server/backend.py
+-rw-rw-rw-   0        0        0    15354 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/server/config.py
+-rw-rw-rw-   0        0        0     4918 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/server/internet.py
+-rw-rw-rw-   0        0        0      839 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/server/website.py
+-rw-rw-rw-   0        0        0     1200 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/gui/webview.py
+-rw-rw-rw-   0        0        0     8399 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/image.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.204446 gskChat-1.1.0/gskChat/local/
+-rw-rw-rw-   0        0        0     1405 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/local/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.207386 gskChat-1.1.0/gskChat/local/__pycache__/
+-rw-rw-rw-   0        0        0     2679 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/local/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3047 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/local/__pycache__/_engine.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2179 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/local/__pycache__/_models.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1832 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/local/_engine.py
+-rw-rw-rw-   0        0        0     2959 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/local/_models.py
+-rw-rw-rw-   0        0        0     7633 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/models.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.213370 gskChat-1.1.0/gskChat/providers/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/providers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.220334 gskChat-1.1.0/gskChat/providers/__pycache__/
+-rw-rw-rw-   0        0        0      199 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/providers/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0    13248 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/providers/__pycache__/base_provider.cpython-312.pyc
+-rw-rw-rw-   0        0        0     7555 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/providers/__pycache__/create_images.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2745 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/providers/__pycache__/helper.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9044 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/providers/__pycache__/retry_provider.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4203 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/providers/__pycache__/types.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9260 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/providers/base_provider.py
+-rw-rw-rw-   0        0        0     6594 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/providers/create_images.py
+-rw-rw-rw-   0        0        0     1528 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/providers/helper.py
+-rw-rw-rw-   0        0        0     6869 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/providers/retry_provider.py
+-rw-rw-rw-   0        0        0     3083 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/providers/types.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.224325 gskChat-1.1.0/gskChat/requests/
+-rw-rw-rw-   0        0        0     3959 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/requests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.231357 gskChat-1.1.0/gskChat/requests/__pycache__/
+-rw-rw-rw-   0        0        0     4981 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/requests/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3226 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/requests/__pycache__/aiohttp.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5284 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/requests/__pycache__/curl_cffi.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1415 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/requests/__pycache__/defaults.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2638 2024-03-25 09:33:27.000000 gskChat-1.1.0/gskChat/requests/__pycache__/raise_for_status.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1775 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/requests/aiohttp.py
+-rw-rw-rw-   0        0        0     3016 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/requests/curl_cffi.py
+-rw-rw-rw-   0        0        0     1091 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/requests/defaults.py
+-rw-rw-rw-   0        0        0     1625 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/requests/raise_for_status.py
+-rw-rw-rw-   0        0        0     2938 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/stubs.py
+-rw-rw-rw-   0        0        0      875 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/typing.py
+-rw-rw-rw-   0        0        0     3821 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/version.py
+-rw-rw-rw-   0        0        0     9953 2024-03-25 09:33:26.000000 gskChat-1.1.0/gskChat/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:00:37.232354 gskChat-1.1.0/gskChat.egg-info/
+-rw-rw-rw-   0        0        0     2874 2024-04-12 14:00:36.000000 gskChat-1.1.0/gskChat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    15760 2024-04-12 14:00:36.000000 gskChat-1.1.0/gskChat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 14:00:36.000000 gskChat-1.1.0/gskChat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-12 14:00:36.000000 gskChat-1.1.0/gskChat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      621 2024-04-12 14:00:36.000000 gskChat-1.1.0/gskChat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 14:00:36.000000 gskChat-1.1.0/gskChat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 14:00:37.242597 gskChat-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     3200 2024-04-12 14:00:30.000000 gskChat-1.1.0/setup.py
```

### Comparing `gskChat-1.0.9/PKG-INFO` & `gskChat-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gskChat
-Version: 1.0.9
+Version: 1.1.0
 Summary: Gsk Chatbot
 Author: tafik
 Author-email: <doneld528@gmail.com>
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gskChat-1.0.9/gskChat/Provider/Aura.py` & `gskChat-1.1.0/gskChat/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/Bing.py` & `gskChat-1.1.0/gskChat/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/BingCreateImages.py` & `gskChat-1.1.0/gskChat/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/ChatForAi.py` & `gskChat-1.1.0/gskChat/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/Chatgpt4Online.py` & `gskChat-1.1.0/gskChat/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/ChatgptAi.py` & `gskChat-1.1.0/gskChat/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/ChatgptFree.py` & `gskChat-1.1.0/gskChat/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/ChatgptNext.py` & `gskChat-1.1.0/gskChat/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/ChatgptX.py` & `gskChat-1.1.0/gskChat/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/DeepInfra.py` & `gskChat-1.1.0/gskChat/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/FlowGpt.py` & `gskChat-1.1.0/gskChat/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/FreeChatgpt.py` & `gskChat-1.1.0/gskChat/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/FreeGpt.py` & `gskChat-1.1.0/gskChat/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/GeminiPro.py` & `gskChat-1.1.0/gskChat/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/GeminiProChat.py` & `gskChat-1.1.0/gskChat/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/GigaChat.py` & `gskChat-1.1.0/gskChat/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/GptTalkRu.py` & `gskChat-1.1.0/gskChat/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/HuggingChat.py` & `gskChat-1.1.0/gskChat/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/HuggingFace.py` & `gskChat-1.1.0/gskChat/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/Koala.py` & `gskChat-1.1.0/gskChat/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/Liaobots.py` & `gskChat-1.1.0/gskChat/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/Llama2.py` & `gskChat-1.1.0/gskChat/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/PerplexityLabs.py` & `gskChat-1.1.0/gskChat/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/Pi.py` & `gskChat-1.1.0/gskChat/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/Vercel.py` & `gskChat-1.1.0/gskChat/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/You.py` & `gskChat-1.1.0/gskChat/Provider/You.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__init__.py` & `gskChat-1.1.0/gskChat/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/Aura.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/Aura.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/Bing.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/Bing.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/BingCreateImages.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/BingCreateImages.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/ChatForAi.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/ChatForAi.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/Chatgpt4Online.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/Chatgpt4Online.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptAi.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/ChatgptAi.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptFree.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/ChatgptFree.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptNext.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/ChatgptNext.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptX.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/ChatgptX.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/DeepInfra.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/DeepInfra.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/FlowGpt.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/FlowGpt.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/FreeChatgpt.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/FreeChatgpt.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/FreeGpt.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/FreeGpt.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/GeminiPro.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/GeminiPro.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/GeminiProChat.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/GeminiProChat.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/GigaChat.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/GigaChat.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/GptTalkRu.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/GptTalkRu.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/HuggingChat.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/HuggingChat.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/HuggingFace.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/HuggingFace.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/Koala.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/Koala.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/Liaobots.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/Liaobots.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/Llama2.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/Llama2.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/PerplexityLabs.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/PerplexityLabs.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/Pi.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/Pi.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/Vercel.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/Vercel.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/You.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/You.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/bing/__pycache__/conversation.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/bing/__pycache__/conversation.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/bing/__pycache__/create_images.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/bing/__pycache__/create_images.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/bing/__pycache__/upload_image.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/bing/__pycache__/upload_image.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/bing/conversation.py` & `gskChat-1.1.0/gskChat/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/bing/create_images.py` & `gskChat-1.1.0/gskChat/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/bing/upload_image.py` & `gskChat-1.1.0/gskChat/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Acytoo.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/AiAsk.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/AiChatOnline.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/AiService.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Aibn.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Aichat.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Ails.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Aivvm.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Berlin.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/ChatAnywhere.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/ChatgptDuo.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/CodeLinkAva.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Cromicle.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/DfeHub.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/EasyChat.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Equing.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/FakeGpt.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/FastGpt.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Forefront.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/GPTalk.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/GeekGpt.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/GetGpt.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/H2o.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Hashnode.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Lockchat.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Myshell.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/NoowAi.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Opchatgpts.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Phind.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/V50.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Vercel.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Vitalentum.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/VoiGpt.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Wewordle.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Wuguokai.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Ylokh.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/Yqcloud.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__init__.py` & `gskChat-1.1.0/gskChat/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Acytoo.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Acytoo.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/AiAsk.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/AiAsk.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/AiChatOnline.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/AiChatOnline.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/AiService.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/AiService.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Aibn.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Aibn.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Aichat.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Aichat.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Ails.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Ails.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Aivvm.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Aivvm.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Berlin.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Berlin.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/ChatAnywhere.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/ChatAnywhere.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/ChatgptDuo.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/ChatgptDuo.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/CodeLinkAva.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/CodeLinkAva.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Cromicle.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Cromicle.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/DfeHub.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/DfeHub.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/EasyChat.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/EasyChat.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Equing.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Equing.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/FakeGpt.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/FakeGpt.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/FastGpt.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/FastGpt.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Forefront.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Forefront.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/GPTalk.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/GPTalk.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/GeekGpt.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/GeekGpt.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/GetGpt.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/GetGpt.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/H2o.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/H2o.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Hashnode.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Hashnode.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Lockchat.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Lockchat.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Myshell.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Myshell.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/NoowAi.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/NoowAi.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Opchatgpts.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Opchatgpts.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Phind.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Phind.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/V50.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/V50.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Vercel.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Vercel.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Vitalentum.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Vitalentum.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/VoiGpt.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/VoiGpt.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Wewordle.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Wewordle.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Wuguokai.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Wuguokai.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Ylokh.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Ylokh.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Yqcloud.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/Yqcloud.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/deprecated/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `gskChat-1.1.0/gskChat/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/needs_auth/Gemini.py` & `gskChat-1.1.0/gskChat/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/needs_auth/OpenAssistant.py` & `gskChat-1.1.0/gskChat/Provider/needs_auth/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/needs_auth/OpenaiChat.py` & `gskChat-1.1.0/gskChat/Provider/needs_auth/OpenaiChat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/needs_auth/Poe.py` & `gskChat-1.1.0/gskChat/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/needs_auth/Raycast.py` & `gskChat-1.1.0/gskChat/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/needs_auth/Theb.py` & `gskChat-1.1.0/gskChat/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/needs_auth/ThebApi.py` & `gskChat-1.1.0/gskChat/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Gemini.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/Gemini.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/OpenAssistant.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/OpenAssistant.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/OpenaiChat.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/OpenaiChat.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Poe.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/Poe.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Raycast.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/Raycast.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Theb.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/Theb.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/ThebApi.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/needs_auth/__pycache__/ThebApi.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/AItianhu.py` & `gskChat-1.1.0/gskChat/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/Bestim.py` & `gskChat-1.1.0/gskChat/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/ChatBase.py` & `gskChat-1.1.0/gskChat/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/ChatgptDemo.py` & `gskChat-1.1.0/gskChat/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/ChatgptDemoAi.py` & `gskChat-1.1.0/gskChat/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/ChatgptLogin.py` & `gskChat-1.1.0/gskChat/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/Chatxyz.py` & `gskChat-1.1.0/gskChat/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/Gpt6.py` & `gskChat-1.1.0/gskChat/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/GptChatly.py` & `gskChat-1.1.0/gskChat/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/GptForLove.py` & `gskChat-1.1.0/gskChat/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/GptGo.py` & `gskChat-1.1.0/gskChat/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/GptGod.py` & `gskChat-1.1.0/gskChat/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/OnlineGpt.py` & `gskChat-1.1.0/gskChat/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/AItianhu.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/AItianhu.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/Bestim.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/Bestim.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatBase.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/ChatBase.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatgptDemo.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/ChatgptDemo.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatgptDemoAi.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/ChatgptDemoAi.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatgptLogin.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/ChatgptLogin.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/Chatxyz.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/Chatxyz.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/Gpt6.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/Gpt6.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptChatly.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/GptChatly.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptForLove.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/GptForLove.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptGo.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/GptGo.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptGod.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/GptGod.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/OnlineGpt.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/OnlineGpt.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/not_working/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/npm/node_modules/crypto-js/README.md` & `gskChat-1.1.0/gskChat/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/npm/node_modules/crypto-js/crypto-js.js` & `gskChat-1.1.0/gskChat/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/npm/package-lock.json` & `gskChat-1.1.0/gskChat/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/selenium/AItianhuSpace.py` & `gskChat-1.1.0/gskChat/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/selenium/Bard.py` & `gskChat-1.1.0/gskChat/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/selenium/MyShell.py` & `gskChat-1.1.0/gskChat/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/selenium/PerplexityAi.py` & `gskChat-1.1.0/gskChat/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/selenium/Phind.py` & `gskChat-1.1.0/gskChat/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/selenium/TalkAi.py` & `gskChat-1.1.0/gskChat/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/AItianhuSpace.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/selenium/__pycache__/AItianhuSpace.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/Bard.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/selenium/__pycache__/Bard.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/MyShell.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/selenium/__pycache__/MyShell.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/PerplexityAi.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/selenium/__pycache__/PerplexityAi.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/Phind.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/selenium/__pycache__/Phind.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/TalkAi.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/selenium/__pycache__/TalkAi.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/unfinished/AiChatting.py` & `gskChat-1.1.0/gskChat/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/unfinished/ChatAiGpt.py` & `gskChat-1.1.0/gskChat/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/unfinished/Komo.py` & `gskChat-1.1.0/gskChat/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/unfinished/MikuChat.py` & `gskChat-1.1.0/gskChat/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/AiChatting.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/unfinished/__pycache__/AiChatting.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/ChatAiGpt.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/unfinished/__pycache__/ChatAiGpt.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/Komo.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/unfinished/__pycache__/Komo.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/MikuChat.cpython-312.pyc` & `gskChat-1.1.0/gskChat/Provider/unfinished/__pycache__/MikuChat.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/__init__.py` & `gskChat-1.1.0/gskChat/__init__.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.1.0/gskChat/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/__pycache__/cli.cpython-312.pyc` & `gskChat-1.1.0/gskChat/__pycache__/cli.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/__pycache__/client.cpython-312.pyc` & `gskChat-1.1.0/gskChat/__pycache__/client.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/__pycache__/cookies.cpython-312.pyc` & `gskChat-1.1.0/gskChat/__pycache__/cookies.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/__pycache__/errors.cpython-312.pyc` & `gskChat-1.1.0/gskChat/__pycache__/errors.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/__pycache__/image.cpython-312.pyc` & `gskChat-1.1.0/gskChat/__pycache__/image.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/__pycache__/models.cpython-312.pyc` & `gskChat-1.1.0/gskChat/__pycache__/models.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/__pycache__/stubs.cpython-312.pyc` & `gskChat-1.1.0/gskChat/__pycache__/stubs.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/__pycache__/typing.cpython-312.pyc` & `gskChat-1.1.0/gskChat/__pycache__/typing.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/__pycache__/version.cpython-312.pyc` & `gskChat-1.1.0/gskChat/__pycache__/version.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/__pycache__/webdriver.cpython-312.pyc` & `gskChat-1.1.0/gskChat/__pycache__/webdriver.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/api/__init__.py` & `gskChat-1.1.0/gskChat/api/__init__.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/api/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.1.0/gskChat/api/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/api/__pycache__/_logging.cpython-312.pyc` & `gskChat-1.1.0/gskChat/api/__pycache__/_logging.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/api/__pycache__/run.cpython-312.pyc` & `gskChat-1.1.0/gskChat/api/__pycache__/run.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/api/_logging.py` & `gskChat-1.1.0/gskChat/api/_logging.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/cli.py` & `gskChat-1.1.0/gskChat/cli.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/client.py` & `gskChat-1.1.0/gskChat/client.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/cookies.py` & `gskChat-1.1.0/gskChat/cookies.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/errors.py` & `gskChat-1.1.0/gskChat/errors.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/__init__.py` & `gskChat-1.1.0/gskChat/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.1.0/gskChat/gui/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/__pycache__/run.cpython-312.pyc` & `gskChat-1.1.0/gskChat/gui/__pycache__/run.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/__pycache__/webview.cpython-312.pyc` & `gskChat-1.1.0/gskChat/gui/__pycache__/webview.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/index.html` & `gskChat-1.1.0/gskChat/gui/client/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -280,29 +280,29 @@
                                 <option value="Gemini">Gemini</option>
                                 <option value="Liaobots">Liaobots</option>
                                 <option value="You">You</option>
                                 <option value="">----</option>
                             </select>
                         </div>
                     </div>
-                    <div class="field">
+                    <div class="field" style="display: none;">
                         <input type="checkbox" id="switch" />
                         <label for="switch" title="Add the pages of the first 5 search results to the query."></label>
                         <span class="about">Доступ к Паутине</span>
                     </div>
                     <!--
                     <div class="field">
                         <input type="checkbox" id="patch" />
                         <label for="patch" title="Enable create images with Bing."></label>
                         <span class="about">Image Generator</span>
                     </div>
                     -->
                     <div class="field">
-                        <input type="checkbox" id="history" />
-                        <label for="history" title="To improve the reaction time or if you have trouble with large conversations."></label>
+                        <input type="checkbox" id="history"/>
+                        <label id="checkvirl" for="history" title="To improve the reaction time or if you have trouble with large conversations."></label>
                         <span class="about">Выключить историю чата</span>
                     </div>
                 </div>
             </div>
         </div>
         <div class="mobile-sidebar">
             <i class="fa-solid fa-bars"></i>
@@ -543,14 +543,15 @@
     }
   }, 3000);
 });
 </script>
 <!--смена в чате-->
 <script>
   document.querySelector('.avtoLogo').addEventListener('click', function() {
+    window.location.href = 'http://127.0.0.1:8080';
   // Включаем стиль display: none для блока с id="prevYou"
   document.querySelector('.row').style.display = 'none';
 document.querySelector('.particles-js-canvas-el').style.backgroundColor = '#083142'
 let imageElement = document.querySelector(".imgLogo");
 imageElement.src = "/static/img/programmer.jpg";
 // Имитация загрузки
   var loadingGif = document.createElement('img');
@@ -623,10 +624,36 @@
     for (var i = 0; i < rows.length; i++) {
       rows[i].style.display = 'flex';
       document.querySelector('.particles-js-canvas-el').style.backgroundColor = ''
     }
   }, 3000);
 });
 </script>
+<!--выборка автоматом-->
+<script>
+  
+    localStorage.history = "true"
+  document.querySelector('#programmer').addEventListener ('click', ()=> {
+    document.querySelector("#provider").value = "You";
+    document.querySelector("#model").value = "gpt-3.5-turbo";
+    document.querySelector("#model2").value = "gpt-3.5-turbo";
+
+
+  });
+  document.querySelector('#teacher').addEventListener ('click', ()=> {
+    document.querySelector("#provider").value = "You";
+    document.querySelector("#model").value = "gpt-3.5-turbo";
+    document.querySelector("#model2").value = "gpt-3.5-turbo";
+
+  });
+  document.querySelector('#writer').addEventListener ('click', ()=> {
+    document.querySelector("#provider").value = "You";
+    document.querySelector("#model").value = "gpt-3.5-turbo";
+    document.querySelector("#model2").value = "gpt-3.5-turbo";
+
+  });
+
+
+</script>
 </body>
         
 </html>
```

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/css/style.css` & `gskChat-1.1.0/gskChat/gui/client/static/css/style.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,35 @@
 @import url("https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap");
+.buttons {
+    position: absolute;
+   opacity: 0;
+   pointer-events: none;
+
+}
+#send-button {
+    transition: 300ms;
+    border-radius: 0px 8px 8px 0px;
+    position: absolute;
+    right: -1px;
+    height: 100%;
 
+    background: rgba(0, 183, 255, 0.6);
+}
+#version_text {
+    display: none;
+}
+#send-button:hover {
+    transition: 300ms;
+    border-radius: 0px 8px 8px 0px;
+    position: absolute;
+    right: -1px;
+    height: 100%;
+    width: 22%;
+    background: rgba(0, 183, 255, 0.9);
+}
 .avtoLogo {
     padding: 5px;
     width: 100%;
     transition: 250ms;
     justify-content: center;
     height: 165px;
 }
@@ -32,17 +58,15 @@
     
     cursor:url('../img/1.png'), default;
 }
 select:hover, button:hover, option:hover, .fa-download, .fa-trash, .deleteChat, .fa-plus, label:hover, a:hover, .new_convo span:hover, .close:hover, .avtoLogo, .avtoLogo img, .modal-content ul li a, .secondAuto, .modal-content img, .modal-content span, .selectAutor, .logoAutor, .contentAutor, .contentAutor h3, .contentAutor span, .logoAutor img {
     cursor:url('../img/favicon-32x32.png'), pointer;
 }
 
-#message-input {
-    cursor:url('../img/favicon-16x16.png'), pointer;
-}
+
 .secondAuto {
     margin-left: 3%;
     width: 100%;
 }
 #autor img {
     width: 40px;
     height: 40px;
@@ -205,25 +229,44 @@
     padding: var(--section-gap);
     overflow: none;
     flex-shrink: 0;
     display: flex;
     flex-direction: column;
     justify-content: space-between;
 }
- 
+
+@media screen and (min-width: 729px) {
+    #send-button {
+        width: 12%;
+    }
+    #send-button:hover {
+        width: 6%;
+    }
+}
 @media screen and (max-width: 728px) {
+    #send-button {
+        width: 20%;
+    }
+    #send-button:hover {
+        width: inherit;
+    }
     #autorCreate .secondAuto {
         font-size: 20px;
     }
     .secondAuto {
         font-size: 20px;
     }
     .modal-content {
-        width: 95%;
-        height: 150%;
+        width: 74%;
+        height: 100%;
+        margin-bottom: 10%;
+        padding-bottom: 1%;
+    }
+    .close {
+        font-size: 60px;
     }
     .ads {
         display: none;
     }
 }
 
 /* :root {
@@ -928,15 +971,17 @@
     user-select: none;
     background: transparent;
     border-radius: var(--border-radius-1);
     width: 100%;
     cursor: default;
     border: 1px dashed rgba(0, 183, 255, 0.3);
 }
-
+select {
+    pointer-events: none;
+}
 .bottom_buttons {
     width: 100%;
     display: flex;
     flex-direction: column;
     gap: 10px;
 }
 .bottom_buttons button:hover {
@@ -1336,40 +1381,44 @@
 }
 .fa-paper-plane-top {
     width: 100%;
    
 margin-top: 2em;
     text-align: center;
 }
-#send-button {
-    transition: 300ms;
-    border-radius: 0px 8px 8px 0px;
-    position: absolute;
-    right: -1px;
-    height: 100%;
-    width: 3%;
-    background: rgba(0, 183, 255, 0.6);
-}
-#version_text {
-    display: none;
-}
-#send-button:hover {
-    transition: 300ms;
-    border-radius: 0px 8px 8px 0px;
-    position: absolute;
-    right: -1px;
-    height: 100%;
-    width: 4%;
-    background: rgba(0, 183, 255, 0.9);
-}
+
 
 #systemPrompt {
     display: none;
     font-size: 15px;
     width: 100%;
     color: var(--colour-3);
     min-height: 59px;
     height: 59px;
     outline: none;
     padding: var(--inner-gap) var(--section-gap);
     resize: vertical;
 }
+@media screen and (min-width: 1100px) {
+    #send-button {
+        width: 12%;
+    }
+}
+@media screen and (min-width: 1350px) {
+    #send-button {
+        width: 4%;
+    }
+    #send-button:hover {
+        width: 6%;
+    }
+}
+@media screen and (max-width: 800px) {
+.loading {
+    width: 50%;
+}
+.imgLogo {
+    width: 50%;
+}
+.avtoLogo {
+    text-align: center;
+}
+}
```

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/1.png` & `gskChat-1.1.0/gskChat/gui/client/static/img/1.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/android-chrome-192x192.png` & `gskChat-1.1.0/gskChat/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/android-chrome-512x512.png` & `gskChat-1.1.0/gskChat/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/apple-touch-icon.png` & `gskChat-1.1.0/gskChat/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/content.png` & `gskChat-1.1.0/gskChat/gui/client/static/img/content.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/favicon-16x16.png` & `gskChat-1.1.0/gskChat/gui/client/static/img/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/favicon-32x32.png` & `gskChat-1.1.0/gskChat/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/gpt.png` & `gskChat-1.1.0/gskChat/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/gpt1.png` & `gskChat-1.1.0/gskChat/gui/client/static/img/gpt1.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/graphic-designer.png` & `gskChat-1.1.0/gskChat/gui/client/static/img/graphic-designer.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/loading-1.gif` & `gskChat-1.1.0/gskChat/gui/client/static/img/loading-1.gif`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/loading-101.gif` & `gskChat-1.1.0/gskChat/gui/client/static/img/loading-101.gif`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/programmer.jpg` & `gskChat-1.1.0/gskChat/gui/client/static/img/programmer.jpg`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/programmer.png` & `gskChat-1.1.0/gskChat/gui/client/static/img/programmer.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/teacher.jpg` & `gskChat-1.1.0/gskChat/gui/client/static/img/teacher.jpg`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/telegram.png` & `gskChat-1.1.0/gskChat/gui/client/static/img/telegram.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/user.png` & `gskChat-1.1.0/gskChat/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/img/write.jpg` & `gskChat-1.1.0/gskChat/gui/client/static/img/write.jpg`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/js/chat.v1.js` & `gskChat-1.1.0/gskChat/gui/client/static/js/chat.v1.js`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/js/highlight.min.js` & `gskChat-1.1.0/gskChat/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/js/highlightjs-copy.min.js` & `gskChat-1.1.0/gskChat/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/client/static/js/icons.js` & `gskChat-1.1.0/gskChat/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/run.py` & `gskChat-1.1.0/gskChat/gui/run.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/server/__pycache__/android_gallery.cpython-312.pyc` & `gskChat-1.1.0/gskChat/gui/server/__pycache__/android_gallery.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/server/__pycache__/api.cpython-312.pyc` & `gskChat-1.1.0/gskChat/gui/server/__pycache__/api.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/server/__pycache__/app.cpython-312.pyc` & `gskChat-1.1.0/gskChat/gui/server/__pycache__/app.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/server/__pycache__/backend.cpython-312.pyc` & `gskChat-1.1.0/gskChat/gui/server/__pycache__/backend.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/server/__pycache__/config.cpython-312.pyc` & `gskChat-1.1.0/gskChat/gui/server/__pycache__/config.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/server/__pycache__/internet.cpython-312.pyc` & `gskChat-1.1.0/gskChat/gui/server/__pycache__/internet.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/server/__pycache__/website.cpython-312.pyc` & `gskChat-1.1.0/gskChat/gui/server/__pycache__/website.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/server/android_gallery.py` & `gskChat-1.1.0/gskChat/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/server/api.py` & `gskChat-1.1.0/gskChat/gui/server/api.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/server/backend.py` & `gskChat-1.1.0/gskChat/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/server/config.py` & `gskChat-1.1.0/gskChat/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/server/internet.py` & `gskChat-1.1.0/gskChat/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/server/website.py` & `gskChat-1.1.0/gskChat/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/gui/webview.py` & `gskChat-1.1.0/gskChat/gui/webview.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/image.py` & `gskChat-1.1.0/gskChat/image.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/local/__init__.py` & `gskChat-1.1.0/gskChat/local/__init__.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/local/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.1.0/gskChat/local/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/local/__pycache__/_engine.cpython-312.pyc` & `gskChat-1.1.0/gskChat/local/__pycache__/_engine.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/local/__pycache__/_models.cpython-312.pyc` & `gskChat-1.1.0/gskChat/local/__pycache__/_models.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/local/_engine.py` & `gskChat-1.1.0/gskChat/local/_engine.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/local/_models.py` & `gskChat-1.1.0/gskChat/local/_models.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/models.py` & `gskChat-1.1.0/gskChat/models.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/providers/__pycache__/base_provider.cpython-312.pyc` & `gskChat-1.1.0/gskChat/providers/__pycache__/base_provider.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/providers/__pycache__/create_images.cpython-312.pyc` & `gskChat-1.1.0/gskChat/providers/__pycache__/create_images.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/providers/__pycache__/helper.cpython-312.pyc` & `gskChat-1.1.0/gskChat/providers/__pycache__/helper.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/providers/__pycache__/retry_provider.cpython-312.pyc` & `gskChat-1.1.0/gskChat/providers/__pycache__/retry_provider.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/providers/__pycache__/types.cpython-312.pyc` & `gskChat-1.1.0/gskChat/providers/__pycache__/types.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/providers/base_provider.py` & `gskChat-1.1.0/gskChat/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/providers/create_images.py` & `gskChat-1.1.0/gskChat/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/providers/helper.py` & `gskChat-1.1.0/gskChat/providers/helper.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/providers/retry_provider.py` & `gskChat-1.1.0/gskChat/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/providers/types.py` & `gskChat-1.1.0/gskChat/providers/types.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/requests/__init__.py` & `gskChat-1.1.0/gskChat/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/requests/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.1.0/gskChat/requests/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/requests/__pycache__/aiohttp.cpython-312.pyc` & `gskChat-1.1.0/gskChat/requests/__pycache__/aiohttp.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/requests/__pycache__/curl_cffi.cpython-312.pyc` & `gskChat-1.1.0/gskChat/requests/__pycache__/curl_cffi.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/requests/__pycache__/defaults.cpython-312.pyc` & `gskChat-1.1.0/gskChat/requests/__pycache__/defaults.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/requests/__pycache__/raise_for_status.cpython-312.pyc` & `gskChat-1.1.0/gskChat/requests/__pycache__/raise_for_status.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/requests/aiohttp.py` & `gskChat-1.1.0/gskChat/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/requests/curl_cffi.py` & `gskChat-1.1.0/gskChat/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/requests/defaults.py` & `gskChat-1.1.0/gskChat/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/requests/raise_for_status.py` & `gskChat-1.1.0/gskChat/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/stubs.py` & `gskChat-1.1.0/gskChat/stubs.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/typing.py` & `gskChat-1.1.0/gskChat/typing.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/version.py` & `gskChat-1.1.0/gskChat/version.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat/webdriver.py` & `gskChat-1.1.0/gskChat/webdriver.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat.egg-info/PKG-INFO` & `gskChat-1.1.0/gskChat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gskChat
-Version: 1.0.9
+Version: 1.1.0
 Summary: Gsk Chatbot
 Author: tafik
 Author-email: <doneld528@gmail.com>
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gskChat-1.0.9/gskChat.egg-info/SOURCES.txt` & `gskChat-1.1.0/gskChat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/gskChat.egg-info/requires.txt` & `gskChat-1.1.0/gskChat.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.9/setup.py` & `gskChat-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 DESCRIPTION = (
     "Gsk Chatbot"
 )
 
 # Setting up
 setup(
     name='gskChat',
-    version="1.0.9",
+    version="1.1.0",
     author='tafik',
     author_email='<doneld528@gmail.com>',
     description=DESCRIPTION,
     long_description_content_type='text/markdown',
     long_description="Gsk Chatbot",
     packages=find_packages(),
     package_data={
```

