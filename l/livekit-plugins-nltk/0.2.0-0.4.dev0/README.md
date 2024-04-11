# Comparing `tmp/livekit-plugins-nltk-0.2.0.tar.gz` & `tmp/livekit-plugins-nltk-0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-plugins-nltk-0.2.0.tar", last modified: Tue Feb 20 16:16:57 2024, max compression
+gzip compressed data, was "livekit-plugins-nltk-0.4.dev0.tar", last modified: Thu Apr 11 22:03:41 2024, max compression
```

## Comparing `livekit-plugins-nltk-0.2.0.tar` & `livekit-plugins-nltk-0.4.dev0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:57.705083 livekit-plugins-nltk-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-02-20 16:16:57.705083 livekit-plugins-nltk-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-20 16:16:44.000000 livekit-plugins-nltk-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:57.701084 livekit-plugins-nltk-0.2.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:57.701084 livekit-plugins-nltk-0.2.0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:57.705083 livekit-plugins-nltk-0.2.0/livekit/plugins/nltk/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-02-20 16:16:44.000000 livekit-plugins-nltk-0.2.0/livekit/plugins/nltk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-02-20 16:16:44.000000 livekit-plugins-nltk-0.2.0/livekit/plugins/nltk/sentence_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-20 16:16:44.000000 livekit-plugins-nltk-0.2.0/livekit/plugins/nltk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:57.705083 livekit-plugins-nltk-0.2.0/livekit_plugins_nltk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-02-20 16:16:57.000000 livekit-plugins-nltk-0.2.0/livekit_plugins_nltk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-20 16:16:57.000000 livekit-plugins-nltk-0.2.0/livekit_plugins_nltk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 16:16:57.000000 livekit-plugins-nltk-0.2.0/livekit_plugins_nltk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-20 16:16:57.000000 livekit-plugins-nltk-0.2.0/livekit_plugins_nltk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-20 16:16:57.000000 livekit-plugins-nltk-0.2.0/livekit_plugins_nltk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-20 16:16:44.000000 livekit-plugins-nltk-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 16:16:57.705083 livekit-plugins-nltk-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-02-20 16:16:44.000000 livekit-plugins-nltk-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:41.785523 livekit-plugins-nltk-0.4.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-11 22:03:41.785523 livekit-plugins-nltk-0.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:41.781523 livekit-plugins-nltk-0.4.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:41.781523 livekit-plugins-nltk-0.4.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:41.781523 livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/sentence_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:41.785523 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-11 22:03:41.000000 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-11 22:03:41.000000 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:03:41.000000 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 22:03:41.000000 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:03:41.000000 livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:03:41.785523 livekit-plugins-nltk-0.4.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-11 22:03:37.000000 livekit-plugins-nltk-0.4.dev0/setup.py
```

### Comparing `livekit-plugins-nltk-0.2.0/PKG-INFO` & `livekit-plugins-nltk-0.4.dev0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-nltk
-Version: 0.2.0
+Version: 0.4.dev0
 Summary: Agent Framework plugin for NLTK-based text processing.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -14,16 +14,17 @@
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit>=0.9.0
+Requires-Dist: livekit~=0.9
 Requires-Dist: nltk<4,>=3
