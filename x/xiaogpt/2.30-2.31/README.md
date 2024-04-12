# Comparing `tmp/xiaogpt-2.30.tar.gz` & `tmp/xiaogpt-2.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-2.30.tar", last modified: Fri Apr 12 15:00:41 2024, max compression
+gzip compressed data, was "xiaogpt-2.31.tar", last modified: Fri Apr 12 15:05:11 2024, max compression
```

## Comparing `xiaogpt-2.30.tar` & `xiaogpt-2.31.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1063 2024-04-12 15:00:36.164055 xiaogpt-2.30/LICENSE
--rw-r--r--   0        0        0    23688 2024-04-12 15:00:36.164055 xiaogpt-2.30/README.md
--rw-r--r--   0        0        0     1263 2024-04-12 15:00:41.880149 xiaogpt-2.30/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/__main__.py
--rw-r--r--   0        0        0     1073 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0      840 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/bard_bot.py
--rw-r--r--   0        0        0     1467 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3656 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1840 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/gemini_bot.py
--rw-r--r--   0        0        0     1825 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     2781 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/gpt3_bot.py
--rw-r--r--   0        0        0     1944 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/langchain_bot.py
--rw-r--r--   0        0        0     2289 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3657 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/bot/qwen_bot.py
--rw-r--r--   0        0        0     5506 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/cli.py
--rw-r--r--   0        0        0     6703 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/config.py
--rw-r--r--   0        0        0     2616 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/langchain/callbacks.py
--rw-r--r--   0        0        0     1495 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/langchain/chain.py
--rw-r--r--   0        0        0     6372 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/langchain/examples/email/mail_box.py
--rw-r--r--   0        0        0     1561 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/langchain/examples/email/mail_summary_tools.py
--rw-r--r--   0        0        0      220 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/tts/__init__.py
--rw-r--r--   0        0        0     3978 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/tts/azure.py
--rw-r--r--   0        0        0     4923 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/tts/base.py
--rw-r--r--   0        0        0     1172 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/tts/edge.py
--rw-r--r--   0        0        0     1096 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/tts/mi.py
--rw-r--r--   0        0        0     1533 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/tts/openai.py
--rw-r--r--   0        0        0     2072 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/utils.py
--rw-r--r--   0        0        0    15400 2024-04-12 15:00:36.168055 xiaogpt-2.30/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    24670 1970-01-01 00:00:00.000000 xiaogpt-2.30/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-12 15:05:01.292487 xiaogpt-2.31/LICENSE
+-rw-r--r--   0        0        0    23688 2024-04-12 15:05:01.292487 xiaogpt-2.31/README.md
+-rw-r--r--   0        0        0     1280 2024-04-12 15:05:11.808405 xiaogpt-2.31/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/__main__.py
+-rw-r--r--   0        0        0     1073 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0      840 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/bard_bot.py
+-rw-r--r--   0        0        0     1467 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3656 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1840 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/gemini_bot.py
+-rw-r--r--   0        0        0     1825 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     2781 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/gpt3_bot.py
+-rw-r--r--   0        0        0     1944 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/langchain_bot.py
+-rw-r--r--   0        0        0     2289 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3657 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/qwen_bot.py
+-rw-r--r--   0        0        0     5506 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/cli.py
+-rw-r--r--   0        0        0     6703 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/config.py
+-rw-r--r--   0        0        0     2616 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/langchain/callbacks.py
+-rw-r--r--   0        0        0     1495 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/langchain/chain.py
+-rw-r--r--   0        0        0     6372 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/langchain/examples/email/mail_box.py
+-rw-r--r--   0        0        0     1561 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/langchain/examples/email/mail_summary_tools.py
+-rw-r--r--   0        0        0      220 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/tts/__init__.py
+-rw-r--r--   0        0        0     3978 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/tts/azure.py
+-rw-r--r--   0        0        0     4923 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/tts/base.py
+-rw-r--r--   0        0        0     1172 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/tts/edge.py
+-rw-r--r--   0        0        0     1096 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/tts/mi.py
+-rw-r--r--   0        0        0     1533 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/tts/openai.py
+-rw-r--r--   0        0        0     2072 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/utils.py
+-rw-r--r--   0        0        0    15400 2024-04-12 15:05:01.296487 xiaogpt-2.31/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    24695 1970-01-01 00:00:00.000000 xiaogpt-2.31/PKG-INFO
```

### Comparing `xiaogpt-2.30/LICENSE` & `xiaogpt-2.31/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/README.md` & `xiaogpt-2.31/README.md`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/pyproject.toml` & `xiaogpt-2.31/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,19 @@
     "langchain>=0.0.343",
     "beautifulsoup4>=4.12.0",
     "google-search-results>=2.4.2",
     "google-generativeai",
     "numexpr>=2.8.6",
     "dashscope==1.10.0",
     "httpcore==0.15.0",
+    "idna==3.7",
     "azure-cognitiveservices-speech>=1.37.0",
 ]
 dynamic = []
-version = "2.30"
+version = "2.31"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
```

