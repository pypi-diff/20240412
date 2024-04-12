# Comparing `tmp/xiaogpt-2.26.tar.gz` & `tmp/xiaogpt-2.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-2.26.tar", last modified: Sat Feb  3 14:36:36 2024, max compression
+gzip compressed data, was "xiaogpt-2.30.tar", last modified: Fri Apr 12 15:00:41 2024, max compression
```

## Comparing `xiaogpt-2.26.tar` & `xiaogpt-2.30.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1063 2024-02-03 14:35:58.402391 xiaogpt-2.26/LICENSE
--rw-r--r--   0        0        0    18020 2024-02-03 14:35:58.402391 xiaogpt-2.26/README.md
--rw-r--r--   0        0        0     1172 2024-02-03 14:36:36.046108 xiaogpt-2.26/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/__main__.py
--rw-r--r--   0        0        0     1073 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0      840 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/bot/bard_bot.py
--rw-r--r--   0        0        0     1467 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3656 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1840 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/bot/gemini_bot.py
--rw-r--r--   0        0        0     1825 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     2781 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/bot/gpt3_bot.py
--rw-r--r--   0        0        0     1944 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/bot/langchain_bot.py
--rw-r--r--   0        0        0     2289 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3657 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/bot/qwen_bot.py
--rw-r--r--   0        0        0     5057 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/cli.py
--rw-r--r--   0        0        0     6287 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/config.py
--rw-r--r--   0        0        0     2616 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/langchain/callbacks.py
--rw-r--r--   0        0        0     1495 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/langchain/chain.py
--rw-r--r--   0        0        0     6372 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/langchain/examples/email/mail_box.py
--rw-r--r--   0        0        0     1561 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/langchain/examples/email/mail_summary_tools.py
--rw-r--r--   0        0        0      130 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/tts/__init__.py
--rw-r--r--   0        0        0     4922 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/tts/base.py
--rw-r--r--   0        0        0     1172 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/tts/edge.py
--rw-r--r--   0        0        0     1096 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/tts/mi.py
--rw-r--r--   0        0        0     1533 2024-02-03 14:35:58.402391 xiaogpt-2.26/xiaogpt/tts/openai.py
--rw-r--r--   0        0        0     2072 2024-02-03 14:35:58.406391 xiaogpt-2.26/xiaogpt/utils.py
--rw-r--r--   0        0        0    15273 2024-02-03 14:35:58.406391 xiaogpt-2.26/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    18887 1970-01-01 00:00:00.000000 xiaogpt-2.26/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-12 15:00:36.164055 xiaogpt-2.30/LICENSE
+-rw-r--r--   0        0        0    23688 2024-04-12 15:00:36.164055 xiaogpt-2.30/README.md
+-rw-r--r--   0        0        0     1263 2024-04-12 15:00:41.880149 xiaogpt-2.30/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/__main__.py
+-rw-r--r--   0        0        0     1073 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0      840 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/bard_bot.py
+-rw-r--r--   0        0        0     1467 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3656 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1840 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/gemini_bot.py
+-rw-r--r--   0        0        0     1825 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     2781 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/gpt3_bot.py
+-rw-r--r--   0        0        0     1944 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/langchain_bot.py
+-rw-r--r--   0        0        0     2289 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3657 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/qwen_bot.py
+-rw-r--r--   0        0        0     5506 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/cli.py
+-rw-r--r--   0        0        0     6703 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/config.py
+-rw-r--r--   0        0        0     2616 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/langchain/callbacks.py
+-rw-r--r--   0        0        0     1495 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/langchain/chain.py
+-rw-r--r--   0        0        0     6372 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/langchain/examples/email/mail_box.py
+-rw-r--r--   0        0        0     1561 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/langchain/examples/email/mail_summary_tools.py
+-rw-r--r--   0        0        0      220 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/tts/__init__.py
+-rw-r--r--   0        0        0     3978 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/tts/azure.py
+-rw-r--r--   0        0        0     4923 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/tts/base.py
+-rw-r--r--   0        0        0     1172 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/tts/edge.py
+-rw-r--r--   0        0        0     1096 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/tts/mi.py
+-rw-r--r--   0        0        0     1533 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/tts/openai.py
+-rw-r--r--   0        0        0     2072 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/utils.py
+-rw-r--r--   0        0        0    15400 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    24670 1970-01-01 00:00:00.000000 xiaogpt-2.30/PKG-INFO
```

### Comparing `xiaogpt-2.26/LICENSE` & `xiaogpt-2.30/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/README.md` & `xiaogpt-2.30/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,23 +16,41 @@
 - ChatGPT
 - New Bing
 - [ChatGLM](http://open.bigmodel.cn/)
 - [Gemini](https://makersuite.google.com/app/apikey)
 - [Bard](https://github.com/dsdanielpark/Bard-API)
 - [通义千问](https://help.aliyun.com/zh/dashscope/developer-reference/api-details)
 
-## Windows 获取小米音响DID
-
-1. `pip install miservice_fork`
-2. `set MI_USER=xxxx`
-3. `set MI_PASS=xxx`
-4. `micli list` 得到did
-5. `set MI_DID=xxxx`
+## 获取小米音响DID
+### Windows(使用 set 设置环境变量）
+```cmd
+pip install miservice_fork
+set MI_USER=xxxx
+set MI_PASS=xxx
+micli list 得到did
+set MI_DID=xxxx
+```
 
 - 如果获取did报错时，请更换一下无线网络，有很大概率解决问题。
+ 
+### Linux(使用 export 设置环境变量）
+```sh
+# 1、安装模块
+pip install miservice_fork
+
+# 2、设置环境用户参数
+export MI_USER=xxxx
+export MI_PASS=xxx
+
+# 3、使用micli list 得到did
+micli list
+
+# 4、根据did设置环境DID参数
+export MI_DID=xxxx
+```
 
 ## 一点原理
 
 [不用 root 使用小爱同学和 ChatGPT 交互折腾记](https://github.com/yihong0618/gitblog/issues/258)
 
 ## 准备
 
@@ -54,14 +72,15 @@
 - 如果有能力可以自行替换唤醒词，也可以去掉唤醒词
 - 使用 `--use_chatgpt_api` 的 api 那样可以更流畅的对话，速度特别快，达到了对话的体验, [openai api](https://platform.openai.com/account/api-keys), 命令 `--use_chatgpt_api`
 - 使用 gpt-3 的 api 那样可以更流畅的对话，速度快, 请 google 如何用 [openai api](https://platform.openai.com/account/api-keys) 命令 --use_gpt3
 - 如果你遇到了墙需要用 Cloudflare Workers 替换 api_base 请使用 `--api_base ${url}` 来替换。 **请注意，此处你输入的api应该是'`https://xxxx/v1`'的字样，域名需要用引号包裹**
 - 可以跟小爱说 `开始持续对话` 自动进入持续对话状态，`结束持续对话` 结束持续对话状态。
 - 可以使用 `--tts edge` 来获取更好的 tts 能力
 - 可以使用 `--tts openai` 来获取 openai tts 能力
+- 可以使用 `--tts azure --azure_tts_speech_key <your-speech-key>` 来获取 Azure TTS 能力
 - 可以使用 `--use_langchain` 替代 `--use_chatgpt_api` 来调用 LangChain（默认 chatgpt）服务，实现上网检索、数学运算..
 
 e.g.
 
 ```shell
 export OPENAI_API_KEY=${your_api_key}
 xiaogpt --hardware LX06 --use_chatgpt_api
@@ -152,45 +171,47 @@
 
 具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
 ChatGLM [文档](http://open.bigmodel.cn/doc/api#chatglm_130b)
 Bard-API [参考](https://github.com/dsdanielpark/Bard-API)
 
 ## 配置项说明
 
-| 参数                  | 说明                                                                    | 默认值                                                                                                    |可选值            |
-| --------------------- | ----------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------- |
-| hardware              | 设备型号                                                                |                                                                                                           |
-| account               | 小爱账户                                                                |                                                                                                           |
-| password              | 小爱账户密码                                                            |                                                                                                           |
-| openai_key            | openai的apikey                                                          |                                                                                                           |
-| serpapi_api_key       | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                       |                                                                                                           |
-| glm_key               | chatglm 的 apikey                                                       |                                                                                                           |
-| gemini_key            | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                                                      |                                                                                                           |
-| qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details)                                                      |                                                                                                           |
-| bard_token            | bard 的 token 参考 [Bard-API](https://github.com/dsdanielpark/Bard-API) |                                                                                                           |
-| cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                             |                                                                                                           |
-| mi_did                | 设备did                                                                 |                                                                                                           |
-| use_command           | 使用 MI command 与小爱交互                                              | `false`                                                                                                   |
-| mute_xiaoai           | 快速停掉小爱自己的回答                                                  | `true`                                                                                                    |
-| verbose               | 是否打印详细日志                                                        | `false`                                                                                                   |
-| bot                   | 使用的 bot 类型，目前支持gpt3,chatgptapi和newbing                       | `chatgptapi`                                                                                              |
-| tts                   | 使用的 TTS 类型                                                         | `mi`                                                                                                      | `edge`、 `openai` | 
-| tts_voice             | TTS 的嗓音                                                              | `zh-CN-XiaoxiaoNeural`(edge), `alloy`(openai)                                                             |
-| prompt                | 自定义prompt                                                            | `请用100字以内回答`                                                                                       |
-| keyword               | 自定义请求词列表                                                        | `["请"]`                                                                                                  |
-| change_prompt_keyword | 更改提示词触发列表                                                      | `["更改提示词"]`                                                                                          |
-| start_conversation    | 开始持续对话关键词                                                      | `开始持续对话`                                                                                            |
-| end_conversation      | 结束持续对话关键词                                                      | `结束持续对话`                                                                                            |
-| stream                | 使用流式响应，获得更快的响应                                            | `false`                                                                                                   |
-| proxy                 | 支持 HTTP 代理，传入 http proxy URL                                     | ""                                                                                                        |
-| gpt_options           | OpenAI API 的参数字典                                                   | `{}`                                                                                                      |
-| bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取                                 | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |
-| bing_cookies          | NewBing使用的cookie字典，参考[这里]获取                                 |                                                                                                           |
-| deployment_id         | Azure OpenAI 服务的 deployment ID                                       | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |
-| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                         | 例如：`https://abc-def.openai.azure.com/`                                                                 |
+| 参数                     | 说明                                                                                        | 默认值                                                                                                    | 可选值                                                                                                                     |
+| ------------------------ | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
+| hardware                 | 设备型号                                                                                    |                                                                                                           |                                                                                                                            |
+| account                  | 小爱账户                                                                                    |                                                                                                           |                                                                                                                            |
+| password                 | 小爱账户密码                                                                                |                                                                                                           |                                                                                                                            |
+| openai_key               | openai的apikey                                                                              |                                                                                                           |                                                                                                                            |
+| serpapi_api_key          | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                           |                                                                                                           |                                                                                                                            |
+| glm_key                  | chatglm 的 apikey                                                                           |                                                                                                           |                                                                                                                            |
+| gemini_key               | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                                                                                            |
+| qwen_key                 | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                                                                                            |
+| bard_token               | bard 的 token 参考 [Bard-API](https://github.com/dsdanielpark/Bard-API)                     |                                                                                                           |                                                                                                                            |
+| cookie                   | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                                                                                            |
+| mi_did                   | 设备did                                                                                     |                                                                                                           |                                                                                                                            |
+| use_command              | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                                                                                            |
+| mute_xiaoai              | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                                                                                            |
+| verbose                  | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                                                                                            |
+| bot                      | 使用的 bot 类型，目前支持gpt3,chatgptapi和newbing                                           | `chatgptapi`                                                                                              |                                                                                                                            |
+| tts                      | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`                                                                                                 |
+| tts_voice                | TTS 的嗓音                                                                                  | `zh-CN-XiaoxiaoNeural`(edge), `alloy`(openai), `zh-CN-XiaoxiaoMultilingualNeural`(azure)                  |                                                                                                                            |
+| prompt                   | 自定义prompt                                                                                | `请用100字以内回答`                                                                                       |                                                                                                                            |
+| keyword                  | 自定义请求词列表                                                                            | `["请"]`                                                                                                  |                                                                                                                            |
+| change_prompt_keyword    | 更改提示词触发列表                                                                          | `["更改提示词"]`                                                                                          |                                                                                                                            |
+| start_conversation       | 开始持续对话关键词                                                                          | `开始持续对话`                                                                                            |                                                                                                                            |
+| end_conversation         | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                                                                                            |
+| stream                   | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                                                                                            |
+| proxy                    | 支持 HTTP 代理，传入 http proxy URL                                                         | ""                                                                                                        |                                                                                                                            |
+| gpt_options              | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                                                                                            |
+| bing_cookie_path         | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                                                                                            |
+| bing_cookies             | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                                                                                            |
+| deployment_id            | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                                                                                            |
+| api_base                 | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |                                                                                                                            |
+| azure_tts_speech_key     | Azure TTS key                                                                               | null                                                                                                      |                                                                                                                            |
+| azure_tts_service_region | Azure TTS 服务地区                                                                          | `eastasia`                                                                                                | [Regions - Speech service - Azure AI services](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/regions) |
 
 [这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
@@ -233,14 +254,20 @@
 
 xiaogpt的配置文件可通过指定volume /config，以及指定参数--config来处理，如
 
 ```shell
 docker run -v <your-config-dir>:/config yihong0618/xiaogpt --config=/config/config.json
 ```
 
+### 网络使用 host 模型
+
+```shell
+docker run -v <your-config-dir>:/config --network=host yihong0618/xiaogpt --config=/config/config.json
+```
+
 ### 本地编译Docker Image
 
 ```shell
  docker build -t xiaogpt .
 ```
 
 如果在安装依赖时构建失败或安装缓慢时，可以在构建 Docker 镜像时使用 `--build-arg` 参数来指定国内源地址：
```

### Comparing `xiaogpt-2.26/pyproject.toml` & `xiaogpt-2.30/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -13,26 +13,29 @@
 requires-python = ">=3.9"
 dependencies = [
     "miservice_fork",
     "openai>=1",
     "aiohttp",
     "rich",
     "zhipuai==2.0.1",
+    "httpx==0.24.1",
     "bardapi",
     "edge-tts>=6.1.3",
     "EdgeGPT==0.1.26",
     "langchain>=0.0.343",
     "beautifulsoup4>=4.12.0",
     "google-search-results>=2.4.2",
     "google-generativeai",
     "numexpr>=2.8.6",
     "dashscope==1.10.0",
+    "httpcore==0.15.0",
+    "azure-cognitiveservices-speech>=1.37.0",
 ]
 dynamic = []
-version = "2.26"
+version = "2.30"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
```

### Comparing `xiaogpt-2.26/xiaogpt/bot/__init__.py` & `xiaogpt-2.30/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/bot/bard_bot.py` & `xiaogpt-2.30/xiaogpt/bot/bard_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/bot/base_bot.py` & `xiaogpt-2.30/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-2.30/xiaogpt/bot/chatgptapi_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def _make_openai_client(self, sess: httpx.AsyncClient) -> openai.AsyncOpenAI:
         import openai
 
         if self.api_base and self.api_base.rstrip("/").endswith("openai.azure.com"):
             return openai.AsyncAzureOpenAI(
                 api_key=self.openai_key,
                 azure_endpoint=self.api_base,
-                api_version="2023-07-01-preview",
+                api_version="2024-02-15-preview",
                 azure_deployment=self.deployment_id,
                 http_client=sess,
             )
         else:
             return openai.AsyncOpenAI(
                 api_key=self.openai_key, http_client=sess, base_url=self.api_base
             )
```

### Comparing `xiaogpt-2.26/xiaogpt/bot/gemini_bot.py` & `xiaogpt-2.30/xiaogpt/bot/gemini_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/bot/glm_bot.py` & `xiaogpt-2.30/xiaogpt/bot/glm_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/bot/gpt3_bot.py` & `xiaogpt-2.30/xiaogpt/bot/gpt3_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/bot/langchain_bot.py` & `xiaogpt-2.30/xiaogpt/bot/langchain_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/bot/newbing_bot.py` & `xiaogpt-2.30/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/bot/qwen_bot.py` & `xiaogpt-2.30/xiaogpt/bot/qwen_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/cli.py` & `xiaogpt-2.30/xiaogpt/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,23 +86,37 @@
     parser.add_argument(
         "--verbose",
         dest="verbose",
         action="store_true",
         default=None,
         help="show info",
     )
+    parser.add_argument(
+        "--azure_tts_speech_key",
+        dest="azure_tts_speech_key",
+        help="if use azure tts",
+    )
+    parser.add_argument(
+        "--azure_tts_service_region",
+        dest="azure_tts_service_region",
+        help="if use azure tts",
+    )
     tts_group = parser.add_mutually_exclusive_group()
     tts_group.add_argument(
         "--enable_edge_tts",
         dest="tts",
         action="store_const",
         const="edge",
         help="if use edge tts",
     )
-    tts_group.add_argument("--tts", help="tts type", choices=["mi", "edge", "openai"])
+    tts_group.add_argument(
+        "--tts",
+        help="tts type",
+        choices=["mi", "edge", "openai", "azure"],
+    )
     bot_group = parser.add_mutually_exclusive_group()
     bot_group.add_argument(
         "--use_gpt3",
         dest="bot",
         action="store_const",
         const="gpt3",
         help="if use openai gpt3 api",
@@ -193,14 +207,17 @@
         dest="deployment_id",
         help="specify deployment id, only used when api_base points to azure",
     )
 
     options = parser.parse_args()
     if options.bot in ["bard"] and options.stream:
         raise Exception("For now Bard do not support stream")
+    if options.tts in ["edge", "openai", "azure"]:
+        print("Will close stream to better tts")
+        options.stream = False
     config = Config.from_options(options)
 
     miboy = MiGPT(config)
     loop = asyncio.get_event_loop()
     loop.run_until_complete(miboy.run_forever())
```

### Comparing `xiaogpt-2.26/xiaogpt/config.py` & `xiaogpt-2.30/xiaogpt/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -77,19 +77,21 @@
     api_base: str | None = None
     deployment_id: str | None = None
     use_command: bool = False
     verbose: bool = False
     start_conversation: str = "开始持续对话"
     end_conversation: str = "结束持续对话"
     stream: bool = False
-    tts: Literal["mi", "edge"] = "mi"
+    tts: Literal["mi", "edge", "azure", "openai"] = "mi"
     tts_voice: str | None = None
     gpt_options: dict[str, Any] = field(default_factory=dict)
     bing_cookie_path: str = ""
     bing_cookies: dict | None = None
+    azure_tts_speech_key: str | None = None
+    azure_tts_service_region: str = "eastasia"
 
     def __post_init__(self) -> None:
         if self.proxy:
             validate_proxy(self.proxy)
         if self.bot == "newbing":
             if not (self.bing_cookie_path or self.bing_cookies):
                 raise Exception(
@@ -106,14 +108,19 @@
                 "https://learn.microsoft.com/en-us/azure/cognitive-services/openai/how-to/chatgpt?pivots=programming-language-chat-completions"
             )
         if self.bot in ["chatgptapi", "gpt3"]:
             if not self.openai_key:
                 raise Exception(
                     "Using GPT api needs openai API key, please google how to"
                 )
+        if self.tts == "azure" and not self.azure_tts_speech_key:
+            raise Exception("Using Azure TTS needs azure speech key")
+        if self.tts in ["azure", "edge", "openai"]:
+            print("Will close stream when use tts: {self.tts} for better experience")
+            self.stream = False
 
     @property
     def tts_command(self) -> str:
         return HARDWARE_COMMAND_DICT.get(self.hardware, DEFAULT_COMMAND)[0]
 
     @property
     def wakeup_command(self) -> str:
```

### Comparing `xiaogpt-2.26/xiaogpt/langchain/callbacks.py` & `xiaogpt-2.30/xiaogpt/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/langchain/chain.py` & `xiaogpt-2.30/xiaogpt/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/langchain/examples/email/mail_box.py` & `xiaogpt-2.30/xiaogpt/langchain/examples/email/mail_box.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/langchain/examples/email/mail_summary_tools.py` & `xiaogpt-2.30/xiaogpt/langchain/examples/email/mail_summary_tools.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/tts/base.py` & `xiaogpt-2.30/xiaogpt/tts/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
             result = done.pop().result()
             if result is True:
                 # finished is set, break the loop
                 break
             else:
                 url, duration = result
-                logger.debug("Playing URL %s(%s seconds)", url, duration)
+                logger.debug("Playing URL %s (%s seconds)", url, duration)
                 await self.mina_service.play_by_url(self.device_id, url)
                 await self.wait_for_duration(duration)
         await task
 
     def _start_http_server(self):
         # set the port range
         port_range = range(8050, 8090)
```

### Comparing `xiaogpt-2.26/xiaogpt/tts/edge.py` & `xiaogpt-2.30/xiaogpt/tts/edge.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/tts/mi.py` & `xiaogpt-2.30/xiaogpt/tts/mi.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/tts/openai.py` & `xiaogpt-2.30/xiaogpt/tts/openai.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/utils.py` & `xiaogpt-2.30/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.26/xiaogpt/xiaogpt.py` & `xiaogpt-2.30/xiaogpt/xiaogpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from xiaogpt.config import (
     COOKIE_TEMPLATE,
     LATEST_ASK_API,
     MI_ASK_SIMULATE_DATA,
     WAKEUP_KEYWORD,
     Config,
 )
-from xiaogpt.tts import TTS, EdgeTTS, MiTTS
+from xiaogpt.tts import TTS, EdgeTTS, MiTTS, AzureTTS
 from xiaogpt.tts.openai import OpenAITTS
 from xiaogpt.utils import (
     parse_cookie_string,
 )
 
 EOF = object()
 
@@ -256,14 +256,16 @@
                 f"{self.config.tts_command} {value}",
             )
 
     @functools.cached_property
     def tts(self) -> TTS:
         if self.config.tts == "edge":
             return EdgeTTS(self.mina_service, self.device_id, self.config)
+        elif self.config.tts == "azure":
+            return AzureTTS(self.mina_service, self.device_id, self.config)
         elif self.config.tts == "openai":
             return OpenAITTS(self.mina_service, self.device_id, self.config)
         else:
             return MiTTS(self.mina_service, self.device_id, self.config)
 
     async def wait_for_tts_finish(self):
         while True:
```

### Comparing `xiaogpt-2.26/PKG-INFO` & `xiaogpt-2.30/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 2.26
+Version: 2.30
 Summary: Play ChatGPT or other LLM with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
 Requires-Python: >=3.9
 Requires-Dist: miservice_fork
 Requires-Dist: openai>=1
 Requires-Dist: aiohttp
 Requires-Dist: rich
 Requires-Dist: zhipuai==2.0.1
+Requires-Dist: httpx==0.24.1
 Requires-Dist: bardapi
 Requires-Dist: edge-tts>=6.1.3
 Requires-Dist: EdgeGPT==0.1.26
 Requires-Dist: langchain>=0.0.343
 Requires-Dist: beautifulsoup4>=4.12.0
 Requires-Dist: google-search-results>=2.4.2
 Requires-Dist: google-generativeai
 Requires-Dist: numexpr>=2.8.6
 Requires-Dist: dashscope==1.10.0
+Requires-Dist: httpcore==0.15.0
+Requires-Dist: azure-cognitiveservices-speech>=1.37.0
 Description-Content-Type: text/markdown
 
 # xiaogpt
 
 [![PyPI](https://img.shields.io/pypi/v/xiaogpt?style=flat-square)](https://pypi.org/project/xiaogpt)
 [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/yihong0618/xiaogpt?color=%23086DCD&label=docker%20image)](https://hub.docker.com/r/yihong0618/xiaogpt)
 
@@ -43,23 +46,41 @@
 - ChatGPT
 - New Bing
 - [ChatGLM](http://open.bigmodel.cn/)
 - [Gemini](https://makersuite.google.com/app/apikey)
 - [Bard](https://github.com/dsdanielpark/Bard-API)
 - [通义千问](https://help.aliyun.com/zh/dashscope/developer-reference/api-details)
 
-## Windows 获取小米音响DID
-
-1. `pip install miservice_fork`
-2. `set MI_USER=xxxx`
-3. `set MI_PASS=xxx`
-4. `micli list` 得到did
-5. `set MI_DID=xxxx`
+## 获取小米音响DID
+### Windows(使用 set 设置环境变量）
+```cmd
+pip install miservice_fork
+set MI_USER=xxxx
+set MI_PASS=xxx
+micli list 得到did
+set MI_DID=xxxx
+```
 
 - 如果获取did报错时，请更换一下无线网络，有很大概率解决问题。
+ 
+### Linux(使用 export 设置环境变量）
+```sh
+# 1、安装模块
+pip install miservice_fork
+
+# 2、设置环境用户参数
+export MI_USER=xxxx
+export MI_PASS=xxx
+
+# 3、使用micli list 得到did
+micli list
+
+# 4、根据did设置环境DID参数
+export MI_DID=xxxx
+```
 
 ## 一点原理
 
 [不用 root 使用小爱同学和 ChatGPT 交互折腾记](https://github.com/yihong0618/gitblog/issues/258)
 
 ## 准备
 
@@ -81,14 +102,15 @@
 - 如果有能力可以自行替换唤醒词，也可以去掉唤醒词
 - 使用 `--use_chatgpt_api` 的 api 那样可以更流畅的对话，速度特别快，达到了对话的体验, [openai api](https://platform.openai.com/account/api-keys), 命令 `--use_chatgpt_api`
 - 使用 gpt-3 的 api 那样可以更流畅的对话，速度快, 请 google 如何用 [openai api](https://platform.openai.com/account/api-keys) 命令 --use_gpt3
 - 如果你遇到了墙需要用 Cloudflare Workers 替换 api_base 请使用 `--api_base ${url}` 来替换。 **请注意，此处你输入的api应该是'`https://xxxx/v1`'的字样，域名需要用引号包裹**
 - 可以跟小爱说 `开始持续对话` 自动进入持续对话状态，`结束持续对话` 结束持续对话状态。
 - 可以使用 `--tts edge` 来获取更好的 tts 能力
 - 可以使用 `--tts openai` 来获取 openai tts 能力
+- 可以使用 `--tts azure --azure_tts_speech_key <your-speech-key>` 来获取 Azure TTS 能力
 - 可以使用 `--use_langchain` 替代 `--use_chatgpt_api` 来调用 LangChain（默认 chatgpt）服务，实现上网检索、数学运算..
 
 e.g.
 
 ```shell
 export OPENAI_API_KEY=${your_api_key}
 xiaogpt --hardware LX06 --use_chatgpt_api
@@ -179,45 +201,47 @@
 
 具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
 ChatGLM [文档](http://open.bigmodel.cn/doc/api#chatglm_130b)
 Bard-API [参考](https://github.com/dsdanielpark/Bard-API)
 
 ## 配置项说明
 
-| 参数                  | 说明                                                                    | 默认值                                                                                                    |可选值            |
-| --------------------- | ----------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------- |
-| hardware              | 设备型号                                                                |                                                                                                           |
-| account               | 小爱账户                                                                |                                                                                                           |
-| password              | 小爱账户密码                                                            |                                                                                                           |
-| openai_key            | openai的apikey                                                          |                                                                                                           |
-| serpapi_api_key       | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                       |                                                                                                           |
-| glm_key               | chatglm 的 apikey                                                       |                                                                                                           |
-| gemini_key            | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                                                      |                                                                                                           |
-| qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details)                                                      |                                                                                                           |
-| bard_token            | bard 的 token 参考 [Bard-API](https://github.com/dsdanielpark/Bard-API) |                                                                                                           |
-| cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                             |                                                                                                           |
-| mi_did                | 设备did                                                                 |                                                                                                           |
-| use_command           | 使用 MI command 与小爱交互                                              | `false`                                                                                                   |
-| mute_xiaoai           | 快速停掉小爱自己的回答                                                  | `true`                                                                                                    |
-| verbose               | 是否打印详细日志                                                        | `false`                                                                                                   |
-| bot                   | 使用的 bot 类型，目前支持gpt3,chatgptapi和newbing                       | `chatgptapi`                                                                                              |
-| tts                   | 使用的 TTS 类型                                                         | `mi`                                                                                                      | `edge`、 `openai` | 
-| tts_voice             | TTS 的嗓音                                                              | `zh-CN-XiaoxiaoNeural`(edge), `alloy`(openai)                                                             |
-| prompt                | 自定义prompt                                                            | `请用100字以内回答`                                                                                       |
-| keyword               | 自定义请求词列表                                                        | `["请"]`                                                                                                  |
-| change_prompt_keyword | 更改提示词触发列表                                                      | `["更改提示词"]`                                                                                          |
-| start_conversation    | 开始持续对话关键词                                                      | `开始持续对话`                                                                                            |
-| end_conversation      | 结束持续对话关键词                                                      | `结束持续对话`                                                                                            |
-| stream                | 使用流式响应，获得更快的响应                                            | `false`                                                                                                   |
-| proxy                 | 支持 HTTP 代理，传入 http proxy URL                                     | ""                                                                                                        |
-| gpt_options           | OpenAI API 的参数字典                                                   | `{}`                                                                                                      |
-| bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取                                 | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |
-| bing_cookies          | NewBing使用的cookie字典，参考[这里]获取                                 |                                                                                                           |
-| deployment_id         | Azure OpenAI 服务的 deployment ID                                       | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |
-| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                         | 例如：`https://abc-def.openai.azure.com/`                                                                 |
+| 参数                     | 说明                                                                                        | 默认值                                                                                                    | 可选值                                                                                                                     |
+| ------------------------ | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
+| hardware                 | 设备型号                                                                                    |                                                                                                           |                                                                                                                            |
+| account                  | 小爱账户                                                                                    |                                                                                                           |                                                                                                                            |
+| password                 | 小爱账户密码                                                                                |                                                                                                           |                                                                                                                            |
+| openai_key               | openai的apikey                                                                              |                                                                                                           |                                                                                                                            |
+| serpapi_api_key          | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                           |                                                                                                           |                                                                                                                            |
+| glm_key                  | chatglm 的 apikey                                                                           |                                                                                                           |                                                                                                                            |
+| gemini_key               | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                                                                                            |
+| qwen_key                 | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                                                                                            |
+| bard_token               | bard 的 token 参考 [Bard-API](https://github.com/dsdanielpark/Bard-API)                     |                                                                                                           |                                                                                                                            |
+| cookie                   | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                                                                                            |
+| mi_did                   | 设备did                                                                                     |                                                                                                           |                                                                                                                            |
+| use_command              | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                                                                                            |
+| mute_xiaoai              | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                                                                                            |
+| verbose                  | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                                                                                            |
+| bot                      | 使用的 bot 类型，目前支持gpt3,chatgptapi和newbing                                           | `chatgptapi`                                                                                              |                                                                                                                            |
+| tts                      | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`                                                                                                 |
+| tts_voice                | TTS 的嗓音                                                                                  | `zh-CN-XiaoxiaoNeural`(edge), `alloy`(openai), `zh-CN-XiaoxiaoMultilingualNeural`(azure)                  |                                                                                                                            |
+| prompt                   | 自定义prompt                                                                                | `请用100字以内回答`                                                                                       |                                                                                                                            |
+| keyword                  | 自定义请求词列表                                                                            | `["请"]`                                                                                                  |                                                                                                                            |
+| change_prompt_keyword    | 更改提示词触发列表                                                                          | `["更改提示词"]`                                                                                          |                                                                                                                            |
+| start_conversation       | 开始持续对话关键词                                                                          | `开始持续对话`                                                                                            |                                                                                                                            |
+| end_conversation         | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                                                                                            |
+| stream                   | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                                                                                            |
+| proxy                    | 支持 HTTP 代理，传入 http proxy URL                                                         | ""                                                                                                        |                                                                                                                            |
+| gpt_options              | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                                                                                            |
+| bing_cookie_path         | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                                                                                            |
+| bing_cookies             | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                                                                                            |
+| deployment_id            | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                                                                                            |
+| api_base                 | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |                                                                                                                            |
+| azure_tts_speech_key     | Azure TTS key                                                                               | null                                                                                                      |                                                                                                                            |
+| azure_tts_service_region | Azure TTS 服务地区                                                                          | `eastasia`                                                                                                | [Regions - Speech service - Azure AI services](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/regions) |
 
 [这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
@@ -260,14 +284,20 @@
 
 xiaogpt的配置文件可通过指定volume /config，以及指定参数--config来处理，如
 
 ```shell
 docker run -v <your-config-dir>:/config yihong0618/xiaogpt --config=/config/config.json
 ```
 
+### 网络使用 host 模型
+
+```shell
+docker run -v <your-config-dir>:/config --network=host yihong0618/xiaogpt --config=/config/config.json
+```
+
 ### 本地编译Docker Image
 
 ```shell
  docker build -t xiaogpt .
 ```
 
 如果在安装依赖时构建失败或安装缓慢时，可以在构建 Docker 镜像时使用 `--build-arg` 参数来指定国内源地址：
```

