# Comparing `tmp/livekit-plugins-openai-0.2.0.tar.gz` & `tmp/livekit-plugins-openai-0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-plugins-openai-0.2.0.tar", last modified: Tue Feb 20 16:17:19 2024, max compression
+gzip compressed data, was "livekit-plugins-openai-0.3.dev0.tar", last modified: Thu Apr 11 22:03:54 2024, max compression
```

## Comparing `livekit-plugins-openai-0.2.0.tar` & `livekit-plugins-openai-0.3.dev0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:17:19.089604 livekit-plugins-openai-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-20 16:17:19.085605 livekit-plugins-openai-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-20 16:16:49.000000 livekit-plugins-openai-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:17:19.085605 livekit-plugins-openai-0.2.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:17:19.085605 livekit-plugins-openai-0.2.0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:17:19.085605 livekit-plugins-openai-0.2.0/livekit/plugins/openai/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-02-20 16:16:49.000000 livekit-plugins-openai-0.2.0/livekit/plugins/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-02-20 16:16:49.000000 livekit-plugins-openai-0.2.0/livekit/plugins/openai/dalle3.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-20 16:16:49.000000 livekit-plugins-openai-0.2.0/livekit/plugins/openai/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-02-20 16:16:49.000000 livekit-plugins-openai-0.2.0/livekit/plugins/openai/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-02-20 16:16:49.000000 livekit-plugins-openai-0.2.0/livekit/plugins/openai/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-20 16:16:49.000000 livekit-plugins-openai-0.2.0/livekit/plugins/openai/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:17:19.085605 livekit-plugins-openai-0.2.0/livekit_plugins_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-20 16:17:19.000000 livekit-plugins-openai-0.2.0/livekit_plugins_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-02-20 16:17:19.000000 livekit-plugins-openai-0.2.0/livekit_plugins_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 16:17:19.000000 livekit-plugins-openai-0.2.0/livekit_plugins_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-20 16:17:19.000000 livekit-plugins-openai-0.2.0/livekit_plugins_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-20 16:17:19.000000 livekit-plugins-openai-0.2.0/livekit_plugins_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-20 16:16:49.000000 livekit-plugins-openai-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 16:17:19.089604 livekit-plugins-openai-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-02-20 16:16:49.000000 livekit-plugins-openai-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:54.473533 livekit-plugins-openai-0.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-11 22:03:54.473533 livekit-plugins-openai-0.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:54.469533 livekit-plugins-openai-0.3.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:54.469533 livekit-plugins-openai-0.3.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:54.469533 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:54.469533 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-11 22:03:54.000000 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-11 22:03:54.000000 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:03:54.000000 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 22:03:54.000000 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:03:54.000000 livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:03:54.473533 livekit-plugins-openai-0.3.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-11 22:03:46.000000 livekit-plugins-openai-0.3.dev0/setup.py
```

### Comparing `livekit-plugins-openai-0.2.0/PKG-INFO` & `livekit-plugins-openai-0.3.dev0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-openai
-Version: 0.2.0
+Version: 0.3.dev0
 Summary: Agent Framework plugin for services from OpenAI
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -15,22 +15,17 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit>=0.9.0
-Requires-Dist: livekit-agents>=0.3.0
-Requires-Dist: torch<3,>=2
-Requires-Dist: torchaudio<3,>=2
-Requires-Dist: numpy>=1.24.0
-Requires-Dist: openai~=1.7.2
-Requires-Dist: audioread<4,>=3
-Requires-Dist: opencv-python<5,>=4
+Requires-Dist: livekit~=0.9
+Requires-Dist: livekit-agents~=0.5.dev0
+Requires-Dist: openai>=1.0.0
 Requires-Dist: requests<3,>=2
 
 # LiveKit Plugins OpenAI
 
 Agent Framework plugin for services from OpenAI. Currently supports STT, TTS, and Dalle 3.
 
 ## Installation
```

### Comparing `livekit-plugins-openai-0.2.0/livekit/plugins/openai/__init__.py` & `livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .models import WhisperModels, TTSModels, TTSVoices
+from .llm import LLM
+from .models import TTSModels, TTSVoices, WhisperModels
 from .stt import STT
 from .tts import TTS
-from .dalle3 import Dalle3
 from .version import __version__
 
 __all__ = [
     "STT",
     "TTS",
+    "LLM",
     "WhisperModels",
     "TTSModels",
     "TTSVoices",
-    "Dalle3",
     "__version__",
 ]
 
 from livekit.agents import Plugin
 
 
 class OpenAIPlugin(Plugin):
-    def __init__(self):
-        super().__init__(__name__, __version__)
+    def __init__(self) -> None:
+        super().__init__(__name__, __version__, __package__)
 
-    def download_files(self):
+    def download_files(self) -> None:
         pass
 
 
 Plugin.register_plugin(OpenAIPlugin())
```

### Comparing `livekit-plugins-openai-0.2.0/livekit/plugins/openai/stt.py` & `livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/stt.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,24 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from __future__ import annotations
+
 import dataclasses
-import os
 import io
+import os
 import wave
-from typing import Optional
 from dataclasses import dataclass
