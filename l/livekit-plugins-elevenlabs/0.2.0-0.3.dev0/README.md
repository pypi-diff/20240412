# Comparing `tmp/livekit-plugins-elevenlabs-0.2.0.tar.gz` & `tmp/livekit-plugins-elevenlabs-0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-plugins-elevenlabs-0.2.0.tar", last modified: Tue Feb 20 16:16:42 2024, max compression
+gzip compressed data, was "livekit-plugins-elevenlabs-0.3.dev0.tar", last modified: Thu Apr 11 22:03:31 2024, max compression
```

## Comparing `livekit-plugins-elevenlabs-0.2.0.tar` & `livekit-plugins-elevenlabs-0.3.dev0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:42.643627 livekit-plugins-elevenlabs-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-02-20 16:16:42.643627 livekit-plugins-elevenlabs-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-20 16:16:34.000000 livekit-plugins-elevenlabs-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:42.639627 livekit-plugins-elevenlabs-0.2.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:42.639627 livekit-plugins-elevenlabs-0.2.0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:42.639627 livekit-plugins-elevenlabs-0.2.0/livekit/plugins/elevenlabs/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-20 16:16:34.000000 livekit-plugins-elevenlabs-0.2.0/livekit/plugins/elevenlabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-20 16:16:34.000000 livekit-plugins-elevenlabs-0.2.0/livekit/plugins/elevenlabs/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-02-20 16:16:34.000000 livekit-plugins-elevenlabs-0.2.0/livekit/plugins/elevenlabs/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-20 16:16:34.000000 livekit-plugins-elevenlabs-0.2.0/livekit/plugins/elevenlabs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:42.643627 livekit-plugins-elevenlabs-0.2.0/livekit_plugins_elevenlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-02-20 16:16:42.000000 livekit-plugins-elevenlabs-0.2.0/livekit_plugins_elevenlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-20 16:16:42.000000 livekit-plugins-elevenlabs-0.2.0/livekit_plugins_elevenlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 16:16:42.000000 livekit-plugins-elevenlabs-0.2.0/livekit_plugins_elevenlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-20 16:16:42.000000 livekit-plugins-elevenlabs-0.2.0/livekit_plugins_elevenlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-20 16:16:42.000000 livekit-plugins-elevenlabs-0.2.0/livekit_plugins_elevenlabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-20 16:16:34.000000 livekit-plugins-elevenlabs-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 16:16:42.643627 livekit-plugins-elevenlabs-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-02-20 16:16:34.000000 livekit-plugins-elevenlabs-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:31.954548 livekit-plugins-elevenlabs-0.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-11 22:03:31.954548 livekit-plugins-elevenlabs-0.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:31.950547 livekit-plugins-elevenlabs-0.3.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:31.950547 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:31.954548 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:31.954548 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-11 22:03:31.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-11 22:03:31.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:03:31.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 22:03:31.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:03:31.000000 livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:03:31.954548 livekit-plugins-elevenlabs-0.3.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-11 22:03:27.000000 livekit-plugins-elevenlabs-0.3.dev0/setup.py
```

### Comparing `livekit-plugins-elevenlabs-0.2.0/PKG-INFO` & `livekit-plugins-elevenlabs-0.3.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-elevenlabs
-Version: 0.2.0
+Version: 0.3.dev0
 Summary: Agent Framework plugin for voice synthesis with ElevenLabs' API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,elevenlabs
