# Comparing `tmp/minimax_client-0.5.0.tar.gz` & `tmp/minimax_client-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minimax_client-0.5.0.tar", last modified: Sun Mar 31 06:10:31 2024, max compression
+gzip compressed data, was "minimax_client-0.5.1.tar", last modified: Fri Apr 12 06:10:14 2024, max compression
```

## Comparing `minimax_client-0.5.0.tar` & `minimax_client-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1067 2024-03-06 16:00:11.906782 minimax_client-0.5.0/LICENSE.md
--rw-r--r--   0        0        0     7789 2024-03-31 06:06:02.099730 minimax_client-0.5.0/README.md
--rw-r--r--   0        0        0     2337 2024-03-31 06:10:31.272395 minimax_client-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       75 2024-03-14 12:30:34.748231 minimax_client-0.5.0/src/minimax_client/__init__.py
--rw-r--r--   0        0        0       44 2024-03-31 06:10:14.692121 minimax_client-0.5.0/src/minimax_client/__version__.py
--rw-r--r--   0        0        0     5575 2024-03-31 05:20:00.545121 minimax_client-0.5.0/src/minimax_client/client.py
--rw-r--r--   0        0        0        0 2024-03-14 12:30:34.748231 minimax_client-0.5.0/src/minimax_client/entities/__init__.py
--rw-r--r--   0        0        0     1620 2024-03-31 05:43:30.509689 minimax_client-0.5.0/src/minimax_client/entities/assistant.py
--rw-r--r--   0        0        0     1375 2024-03-27 15:27:03.253803 minimax_client-0.5.0/src/minimax_client/entities/chat_completion.py
--rw-r--r--   0        0        0      622 2024-03-27 15:27:03.253803 minimax_client-0.5.0/src/minimax_client/entities/common.py
--rw-r--r--   0        0        0      274 2024-03-27 15:27:03.253803 minimax_client-0.5.0/src/minimax_client/entities/embedding.py
--rw-r--r--   0        0        0     1087 2024-03-27 15:27:03.253803 minimax_client-0.5.0/src/minimax_client/entities/file.py
--rw-r--r--   0        0        0     1874 2024-03-27 15:27:03.253803 minimax_client-0.5.0/src/minimax_client/entities/fine_tuning.py
--rw-r--r--   0        0        0        0 2024-03-14 12:30:34.748231 minimax_client-0.5.0/src/minimax_client/interfaces/__init__.py
--rw-r--r--   0        0        0    15755 2024-03-31 05:58:45.886554 minimax_client-0.5.0/src/minimax_client/interfaces/assistant.py
--rw-r--r--   0        0        0      505 2024-03-24 13:14:28.460715 minimax_client-0.5.0/src/minimax_client/interfaces/base.py
--rw-r--r--   0        0        0     8593 2024-03-26 15:09:08.468225 minimax_client-0.5.0/src/minimax_client/interfaces/chat_completion.py
--rw-r--r--   0        0        0     3066 2024-03-26 15:09:08.468225 minimax_client-0.5.0/src/minimax_client/interfaces/embedding.py
--rw-r--r--   0        0        0     7877 2024-03-26 15:09:08.468225 minimax_client-0.5.0/src/minimax_client/interfaces/file.py
--rw-r--r--   0        0        0    11977 2024-03-27 15:27:03.253803 minimax_client-0.5.0/src/minimax_client/interfaces/fine_tuning.py
--rw-r--r--   0        0        0        0 2024-03-06 16:00:11.906782 minimax_client-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     2352 2024-03-26 15:09:08.472226 minimax_client-0.5.0/tests/test_client.py
--rw-r--r--   0        0        0     9229 1970-01-01 00:00:00.000000 minimax_client-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-03-06 04:02:14.299362 minimax_client-0.5.1/LICENSE.md
+-rw-r--r--   0        0        0     9018 2024-04-12 05:59:17.131453 minimax_client-0.5.1/README.md
+-rw-r--r--   0        0        0     2337 2024-04-12 06:10:14.882860 minimax_client-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-03-13 04:59:39.590202 minimax_client-0.5.1/src/minimax_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-12 06:09:39.998660 minimax_client-0.5.1/src/minimax_client/__version__.py
+-rw-r--r--   0        0        0     5749 2024-04-01 07:19:59.583999 minimax_client-0.5.1/src/minimax_client/client.py
+-rw-r--r--   0        0        0        0 2024-03-12 08:42:19.334547 minimax_client-0.5.1/src/minimax_client/entities/__init__.py
+-rw-r--r--   0        0        0     2623 2024-04-12 05:40:39.242177 minimax_client-0.5.1/src/minimax_client/entities/assistant.py
+-rw-r--r--   0        0        0     1431 2024-03-27 06:52:42.426086 minimax_client-0.5.1/src/minimax_client/entities/chat_completion.py
+-rw-r--r--   0        0        0      651 2024-03-26 08:25:32.233150 minimax_client-0.5.1/src/minimax_client/entities/common.py
+-rw-r--r--   0        0        0      288 2024-03-27 06:51:31.873794 minimax_client-0.5.1/src/minimax_client/entities/embedding.py
+-rw-r--r--   0        0        0     1144 2024-03-27 06:50:23.603022 minimax_client-0.5.1/src/minimax_client/entities/file.py
+-rw-r--r--   0        0        0     1956 2024-03-27 09:21:05.226495 minimax_client-0.5.1/src/minimax_client/entities/fine_tuning.py
+-rw-r--r--   0        0        0        0 2024-03-12 08:49:51.948241 minimax_client-0.5.1/src/minimax_client/interfaces/__init__.py
+-rw-r--r--   0        0        0    23479 2024-04-12 05:59:39.461781 minimax_client-0.5.1/src/minimax_client/interfaces/assistant.py
+-rw-r--r--   0        0        0      532 2024-03-15 09:50:38.059327 minimax_client-0.5.1/src/minimax_client/interfaces/base.py
+-rw-r--r--   0        0        0     8832 2024-03-21 09:50:23.229159 minimax_client-0.5.1/src/minimax_client/interfaces/chat_completion.py
+-rw-r--r--   0        0        0     3168 2024-03-21 09:42:08.928420 minimax_client-0.5.1/src/minimax_client/interfaces/embedding.py
+-rw-r--r--   0        0        0     8150 2024-03-27 06:44:53.186708 minimax_client-0.5.1/src/minimax_client/interfaces/file.py
+-rw-r--r--   0        0        0    12362 2024-03-27 07:04:43.648435 minimax_client-0.5.1/src/minimax_client/interfaces/fine_tuning.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:45:59.529113 minimax_client-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0     2412 2024-03-25 11:51:29.057995 minimax_client-0.5.1/tests/test_client.py
+-rw-r--r--   0        0        0    10094 1970-01-01 00:00:00.000000 minimax_client-0.5.1/PKG-INFO
```

### Comparing `minimax_client-0.5.0/LICENSE.md` & `minimax_client-0.5.1/LICENSE.md`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-MIT License
-
-Copyright (c) 2024 Zeyang Lin
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Zeyang Lin
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `minimax_client-0.5.0/README.md` & `minimax_client-0.5.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,331 +1,364 @@
-# MiniMax Python Client
-
-[![PyPI version](https://img.shields.io/pypi/v/minimax-client.svg)](https://pypi.org/project/minimax-client/)
-[![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json)](https://pydantic.dev)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm-project.org)
-[![License](https://img.shields.io/pypi/l/minimax-client.svg)](https://pypi.org/project/minimax-client)
-[![python-versions](https://img.shields.io/pypi/pyversions/minimax-client.svg)](https://pypi.org/project/minimax-client)
-[![Main Workflow](https://github.com/linzeyang/minimax-python-client/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/linzeyang/minimax-python-client/actions/workflows/main.yml)
-
-An (unofficial) python native client for easy interaction with [MiniMax Open Platform](https://www.minimaxi.com/platform)
-
-The current implementation includes the following official APIs offered by MiniMax:
-- ChatCompletion v2
-- Embeddings
-- File
-- Finetune
-- Assistants
-
-## Prerequisites
-- Python >= 3.8
-- pip (or any other tool that does the same job)
-- Internet connection
-- An API KEY acquired from [MiniMax Open Platform](https://www.minimaxi.com/user-center/basic-information/interface-key)
-
-## Quick Start
-
-### 1. Install the package
-
-```bash
-pip install minimax-client
-```
-
-### 2. Import the package and invoke the client
-
-#### 2.1 Sync call
-
-```python
-from minimax_client import MiniMax
-
-
-client = MiniMax(api_key="<YOUR_API_KEY>")
-
-
-response = client.chat.completions.create(
-    messages=[
-        {
-            "role": "user",
-            "content": "1 + 1 equals: ",
-        }
-    ]
-)
-
-
-print(response.choices[0].message.content)
-```
-
-#### 2.2 Sync call with streaming
-
-```python
-from minimax_client import MiniMax
-
-
-client = MiniMax(api_key="<YOUR_API_KEY>")
-
-
-stream = client.chat.completions.create(
-    messages=[
-        {
-            "role": "user",
-            "content": "What is the term GPT short for?",
-        }
-    ],
-    stream=True,
-)
-
-
-for chunk in stream:
-    print(chunk.choices[0].delta.content if chunk.choices[0].delta else "", end="")
-```
-
-#### 2.3 Sync call with tools, stream enabled
-
-```python
-from minimax_client import MiniMax
-
-
-client = MiniMax(api_key="<YOUR_API_KEY>")
-
-
-stream = client.chat.completions.create(
-    model="abab5.5-chat",
-    messages=[
-        {
-            "role": "system",
-            "content": "You are a helpful assistant",
-        },
-        {
-            "role": "user",
-            "content": "What's the weather like in Log Angeles right now?",
-        },
-        {
-            "role": "assistant",
-            "tool_calls": [
-                {
-                    "id": "call_function_2936815621",
-                    "type": "function",
-                    "function": {
-                        "name": "get_current_weather",
-                        "arguments": '{"location": "LogAngeles"}',
-                    },
-                }
-            ],
-        },
-        {
-            "role": "tool",
-            "tool_call_id": "call_function_2936815621",
-            "content": "LogAngeles / Sunny / 51°F / Wind: East 5 mph",
-        },
-    ],
-    stream=True,
-    tool_choice="auto",
-    tools=[
-        {
-            "type": "function",
-            "function": {
-                "name": "get_current_weather",
-                "description": "Retrieve the current weather of given location",
-                "parameters": '{"type": "object", "properties": {"location": {"type": "string", "description": "Name of a city, eg. Paris, London"}}, "required": ["location"]}',
-            },
-        }
-    ],
-)
-
-for chunk in stream:
-    print(chunk.choices[0].delta.content if chunk.choices[0].delta else "", end="")
-
-# It's currently sunny in Log Angeles, with a temperature of 51°F and wind from the east at 5 mph.
-```
-
-
-#### 2.4 Async call
-
-```python
-import asyncio
-
-from minimax_client import AsyncMiniMax
-
-
-async def demo():
-    client = AsyncMiniMax(api_key="<YOUR_API_KEY>")
-
-    response = await client.chat.completions.create(
-        messages=[
-            {
-                "role": "user",
-                "content": "1 + 1 equals: ",
-            }
-        ]
-    )
-
-    print(response.choices[0].message.content)
-
-
-asyncio.run(demo())
-```
-
-#### 2.5 Async call with streaming
-
-```python
-import asyncio
-
-from minimax_client import AsyncMiniMax
-
-
-async def demo():
-    client = AsyncMiniMax(api_key="<YOUR_API_KEY>")
-
-    stream = await client.chat.completions.create(
-        messages=[
-            {
-                "role": "user",
-                "content": "What is the term GPT short for?",
-            }
-        ],
-        stream=True,
-    )
-
-    async for chunk in stream:
-        print(chunk.choices[0].delta.content if chunk.choices[0].delta else "", end="")
-
-
-asyncio.run(demo())
-```
-
-#### 2.6 Sync call for embeddings
-
-```python
-from minimax_client import MiniMax
-
-
-client = MiniMax(api_key="<YOUR_API_KEY>")
-
-
-response = client.embeddings.create(
-    input=["Hello world!", "Nice to meet you!"],
-    target="db",
-)
-
-print(response.vectors[0][:10])
-print(response.vectors[1][:10])
-```
-
-#### 2.7 Async call for embeddings
-
-```python
-import asyncio
-
-from minimax_client import AsyncMiniMax
-
-
-async def demo():
-    client = AsyncMiniMax(api_key="<YOUR_API_KEY>")
-
-    response = await client.embeddings.create(
-        input=["Hello async world!", "Nice to meet you async!"],
-        target="query",
-    )
-
-    print(response.vectors[0][:10])
-    print(response.vectors[1][:10])
-
-
-asyncio.run(demo())
-```
-
-#### 2.8 Sync call for files
-
-```python
-from minimax_client import MiniMax
-
-
-client = MiniMax(api_key="<YOUR_API_KEY>")
-
-
-resp = client.files.create(filepath="sample.txt", purpose="retrieval")
-print(resp.file.file_id)
-
-resp = client.files.list(purpose="retrieval")
-print(resp.files[0].file_id)
-
-resp = client.files.retrieve(file_id=resp.files[0].file_id)
-print(resp.file.bytes)
-
-resp = client.files.delete(file_id=resp.file.file_id)
-print(resp.file_id)
-```
-
-#### 2.9 Async call for files
-
-```python
-import asyncio
-
-from minimax_client import AsyncMiniMax
-
-
-async def demo():
-    client = AsyncMiniMax(api_key="<YOUR_API_KEY>")
-
-    resp = await client.files.create(filepath="sample.txt", purpose="retrieval")
-    print(resp.file.file_id)
-
-    resp = await client.files.list(purpose="retrieval")
-    print(resp.files[0].file_id)
-
-    resp = await client.files.retrieve(file_id=resp.files[0].file_id)
-    print(resp.file.bytes)
-
-    resp = await client.files.delete(file_id=resp.file.file_id)
-    print(resp.file_id)
-
-asyncio.run(demo())
-```
-
-#### 2.10 Sync call for files
-
-```python
-from minimax_client import MiniMax
-
-
-client = MiniMax(api_key="<YOUR_API_KEY>")
-
-resp = client.fine_tuning.jobs.create(
-    model="abab5.5s-chat-240123", training_file=..., suffix="test"
-)
-print(resp.id)
-print(resp.fine_tuned_model)
-
-resp = client.fine_tuning.jobs.list(limit=5)
-print(resp.job_list[0])
-
-resp = client.model.list()
-print(resp.model_list[0])
-
-resp = client.model.retrieve(model="ft:abab5.5s-chat-240123_XXXXXXXXXXXXX:test")
-print(resp.model.id)
-```
-
-#### 2.11 Sync call for assistants
-
-```python
-from minimax_client import MiniMax
-
-
-client = MiniMax(api_key="<YOUR_API_KEY>")
-
-resp = client.assistants.create(model="abab5.5s-chat-240123")
-
-client.assistants.update(
-    assistant_id=resp.id,
-    model="abab5.5s-chat-240123",
-    name="test-assistant",
-    instructions="You are a helpful assistant.",
-)
-
-client.assistants.retrieve(assistant_id=resp.id)
-
-client.assistants.list(limit=5)
-
-client.assistants.delete(assistant_id=resp.id)
-```
+# MiniMax Python Client
+
+[![PyPI version](https://img.shields.io/pypi/v/minimax-client.svg)](https://pypi.org/project/minimax-client/)
+[![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json)](https://pydantic.dev)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm-project.org)
+[![License](https://img.shields.io/pypi/l/minimax-client.svg)](https://pypi.org/project/minimax-client)
+[![python-versions](https://img.shields.io/pypi/pyversions/minimax-client.svg)](https://pypi.org/project/minimax-client)
+[![Main Workflow](https://github.com/linzeyang/minimax-python-client/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/linzeyang/minimax-python-client/actions/workflows/main.yml)
+
+An (unofficial) python native client for easy interaction with [MiniMax Open Platform](https://www.minimaxi.com/platform)
+
+The current implementation includes the following official APIs offered by MiniMax:
+- ChatCompletion v2
+- Embeddings
+- File
+- Finetune
+- Assistants
+    - Assistant
+    - Assistant File
+
+## Prerequisites
+- Python >= 3.8
+- pip (or any other tool that does the same job)
+- Internet connection
+- An API KEY acquired from [MiniMax Open Platform](https://www.minimaxi.com/user-center/basic-information/interface-key)
+
+## Quick Start
+
+### 1. Install the package
+
+```bash
+pip install minimax-client
+```
+
+### 2. Import the package and invoke the client
+
+#### 2.1 Sync call
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+
+response = client.chat.completions.create(
+    messages=[
+        {
+            "role": "user",
+            "content": "1 + 1 equals: ",
+        }
+    ]
+)
+
+
+print(response.choices[0].message.content)
+```
+
+#### 2.2 Sync call with streaming
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+
+stream = client.chat.completions.create(
+    messages=[
+        {
+            "role": "user",
+            "content": "What is the term GPT short for?",
+        }
+    ],
+    stream=True,
+)
+
+
+for chunk in stream:
+    print(chunk.choices[0].delta.content if chunk.choices[0].delta else "", end="")
+```
+
+#### 2.3 Sync call with tools, stream enabled
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+
+stream = client.chat.completions.create(
+    model="abab5.5-chat",
+    messages=[
+        {
+            "role": "system",
+            "content": "You are a helpful assistant",
+        },
+        {
+            "role": "user",
+            "content": "What's the weather like in Log Angeles right now?",
+        },
+        {
+            "role": "assistant",
+            "tool_calls": [
+                {
+                    "id": "call_function_2936815621",
+                    "type": "function",
+                    "function": {
+                        "name": "get_current_weather",
+                        "arguments": '{"location": "LogAngeles"}',
+                    },
+                }
+            ],
+        },
+        {
+            "role": "tool",
+            "tool_call_id": "call_function_2936815621",
+            "content": "LogAngeles / Sunny / 51°F / Wind: East 5 mph",
+        },
+    ],
+    stream=True,
+    tool_choice="auto",
+    tools=[
+        {
+            "type": "function",
+            "function": {
+                "name": "get_current_weather",
+                "description": "Retrieve the current weather of given location",
+                "parameters": '{"type": "object", "properties": {"location": {"type": "string", "description": "Name of a city, eg. Paris, London"}}, "required": ["location"]}',
+            },
+        }
+    ],
+)
+
+for chunk in stream:
+    print(chunk.choices[0].delta.content if chunk.choices[0].delta else "", end="")
+
+# It's currently sunny in Log Angeles, with a temperature of 51°F and wind from the east at 5 mph.
+```
+
+
+#### 2.4 Async call
+
+```python
+import asyncio
+
+from minimax_client import AsyncMiniMax
+
+
+async def demo():
+    client = AsyncMiniMax(api_key="<YOUR_API_KEY>")
+
+    response = await client.chat.completions.create(
+        messages=[
+            {
+                "role": "user",
+                "content": "1 + 1 equals: ",
+            }
+        ]
+    )
+
+    print(response.choices[0].message.content)
+
+
+asyncio.run(demo())
+```
+
+#### 2.5 Async call with streaming
+
+```python
+import asyncio
+
+from minimax_client import AsyncMiniMax
+
+
+async def demo():
+    client = AsyncMiniMax(api_key="<YOUR_API_KEY>")
+
+    stream = await client.chat.completions.create(
+        messages=[
+            {
+                "role": "user",
+                "content": "What is the term GPT short for?",
+            }
+        ],
+        stream=True,
+    )
+
+    async for chunk in stream:
+        print(chunk.choices[0].delta.content if chunk.choices[0].delta else "", end="")
+
+
+asyncio.run(demo())
+```
+
+#### 2.6 Sync call for embeddings
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+
+response = client.embeddings.create(
+    input=["Hello world!", "Nice to meet you!"],
+    target="db",
+)
+
+print(response.vectors[0][:10])
+print(response.vectors[1][:10])
+```
+
+#### 2.7 Async call for embeddings
+
+```python
+import asyncio
+
+from minimax_client import AsyncMiniMax
+
+
+async def demo():
+    client = AsyncMiniMax(api_key="<YOUR_API_KEY>")
+
+    response = await client.embeddings.create(
+        input=["Hello async world!", "Nice to meet you async!"],
+        target="query",
+    )
+
+    print(response.vectors[0][:10])
+    print(response.vectors[1][:10])
+
+
+asyncio.run(demo())
+```
+
+#### 2.8 Sync call for files
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+
+resp = client.files.create(filepath="sample.txt", purpose="retrieval")
+print(resp.file.file_id)
+
+resp = client.files.list(purpose="retrieval")
+print(resp.files[0].file_id)
+
+resp = client.files.retrieve(file_id=resp.files[0].file_id)
+print(resp.file.bytes)
+
+resp = client.files.delete(file_id=resp.file.file_id)
+print(resp.file_id)
+```
+
+#### 2.9 Async call for files
+
+```python
+import asyncio
+
+from minimax_client import AsyncMiniMax
+
+
+async def demo():
+    client = AsyncMiniMax(api_key="<YOUR_API_KEY>")
+
+    resp = await client.files.create(filepath="sample.txt", purpose="retrieval")
+    print(resp.file.file_id)
+
+    resp = await client.files.list(purpose="retrieval")
+    print(resp.files[0].file_id)
+
+    resp = await client.files.retrieve(file_id=resp.files[0].file_id)
+    print(resp.file.bytes)
+
+    resp = await client.files.delete(file_id=resp.file.file_id)
+    print(resp.file_id)
+
+asyncio.run(demo())
+```
+
+#### 2.10 Sync call for files
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+resp = client.fine_tuning.jobs.create(
+    model="abab5.5s-chat-240123", training_file=..., suffix="test"
+)
+print(resp.id)
+print(resp.fine_tuned_model)
+
+resp = client.fine_tuning.jobs.list(limit=5)
+print(resp.job_list[0])
+
+resp = client.model.list()
+print(resp.model_list[0])
+
+resp = client.model.retrieve(model="ft:abab5.5s-chat-240123_XXXXXXXXXXXXX:test")
+print(resp.model.id)
+```
+
+#### 2.11 Sync call for assistants
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+resp = client.assistants.create(model="abab5.5s-chat-240123")
+
+client.assistants.update(
+    assistant_id=resp.id,
+    model="abab5.5s-chat-240123",
+    name="test-assistant",
+    instructions="You are a helpful assistant.",
+)
+
+client.assistants.retrieve(assistant_id=resp.id)
+
+client.assistants.list(limit=5)
+
+client.assistants.delete(assistant_id=resp.id)
+```
+
+#### 2.12 Sync call for assistant files
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+resp = client.files.create(filepath="sample.txt", purpose="retrieval")
+
+file_id = resp.file.file_id
+
+resp = client.assistants.create(
+    model="abab5.5s-chat-240123",
+    name="test-assistant",
+    instructions="You are a helpful assistant.",
+    description="test-assistant",
+    tools=[{"type": "retrieval"}],
+)
+
+assistant_id = resp.id
+
+resp = client.assistants.files.create(assistant_id=assistant_id, file_id=str(file_id))
+
+resp = client.assistants.files.retrieve(assistant_id=assistant_id, file_id=str(file_id))
+
+resp = client.assistants.files.list(assistant_id=assistant_id, limit=5, order="asc")
+
+resp = client.assistants.files.delete(assistant_id=assistant_id, file_id=str(file_id))
+```
```

### Comparing `minimax_client-0.5.0/pyproject.toml` & `minimax_client-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP",
     "Typing :: Typed",
 ]
 dynamic = []
-version = "0.5.0"
+version = "0.5.1"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 dev = [
     "pytest>=8.1.1,<9",
```

### Comparing `minimax_client-0.5.0/src/minimax_client/client.py` & `minimax_client-0.5.1/src/minimax_client/client.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-"""client.py"""
-
-import asyncio
-import os
-from typing import Optional
-
-import httpx
-from dotenv import find_dotenv, load_dotenv
-
-from minimax_client.interfaces.assistant import Assistant, AsyncAssistant
-from minimax_client.interfaces.chat_completion import AsyncChat, Chat
-from minimax_client.interfaces.embedding import AsyncEmbedding, Embedding
-from minimax_client.interfaces.file import AsyncFiles, Files
-from minimax_client.interfaces.fine_tuning import (
-    AsyncFineTuning,
-    AsyncModel,
-    FineTuning,
-    Model,
-)
-
-BASE_URL = "https://api.minimax.chat/v1"
-
-
-class BaseMiniMaxClient:
-    """MiniMax client base class"""
-
-    api_key: str
-    group_id: str
-    timeout: float
-
-    def __init__(
-        self,
-        api_key: Optional[str] = None,
-        group_id: Optional[str] = None,
-        timeout: float = 60,
-    ) -> None:
-        if not api_key:
-            api_key = self._get_api_key_from_env()
-
-        if not group_id:
-            group_id = os.getenv("MINIMAX_GROUP_ID", "")
-
-        self.api_key = api_key
-        self.group_id = group_id
-        self.timeout = timeout
-        self.http_client = self._get_http_client()
-
-    def _get_api_key_from_env(self) -> str:
-        """
-        Retrieves the MiniMax API key from the environment.
-
-        First it tries to find a `.env` file in the current
-        directory or any of its parent directories. If such a file is found,
-        it loads the environment variables from it.
-
-        Then, it retrieves the `MINIMAX_API_KEY` environment variable. If it
-        contains a valid API key, it returns it. Otherwise, it raises a
-        `ValueError`.
-
-        Returns:
-            str: The MiniMax API key.
-        """
-        env_file = find_dotenv()
-
-        if env_file:
-            load_dotenv(dotenv_path=env_file)
-
-        api_key = os.getenv("MINIMAX_API_KEY")
-
-        if not api_key:
-            raise ValueError("A valid MiniMax API key must be provided!")
-
-        return api_key
-
-    def _get_http_client(self):
-        raise NotImplementedError
-
-
-class MiniMax(BaseMiniMaxClient):
-    """MiniMax client"""
-
-    http_client: httpx.Client
-    assistants: Assistant
-    chat: Chat
-    embeddings: Embedding
-    files: Files
-    fine_tuning: FineTuning
-    model: Model
-
-    def __init__(self, *, api_key: Optional[str] = None, timeout: float = 60) -> None:
-        super().__init__(api_key=api_key, timeout=timeout)
-        self.assistants = Assistant(http_client=self.http_client)
-        self.chat = Chat(http_client=self.http_client)
-        self.embeddings = Embedding(http_client=self.http_client)
-        self.files = Files(http_client=self.http_client)
-        self.fine_tuning = FineTuning(http_client=self.http_client)
-        self.model = Model(http_client=self.http_client)
-
-    def __del__(self) -> None:
-        """Closes the HTTP client if it is not already closed."""
-        if hasattr(self, "http_client") and not self.http_client.is_closed:
-            self.http_client.close()
-
-    def _get_http_client(self) -> httpx.Client:
-        """
-        Returns a synchronous HTTP client with the base URL and authentication
-        header configured.
-
-        The client is configured to send requests to the MiniMax API with the
-        provided API key.
-
-        Returns:
-            httpx.Client: The synchronous HTTP client.
-        """
-        return httpx.Client(
-            base_url=BASE_URL,
-            headers={"Authorization": f"Bearer {self.api_key}"},
-            timeout=self.timeout,
-        )
-
-
-class AsyncMiniMax(BaseMiniMaxClient):
-    """MiniMax async client"""
-
-    http_client: httpx.AsyncClient
-    assistants: AsyncAssistant
-    chat: AsyncChat
-    embeddings: AsyncEmbedding
-    files: AsyncFiles
-    fine_tuning: AsyncFineTuning
-    model: AsyncModel
-
-    def __init__(self, *, api_key: Optional[str] = None, timeout: float = 60) -> None:
-        super().__init__(api_key=api_key, timeout=timeout)
-        self.assistants = AsyncAssistant(http_client=self.http_client)
-        self.chat = AsyncChat(http_client=self.http_client)
-        self.embeddings = AsyncEmbedding(http_client=self.http_client)
-        self.files = AsyncFiles(http_client=self.http_client)
-        self.fine_tuning = AsyncFineTuning(http_client=self.http_client)
-        self.model = AsyncModel(http_client=self.http_client)
-
-    def __del__(self) -> None:
-        async def __del_client() -> None:
-            """
-            Closes the async HTTP client if it is not already closed.
-
-            This coroutine is called when the AsyncMiniMax instance is garbage
-            collected. It asynchronously closes the HTTP client if it is not
-            already closed.
-            """
-            if hasattr(self, "http_client") and not self.http_client.is_closed:
-                await self.http_client.aclose()
-
-        # Create a task to close the HTTP client. This task is scheduled to run
-        # asyncio's event loop, but it does not block the interpreter from
-        # exiting.
-        asyncio.create_task(__del_client())
-
-    def _get_http_client(self) -> httpx.AsyncClient:
-        """
-        Returns a new asynchronous HTTP client with the base URL and
-        authentication header configured.
-
-        The client is configured to send requests to the MiniMax API with the
-        provided API key.
-
-        Returns:
-            httpx.AsyncClient: The asynchronous HTTP client.
-        """
-        return httpx.AsyncClient(
-            base_url=BASE_URL,
-            headers={"Authorization": f"Bearer {self.api_key}"},
-            timeout=self.timeout,
-        )
+"""client.py"""
+
+import asyncio
+import os
+from typing import Optional
+
+import httpx
+from dotenv import find_dotenv, load_dotenv
+
+from minimax_client.interfaces.assistant import Assistant, AsyncAssistant
+from minimax_client.interfaces.chat_completion import AsyncChat, Chat
+from minimax_client.interfaces.embedding import AsyncEmbedding, Embedding
+from minimax_client.interfaces.file import AsyncFiles, Files
+from minimax_client.interfaces.fine_tuning import (
+    AsyncFineTuning,
+    AsyncModel,
+    FineTuning,
+    Model,
+)
+
+BASE_URL = "https://api.minimax.chat/v1"
+
+
+class BaseMiniMaxClient:
+    """MiniMax client base class"""
+
+    api_key: str
+    group_id: str
+    timeout: float
+
+    def __init__(
+        self,
+        api_key: Optional[str] = None,
+        group_id: Optional[str] = None,
+        timeout: float = 60,
+    ) -> None:
+        if not api_key:
+            api_key = self._get_api_key_from_env()
+
+        if not group_id:
+            group_id = os.getenv("MINIMAX_GROUP_ID", "")
+
+        self.api_key = api_key
+        self.group_id = group_id
+        self.timeout = timeout
+        self.http_client = self._get_http_client()
+
+    def _get_api_key_from_env(self) -> str:
+        """
+        Retrieves the MiniMax API key from the environment.
+
+        First it tries to find a `.env` file in the current
+        directory or any of its parent directories. If such a file is found,
+        it loads the environment variables from it.
+
+        Then, it retrieves the `MINIMAX_API_KEY` environment variable. If it
+        contains a valid API key, it returns it. Otherwise, it raises a
+        `ValueError`.
+
+        Returns:
+            str: The MiniMax API key.
+        """
+        env_file = find_dotenv()
+
+        if env_file:
+            load_dotenv(dotenv_path=env_file)
+
+        api_key = os.getenv("MINIMAX_API_KEY")
+
+        if not api_key:
+            raise ValueError("A valid MiniMax API key must be provided!")
+
+        return api_key
+
+    def _get_http_client(self):
+        raise NotImplementedError
+
+
+class MiniMax(BaseMiniMaxClient):
+    """MiniMax client"""
+
+    http_client: httpx.Client
+    assistants: Assistant
+    chat: Chat
+    embeddings: Embedding
+    files: Files
+    fine_tuning: FineTuning
+    model: Model
+
+    def __init__(self, *, api_key: Optional[str] = None, timeout: float = 60) -> None:
+        super().__init__(api_key=api_key, timeout=timeout)
+        self.assistants = Assistant(http_client=self.http_client)
+        self.chat = Chat(http_client=self.http_client)
+        self.embeddings = Embedding(http_client=self.http_client)
+        self.files = Files(http_client=self.http_client)
+        self.fine_tuning = FineTuning(http_client=self.http_client)
+        self.model = Model(http_client=self.http_client)
+
+    def __del__(self) -> None:
+        """Closes the HTTP client if it is not already closed."""
+        if hasattr(self, "http_client") and not self.http_client.is_closed:
+            self.http_client.close()
+
+    def _get_http_client(self) -> httpx.Client:
+        """
+        Returns a synchronous HTTP client with the base URL and authentication
+        header configured.
+
+        The client is configured to send requests to the MiniMax API with the
+        provided API key.
+
+        Returns:
+            httpx.Client: The synchronous HTTP client.
+        """
+        return httpx.Client(
+            base_url=BASE_URL,
+            headers={"Authorization": f"Bearer {self.api_key}"},
+            timeout=self.timeout,
+        )
+
+
+class AsyncMiniMax(BaseMiniMaxClient):
+    """MiniMax async client"""
+
+    http_client: httpx.AsyncClient
+    assistants: AsyncAssistant
+    chat: AsyncChat
+    embeddings: AsyncEmbedding
+    files: AsyncFiles
+    fine_tuning: AsyncFineTuning
+    model: AsyncModel
+
+    def __init__(self, *, api_key: Optional[str] = None, timeout: float = 60) -> None:
+        super().__init__(api_key=api_key, timeout=timeout)
+        self.assistants = AsyncAssistant(http_client=self.http_client)
+        self.chat = AsyncChat(http_client=self.http_client)
+        self.embeddings = AsyncEmbedding(http_client=self.http_client)
+        self.files = AsyncFiles(http_client=self.http_client)
+        self.fine_tuning = AsyncFineTuning(http_client=self.http_client)
+        self.model = AsyncModel(http_client=self.http_client)
+
+    def __del__(self) -> None:
+        async def __del_client() -> None:
+            """
+            Closes the async HTTP client if it is not already closed.
+
+            This coroutine is called when the AsyncMiniMax instance is garbage
+            collected. It asynchronously closes the HTTP client if it is not
+            already closed.
+            """
+            if hasattr(self, "http_client") and not self.http_client.is_closed:
+                await self.http_client.aclose()
+
+        # Create a task to close the HTTP client. This task is scheduled to run
+        # asyncio's event loop, but it does not block the interpreter from
+        # exiting.
+        asyncio.create_task(__del_client())
+
+    def _get_http_client(self) -> httpx.AsyncClient:
+        """
+        Returns a new asynchronous HTTP client with the base URL and
+        authentication header configured.
+
+        The client is configured to send requests to the MiniMax API with the
+        provided API key.
+
+        Returns:
+            httpx.AsyncClient: The asynchronous HTTP client.
+        """
+        return httpx.AsyncClient(
+            base_url=BASE_URL,
+            headers={"Authorization": f"Bearer {self.api_key}"},
+            timeout=self.timeout,
+        )
```

### Comparing `minimax_client-0.5.0/src/minimax_client/entities/assistant.py` & `minimax_client-0.5.1/src/minimax_client/entities/assistant.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,117 @@
-"""assistant.py"""
-
-from typing import Dict, List, Literal, Optional
-
-from pydantic import BaseModel, PositiveInt
-
-from minimax_client.entities.common import BareResponse
-
-
-class AssistantToolFunction(BaseModel):
-    """Assistant Tool Function"""
-
-    description: str
-    name: str
-    parameters: Optional[Dict] = None
-
-
-class AssistantTool(BaseModel):
-    """Assistant Tool"""
-
-    type: Literal["function", "code_interpreter", "web_search", "retrieval"]
-    function: Optional[AssistantToolFunction] = None
-
-
-class Assistant(BaseModel):
-    """Assistant"""
-
-    id: str
-    object: Literal["assistant"]
-    created_at: PositiveInt
-    name: str
-    description: str
-    model: Literal[
-        "abab6-chat",
-        "abab5.5-chat",
-        "abab5.5s-chat",
-        "abab5.5-chat-240131",
-        "abab5.5s-chat-240123",
-    ]
-    instructions: str
-    tools: List[AssistantTool] = []
-    file_ids: List[str] = []
-    metadata: Dict = {}
-    rolemeta: Dict
-    status: str
-
-
-class AssistantCreateResponse(BareResponse, Assistant):
-    """Assistant Create Response"""
-
-
-class AssistantRetrieveResponse(BareResponse, Assistant):
-    """Assistant Retrieve Response"""
-
-
-class AssistantUpdateResponse(BareResponse):
-    """Assistant Update Response"""
-
-    assistant: Assistant
-
-
-class AssistantDeleteResponse(BareResponse):
-    """Assistant Delete Response"""
-
-    id: str
-    object: Literal["assistant.deleted"]
-    deleted: bool
-
-
-class AssistantListResponse(BareResponse):
-    """Assistant List Response"""
-
-    object: Literal["list"]
-    data: List[Assistant]
-    has_more: bool
-    first_id: str
-    last_id: str
+"""assistant.py"""
+
+from typing import Dict, List, Literal, Optional
+
+from pydantic import BaseModel, PositiveInt
+
+from minimax_client.entities.common import BareResponse
+
+
+class AssistantToolFunction(BaseModel):
+    """Assistant Tool Function"""
+
+    description: str
+    name: str
+    parameters: Optional[Dict] = None
+
+
+class AssistantTool(BaseModel):
+    """Assistant Tool"""
+
+    type: Literal["code_interpreter", "retrieval", "function", "web_search"]
+    function: Optional[AssistantToolFunction] = None
+
+
+class AssistantT2AOption(BaseModel):
+    """Assistant T2A Option"""
+
+    model: str
+    voice_id: str
+    format: Literal["mp3", "flac", "pcm"] = "mp3"
+
+
+class Assistant(BaseModel):
+    """Assistant"""
+
+    id: str
+    object: Literal["assistant"]
+    created_at: PositiveInt
+    updated_at: Optional[PositiveInt] = None
+    name: str
+    description: str
+    model: Literal[
+        "abab6-chat",
+        "abab5.5-chat",
+        "abab5.5-chat-240131",
+        "abab5.5s-chat",
+        "abab5.5s-chat-240123",
+    ]
+    instructions: str
+    tools: List[AssistantTool] = []
+    file_ids: List[str] = []
+    metadata: Dict = {}
+    rolemeta: Dict
+    status: str
+    t2a_option: Optional[AssistantT2AOption] = None
+
+
+class AssistantCreateResponse(BareResponse, Assistant):
+    """Assistant Create Response"""
+
+
+class AssistantRetrieveResponse(BareResponse, Assistant):
+    """Assistant Retrieve Response"""
+
+
+class AssistantUpdateResponse(BareResponse):
+    """Assistant Update Response"""
+
+    assistant: Assistant
+
+
+class AssistantDeleteResponse(BareResponse):
+    """Assistant Delete Response"""
+
+    id: str
+    object: Literal["assistant.deleted"]
+    deleted: bool
+
+
+class AssistantListResponse(BareResponse):
+    """Assistant List Response"""
+
+    object: Literal["list"]
+    data: List[Assistant]
+    has_more: bool
+    first_id: str
+    last_id: str
+
+
+class AssistantFile(BaseModel):
+    """Assistant File"""
+
+    id: str
+    object: Literal["assistant.file"]
+    created_at: PositiveInt
+    assistant_id: str
+
+
+class AssistantFileCreateResponse(BareResponse, AssistantFile):
+    """Assistant File Create Response"""
+
+
+class AssistantFileRetrieveResponse(BareResponse, AssistantFile):
+    """Assistant File Retrieve Response"""
+
+
+class AssistantFileListResponse(BareResponse):
+    """Assistant File List Response"""
+
+    object: Literal["list"]
+    data: List[AssistantFile]
+
+
+class AssistantFileDeleteResponse(BareResponse):
+    """Assistant File Delete Response"""
+
+    file_id: str
```

### Comparing `minimax_client-0.5.0/src/minimax_client/entities/chat_completion.py` & `minimax_client-0.5.1/src/minimax_client/entities/chat_completion.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-"""chat_completion.py"""
-
-from typing import List, Literal, Optional
-
-from pydantic import BaseModel, NonNegativeInt
-
-from minimax_client.entities.common import BareResponse
-
-
-class ChoiceMessageToolCallFunction(BaseModel):
-    """Chat Completion Choice Message ToolCall Function"""
-
-    name: str
-    arguments: str
-
-
-class ChoiceMessageToolCall(BaseModel):
-    """Chat Completion Choice Message ToolCall"""
-
-    id: str
-    type: Literal["function"]
-    function: ChoiceMessageToolCallFunction
-
-
-class ChoiceMessage(BaseModel):
-    """Chat Completion Choice Message"""
-
-    role: Literal["assistant", "user", "system", "tool"]
-    content: Optional[str] = None
-    tool_calls: Optional[List[ChoiceMessageToolCall]] = None
-
-
-class Choice(BaseModel):
-    """Chat Completion Choice"""
-
-    index: NonNegativeInt
-    message: Optional[ChoiceMessage] = None
-    delta: Optional[ChoiceMessage] = None
-    finish_reason: Optional[Literal["length", "stop", "tool_calls"]] = None
-
-
-class Usage(BaseModel):
-    """Chat Completion Response Usage"""
-
-    total_tokens: NonNegativeInt
-
-
-class ChatCompletionResponse(BareResponse):
-    """Chat Completion Response"""
-
-    id: str
-    choices: List[Choice]
-    created: int
-    model: Literal["abab5.5s-chat", "abab5.5-chat", "abab6-chat"]
-    object: Literal["chat.completion", "chat.completion.chunk"]
-    usage: Optional[Usage] = None
+"""chat_completion.py"""
+
+from typing import List, Literal, Optional
+
+from pydantic import BaseModel, NonNegativeInt
+
+from minimax_client.entities.common import BareResponse
+
+
+class ChoiceMessageToolCallFunction(BaseModel):
+    """Chat Completion Choice Message ToolCall Function"""
+
+    name: str
+    arguments: str
+
+
+class ChoiceMessageToolCall(BaseModel):
+    """Chat Completion Choice Message ToolCall"""
+
+    id: str
+    type: Literal["function"]
+    function: ChoiceMessageToolCallFunction
+
+
+class ChoiceMessage(BaseModel):
+    """Chat Completion Choice Message"""
+
+    role: Literal["assistant", "user", "system", "tool"]
+    content: Optional[str] = None
+    tool_calls: Optional[List[ChoiceMessageToolCall]] = None
+
+
+class Choice(BaseModel):
+    """Chat Completion Choice"""
+
+    index: NonNegativeInt
+    message: Optional[ChoiceMessage] = None
+    delta: Optional[ChoiceMessage] = None
+    finish_reason: Optional[Literal["length", "stop", "tool_calls"]] = None
+
+
+class Usage(BaseModel):
+    """Chat Completion Response Usage"""
+
+    total_tokens: NonNegativeInt
+
+
+class ChatCompletionResponse(BareResponse):
+    """Chat Completion Response"""
+
+    id: str
+    choices: List[Choice]
+    created: int
+    model: Literal["abab5.5s-chat", "abab5.5-chat", "abab6-chat"]
+    object: Literal["chat.completion", "chat.completion.chunk"]
+    usage: Optional[Usage] = None
```

### Comparing `minimax_client-0.5.0/src/minimax_client/entities/file.py` & `minimax_client-0.5.1/src/minimax_client/entities/file.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-"""file.py"""
-
-from typing import List, Optional
-
-from pydantic import BaseModel, NonNegativeInt
-
-from minimax_client.entities.common import BareResponse
-
-
-class File(BaseModel):
-    """
-    File entity
-
-    purpose:
-        retrieval -> pdf, docx, txt
-        fine-tune -> jsonl
-        voice_clone -> mp3, m4a, wav
-        assistants -> refer to official documents
-        role-recognition -> json, txt(with json content)
-    """
-
-    file_id: NonNegativeInt
-    bytes: NonNegativeInt
-    created_at: int
-    filename: str
-    purpose: str
-    download_url: Optional[str] = None
-
-
-class FileCreateResponse(BareResponse):
-    """File Create Response"""
-
-    file: File
-
-
-class FileListResponse(BareResponse):
-    """File List Response"""
-
-    files: List[File]
-
-
-class FileRetriveResponse(BareResponse):
-    """File Retrieve Response"""
-
-    file: File
-
-
-class FileRetrieveContentResponse(BareResponse):
-    """File Retrieve Content Response"""
-
-    content: bytes  # to be confirmed
-
-
-class FileDeleteResponse(BareResponse):
-    """File Delete Response"""
-
-    file_id: NonNegativeInt
+"""file.py"""
+
+from typing import List, Optional
+
+from pydantic import BaseModel, NonNegativeInt
+
+from minimax_client.entities.common import BareResponse
+
+
+class File(BaseModel):
+    """
+    File entity
+
+    purpose:
+        retrieval -> pdf, docx, txt
+        fine-tune -> jsonl
+        voice_clone -> mp3, m4a, wav
+        assistants -> refer to official documents
+        role-recognition -> json, txt(with json content)
+    """
+
+    file_id: NonNegativeInt
+    bytes: NonNegativeInt
+    created_at: int
+    filename: str
+    purpose: str
+    download_url: Optional[str] = None
+
+
+class FileCreateResponse(BareResponse):
+    """File Create Response"""
+
+    file: File
+
+
+class FileListResponse(BareResponse):
+    """File List Response"""
+
+    files: List[File]
+
+
+class FileRetriveResponse(BareResponse):
+    """File Retrieve Response"""
+
+    file: File
+
+
+class FileRetrieveContentResponse(BareResponse):
+    """File Retrieve Content Response"""
+
+    content: bytes  # to be confirmed
+
+
+class FileDeleteResponse(BareResponse):
+    """File Delete Response"""
+
+    file_id: NonNegativeInt
```

### Comparing `minimax_client-0.5.0/src/minimax_client/interfaces/chat_completion.py` & `minimax_client-0.5.1/src/minimax_client/interfaces/chat_completion.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,239 +1,239 @@
-"""chat_completion.py"""
-
-import json
-from http import HTTPStatus
-from typing import Any, AsyncGenerator, Dict, Generator, List, Optional, Union
-
-import httpx
-
-from minimax_client.entities.chat_completion import ChatCompletionResponse
-from minimax_client.interfaces.base import BaseAsyncInterface, BaseSyncInterface
-
-
-class ChatCompletions(BaseSyncInterface):
-    """Synchronous Chat Completions interface"""
-
-    url_path: str = "text/chatcompletion_v2"
-
-    def create(
-        self,
-        *,
-        messages: List[Dict[str, Union[str, List[Dict[str, Any]]]]],
-        model: str = "abab5.5s-chat",
-        max_tokens: int = 256,
-        temperature: float = 0.9,
-        top_p: float = 0.95,
-        stream: bool = False,
-        tool_choice: str = "auto",
-        tools: Optional[List[Dict[str, Union[str, Dict[str, str]]]]] = None,
-    ) -> Union[ChatCompletionResponse, Generator[ChatCompletionResponse, None, None]]:
-        """
-        Create a new chat completion request.
-
-        Requests can be sent in or not in stream by setting the "stream" parameter.
-        Streaming requests return a generator that yields ResponseEntities,
-        while non-streaming requests return a single ResponseEntity.
-
-        Args:
-            messages (list[dict[str, Union[str, list[dict[str, Any]]]]]):
-                The messages to generate responses to
-            model (str, optional):
-                The chatbot model to use. Defaults to "abab5.5s-chat".
-            max_tokens (int, optional):
-                The maximum number of tokens to generate. Defaults to 256.
-            temperature (float, optional):
-                The temperature of the chatbot's responses. Defaults to 0.9.
-            top_p (float, optional):
-                The top_p of the chatbot's responses. Defaults to 0.95.
-            stream (bool, optional):
-                Whether to stream the responses or not. Defaults to False.
-            tool_choice (str, optional):
-                The tool choice mode. Defaults to "auto".
-            tools (Optional[list[dict[str, Union[str, dict[str, str]]]]], optional):
-                The tools to use. Defaults to None.
-
-        Returns:
-            ChatCompletionResponse | Generator[ChatCompletionResponse, None, None]:
-                The response from the API or a generator of responses
-        """
-        json_body = {
-            "messages": messages,
-            "model": model,
-            "max_tokens": max_tokens,
-            "temperature": temperature,
-            "top_p": top_p,
-            "stream": stream,
-            "tool_choice": tool_choice,
-            "tools": tools if tools else [],
-        }
-
-        if not stream:
-            resp = self.client.post(url=self.url_path, json=json_body)
-            return self._build_response(resp=resp)
-
-        return self._build_stream_response(json_body=json_body)
-
-    def _build_response(self, resp: httpx.Response) -> ChatCompletionResponse:
-        """
-        Builds a Chat Completion response from an HTTP response
-
-        Args:
-            resp (httpx.Response): The HTTP response
-
-        Raises:
-            Exception: If the HTTP response is not OK or if parsing the response fails
-
-        Returns:
-            ChatCompletionResponse: The response from the API
-        """
-        if resp.status_code != HTTPStatus.OK:
-            raise Exception(f"status: {resp.status_code}; {resp.text}")
-
-        try:
-            chat_response = ChatCompletionResponse(**resp.json())
-        except Exception as e:
-            raise Exception(f"Failed to parse response: {e}")  # noqa: B904
-
-        return chat_response
-
-    def _build_stream_response(
-        self, json_body: Dict[str, Any]
-    ) -> Generator[ChatCompletionResponse, None, None]:
-        """
-        Builds a stream of Chat Completion responses from an HTTP response
-
-        Args:
-            json_body (dict): The JSON body of the request
-
-        Yields:
-            ChatCompletionResponse: The response from the API
-        """
-        with self.client.stream(
-            method="post", url=self.url_path, json=json_body
-        ) as resp:
-            if resp.status_code != HTTPStatus.OK:
-                raise Exception(f"status: {resp.status_code}; {resp.text}")
-
-            for data in resp.iter_text():
-                json_body = json.loads(data.split("data: ", 2)[1])
-
-                yield ChatCompletionResponse(**json_body)
-
-                # If the stream is finished, break out of the loop
-                if "finish_reason" in json_body["choices"][0]:
-                    break
-
-
-class AsyncChatCompletions(BaseAsyncInterface, ChatCompletions):
-    """Asynchronous Chat Completions interface"""
-
-    async def create(
-        self,
-        *,
-        messages: List[Dict[str, Union[str, List[Dict[str, Any]]]]],
-        model: str = "abab5.5s-chat",
-        max_tokens: int = 256,
-        temperature: float = 0.9,
-        top_p: float = 0.95,
-        stream: bool = False,
-        tool_choice: str = "auto",
-        tools: Optional[List[Dict[str, Union[str, Dict[str, str]]]]] = None,
-    ) -> Union[ChatCompletionResponse, AsyncGenerator[ChatCompletionResponse, None]]:
-        """
-        Create a new chat completion for the given messages.
-
-        Args:
-            messages (list[dict[str, Union[str, list[dict[str, Any]]]]]):
-                The messages to generate responses to
-            model (str, optional):
-                The chatbot model to use. Defaults to "abab5.5s-chat".
-            max_tokens (int, optional):
-                The maximum number of tokens to generate. Defaults to 256.
-            temperature (float, optional):
-                The temperature of the chatbot's responses. Defaults to 0.9.
-            top_p (float, optional):
-                The top_p of the chatbot's responses. Defaults to 0.95.
-            stream (bool, optional):
-                Whether to stream the responses or not. Defaults to False.
-            tool_choice (str, optional):
-                The tool choice mode. Defaults to "auto".
-            tools (Optional[list[dict[str, Union[str, dict[str, str]]]]], optional):
-                The tools to use. Defaults to None.
-
-        Returns:
-            ChatCompletionResponse | AsyncGenerator[ChatCompletionResponse, None]:
-                The response from the API or a generator of responses
-        """
-        json_body = {
-            "messages": messages,
-            "model": model,
-            "max_tokens": max_tokens,
-            "temperature": temperature,
-            "top_p": top_p,
-            "stream": stream,
-            "tool_choice": tool_choice,
-            "tools": tools if tools else [],
-        }
-
-        if not stream:
-            resp = await self.client.post(url=self.url_path, json=json_body)
-            return self._build_response(resp=resp)
-
-        return self._build_stream_response(json_body=json_body)
-
-    async def _build_stream_response(
-        self, json_body: Dict[str, Any]
-    ) -> AsyncGenerator[ChatCompletionResponse, None]:
-        """
-        Builds a stream of Chat Completion responses from an HTTP response
-
-        Args:
-            json_body (dict): The JSON body of the request
-
-        Yields:
-            ChatCompletionResponse: The response from the API
-        """
-        async with self.client.stream(
-            method="post", url=self.url_path, json=json_body
-        ) as resp:
-            if resp.status_code != HTTPStatus.OK:
-                raise Exception(f"status: {resp.status_code}; {resp.text}")
-
-            async for data in resp.aiter_text():
-                json_body = json.loads(data.split("data: ", 2)[1])
-
-                yield ChatCompletionResponse(**json_body)
-
-                # If the stream is finished, break out of the loop
-                if "finish_reason" in json_body["choices"][0]:
-                    break
-
-
-class Chat:
-    """Synchronous Chat interface"""
-
-    completions: ChatCompletions
-
-    def __init__(self, http_client: httpx.Client) -> None:
-        """
-        Initializes the Chat interface
-
-        Args:
-            http_client (httpx.Client): The HTTP client to use
-        """
-        self.completions = ChatCompletions(http_client=http_client)
-
-
-class AsyncChat:
-    """Asynchronous Chat interface"""
-
-    completions: AsyncChatCompletions
-
-    def __init__(self, http_client: httpx.AsyncClient) -> None:
-        """
-        Initializes the AsyncChat interface
-
-        Args:
-            http_client (httpx.AsyncClient): The HTTP client to use
-        """
-        self.completions = AsyncChatCompletions(http_client=http_client)
+"""chat_completion.py"""
+
+import json
+from http import HTTPStatus
+from typing import Any, AsyncGenerator, Dict, Generator, List, Optional, Union
+
+import httpx
+
+from minimax_client.entities.chat_completion import ChatCompletionResponse
+from minimax_client.interfaces.base import BaseAsyncInterface, BaseSyncInterface
+
+
+class ChatCompletions(BaseSyncInterface):
+    """Synchronous Chat Completions interface"""
+
+    url_path: str = "text/chatcompletion_v2"
+
+    def create(
+        self,
+        *,
+        messages: List[Dict[str, Union[str, List[Dict[str, Any]]]]],
+        model: str = "abab5.5s-chat",
+        max_tokens: int = 256,
+        temperature: float = 0.9,
+        top_p: float = 0.95,
+        stream: bool = False,
+        tool_choice: str = "auto",
+        tools: Optional[List[Dict[str, Union[str, Dict[str, str]]]]] = None,
+    ) -> Union[ChatCompletionResponse, Generator[ChatCompletionResponse, None, None]]:
+        """
+        Create a new chat completion request.
+
+        Requests can be sent in or not in stream by setting the "stream" parameter.
+        Streaming requests return a generator that yields ResponseEntities,
+        while non-streaming requests return a single ResponseEntity.
+
+        Args:
+            messages (list[dict[str, Union[str, list[dict[str, Any]]]]]):
+                The messages to generate responses to
+            model (str, optional):
+                The chatbot model to use. Defaults to "abab5.5s-chat".
+            max_tokens (int, optional):
+                The maximum number of tokens to generate. Defaults to 256.
+            temperature (float, optional):
+                The temperature of the chatbot's responses. Defaults to 0.9.
+            top_p (float, optional):
+                The top_p of the chatbot's responses. Defaults to 0.95.
+            stream (bool, optional):
+                Whether to stream the responses or not. Defaults to False.
+            tool_choice (str, optional):
+                The tool choice mode. Defaults to "auto".
+            tools (Optional[list[dict[str, Union[str, dict[str, str]]]]], optional):
+                The tools to use. Defaults to None.
+
+        Returns:
+            ChatCompletionResponse | Generator[ChatCompletionResponse, None, None]:
+                The response from the API or a generator of responses
+        """
+        json_body = {
+            "messages": messages,
+            "model": model,
+            "max_tokens": max_tokens,
+            "temperature": temperature,
+            "top_p": top_p,
+            "stream": stream,
+            "tool_choice": tool_choice,
+            "tools": tools if tools else [],
+        }
+
+        if not stream:
+            resp = self.client.post(url=self.url_path, json=json_body)
+            return self._build_response(resp=resp)
+
+        return self._build_stream_response(json_body=json_body)
+
+    def _build_response(self, resp: httpx.Response) -> ChatCompletionResponse:
+        """
+        Builds a Chat Completion response from an HTTP response
+
+        Args:
+            resp (httpx.Response): The HTTP response
+
+        Raises:
+            Exception: If the HTTP response is not OK or if parsing the response fails
+
+        Returns:
+            ChatCompletionResponse: The response from the API
+        """
+        if resp.status_code != HTTPStatus.OK:
+            raise Exception(f"status: {resp.status_code}; {resp.text}")
+
+        try:
+            chat_response = ChatCompletionResponse(**resp.json())
+        except Exception as e:
+            raise Exception(f"Failed to parse response: {e}")  # noqa: B904
+
+        return chat_response
+
+    def _build_stream_response(
+        self, json_body: Dict[str, Any]
+    ) -> Generator[ChatCompletionResponse, None, None]:
+        """
+        Builds a stream of Chat Completion responses from an HTTP response
+
+        Args:
+            json_body (dict): The JSON body of the request
+
+        Yields:
+            ChatCompletionResponse: The response from the API
+        """
+        with self.client.stream(
+            method="post", url=self.url_path, json=json_body
+        ) as resp:
+            if resp.status_code != HTTPStatus.OK:
+                raise Exception(f"status: {resp.status_code}; {resp.text}")
+
+            for data in resp.iter_text():
+                json_body = json.loads(data.split("data: ", 2)[1])
+
+                yield ChatCompletionResponse(**json_body)
+
+                # If the stream is finished, break out of the loop
+                if "finish_reason" in json_body["choices"][0]:
+                    break
+
+
+class AsyncChatCompletions(BaseAsyncInterface, ChatCompletions):
+    """Asynchronous Chat Completions interface"""
+
+    async def create(
+        self,
+        *,
+        messages: List[Dict[str, Union[str, List[Dict[str, Any]]]]],
+        model: str = "abab5.5s-chat",
+        max_tokens: int = 256,
+        temperature: float = 0.9,
+        top_p: float = 0.95,
+        stream: bool = False,
+        tool_choice: str = "auto",
+        tools: Optional[List[Dict[str, Union[str, Dict[str, str]]]]] = None,
+    ) -> Union[ChatCompletionResponse, AsyncGenerator[ChatCompletionResponse, None]]:
+        """
+        Create a new chat completion for the given messages.
+
+        Args:
+            messages (list[dict[str, Union[str, list[dict[str, Any]]]]]):
+                The messages to generate responses to
+            model (str, optional):
+                The chatbot model to use. Defaults to "abab5.5s-chat".
+            max_tokens (int, optional):
+                The maximum number of tokens to generate. Defaults to 256.
+            temperature (float, optional):
+                The temperature of the chatbot's responses. Defaults to 0.9.
+            top_p (float, optional):
+                The top_p of the chatbot's responses. Defaults to 0.95.
+            stream (bool, optional):
+                Whether to stream the responses or not. Defaults to False.
+            tool_choice (str, optional):
+                The tool choice mode. Defaults to "auto".
+            tools (Optional[list[dict[str, Union[str, dict[str, str]]]]], optional):
+                The tools to use. Defaults to None.
+
+        Returns:
+            ChatCompletionResponse | AsyncGenerator[ChatCompletionResponse, None]:
+                The response from the API or a generator of responses
+        """
+        json_body = {
+            "messages": messages,
+            "model": model,
+            "max_tokens": max_tokens,
+            "temperature": temperature,
+            "top_p": top_p,
+            "stream": stream,
+            "tool_choice": tool_choice,
+            "tools": tools if tools else [],
+        }
+
+        if not stream:
+            resp = await self.client.post(url=self.url_path, json=json_body)
+            return self._build_response(resp=resp)
+
+        return self._build_stream_response(json_body=json_body)
+
+    async def _build_stream_response(
+        self, json_body: Dict[str, Any]
+    ) -> AsyncGenerator[ChatCompletionResponse, None]:
+        """
+        Builds a stream of Chat Completion responses from an HTTP response
+
+        Args:
+            json_body (dict): The JSON body of the request
+
+        Yields:
+            ChatCompletionResponse: The response from the API
+        """
+        async with self.client.stream(
+            method="post", url=self.url_path, json=json_body
+        ) as resp:
+            if resp.status_code != HTTPStatus.OK:
+                raise Exception(f"status: {resp.status_code}; {resp.text}")
+
+            async for data in resp.aiter_text():
+                json_body = json.loads(data.split("data: ", 2)[1])
+
+                yield ChatCompletionResponse(**json_body)
+
+                # If the stream is finished, break out of the loop
+                if "finish_reason" in json_body["choices"][0]:
+                    break
+
+
+class Chat:
+    """Synchronous Chat interface"""
+
+    completions: ChatCompletions
+
+    def __init__(self, http_client: httpx.Client) -> None:
+        """
+        Initializes the Chat interface
+
+        Args:
+            http_client (httpx.Client): The HTTP client to use
+        """
+        self.completions = ChatCompletions(http_client=http_client)
+
+
+class AsyncChat:
+    """Asynchronous Chat interface"""
+
+    completions: AsyncChatCompletions
+
+    def __init__(self, http_client: httpx.AsyncClient) -> None:
+        """
+        Initializes the AsyncChat interface
+
+        Args:
+            http_client (httpx.AsyncClient): The HTTP client to use
+        """
+        self.completions = AsyncChatCompletions(http_client=http_client)
```

### Comparing `minimax_client-0.5.0/src/minimax_client/interfaces/fine_tuning.py` & `minimax_client-0.5.1/src/minimax_client/interfaces/fine_tuning.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,385 +1,385 @@
-"""fine_tuning.py"""
-
-from typing import Dict, Literal, Optional, Union
-
-import httpx
-
-from minimax_client.entities.common import BareResponse
-from minimax_client.entities.fine_tuning import (
-    FineTuningJobCreateResponse,
-    FineTuningJobEventListResponse,
-    FineTuningJobListResponse,
-    FineTuningModelListResponse,
-    FineTuningModelRetrieveResponse,
-)
-from minimax_client.interfaces.base import BaseAsyncInterface, BaseSyncInterface
-
-
-class FineTuningJob(BaseSyncInterface):
-    """Synchronous Fine Tuning Jobs interface"""
-
-    url_path = ""
-
-    def create(
-        self,
-        *,
-        model: Literal["abab5.5-chat-240119", "abab5.5s-chat-240123"],
-        training_file: int,
-        validation_file: Optional[int] = None,
-        hyperparameters: Optional[Dict[str, Union[int, float]]] = None,
-        suffix: Optional[str] = None,
-    ) -> FineTuningJobCreateResponse:
-        """
-        Create a new fine tuning job
-
-        Args:
-            model (Literal["abab5.5-chat-240119", "abab5.5s-chat-240123"]):
-                The model to fine tune
-            training_file (int): The ID of the training file
-            validation_file (Optional[int], optional): The ID of the validation file.
-                Defaults to None.
-            hyperparameters (Optional[Dict[str, Union[int, float]]], optional):
-                The hyperparameters to fine tune. Defaults to None.
-            suffix (Optional[str], optional): The suffix to use for the fine tuning job.
-                Defaults to None.
-
-        Returns:
-            FineTuningJobCreateResponse: The created fine tuning job
-        """
-        json_body = {
-            "model": model,
-            "training_file": training_file,
-        }
-
-        if validation_file:
-            json_body["validation_file"] = validation_file
-
-        if hyperparameters:
-            json_body["hyperparameters"] = hyperparameters
-
-        if suffix:
-            json_body["suffix"] = suffix
-
-        resp = self.client.post(url="create_finetune_job", json=json_body)
-
-        return FineTuningJobCreateResponse(**resp.json())
-
-    def list(
-        self, limit: int, after: Optional[str] = None
-    ) -> FineTuningJobListResponse:
-        """
-        List all fine tuning jobs
-
-        Args:
-            limit (int): The number of fine tuning jobs to return
-            after (Optional[str], optional):
-                The ID of the fine tuning job to start after. Defaults to None.
-
-        Returns:
-            FineTuningJobListResponse: The list of fine tuning jobs
-        """
-        json_body: Dict[str, Union[int, str]] = {"limit": limit}
-
-        if after:
-            json_body["after"] = after
-
-        resp = self.client.post(url="list_finetune_job", json=json_body)
-
-        return FineTuningJobListResponse(**resp.json())
-
-    def retrieve(self, fine_tuning_job_id: str) -> FineTuningJobCreateResponse:
-        """
-        Retrieve a fine tuning job
-
-        Args:
-            fine_tuning_job_id (str): The ID of the fine tuning job to retrieve
-
-        Returns:
-            FineTuningJobCreateResponse: The retrieved fine tuning job
-        """
-        json_body = {"fine_tuning_job_id": fine_tuning_job_id}
-
-        resp = self.client.post(url="retrieve_finetune_job", json=json_body)
-
-        return FineTuningJobCreateResponse(**resp.json())
-
-    def cancel(self, fine_tuning_job_id: str) -> BareResponse:
-        """
-        Cancel a fine tuning job
-
-        Args:
-            fine_tuning_job_id (str): The ID of the fine tuning job to cancel
-
-        Returns:
-            BareResponse: The response from the API
-        """
-        json_body = {"fine_tuning_job_id": fine_tuning_job_id}
-
-        resp = self.client.post(url="delete_finetune_job", json=json_body)
-
-        return BareResponse(**resp.json())
-
-    def list_events(
-        self, fine_tuning_job_id: str, limit: int, after: Optional[str] = None
-    ) -> FineTuningJobEventListResponse:
-        """
-        List events for a fine tuning job
-
-        Args:
-            fine_tuning_job_id (str): The ID of the fine tuning job
-            limit (int): The number of events to return
-            after (Optional[str], optional):
-                The ID of the event to start after. Defaults to None.
-
-        Returns:
-            FineTuningJobEventListResponse: The list of events
-        """
-        json_body = {"fine_tuning_job_id": fine_tuning_job_id, "limit": limit}
-
-        if after:
-            json_body["after"] = after
-
-        resp = self.client.post(url="list_finetune_event", json=json_body)
-
-        return FineTuningJobEventListResponse(**resp.json())
-
-
-class AsyncFineTuningJob(BaseAsyncInterface, FineTuningJob):
-    """Asynchronous Fine Tuning Jobs interface"""
-
-    async def create(
-        self,
-        *,
-        model: Literal["abab5.5-chat-240119", "abab5.5s-chat-240123"],
-        training_file: int,
-        validation_file: Optional[int] = None,
-        hyperparameters: Optional[Dict[str, Union[int, float]]] = None,
-        suffix: Optional[str] = None,
-    ) -> FineTuningJobCreateResponse:
-        """
-        Create a new fine tuning job
-
-        Args:
-            model (Literal["abab5.5-chat-240119", "abab5.5s-chat-240123"]):
-                The model to fine tune
-            training_file (int): The ID of the training file
-            validation_file (Optional[int], optional): The ID of the validation file.
-                Defaults to None.
-            hyperparameters (Optional[Dict[str, Union[int, float]]], optional):
-                The hyperparameters to fine tune. Defaults to None.
-            suffix (Optional[str], optional): The suffix to use for the fine tuning job.
-                Defaults to None.
-
-        Returns:
-            FineTuningJobCreateResponse: The created fine tuning job
-        """
-        json_body = {
-            "model": model,
-            "training_file": training_file,
-        }
-
-        if validation_file:
-            json_body["validation_file"] = validation_file
-
-        if hyperparameters:
-            json_body["hyperparameters"] = hyperparameters
-
-        if suffix:
-            json_body["suffix"] = suffix
-
-        resp = await self.client.post(url="create_finetune_job", json=json_body)
-
-        return FineTuningJobCreateResponse(**resp.json())
-
-    async def list(
-        self, limit: int, after: Optional[str] = None
-    ) -> FineTuningJobListResponse:
-        """
-        List all fine tuning jobs
-
-        Args:
-            limit (int): The number of fine tuning jobs to return
-            after (Optional[str], optional):
-                The ID of the fine tuning job to start after. Defaults to None.
-
-        Returns:
-            FineTuningJobListResponse: The list of fine tuning jobs
-        """
-        json_body: Dict[str, Union[int, str]] = {"limit": limit}
-
-        if after:
-            json_body["after"] = after
-
-        resp = await self.client.post(url="list_finetune_job", json=json_body)
-
-        return FineTuningJobListResponse(**resp.json())
-
-    async def retrieve(self, fine_tuning_job_id: str) -> FineTuningJobCreateResponse:
-        """
-        Retrieve a fine tuning job
-
-        Args:
-            fine_tuning_job_id (str): The ID of the fine tuning job to retrieve
-
-        Returns:
-            FineTuningJobCreateResponse: The retrieved fine tuning job
-        """
-        json_body = {"fine_tuning_job_id": fine_tuning_job_id}
-
-        resp = await self.client.post(url="retrieve_finetune_job", json=json_body)
-
-        return FineTuningJobCreateResponse(**resp.json())
-
-    async def cancel(self, fine_tuning_job_id: str) -> BareResponse:
-        """
-        Cancel a fine tuning job
-
-        Args:
-            fine_tuning_job_id (str): The ID of the fine tuning job to cancel
-
-        Returns:
-            BareResponse: The response from the API
-        """
-        json_body = {"fine_tuning_job_id": fine_tuning_job_id}
-
-        resp = await self.client.post(url="delete_finetune_job", json=json_body)
-
-        return BareResponse(**resp.json())
-
-    async def list_events(
-        self, fine_tuning_job_id: str, limit: int, after: Optional[str] = None
-    ) -> FineTuningJobEventListResponse:
-        """
-        List events for a fine tuning job
-
-        Args:
-            fine_tuning_job_id (str): The ID of the fine tuning job
-            limit (int): The number of events to return
-            after (Optional[str], optional):
-                The ID of the event to start after. Defaults to None.
-
-        Returns:
-            FineTuningJobEventListResponse: The list of events
-        """
-        json_body = {"fine_tuning_job_id": fine_tuning_job_id, "limit": limit}
-
-        if after:
-            json_body["after"] = after
-
-        resp = await self.client.post(url="list_finetune_event", json=json_body)
-
-        return FineTuningJobEventListResponse(**resp.json())
-
-
-class FineTuning:
-    """Synchronous Fine Tuning interface"""
-
-    jobs: FineTuningJob
-
-    def __init__(self, http_client: httpx.Client) -> None:
-        self.jobs = FineTuningJob(http_client=http_client)
-
-
-class AsyncFineTuning:
-    """Asynchronous Fine Tuning interface"""
-
-    jobs: AsyncFineTuningJob
-
-    def __init__(self, http_client: httpx.AsyncClient) -> None:
-        self.jobs = AsyncFineTuningJob(http_client=http_client)
-
-
-class Model(BaseSyncInterface):
-    """Synchronous Model interface"""
-
-    url_path = ""
-
-    def list(self) -> FineTuningModelListResponse:
-        """
-        List all fine tuning models
-
-        Returns:
-            FineTuningModelListResponse: The list of fine tuning models
-        """
-        resp = self.client.post(url="list_finetune_model")
-
-        return FineTuningModelListResponse(**resp.json())
-
-    def retrieve(self, model: str) -> FineTuningModelRetrieveResponse:
-        """
-        Retrieve a fine tuning model
-
-        Args:
-            model (str): The ID of the fine tuning model to retrieve
-
-        Returns:
-            FineTuningModelRetrieveResponse: The retrieved fine tuning model
-        """
-        json_body = {"model_id": model}
-
-        resp = self.client.post(url="retrieve_finetune_model", json=json_body)
-
-        return FineTuningModelRetrieveResponse(**resp.json())
-
-    def delete(self, model: str) -> BareResponse:
-        """
-        Delete a fine tuning model
-
-        Args:
-            model (str): The ID of the fine tuning model to delete
-
-        Returns:
-            BareResponse: The response from the API
-        """
-        json_body = {"model_id": model}
-
-        resp = self.client.post(url="delete_finetune_model", json=json_body)
-
-        return BareResponse(**resp.json())
-
-
-class AsyncModel(BaseAsyncInterface, Model):
-    """Asynchronous Model interface"""
-
-    async def list(self) -> FineTuningModelListResponse:
-        """
-        List all fine tuning models
-
-        Returns:
-            FineTuningModelListResponse: The list of fine tuning models
-        """
-        resp = await self.client.post(url="list_finetune_model")
-
-        return FineTuningModelListResponse(**resp.json())
-
-    async def retrieve(self, model: str) -> FineTuningModelRetrieveResponse:
-        """
-        Retrieve a fine tuning model
-
-        Args:
-            model (str): The ID of the fine tuning model to retrieve
-
-        Returns:
-            FineTuningModelRetrieveResponse: The retrieved fine tuning model
-        """
-        json_body = {"model_id": model}
-
-        resp = await self.client.post(url="retrieve_finetune_model", json=json_body)
-
-        return FineTuningModelRetrieveResponse(**resp.json())
-
-    async def delete(self, model: str) -> BareResponse:
-        """
-        Delete a fine tuning model
-
-        Args:
-            model (str): The ID of the fine tuning model to delete
-
-        Returns:
-            BareResponse: The response from the API
-        """
-        json_body = {"model_id": model}
-
-        resp = await self.client.post(url="delete_finetune_model", json=json_body)
-
-        return BareResponse(**resp.json())
+"""fine_tuning.py"""
+
+from typing import Dict, Literal, Optional, Union
+
+import httpx
+
+from minimax_client.entities.common import BareResponse
+from minimax_client.entities.fine_tuning import (
+    FineTuningJobCreateResponse,
+    FineTuningJobEventListResponse,
+    FineTuningJobListResponse,
+    FineTuningModelListResponse,
+    FineTuningModelRetrieveResponse,
+)
+from minimax_client.interfaces.base import BaseAsyncInterface, BaseSyncInterface
+
+
+class FineTuningJob(BaseSyncInterface):
+    """Synchronous Fine Tuning Jobs interface"""
+
+    url_path = ""
+
+    def create(
+        self,
+        *,
+        model: Literal["abab5.5-chat-240119", "abab5.5s-chat-240123"],
+        training_file: int,
+        validation_file: Optional[int] = None,
+        hyperparameters: Optional[Dict[str, Union[int, float]]] = None,
+        suffix: Optional[str] = None,
+    ) -> FineTuningJobCreateResponse:
+        """
+        Create a new fine tuning job
+
+        Args:
+            model (Literal["abab5.5-chat-240119", "abab5.5s-chat-240123"]):
+                The model to fine tune
+            training_file (int): The ID of the training file
+            validation_file (Optional[int], optional): The ID of the validation file.
+                Defaults to None.
+            hyperparameters (Optional[Dict[str, Union[int, float]]], optional):
+                The hyperparameters to fine tune. Defaults to None.
+            suffix (Optional[str], optional): The suffix to use for the fine tuning job.
+                Defaults to None.
+
+        Returns:
+            FineTuningJobCreateResponse: The created fine tuning job
+        """
+        json_body = {
+            "model": model,
+            "training_file": training_file,
+        }
+
+        if validation_file:
+            json_body["validation_file"] = validation_file
+
+        if hyperparameters:
+            json_body["hyperparameters"] = hyperparameters
+
+        if suffix:
+            json_body["suffix"] = suffix
+
+        resp = self.client.post(url="create_finetune_job", json=json_body)
+
+        return FineTuningJobCreateResponse(**resp.json())
+
+    def list(
+        self, limit: int, after: Optional[str] = None
+    ) -> FineTuningJobListResponse:
+        """
+        List all fine tuning jobs
+
+        Args:
+            limit (int): The number of fine tuning jobs to return
+            after (Optional[str], optional):
+                The ID of the fine tuning job to start after. Defaults to None.
+
+        Returns:
+            FineTuningJobListResponse: The list of fine tuning jobs
+        """
+        json_body: Dict[str, Union[int, str]] = {"limit": limit}
+
+        if after:
+            json_body["after"] = after
+
+        resp = self.client.post(url="list_finetune_job", json=json_body)
+
+        return FineTuningJobListResponse(**resp.json())
+
+    def retrieve(self, fine_tuning_job_id: str) -> FineTuningJobCreateResponse:
+        """
+        Retrieve a fine tuning job
+
+        Args:
+            fine_tuning_job_id (str): The ID of the fine tuning job to retrieve
+
+        Returns:
+            FineTuningJobCreateResponse: The retrieved fine tuning job
+        """
+        json_body = {"fine_tuning_job_id": fine_tuning_job_id}
+
+        resp = self.client.post(url="retrieve_finetune_job", json=json_body)
+
+        return FineTuningJobCreateResponse(**resp.json())
+
+    def cancel(self, fine_tuning_job_id: str) -> BareResponse:
+        """
+        Cancel a fine tuning job
+
+        Args:
+            fine_tuning_job_id (str): The ID of the fine tuning job to cancel
+
+        Returns:
+            BareResponse: The response from the API
+        """
+        json_body = {"fine_tuning_job_id": fine_tuning_job_id}
+
+        resp = self.client.post(url="delete_finetune_job", json=json_body)
+
+        return BareResponse(**resp.json())
+
+    def list_events(
+        self, fine_tuning_job_id: str, limit: int, after: Optional[str] = None
+    ) -> FineTuningJobEventListResponse:
+        """
+        List events for a fine tuning job
+
+        Args:
+            fine_tuning_job_id (str): The ID of the fine tuning job
+            limit (int): The number of events to return
+            after (Optional[str], optional):
+                The ID of the event to start after. Defaults to None.
+
+        Returns:
+            FineTuningJobEventListResponse: The list of events
+        """
+        json_body = {"fine_tuning_job_id": fine_tuning_job_id, "limit": limit}
+
+        if after:
+            json_body["after"] = after
+
+        resp = self.client.post(url="list_finetune_event", json=json_body)
+
+        return FineTuningJobEventListResponse(**resp.json())
+
+
+class AsyncFineTuningJob(BaseAsyncInterface, FineTuningJob):
+    """Asynchronous Fine Tuning Jobs interface"""
+
+    async def create(
+        self,
+        *,
+        model: Literal["abab5.5-chat-240119", "abab5.5s-chat-240123"],
+        training_file: int,
+        validation_file: Optional[int] = None,
+        hyperparameters: Optional[Dict[str, Union[int, float]]] = None,
+        suffix: Optional[str] = None,
+    ) -> FineTuningJobCreateResponse:
+        """
+        Create a new fine tuning job
+
+        Args:
+            model (Literal["abab5.5-chat-240119", "abab5.5s-chat-240123"]):
+                The model to fine tune
+            training_file (int): The ID of the training file
+            validation_file (Optional[int], optional): The ID of the validation file.
+                Defaults to None.
+            hyperparameters (Optional[Dict[str, Union[int, float]]], optional):
+                The hyperparameters to fine tune. Defaults to None.
+            suffix (Optional[str], optional): The suffix to use for the fine tuning job.
+                Defaults to None.
+
+        Returns:
+            FineTuningJobCreateResponse: The created fine tuning job
+        """
+        json_body = {
+            "model": model,
+            "training_file": training_file,
+        }
+
+        if validation_file:
+            json_body["validation_file"] = validation_file
+
+        if hyperparameters:
+            json_body["hyperparameters"] = hyperparameters
+
+        if suffix:
+            json_body["suffix"] = suffix
+
+        resp = await self.client.post(url="create_finetune_job", json=json_body)
+
+        return FineTuningJobCreateResponse(**resp.json())
+
+    async def list(
+        self, limit: int, after: Optional[str] = None
+    ) -> FineTuningJobListResponse:
+        """
+        List all fine tuning jobs
+
+        Args:
+            limit (int): The number of fine tuning jobs to return
+            after (Optional[str], optional):
+                The ID of the fine tuning job to start after. Defaults to None.
+
+        Returns:
+            FineTuningJobListResponse: The list of fine tuning jobs
+        """
+        json_body: Dict[str, Union[int, str]] = {"limit": limit}
+
+        if after:
+            json_body["after"] = after
+
+        resp = await self.client.post(url="list_finetune_job", json=json_body)
+
+        return FineTuningJobListResponse(**resp.json())
+
+    async def retrieve(self, fine_tuning_job_id: str) -> FineTuningJobCreateResponse:
+        """
+        Retrieve a fine tuning job
+
+        Args:
+            fine_tuning_job_id (str): The ID of the fine tuning job to retrieve
+
+        Returns:
+            FineTuningJobCreateResponse: The retrieved fine tuning job
+        """
+        json_body = {"fine_tuning_job_id": fine_tuning_job_id}
+
+        resp = await self.client.post(url="retrieve_finetune_job", json=json_body)
+
+        return FineTuningJobCreateResponse(**resp.json())
+
+    async def cancel(self, fine_tuning_job_id: str) -> BareResponse:
+        """
+        Cancel a fine tuning job
+
+        Args:
+            fine_tuning_job_id (str): The ID of the fine tuning job to cancel
+
+        Returns:
+            BareResponse: The response from the API
+        """
+        json_body = {"fine_tuning_job_id": fine_tuning_job_id}
+
+        resp = await self.client.post(url="delete_finetune_job", json=json_body)
+
+        return BareResponse(**resp.json())
+
+    async def list_events(
+        self, fine_tuning_job_id: str, limit: int, after: Optional[str] = None
+    ) -> FineTuningJobEventListResponse:
+        """
+        List events for a fine tuning job
+
+        Args:
+            fine_tuning_job_id (str): The ID of the fine tuning job
+            limit (int): The number of events to return
+            after (Optional[str], optional):
+                The ID of the event to start after. Defaults to None.
+
+        Returns:
+            FineTuningJobEventListResponse: The list of events
+        """
+        json_body = {"fine_tuning_job_id": fine_tuning_job_id, "limit": limit}
+
+        if after:
+            json_body["after"] = after
+
+        resp = await self.client.post(url="list_finetune_event", json=json_body)
+
+        return FineTuningJobEventListResponse(**resp.json())
+
+
+class FineTuning:
+    """Synchronous Fine Tuning interface"""
+
+    jobs: FineTuningJob
+
+    def __init__(self, http_client: httpx.Client) -> None:
+        self.jobs = FineTuningJob(http_client=http_client)
+
+
+class AsyncFineTuning:
+    """Asynchronous Fine Tuning interface"""
+
+    jobs: AsyncFineTuningJob
+
+    def __init__(self, http_client: httpx.AsyncClient) -> None:
+        self.jobs = AsyncFineTuningJob(http_client=http_client)
+
+
+class Model(BaseSyncInterface):
+    """Synchronous Model interface"""
+
+    url_path = ""
+
+    def list(self) -> FineTuningModelListResponse:
+        """
+        List all fine tuning models
+
+        Returns:
+            FineTuningModelListResponse: The list of fine tuning models
+        """
+        resp = self.client.post(url="list_finetune_model")
+
+        return FineTuningModelListResponse(**resp.json())
+
+    def retrieve(self, model: str) -> FineTuningModelRetrieveResponse:
+        """
+        Retrieve a fine tuning model
+
+        Args:
+            model (str): The ID of the fine tuning model to retrieve
+
+        Returns:
+            FineTuningModelRetrieveResponse: The retrieved fine tuning model
+        """
+        json_body = {"model_id": model}
+
+        resp = self.client.post(url="retrieve_finetune_model", json=json_body)
+
+        return FineTuningModelRetrieveResponse(**resp.json())
+
+    def delete(self, model: str) -> BareResponse:
+        """
+        Delete a fine tuning model
+
+        Args:
+            model (str): The ID of the fine tuning model to delete
+
+        Returns:
+            BareResponse: The response from the API
+        """
+        json_body = {"model_id": model}
+
+        resp = self.client.post(url="delete_finetune_model", json=json_body)
+
+        return BareResponse(**resp.json())
+
+
+class AsyncModel(BaseAsyncInterface, Model):
+    """Asynchronous Model interface"""
+
+    async def list(self) -> FineTuningModelListResponse:
+        """
+        List all fine tuning models
+
+        Returns:
+            FineTuningModelListResponse: The list of fine tuning models
+        """
+        resp = await self.client.post(url="list_finetune_model")
+
+        return FineTuningModelListResponse(**resp.json())
+
+    async def retrieve(self, model: str) -> FineTuningModelRetrieveResponse:
+        """
+        Retrieve a fine tuning model
+
+        Args:
+            model (str): The ID of the fine tuning model to retrieve
+
+        Returns:
+            FineTuningModelRetrieveResponse: The retrieved fine tuning model
+        """
+        json_body = {"model_id": model}
+
+        resp = await self.client.post(url="retrieve_finetune_model", json=json_body)
+
+        return FineTuningModelRetrieveResponse(**resp.json())
+
+    async def delete(self, model: str) -> BareResponse:
+        """
+        Delete a fine tuning model
+
+        Args:
+            model (str): The ID of the fine tuning model to delete
+
+        Returns:
+            BareResponse: The response from the API
+        """
+        json_body = {"model_id": model}
+
+        resp = await self.client.post(url="delete_finetune_model", json=json_body)
+
+        return BareResponse(**resp.json())
```

### Comparing `minimax_client-0.5.0/tests/test_client.py` & `minimax_client-0.5.1/tests/test_client.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-"""test_client.py"""
-
-import os
-import unittest
-
-import httpx
-
-from minimax_client import AsyncMiniMax, MiniMax
-from minimax_client.interfaces.chat_completion import AsyncChat
-
-
-class TestMiniMax(unittest.TestCase):
-    """Unit tests for the MiniMax client."""
-
-    def test_init_without_api_key(self):
-        """Test that an error is raised if no API key is provided."""
-        with self.assertRaises(ValueError):
-            if os.environ.get("MINIMAX_API_KEY"):
-                del os.environ["MINIMAX_API_KEY"]
-
-            MiniMax()
-
-    def test_init_with_valid_api_key(self):
-        """Test that the client is initialized with a valid API key."""
-        client = MiniMax(api_key="valid_api_key")
-        self.assertEqual(client.api_key, "valid_api_key")
-
-    def test_del_closes_http_client(self):
-        """Test that the __del__ method closes the HTTP client."""
-        client = MiniMax(api_key="valid_api_key")
-        client.http_client.close()
-        self.assertTrue(client.http_client.is_closed)
-
-
-class TestAsyncMiniMax(unittest.IsolatedAsyncioTestCase):
-    """Unit tests for AsyncMiniMax"""
-
-    async def test_constructor(self) -> None:
-        """Test that the AsyncMiniMax constructor sets the API key and creates
-        an AsyncChat instance with the HTTP client"""
-        api_key = "test_api_key"
-        async_minimax = AsyncMiniMax(api_key=api_key)
-        self.assertEqual(async_minimax.api_key, api_key)
-        self.assertIsInstance(async_minimax.chat, AsyncChat)
-        self.assertIs(async_minimax.chat.completions.client, async_minimax.http_client)
-
-    async def test_del_closes_http_client(self) -> None:
-        """Test that the __del__ method closes the HTTP client"""
-        async_minimax = AsyncMiniMax(api_key="valid_api_key")
-        await async_minimax.http_client.aclose()
-        self.assertTrue(async_minimax.http_client.is_closed)
-
-    async def test_get_http_client(self) -> None:
-        """Test that _get_http_client returns a new AsyncClient instance with
-        the base URL and authorization header set"""
-        api_key = "test_api_key"
-        async_minimax = AsyncMiniMax(api_key=api_key)
-        http_client = async_minimax._get_http_client()
-        self.assertIsInstance(http_client, httpx.AsyncClient)
-        self.assertEqual(http_client.headers["Authorization"], f"Bearer {api_key}")
+"""test_client.py"""
+
+import os
+import unittest
+
+import httpx
+
+from minimax_client import AsyncMiniMax, MiniMax
+from minimax_client.interfaces.chat_completion import AsyncChat
+
+
+class TestMiniMax(unittest.TestCase):
+    """Unit tests for the MiniMax client."""
+
+    def test_init_without_api_key(self):
+        """Test that an error is raised if no API key is provided."""
+        with self.assertRaises(ValueError):
+            if os.environ.get("MINIMAX_API_KEY"):
+                del os.environ["MINIMAX_API_KEY"]
+
+            MiniMax()
+
+    def test_init_with_valid_api_key(self):
+        """Test that the client is initialized with a valid API key."""
+        client = MiniMax(api_key="valid_api_key")
+        self.assertEqual(client.api_key, "valid_api_key")
+
+    def test_del_closes_http_client(self):
+        """Test that the __del__ method closes the HTTP client."""
+        client = MiniMax(api_key="valid_api_key")
+        client.http_client.close()
+        self.assertTrue(client.http_client.is_closed)
+
+
+class TestAsyncMiniMax(unittest.IsolatedAsyncioTestCase):
+    """Unit tests for AsyncMiniMax"""
+
+    async def test_constructor(self) -> None:
+        """Test that the AsyncMiniMax constructor sets the API key and creates
+        an AsyncChat instance with the HTTP client"""
+        api_key = "test_api_key"
+        async_minimax = AsyncMiniMax(api_key=api_key)
+        self.assertEqual(async_minimax.api_key, api_key)
+        self.assertIsInstance(async_minimax.chat, AsyncChat)
+        self.assertIs(async_minimax.chat.completions.client, async_minimax.http_client)
+
+    async def test_del_closes_http_client(self) -> None:
+        """Test that the __del__ method closes the HTTP client"""
+        async_minimax = AsyncMiniMax(api_key="valid_api_key")
+        await async_minimax.http_client.aclose()
+        self.assertTrue(async_minimax.http_client.is_closed)
+
+    async def test_get_http_client(self) -> None:
+        """Test that _get_http_client returns a new AsyncClient instance with
+        the base URL and authorization header set"""
+        api_key = "test_api_key"
+        async_minimax = AsyncMiniMax(api_key=api_key)
+        http_client = async_minimax._get_http_client()
+        self.assertIsInstance(http_client, httpx.AsyncClient)
+        self.assertEqual(http_client.headers["Authorization"], f"Bearer {api_key}")
```

### Comparing `minimax_client-0.5.0/PKG-INFO` & `minimax_client-0.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minimax-client
-Version: 0.5.0
+Version: 0.5.1
 Summary: An (unofficial) python native client for easy interaction with MiniMax Open Platform
 Keywords: web api llm
 Author-Email: Zeyang Lin <4020306+linzeyang@users.noreply.github.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -46,14 +46,16 @@
 
 The current implementation includes the following official APIs offered by MiniMax:
 - ChatCompletion v2
 - Embeddings
 - File
 - Finetune
 - Assistants
+    - Assistant
+    - Assistant File
 
 ## Prerequisites
 - Python >= 3.8
 - pip (or any other tool that does the same job)
 - Internet connection
 - An API KEY acquired from [MiniMax Open Platform](https://www.minimaxi.com/user-center/basic-information/interface-key)
 
@@ -359,7 +361,38 @@
 
 client.assistants.retrieve(assistant_id=resp.id)
 
 client.assistants.list(limit=5)
 
 client.assistants.delete(assistant_id=resp.id)
 ```
+
+#### 2.12 Sync call for assistant files
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+resp = client.files.create(filepath="sample.txt", purpose="retrieval")
+
+file_id = resp.file.file_id
+
+resp = client.assistants.create(
+    model="abab5.5s-chat-240123",
+    name="test-assistant",
+    instructions="You are a helpful assistant.",
+    description="test-assistant",
+    tools=[{"type": "retrieval"}],
+)
+
+assistant_id = resp.id
+
+resp = client.assistants.files.create(assistant_id=assistant_id, file_id=str(file_id))
+
+resp = client.assistants.files.retrieve(assistant_id=assistant_id, file_id=str(file_id))
+
+resp = client.assistants.files.list(assistant_id=assistant_id, limit=5, order="asc")
+
+resp = client.assistants.files.delete(assistant_id=assistant_id, file_id=str(file_id))
+```
```