+Requires-Dist: livekit-agents~=0.5.dev0
 
 # LiveKit Plugins NLTK
 
 Agent Framework plugin for [NLTK](https://www.nltk.org/)-based text processing. Currently featuring a `SentenceTokenizer`.
 
 ## Installation
```

### Comparing `livekit-plugins-nltk-0.2.0/livekit/plugins/nltk/__init__.py` & `livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,31 +9,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from .sentence_tokenizer import SentenceTokenizer, SentenceStream
+from .sentence_tokenizer import SentenceStream, SentenceTokenizer
 from .version import __version__
 
 __all__ = [
     "SentenceTokenizer",
     "SentenceStream",
     "__version__",
 ]
 
 
 from livekit.agents import Plugin
-import nltk
+
+import nltk  # type: ignore
 
 
 class NltkPlugin(Plugin):
     def __init__(self):
-        super().__init__(__name__, __version__)
+        super().__init__(__name__, __version__, __package__)
 
     def download_files(self):
         try:
             _ = nltk.data.find("tokenizers/punkt")
         except LookupError:
             nltk.download("punkt")
```

### Comparing `livekit-plugins-nltk-0.2.0/livekit/plugins/nltk/sentence_tokenizer.py` & `livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/sentence_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from typing import List
-from livekit import agents
-from dataclasses import dataclass
-import dataclasses
-from typing import Optional
+from __future__ import annotations
+
 import asyncio
-import nltk
+import dataclasses
+import logging
+from dataclasses import dataclass
+from typing import List, Optional
+
+from livekit import agents
+
+import nltk  # type: ignore
 
 # nltk is using the punkt tokenizer
 # https://www.nltk.org/_modules/nltk/tokenize/punkt.html
 # this code is using a whitespace to concatenate small sentences together
 # (languages such as Chinese and Japanese are not yet supported)
 
 
@@ -73,20 +77,25 @@
 class SentenceStream(agents.tokenize.SentenceStream):
     def __init__(
         self, *, language: str, min_sentence_len: int, context_len: int
     ) -> None:
         self._language = language
         self._context_len = context_len
         self._min_sentence_len = min_sentence_len
-        self._event_queue = asyncio.Queue()
+        self._event_queue = asyncio.Queue[agents.tokenize.SegmentedSentence | None]()
+        self._closed = False
 
-        self._incomplete_sentences = []  # <= min_sentence_len
+        self._incomplete_sentences: List[str] = []  # <= min_sentence_len
         self._buffer = ""
 
     def push_text(self, text: str) -> None:
+        if self._closed:
+            logging.error("Cannot push text to closed stream")
+            return
+
         for char in text:
             self._buffer += char
 
             if len(self._buffer) < self._context_len:
                 continue
 
             sentences = nltk.tokenize.sent_tokenize(self._buffer, self._language)
@@ -114,15 +123,20 @@
                     agents.tokenize.SegmentedSentence(text=buff)
                 )
                 buff = ""
 
         if buff:
             await self._event_queue.put(agents.tokenize.SegmentedSentence(text=buff))
 
+    async def aclose(self) -> None:
+        self._closed = True
+        self._event_queue.put_nowait(None)
+
     async def __anext__(self) -> agents.tokenize.SegmentedSentence:
-        if self._event_queue.empty():
+        event = await self._event_queue.get()
+        if event is None:
             raise StopAsyncIteration
 
-        return await self._event_queue.get()
+        return event
 
     def __aiter__(self) -> "SentenceStream":
         return self
```

### Comparing `livekit-plugins-nltk-0.2.0/livekit/plugins/nltk/version.py` & `livekit-plugins-nltk-0.4.dev0/livekit/plugins/nltk/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.0"
+__version__ = "0.4.dev0"
```

### Comparing `livekit-plugins-nltk-0.2.0/livekit_plugins_nltk.egg-info/PKG-INFO` & `livekit-plugins-nltk-0.4.dev0/livekit_plugins_nltk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-nltk
-Version: 0.2.0
+Version: 0.4.dev0
 Summary: Agent Framework plugin for NLTK-based text processing.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -14,16 +14,17 @@
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit>=0.9.0
+Requires-Dist: livekit~=0.9
 Requires-Dist: nltk<4,>=3
+Requires-Dist: livekit-agents~=0.5.dev0
 
 # LiveKit Plugins NLTK
 
 Agent Framework plugin for [NLTK](https://www.nltk.org/)-based text processing. Currently featuring a `SentenceTokenizer`.
 
 ## Installation
```

### Comparing `livekit-plugins-nltk-0.2.0/setup.py` & `livekit-plugins-nltk-0.4.dev0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 import os
 import pathlib
 
 import setuptools
 import setuptools.command.build_py
 
-
 here = pathlib.Path(__file__).parent.resolve()
 about = {}
 with open(os.path.join(here, "livekit", "plugins", "nltk", "version.py"), "r") as f:
     exec(f.read(), about)
 
 
 setuptools.setup(
@@ -43,14 +42,21 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.9.0",
-    install_requires=["livekit >= 0.9.0", "nltk >= 3, < 4"],
+    install_requires=[
+        "livekit~=0.9",
+        "nltk >= 3, < 4",
+        "livekit-agents~=0.5.dev0",
+    ],
+    package_data={
+        "livekit.plugins.nltk": ["py.typed"],
+    },
     project_urls={
         "Documentation": "https://docs.livekit.io",
         "Website": "https://livekit.io/",
         "Source": "https://github.com/livekit/agents",
     },
 )
```