+
 from livekit import agents
-from livekit.agents.utils import AudioBuffer
 from livekit.agents import stt
+from livekit.agents.utils import AudioBuffer
+
 import openai
+
 from .models import WhisperModels
 
 
 @dataclass
 class STTOptions:
     language: str
     detect_language: bool
@@ -35,15 +39,15 @@
 class STT(stt.STT):
     def __init__(
         self,
         *,
         language: str = "en",
         detect_language: bool = False,
         model: WhisperModels = "whisper-1",
-        api_key: Optional[str] = None,
+        api_key: str | None = None,
     ):
         super().__init__(streaming_supported=False)
         api_key = api_key or os.environ.get("OPENAI_API_KEY")
         if not api_key:
             raise ValueError("OPENAI_API_KEY must be set")
 
         self._client = openai.AsyncOpenAI(api_key=api_key)
@@ -56,25 +60,25 @@
             detect_language=detect_language,
             model=model,
         )
 
     def _sanitize_options(
         self,
         *,
-        language: Optional[str] = None,
+        language: str | None = None,
     ) -> STTOptions:
         config = dataclasses.replace(self._config)
         config.language = language or config.language
         return config
 
     async def recognize(
         self,
         *,
         buffer: AudioBuffer,
-        language: Optional[str] = None,
+        language: str | None = None,
     ) -> stt.SpeechEvent:
         config = self._sanitize_options(language=language)
 
         buffer = agents.utils.merge_frames(buffer)
         io_buffer = io.BytesIO()
         with wave.open(io_buffer, "wb") as wav:
             wav.setnchannels(buffer.num_channels)
@@ -84,16 +88,15 @@
 
         resp = await self._client.audio.transcriptions.create(
             file=("a.wav", io_buffer),
             model=config.model,
             language=config.language,
             response_format="json",
         )
-        return transcription_to_speech_event(resp)
+        return transcription_to_speech_event(resp, config.language)
 
 
-def transcription_to_speech_event(transcription) -> stt.SpeechEvent:
+def transcription_to_speech_event(transcription, language) -> stt.SpeechEvent:
     return stt.SpeechEvent(
-        is_final=True,
-        end_of_speech=True,
-        alternatives=[stt.SpeechData(text=transcription.text, language="")],
+        type=stt.SpeechEventType.FINAL_TRANSCRIPT,
+        alternatives=[stt.SpeechData(text=transcription.text, language=language)],
     )
```

### Comparing `livekit-plugins-openai-0.2.0/livekit/plugins/openai/version.py` & `livekit-plugins-openai-0.3.dev0/livekit/plugins/openai/version.py`

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
+__version__ = "0.3.dev0"
```

### Comparing `livekit-plugins-openai-0.2.0/livekit_plugins_openai.egg-info/PKG-INFO` & `livekit-plugins-openai-0.3.dev0/livekit_plugins_openai.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-openai
-Version: 0.2.0
+Version: 0.3.dev0
 Summary: Agent Framework plugin for services from OpenAI
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -15,22 +15,17 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit>=0.9.0
-Requires-Dist: livekit-agents>=0.3.0
-Requires-Dist: torch<3,>=2
-Requires-Dist: torchaudio<3,>=2
-Requires-Dist: numpy>=1.24.0
-Requires-Dist: openai~=1.7.2
-Requires-Dist: audioread<4,>=3
-Requires-Dist: opencv-python<5,>=4
+Requires-Dist: livekit~=0.9
+Requires-Dist: livekit-agents~=0.5.dev0
+Requires-Dist: openai>=1.0.0
 Requires-Dist: requests<3,>=2
 
 # LiveKit Plugins OpenAI
 
 Agent Framework plugin for services from OpenAI. Currently supports STT, TTS, and Dalle 3.
 
 ## Installation
```

### Comparing `livekit-plugins-openai-0.2.0/setup.py` & `livekit-plugins-openai-0.3.dev0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 import os
 import pathlib
 
 import setuptools
 import setuptools.command.build_py
 
-
 here = pathlib.Path(__file__).parent.resolve()
 about = {}
 with open(os.path.join(here, "livekit", "plugins", "openai", "version.py"), "r") as f:
     exec(f.read(), about)
 
 
 setuptools.setup(
@@ -45,24 +44,21 @@
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.9.0",
     install_requires=[
-        "livekit >= 0.9.0",
-        "livekit-agents >= 0.3.0",
-        "torch >= 2, < 3",
-        "torchaudio >= 2, < 3",
-        "numpy >= 1.24.0",
-        "openai ~= 1.7.2",
-        "audioread >= 3, < 4",
-        "opencv-python >= 4, < 5",
+        "livekit ~= 0.9",
+        "livekit-agents~=0.5.dev0",
+        "openai >= 1.0.0",
         "requests >= 2, < 3",
     ],
-    package_data={},
+    package_data={
+        "livekit.plugins.openai": ["py.typed"],
+    },
     project_urls={
         "Documentation": "https://docs.livekit.io",
         "Website": "https://livekit.io/",
         "Source": "https://github.com/livekit/agents",
     },
 )
```

