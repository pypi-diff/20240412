# Comparing `tmp/livekit-plugins-silero-0.2.0.tar.gz` & `tmp/livekit-plugins-silero-0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-plugins-silero-0.2.0.tar", last modified: Tue Feb 20 16:17:05 2024, max compression
+gzip compressed data, was "livekit-plugins-silero-0.3.dev0.tar", last modified: Thu Apr 11 22:03:55 2024, max compression
```

## Comparing `livekit-plugins-silero-0.2.0.tar` & `livekit-plugins-silero-0.3.dev0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:17:05.668113 livekit-plugins-silero-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-02-20 16:17:05.668113 livekit-plugins-silero-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-20 16:16:50.000000 livekit-plugins-silero-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:17:05.664113 livekit-plugins-silero-0.2.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:17:05.668113 livekit-plugins-silero-0.2.0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:17:05.668113 livekit-plugins-silero-0.2.0/livekit/plugins/silero/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-02-20 16:16:50.000000 livekit-plugins-silero-0.2.0/livekit/plugins/silero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-02-20 16:16:50.000000 livekit-plugins-silero-0.2.0/livekit/plugins/silero/vad.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-20 16:16:50.000000 livekit-plugins-silero-0.2.0/livekit/plugins/silero/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:17:05.668113 livekit-plugins-silero-0.2.0/livekit_plugins_silero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-02-20 16:17:05.000000 livekit-plugins-silero-0.2.0/livekit_plugins_silero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-20 16:17:05.000000 livekit-plugins-silero-0.2.0/livekit_plugins_silero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 16:17:05.000000 livekit-plugins-silero-0.2.0/livekit_plugins_silero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-20 16:17:05.000000 livekit-plugins-silero-0.2.0/livekit_plugins_silero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-20 16:17:05.000000 livekit-plugins-silero-0.2.0/livekit_plugins_silero.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-20 16:16:50.000000 livekit-plugins-silero-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 16:17:05.668113 livekit-plugins-silero-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-02-20 16:16:50.000000 livekit-plugins-silero-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:55.044035 livekit-plugins-silero-0.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-11 22:03:55.044035 livekit-plugins-silero-0.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-11 22:03:50.000000 livekit-plugins-silero-0.3.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:55.040035 livekit-plugins-silero-0.3.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:55.040035 livekit-plugins-silero-0.3.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:55.040035 livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-11 22:03:50.000000 livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:50.000000 livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-11 22:03:50.000000 livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:03:50.000000 livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:55.044035 livekit-plugins-silero-0.3.dev0/livekit_plugins_silero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-11 22:03:55.000000 livekit-plugins-silero-0.3.dev0/livekit_plugins_silero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-11 22:03:55.000000 livekit-plugins-silero-0.3.dev0/livekit_plugins_silero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:03:55.000000 livekit-plugins-silero-0.3.dev0/livekit_plugins_silero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 22:03:55.000000 livekit-plugins-silero-0.3.dev0/livekit_plugins_silero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:03:55.000000 livekit-plugins-silero-0.3.dev0/livekit_plugins_silero.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:03:50.000000 livekit-plugins-silero-0.3.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:03:55.044035 livekit-plugins-silero-0.3.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-11 22:03:50.000000 livekit-plugins-silero-0.3.dev0/setup.py
```

### Comparing `livekit-plugins-silero-0.2.0/PKG-INFO` & `livekit-plugins-silero-0.3.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-silero
-Version: 0.2.0
+Version: 0.3.dev0
 Summary: Agent Framework Plugin for Silero
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -16,18 +16,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit>=0.9.0
-Requires-Dist: livekit-agents>=0.4.0
+Requires-Dist: livekit~=0.9
+Requires-Dist: livekit-agents~=0.5.dev0
 Requires-Dist: torch<3,>=2
+Requires-Dist: torchaudio>=2
 Requires-Dist: numpy<2,>=1