@@ -15,16 +15,16 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit>=0.9.0
-Requires-Dist: livekit-agents>=0.3.0
+Requires-Dist: livekit~=0.9
+Requires-Dist: livekit-agents~=0.5.dev0
 Requires-Dist: aiohttp>=3.8.5
 
 # LiveKit Plugins Elevenlabs
 
 Agent Framework plugin for voice synthesis with [ElevenLabs](https://elevenlabs.io/) API.
 
 ## Installation
```

### Comparing `livekit-plugins-elevenlabs-0.2.0/livekit/plugins/elevenlabs/__init__.py` & `livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,25 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-from .tts import TTS, Voice, VoiceSettings, DEFAULT_VOICE
+from .tts import DEFAULT_VOICE, TTS, Voice, VoiceSettings
 from .version import __version__
 
 __all__ = ["TTS", "Voice", "VoiceSettings", "DEFAULT_VOICE", "__version__"]
 
 from livekit.agents import Plugin
 
 
 class ElevenLabsPlugin(Plugin):
     def __init__(self):
-        super().__init__(__name__, __version__)
+        super().__init__(__name__, __version__, __package__)
 
     def download_files(self):
         pass
 
 
 Plugin.register_plugin(ElevenLabsPlugin())
```

### Comparing `livekit-plugins-elevenlabs-0.2.0/livekit/plugins/elevenlabs/tts.py` & `livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/tts.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import contextlib
 import asyncio
-import logging
 import base64
+import contextlib
 import dataclasses
 import json
+import logging
 import os
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import Any, AsyncIterable, Dict, List, Optional
+
 import aiohttp
 from livekit import rtc
 from livekit.agents import tts
+
 from .models import TTSModels
 
 
 @dataclass
 class Voice:
     id: str
     name: str
@@ -97,45 +99,48 @@
         async with self._session.get(
             f"{self._config.base_url}/voices",
             headers={AUTHORIZATION_HEADER: self._config.api_key},
         ) as resp:
             data = await resp.json()
             return dict_to_voices_list(data)
 
-    async def synthesize(
+    def synthesize(
         self,
-        *,
         text: str,
-    ) -> tts.SynthesizedAudio:
+    ) -> AsyncIterable[tts.SynthesizedAudio]:
         voice = self._config.voice
-        async with self._session.post(
-            f"{self._config.base_url}/text-to-speech/{voice.id}?output_format=pcm_44100",
-            headers={AUTHORIZATION_HEADER: self._config.api_key},
-            json=dict(
-                text=text,
-                model_id=self._config.model_id,
-                voice_settings=dataclasses.asdict(voice.settings)
-                if voice.settings
-                else None,
-            ),
-        ) as resp:
-            data = await resp.read()
-            return tts.SynthesizedAudio(
-                text=text,
-                data=rtc.AudioFrame(
-                    data=data,
-                    sample_rate=44100,
-                    num_channels=1,
-                    samples_per_channel=len(data) // 2,  # 16-bit
+
+        async def generator():
+            async with self._session.post(
+                f"{self._config.base_url}/text-to-speech/{voice.id}?output_format=pcm_44100",
+                headers={AUTHORIZATION_HEADER: self._config.api_key},
+                json=dict(
+                    text=text,
+                    model_id=self._config.model_id,
+                    voice_settings=dataclasses.asdict(voice.settings)
+                    if voice.settings
+                    else None,
                 ),
-            )
+            ) as resp:
+                data = await resp.read()
+                yield tts.SynthesizedAudio(
+                    text=text,
+                    data=rtc.AudioFrame(
+                        data=data,
+                        sample_rate=44100,
+                        num_channels=1,
+                        samples_per_channel=len(data) // 2,  # 16-bit
+                    ),
+                )
+
+        return generator()
 
     def stream(
         self,
-    ) -> tts.SynthesizeStream:
+    ) -> "SynthesizeStream":
         return SynthesizeStream(self._session, self._config)
 
 
 class SynthesizeStream(tts.SynthesizeStream):
     def __init__(
         self,
         session: aiohttp.ClientSession,
@@ -159,15 +164,15 @@
 
     def _stream_url(self) -> str:
         base_url = self._config.base_url
         voice_id = self._config.voice.id
         model_id = self._config.model_id
         return f"{base_url}/text-to-speech/{voice_id}/stream-input?model_id={model_id}&output_format=pcm_{self._config.sample_rate}&optimize_streaming_latency={self._config.latency}"
 
-    def push_text(self, token: str) -> None:
+    def push_text(self, token: str | None) -> None:
         if self._closed:
             raise ValueError("cannot push to a closed stream")
 
         if not token or len(token) == 0:
             return
 
         # TODO: Native word boundary detection may not be good enough for all languages
@@ -279,41 +284,45 @@
                 aiohttp.WSMsgType.CLOSING,
             ):
                 break
 
             if msg.type != aiohttp.WSMsgType.TEXT:
                 continue
 
-            msg = json.loads(msg.data)
-            if msg.get("audio"):
-                data = base64.b64decode(msg["audio"])
+            jsonMessage: Dict[str, Any] = json.loads(str(msg.data))
+            if jsonMessage.get("audio"):
+                data = base64.b64decode(jsonMessage["audio"])
                 audio_frame = rtc.AudioFrame(
                     data=data,
                     sample_rate=self._config.sample_rate,
                     num_channels=1,
                     samples_per_channel=len(data) // 2,
                 )
                 self._event_queue.put_nowait(
                     tts.SynthesisEvent(
                         type=tts.SynthesisEventType.AUDIO,
                         audio=tts.SynthesizedAudio(text="", data=audio_frame),
                     )
                 )
-            elif msg.get("isFinal"):
+            elif jsonMessage.get("isFinal"):
                 break
             else:
                 logging.error(f"Unhandled message from ElevenLabs: {msg}")
 
     async def flush(self) -> None:
         self._queue.put_nowait(self._text + " ")
         self._text = ""
         self._queue.put_nowait(STREAM_EOS)
         await self._queue.join()
 
-    async def aclose(self) -> None:
+    async def aclose(self, wait=False) -> None:
+        if wait:
+            logging.warning(
+                "wait=True is not yet supported for ElevenLabs TTS. Closing immediately."
+            )
         self._main_task.cancel()
         with contextlib.suppress(asyncio.CancelledError):
             await self._main_task
 
     async def __anext__(self) -> tts.SynthesisEvent:
         if self._closed and self._event_queue.empty():
             raise StopAsyncIteration
```

### Comparing `livekit-plugins-elevenlabs-0.2.0/livekit/plugins/elevenlabs/version.py` & `livekit-plugins-elevenlabs-0.3.dev0/livekit/plugins/elevenlabs/version.py`

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

### Comparing `livekit-plugins-elevenlabs-0.2.0/livekit_plugins_elevenlabs.egg-info/PKG-INFO` & `livekit-plugins-elevenlabs-0.3.dev0/livekit_plugins_elevenlabs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-elevenlabs
-Version: 0.2.0
+Version: 0.3.dev0
 Summary: Agent Framework plugin for voice synthesis with ElevenLabs' API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,elevenlabs
@@ -15,16 +15,16 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit>=0.9.0
-Requires-Dist: livekit-agents>=0.3.0
+Requires-Dist: livekit~=0.9
+Requires-Dist: livekit-agents~=0.5.dev0
 Requires-Dist: aiohttp>=3.8.5
 
 # LiveKit Plugins Elevenlabs
 
 Agent Framework plugin for voice synthesis with [ElevenLabs](https://elevenlabs.io/) API.
 
 ## Installation
```

### Comparing `livekit-plugins-elevenlabs-0.2.0/setup.py` & `livekit-plugins-elevenlabs-0.3.dev0/setup.py`

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
 with open(
     os.path.join(here, "livekit", "plugins", "elevenlabs", "version.py"), "r"
 ) as f:
     exec(f.read(), about)
 
@@ -47,18 +46,20 @@
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit", "elevenlabs"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.9.0",
     install_requires=[
-        "livekit >= 0.9.0",
-        "livekit-agents >= 0.3.0",
+        "livekit ~= 0.9",
+        "livekit-agents~=0.5.dev0",
         "aiohttp >= 3.8.5",
     ],
-    package_data={},
+    package_data={
+        "livekit.plugins.elevenlabs": ["py.typed"],
+    },
     project_urls={
         "Documentation": "https://docs.livekit.io",
         "Website": "https://livekit.io/",
         "Source": "https://github.com/livekit/agents",
     },
 )
```