### Comparing `xiaogpt-2.30/xiaogpt/bot/__init__.py` & `xiaogpt-2.31/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/bot/bard_bot.py` & `xiaogpt-2.31/xiaogpt/bot/bard_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/bot/base_bot.py` & `xiaogpt-2.31/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-2.31/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/bot/gemini_bot.py` & `xiaogpt-2.31/xiaogpt/bot/gemini_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/bot/glm_bot.py` & `xiaogpt-2.31/xiaogpt/bot/glm_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/bot/gpt3_bot.py` & `xiaogpt-2.31/xiaogpt/bot/gpt3_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/bot/langchain_bot.py` & `xiaogpt-2.31/xiaogpt/bot/langchain_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/bot/newbing_bot.py` & `xiaogpt-2.31/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/bot/qwen_bot.py` & `xiaogpt-2.31/xiaogpt/bot/qwen_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/cli.py` & `xiaogpt-2.31/xiaogpt/cli.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/config.py` & `xiaogpt-2.31/xiaogpt/config.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/langchain/callbacks.py` & `xiaogpt-2.31/xiaogpt/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/langchain/chain.py` & `xiaogpt-2.31/xiaogpt/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/langchain/examples/email/mail_box.py` & `xiaogpt-2.31/xiaogpt/langchain/examples/email/mail_box.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/langchain/examples/email/mail_summary_tools.py` & `xiaogpt-2.31/xiaogpt/langchain/examples/email/mail_summary_tools.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/tts/azure.py` & `xiaogpt-2.31/xiaogpt/tts/azure.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/tts/base.py` & `xiaogpt-2.31/xiaogpt/tts/base.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/tts/edge.py` & `xiaogpt-2.31/xiaogpt/tts/edge.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/tts/mi.py` & `xiaogpt-2.31/xiaogpt/tts/mi.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/tts/openai.py` & `xiaogpt-2.31/xiaogpt/tts/openai.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/utils.py` & `xiaogpt-2.31/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/xiaogpt/xiaogpt.py` & `xiaogpt-2.31/xiaogpt/xiaogpt.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.30/PKG-INFO` & `xiaogpt-2.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 2.30
+Version: 2.31
 Summary: Play ChatGPT or other LLM with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
@@ -21,14 +21,15 @@
 Requires-Dist: langchain>=0.0.343
 Requires-Dist: beautifulsoup4>=4.12.0
 Requires-Dist: google-search-results>=2.4.2
 Requires-Dist: google-generativeai
 Requires-Dist: numexpr>=2.8.6
 Requires-Dist: dashscope==1.10.0
 Requires-Dist: httpcore==0.15.0
+Requires-Dist: idna==3.7
 Requires-Dist: azure-cognitiveservices-speech>=1.37.0
 Description-Content-Type: text/markdown
 
 # xiaogpt
 
 [![PyPI](https://img.shields.io/pypi/v/xiaogpt?style=flat-square)](https://pypi.org/project/xiaogpt)
 [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/yihong0618/xiaogpt?color=%23086DCD&label=docker%20image)](https://hub.docker.com/r/yihong0618/xiaogpt)
```