+Requires-Dist: onnxruntime~=1.17.0
 
 # LiveKit Plugins Silero
 
 Agent Framework Plugin for Silero. Currently supports Voice Activity Detection.
 
 ## Installation
```

### Comparing `livekit-plugins-silero-0.2.0/livekit/plugins/silero/__init__.py` & `livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 # limitations under the License.
 
 from .vad import VAD, VADStream
 from .version import __version__
 
 __all__ = ["VAD", "VADStream", "__version__"]
 
-from livekit.agents import Plugin
 import torch
+from livekit.agents import Plugin
 
 
 class SileroPlugin(Plugin):
     def __init__(self):
-        super().__init__(__name__, __version__)
+        super().__init__(__name__, __version__, __package__)
 
     def download_files(self):
         _ = torch.hub.load(
             repo_or_dir="snakers4/silero-vad",
             model="silero_vad",
         )
```

### Comparing `livekit-plugins-silero-0.2.0/livekit/plugins/silero/vad.py` & `livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/vad.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,27 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from __future__ import annotations
+
+import asyncio
 import contextlib
 import logging
-import asyncio
+from collections import deque
 from typing import List, Optional
-from livekit import rtc, agents
-import torch
+
 import numpy as np
-from collections import deque
+import torch
+from livekit import agents, rtc
 
 
 class VAD(agents.vad.VAD):
     def __init__(
-        self, *, model_path: Optional[str] = None, use_onnx: bool = False
+        self, *, model_path: Optional[str] = None, use_onnx: bool = True
     ) -> None:
         if model_path:
             model = torch.jit.load(model_path)
             model.eval()
         else:
             model, _ = torch.hub.load(
                 repo_or_dir="snakers4/silero-vad",
@@ -77,16 +80,16 @@
         self._sample_rate = sample_rate
         self._max_buffered_speech = max_buffered_speech
         self._threshold = threshold
 
         if sample_rate not in [8000, 16000]:
             raise ValueError("Silero VAD only supports 8KHz and 16KHz sample rates")
 
-        self._queue = asyncio.Queue[rtc.AudioFrame]()
-        self._event_queue = asyncio.Queue[agents.vad.VADEvent]()
+        self._queue = asyncio.Queue[rtc.AudioFrame | None]()
+        self._event_queue = asyncio.Queue[agents.vad.VADEvent | None]()
         self._model = model
 
         self._closed = False
         self._speaking = False
         self._waiting_start = False
         self._waiting_end = False
         self._current_sample = 0
@@ -103,53 +106,57 @@
         def log_exception(task: asyncio.Task) -> None:
             if not task.cancelled() and task.exception():
                 logging.error(f"silero vad task failed: {task.exception()}")
 
         self._main_task.add_done_callback(log_exception)
 
     def push_frame(self, frame: rtc.AudioFrame) -> None:
+        if self._closed:
+            raise ValueError("cannot push frame to closed stream")
+
         self._queue.put_nowait(frame)
 
-    async def flush(self) -> None:
-        await self._queue.join()
+    async def aclose(self, *, wait: bool = True) -> None:
+        self._closed = True
+        if not wait:
+            self._main_task.cancel()
 
-    async def aclose(self) -> None:
-        self._main_task.cancel()
+        self._queue.put_nowait(None)
         with contextlib.suppress(asyncio.CancelledError):
             await self._main_task
 
     async def _run(self):
-        while True:
-            try:
-                frame = await self._queue.get()
-            except asyncio.CancelledError:
-                break
-
-            self._queue.task_done()
-
-            # resample to silero's sample rate
-            resampled_frame = frame.remix_and_resample(
-                self._sample_rate, 1
-            )  # TODO: This is technically wrong, fix when we have a better resampler
-            self._original_frames.append(frame)
-            self._queued_frames.append(resampled_frame)
-
-            # run inference by chunks of 40ms until we run out of data
+        try:
             while True:
-                available_length = sum(
-                    f.samples_per_channel for f in self._queued_frames
-                )
-
-                samples_40ms = self._sample_rate // 1000 * 40
-                if available_length < samples_40ms:
-                    break
+                frame = await self._queue.get()
+                if frame is None:
+                    break  # None is sent inside aclose
 
-                await asyncio.shield(self._run_inference())
+                self._queue.task_done()
 
-        self._closed = True
+                # resample to silero's sample rate
+                resampled_frame = frame.remix_and_resample(
+                    self._sample_rate, 1
+                )  # TODO: This is technically wrong, fix when we have a better resampler
+                self._original_frames.append(frame)
+                self._queued_frames.append(resampled_frame)
+
+                # run inference by chunks of 40ms until we run out of data
+                while True:
+                    available_length = sum(
+                        f.samples_per_channel for f in self._queued_frames
+                    )
+
+                    samples_40ms = self._sample_rate // 1000 * 40
+                    if available_length < samples_40ms:
+                        break
+
+                    await asyncio.shield(self._run_inference())
+        finally:
+            self._event_queue.put_nowait(None)
 
     async def _run_inference(self) -> None:
         # merge the first 4 frames (we know each is 10ms)
         if len(self._queued_frames) < 4:
             return
 
         original_frames = [self._original_frames.popleft() for _ in range(4)]
@@ -158,16 +165,16 @@
         )
 
         # convert data_40ms to tensor & f32
         tensor = torch.from_numpy(np.frombuffer(merged_frame.data, dtype=np.int16))
         tensor = tensor.to(torch.float32) / 32768.0
 
         # run inference
-        speech_prob = await asyncio.get_event_loop().run_in_executor(
-            None, lambda: self._model(tensor, self._sample_rate).item()
+        speech_prob = await asyncio.to_thread(
+            lambda: self._model(tensor, self._sample_rate).item()
         )
         self._dispatch_event(speech_prob, original_frames)
         self._current_sample += merged_frame.samples_per_channel
 
     def _dispatch_event(self, speech_prob: int, original_frames: List[rtc.AudioFrame]):
         """
         Dispatches a VAD event based on the speech probability and the options
@@ -188,47 +195,47 @@
             and len(self._buffered_frames) > padding_count
         ):
             self._buffered_frames = self._buffered_frames[
                 len(self._buffered_frames) - padding_count :
             ]
 
         max_buffer_len = padding_count + max(
-            self._max_buffered_samples // samples_10ms,
-            self._min_speaking_samples // samples_10ms,
+            int(self._max_buffered_samples // samples_10ms),
+            int(self._min_speaking_samples // samples_10ms),
         )
         if len(self._buffered_frames) > max_buffer_len:
             # if unaware of this, may be hard to debug, so logging seems ok here
             logging.warning(
                 f"VAD buffer overflow, dropping {len(self._buffered_frames) - max_buffer_len} frames"
             )
             self._buffered_frames = self._buffered_frames[
                 len(self._buffered_frames) - max_buffer_len :
             ]
 
         if speech_prob >= self._threshold:
-            # speaking, wait for min_speaking_duration to trigger START_SPEAKING
+            # speaking, wait for min_speaking_duration to trigger START_OF_SPEECH
             self._waiting_end = False
             if not self._waiting_start and not self._speaking:
                 self._waiting_start = True
                 self._start_speech = self._current_sample
 
             if self._waiting_start and (
                 self._current_sample - self._start_speech >= self._min_speaking_samples
             ):
                 self._waiting_start = False
                 self._speaking = True
                 event = agents.vad.VADEvent(
-                    type=agents.vad.VADEventType.START_SPEAKING,
+                    type=agents.vad.VADEventType.START_OF_SPEECH,
                     samples_index=self._start_speech,
                 )
                 self._event_queue.put_nowait(event)
 
-                # since we're waiting for the min_spaking_duration to trigger START_SPEAKING,
+                # since we're waiting for the min_spaking_duration to trigger START_OF_SPEECH,
                 # the SPEAKING data is missing the first few frames, trigger it here
-                # TODO(theomonnom): Maybe it is better to put the data inside the START_SPEAKING event?
+                # TODO(theomonnom): Maybe it is better to put the data inside the START_OF_SPEECH event?
                 event = agents.vad.VADEvent(
                     type=agents.vad.VADEventType.SPEAKING,
                     samples_index=self._start_speech,
                     speech=self._buffered_frames[padding_count:],
                 )
 
                 return
@@ -239,33 +246,34 @@
                 type=agents.vad.VADEventType.SPEAKING,
                 samples_index=self._current_sample,
                 speech=original_frames,
             )
             self._event_queue.put_nowait(event)
 
         if speech_prob < self._threshold:
-            # stopped speaking, wait for min_silence_duration to trigger END_SPEAKING
+            # stopped speaking, wait for min_silence_duration to trigger END_OF_SPEECH,
             self._waiting_start = False
             if not self._waiting_end and self._speaking:
                 self._waiting_end = True
                 self._end_speech = self._current_sample
 
             if self._waiting_end and (
                 self._current_sample - self._end_speech
                 >= max(self._min_silence_samples, self._padding_duration_samples)
             ):
                 self._waiting_end = False
                 self._speaking = False
                 event = agents.vad.VADEvent(
-                    type=agents.vad.VADEventType.END_SPEAKING,
+                    type=agents.vad.VADEventType.END_OF_SPEECH,
                     samples_index=self._end_speech,
                     duration=(self._current_sample - self._start_speech)
                     / self._sample_rate,
                     speech=self._buffered_frames,
                 )
                 self._event_queue.put_nowait(event)
 
     async def __anext__(self) -> agents.vad.VADEvent:
-        if self._closed and self._event_queue.empty():
+        evt = await self._event_queue.get()
+        if evt is None:
             raise StopAsyncIteration
 
-        return await self._event_queue.get()
+        return evt
```

### Comparing `livekit-plugins-silero-0.2.0/livekit/plugins/silero/version.py` & `livekit-plugins-silero-0.3.dev0/livekit/plugins/silero/version.py`

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

### Comparing `livekit-plugins-silero-0.2.0/livekit_plugins_silero.egg-info/PKG-INFO` & `livekit-plugins-silero-0.3.dev0/livekit_plugins_silero.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-silero
-Version: 0.2.0
+Version: 0.3.dev0
 Summary: Agent Framework Plugin for Silero
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -16,18 +16,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit>=0.9.0
-Requires-Dist: livekit-agents>=0.4.0
+Requires-Dist: livekit~=0.9
+Requires-Dist: livekit-agents~=0.5.dev0
 Requires-Dist: torch<3,>=2
+Requires-Dist: torchaudio>=2
 Requires-Dist: numpy<2,>=1
+Requires-Dist: onnxruntime~=1.17.0
 
 # LiveKit Plugins Silero
 
 Agent Framework Plugin for Silero. Currently supports Voice Activity Detection.
 
 ## Installation
```

### Comparing `livekit-plugins-silero-0.2.0/setup.py` & `livekit-plugins-silero-0.3.dev0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 import os
 import pathlib
 
 import setuptools
 import setuptools.command.build_py
 
-
 here = pathlib.Path(__file__).parent.resolve()
 about = {}
 with open(os.path.join(here, "livekit", "plugins", "silero", "version.py"), "r") as f:
     exec(f.read(), about)
 
 
 setuptools.setup(
@@ -46,18 +45,20 @@
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.8.0",
     install_requires=[
-        "livekit >= 0.9.0",
-        "livekit-agents >= 0.4.0",
+        "livekit ~= 0.9",
+        "livekit-agents~=0.5.dev0",
         "torch >= 2, < 3",
+        "torchaudio >= 2",
         "numpy >= 1, < 2",
+        "onnxruntime~=1.17.0",
     ],
     package_data={"livekit.plugins.silero": ["files/silero_vad.jit"]},
     project_urls={
         "Documentation": "https://docs.livekit.io",
         "Website": "https://livekit.io/",
         "Source": "https://github.com/livekit/agents",
     },
```

