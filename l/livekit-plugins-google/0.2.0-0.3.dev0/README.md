# Comparing `tmp/livekit-plugins-google-0.2.0.tar.gz` & `tmp/livekit-plugins-google-0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-plugins-google-0.2.0.tar", last modified: Tue Feb 20 16:16:45 2024, max compression
+gzip compressed data, was "livekit-plugins-google-0.3.dev0.tar", last modified: Thu Apr 11 22:03:37 2024, max compression
```

## Comparing `livekit-plugins-google-0.2.0.tar` & `livekit-plugins-google-0.3.dev0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:45.844178 livekit-plugins-google-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-02-20 16:16:45.844178 livekit-plugins-google-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-20 16:16:38.000000 livekit-plugins-google-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:45.844178 livekit-plugins-google-0.2.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:45.844178 livekit-plugins-google-0.2.0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:45.844178 livekit-plugins-google-0.2.0/livekit/plugins/google/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-20 16:16:38.000000 livekit-plugins-google-0.2.0/livekit/plugins/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-02-20 16:16:38.000000 livekit-plugins-google-0.2.0/livekit/plugins/google/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-02-20 16:16:38.000000 livekit-plugins-google-0.2.0/livekit/plugins/google/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-20 16:16:38.000000 livekit-plugins-google-0.2.0/livekit/plugins/google/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:45.844178 livekit-plugins-google-0.2.0/livekit_plugins_google.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-02-20 16:16:45.000000 livekit-plugins-google-0.2.0/livekit_plugins_google.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-20 16:16:45.000000 livekit-plugins-google-0.2.0/livekit_plugins_google.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 16:16:45.000000 livekit-plugins-google-0.2.0/livekit_plugins_google.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-20 16:16:45.000000 livekit-plugins-google-0.2.0/livekit_plugins_google.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-20 16:16:45.000000 livekit-plugins-google-0.2.0/livekit_plugins_google.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-20 16:16:38.000000 livekit-plugins-google-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 16:16:45.844178 livekit-plugins-google-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-02-20 16:16:38.000000 livekit-plugins-google-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:37.733574 livekit-plugins-google-0.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-11 22:03:37.733574 livekit-plugins-google-0.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:37.729574 livekit-plugins-google-0.3.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:37.729574 livekit-plugins-google-0.3.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:37.733574 livekit-plugins-google-0.3.dev0/livekit/plugins/google/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/livekit/plugins/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/livekit/plugins/google/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/livekit/plugins/google/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/livekit/plugins/google/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/livekit/plugins/google/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:03:37.733574 livekit-plugins-google-0.3.dev0/livekit_plugins_google.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-11 22:03:37.000000 livekit-plugins-google-0.3.dev0/livekit_plugins_google.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-11 22:03:37.000000 livekit-plugins-google-0.3.dev0/livekit_plugins_google.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:03:37.000000 livekit-plugins-google-0.3.dev0/livekit_plugins_google.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-11 22:03:37.000000 livekit-plugins-google-0.3.dev0/livekit_plugins_google.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:03:37.000000 livekit-plugins-google-0.3.dev0/livekit_plugins_google.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:03:37.733574 livekit-plugins-google-0.3.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-11 22:03:33.000000 livekit-plugins-google-0.3.dev0/setup.py
```

### Comparing `livekit-plugins-google-0.2.0/PKG-INFO` & `livekit-plugins-google-0.3.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-google
-Version: 0.2.0
+Version: 0.3.dev0
 Summary: Agent Framework plugin for services from Google Cloud
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -25,16 +25,16 @@
 Requires-Dist: google-api-core<3,>=2
 Requires-Dist: google-auth<3,>=2
 Requires-Dist: google-cloud-core<3,>=2
 Requires-Dist: google-cloud-speech<3,>=2
 Requires-Dist: google-cloud-texttospeech<3,>=2
 Requires-Dist: google-cloud-translate<4,>=3
 Requires-Dist: googleapis-common-protos<2,>=1
-Requires-Dist: livekit>=0.9.0
-Requires-Dist: livekit-agents>=0.3.0
+Requires-Dist: livekit>=0.9.2
+Requires-Dist: livekit-agents~=0.5.dev0
 
 # LiveKit Plugins Google
 
 Agent Framework plugin for services from Google Cloud. Currently supporting Google's [Speech-to-Text](https://cloud.google.com/speech-to-text) API.
 
 ## Installation
```

### Comparing `livekit-plugins-google-0.2.0/README.md` & `livekit-plugins-google-0.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `livekit-plugins-google-0.2.0/livekit/plugins/google/__init__.py` & `livekit-plugins-google-0.3.dev0/livekit/plugins/google/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 __all__ = ["STT", "SpeechStream", "__version__"]
 
 from livekit.agents import Plugin
 
 
 class GooglePlugin(Plugin):
     def __init__(self):
-        super().__init__(__name__, __version__)
+        super().__init__(__name__, __version__, __package__)
 
     def download_files(self):
         pass
 
 
 Plugin.register_plugin(GooglePlugin())
```

### Comparing `livekit-plugins-google-0.2.0/livekit/plugins/google/models.py` & `livekit-plugins-google-0.3.dev0/livekit/plugins/google/models.py`

 * *Files identical despite different names*

### Comparing `livekit-plugins-google-0.2.0/livekit/plugins/google/stt.py` & `livekit-plugins-google-0.3.dev0/livekit/plugins/google/stt.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,31 +8,35 @@
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
-from typing import Optional, Union, List
-from google.auth import credentials
-from google.cloud.speech_v2 import SpeechAsyncClient
-from google.cloud.speech_v2.types import cloud_speech
-from livekit import rtc, agents
-from livekit.agents.utils import AudioBuffer
-from livekit.agents import stt
-from .models import SpeechModels, SpeechLanguages
-from dataclasses import dataclass
 import dataclasses
-import asyncio
 import logging
+from dataclasses import dataclass
+from typing import Any, AsyncIterable, Dict, List
 
+from livekit import agents, rtc
+from livekit.agents import stt
+from livekit.agents.utils import AudioBuffer
+
+from google.auth import credentials  # type: ignore
+from google.cloud.speech_v2 import SpeechAsyncClient
+from google.cloud.speech_v2.types import cloud_speech
 
-LgType = Union[SpeechLanguages, str]
-LanguageCode = Union[LgType, List[LgType]]
+from .models import SpeechLanguages, SpeechModels
+
+LgType = SpeechLanguages | str
+LanguageCode = LgType | List[LgType]
 
 
 # This class is only be used internally to encapsulate the options
 @dataclass
 class STTOptions:
     languages: List[LgType]
     detect_language: bool
@@ -48,16 +52,16 @@
         *,
         languages: LanguageCode = "en-US",  # Google STT can accept multiple languages
         detect_language: bool = True,
         interim_results: bool = True,
         punctuate: bool = True,
         spoken_punctuation: bool = True,
         model: SpeechModels = "long",
-        credentials_info: Optional[dict] = None,
-        credentials_file: Optional[str] = None,
+        credentials_info: Dict[str, Any] | None = None,
+        credentials_file: str | None = None,
     ):
         """
         if no credentials is provided, it will use the credentials on the environment
         GOOGLE_APPLICATION_CREDENTIALS (Default behavior of Google SpeechAsyncClient)
         """
         super().__init__(streaming_supported=True)
 
@@ -86,15 +90,15 @@
         # TODO(theomonnom): should we use recognizers?
         # Recognizers may improve latency https://cloud.google.com/speech-to-text/v2/docs/recognizers#understand_recognizers
         return f"projects/{self._creds.project_id}/locations/global/recognizers/_"  # type: ignore
 
     def _sanitize_options(
         self,
         *,
-        language: Optional[str] = None,
+        language: str | None = None,
     ) -> STTOptions:
         config = dataclasses.replace(self._config)
 
         if language:
             config.languages = [language]
 
         if not isinstance(config.languages, list):
@@ -108,15 +112,15 @@
 
         return config
 
     async def recognize(
         self,
         *,
         buffer: AudioBuffer,
-        language: Optional[Union[SpeechLanguages, str]] = None,
+        language: SpeechLanguages | str | None = None,
     ) -> stt.SpeechEvent:
         config = self._sanitize_options(language=language)
         buffer = agents.utils.merge_frames(buffer)
 
         config = cloud_speech.RecognitionConfig(
             explicit_decoding_config=cloud_speech.ExplicitDecodingConfig(
                 encoding=cloud_speech.ExplicitDecodingConfig.AudioEncoding.LINEAR16,
@@ -140,15 +144,15 @@
                 )
             )
         )
 
     def stream(
         self,
         *,
-        language: Optional[Union[SpeechLanguages, str]] = None,
+        language: SpeechLanguages | str | None = None,
     ) -> "SpeechStream":
         config = self._sanitize_options(language=language)
         return SpeechStream(
             self._client,
             self._creds,
             self._recognizer,
             config,
@@ -160,159 +164,239 @@
         self,
         client: SpeechAsyncClient,
         creds: credentials.Credentials,
         recognizer: str,
         config: STTOptions,
         sample_rate: int = 24000,
         num_channels: int = 1,
+        max_retry: int = 32,
     ) -> None:
         super().__init__()
 
         self._client = client
         self._creds = creds
         self._recognizer = recognizer
         self._config = config
         self._sample_rate = sample_rate
         self._num_channels = num_channels
 
-        self._queue = asyncio.Queue[rtc.AudioFrame]()
-        self._event_queue = asyncio.Queue[stt.SpeechEvent]()
+        self._queue = asyncio.Queue[rtc.AudioFrame | None]()
+        self._event_queue = asyncio.Queue[stt.SpeechEvent | None]()
         self._closed = False
-        self._main_task = asyncio.create_task(self._run(max_retry=32))
-
-        def log_exception(task: asyncio.Task) -> None:
-            if not task.cancelled() and task.exception():
-                logging.error(f"google speech task failed: {task.exception()}")
+        self._main_task = asyncio.create_task(self._run(max_retry=max_retry))
 
-        self._main_task.add_done_callback(log_exception)
-
-    def push_frame(self, frame: rtc.AudioFrame) -> None:
-        if self._closed:
-            raise ValueError("cannot push frame to closed stream")
-
-        self._queue.put_nowait(frame)
-
-    async def flush(self) -> None:
-        await self._queue.join()
-
-    async def aclose(self) -> None:
-        self._main_task.cancel()
-        with contextlib.suppress(asyncio.CancelledError):
-            await self._main_task
+        self._final_events: List[stt.SpeechEvent] = []
+        self._speaking = False
 
-    def _streaming_config(self) -> cloud_speech.StreamingRecognitionConfig:
-        return cloud_speech.StreamingRecognitionConfig(
+        self._streaming_config = cloud_speech.StreamingRecognitionConfig(
             config=cloud_speech.RecognitionConfig(
                 explicit_decoding_config=cloud_speech.ExplicitDecodingConfig(
                     encoding=cloud_speech.ExplicitDecodingConfig.AudioEncoding.LINEAR16,
                     sample_rate_hertz=self._sample_rate,
                     audio_channel_count=self._num_channels,
                 ),
                 language_codes=self._config.languages,
                 model=self._config.model,
                 features=cloud_speech.RecognitionFeatures(
                     enable_automatic_punctuation=self._config.punctuate,
                 ),
             ),
             streaming_features=cloud_speech.StreamingRecognitionFeatures(
+                enable_voice_activity_events=True,
                 interim_results=self._config.interim_results,
             ),
         )
 
+        def log_exception(task: asyncio.Task) -> None:
+            if not task.cancelled() and task.exception():
+                logging.error(f"google stt task failed: {task.exception()}")
+
+        self._main_task.add_done_callback(log_exception)
+
+    def push_frame(self, frame: rtc.AudioFrame) -> None:
+        if self._closed:
+            raise ValueError("cannot push frame to closed stream")
+
+        self._queue.put_nowait(frame)
+
+    async def aclose(self, wait: bool = True) -> None:
+        self._closed = True
+        if not wait:
+            self._main_task.cancel()
+
+        self._queue.put_nowait(None)
+        with contextlib.suppress(asyncio.CancelledError):
+            await self._main_task
+
     async def _run(self, max_retry: int) -> None:
-        """Try to connect to Google Speech API and forward frames"""
         retry_count = 0
-        while True:
-            try:
-                input_gen = self._input_gen(self._streaming_config())
-                stream = await self._client.streaming_recognize(requests=input_gen)
-                retry_count = 0
-
-                async for resp in stream:
-                    self._event_queue.put_nowait(
-                        streaming_recognize_response_to_speech_event(resp)
+        try:
+            while not self._closed:
+                try:
+                    # google requires a async generator when calling streaming_recognize
+                    # this function basically convert the queue into a async generator
+                    async def input_generator():
+                        try:
+                            # first request should contain the config
+                            yield cloud_speech.StreamingRecognizeRequest(
+                                recognizer=self._recognizer,
+                                streaming_config=self._streaming_config,
+                            )
+                            while True:
+                                frame = (
+                                    await self._queue.get()
+                                )  # wait for a new rtc.AudioFrame
+                                if frame is None:
+                                    break  # None is sent inside aclose
+
+                                self._queue.task_done()
+                                frame = frame.remix_and_resample(
+                                    self._sample_rate, self._num_channels
+                                )
+                                yield cloud_speech.StreamingRecognizeRequest(
+                                    audio=frame.data.tobytes(),
+                                )
+                        except Exception as e:
+                            logging.error(
+                                f"an error occurred while streaming inputs: {e}"
+                            )
+
+                    # try to connect
+                    stream = await self._client.streaming_recognize(
+                        requests=input_generator()
                     )
+                    retry_count = 0  # connection successful, reset retry count
 
-            except asyncio.CancelledError:
-                break
-            except Exception as e:
-                if retry_count > max_retry and max_retry > 0:
-                    logging.error(f"failed to connect to Google Speech: {e}")
-                    break
+                    await self._run_stream(stream)
+                except Exception as e:
+                    if retry_count >= max_retry:
+                        logging.error(
+                            f"failed to connect to google stt after {max_retry} tries",
+                            exc_info=e,
+                        )
+                        break
+
+                    retry_delay = min(retry_count * 2, 10)  # max 10s
+                    retry_count += 1
+                    logging.warning(
+                        f"google stt connection failed, retrying in {retry_delay}s",
+                        exc_info=e,
+                    )
+                    await asyncio.sleep(retry_delay)
+        finally:
+            self._event_queue.put_nowait(None)
 
-                retry_delay = min(retry_count * 5, 5)  # max 5s
-                retry_count += 1
-                logging.warning(
-                    f"failed to connect to Google Speech: {e} - retrying in {retry_delay}s"
+    async def _run_stream(
+        self, stream: AsyncIterable[cloud_speech.StreamingRecognizeResponse]
+    ):
+        async for resp in stream:
+            if (
+                resp.speech_event_type
+                == cloud_speech.StreamingRecognizeResponse.SpeechEventType.SPEECH_ACTIVITY_BEGIN
+            ):
+                self._speaking = True
+                start_event = stt.SpeechEvent(
+                    type=stt.SpeechEventType.START_OF_SPEECH,
                 )
-                await asyncio.sleep(retry_delay)
+                self._event_queue.put_nowait(start_event)
 
-        self._closed = True
+            if (
+                resp.speech_event_type
+                == cloud_speech.StreamingRecognizeResponse.SpeechEventType.SPEECH_EVENT_TYPE_UNSPECIFIED
+            ):
+                result = resp.results[0]
+                if not result.is_final:
+                    # interim results
+                    iterim_event = stt.SpeechEvent(
+                        type=stt.SpeechEventType.INTERIM_TRANSCRIPT,
+                        alternatives=streaming_recognize_response_to_speech_data(resp),
+                    )
+                    self._event_queue.put_nowait(iterim_event)
 
-    async def _input_gen(self, config):
-        """
-        Convert our input queue to a generator (needed by the Google Speech client in Python)
-        """
-        try:
-            yield cloud_speech.StreamingRecognizeRequest(
-                recognizer=self._recognizer,
-                streaming_config=config,
-            )
-            while True:
-                frame = await self._queue.get()  # wait for a new rtc.AudioFrame
-                frame = frame.remix_and_resample(self._sample_rate, self._num_channels)
-                yield cloud_speech.StreamingRecognizeRequest(
-                    audio=frame.data.tobytes(),
-                )
-                self._queue.task_done()
-        except Exception as e:
-            logging.error(f"an error occurred while streaming inputs: {e}")
+                else:
+                    final_event = stt.SpeechEvent(
+                        type=stt.SpeechEventType.FINAL_TRANSCRIPT,
+                        alternatives=streaming_recognize_response_to_speech_data(resp),
+                    )
+                    self._final_events.append(final_event)
+                    self._event_queue.put_nowait(final_event)
+
+                    if not self._speaking:
+                        # With Google STT, we receive the final event after the END_OF_SPEECH event
+                        sentence = ""
+                        confidence = 0.0
+                        for alt in self._final_events:
+                            sentence += f"{alt.alternatives[0].text.strip()} "
+                            confidence += alt.alternatives[0].confidence
+
+                        sentence = sentence.rstrip()
+                        confidence /= len(self._final_events)  # avg. of confidence
+
+                        end_event = stt.SpeechEvent(
+                            type=stt.SpeechEventType.END_OF_SPEECH,
+                            alternatives=[
+                                stt.SpeechData(
+                                    language=result.language_code,
+                                    start_time=self._final_events[0]
+                                    .alternatives[0]
+                                    .start_time,
+                                    end_time=self._final_events[-1]
+                                    .alternatives[0]
+                                    .end_time,
+                                    confidence=confidence,
+                                    text=sentence,
+                                )
+                            ],
+                        )
+
+                        self._final_events = []
+                        self._event_queue.put_nowait(end_event)
+
+            if (
+                resp.speech_event_type
+                == cloud_speech.StreamingRecognizeResponse.SpeechEventType.SPEECH_ACTIVITY_END
+            ):
+                self._speaking = False
 
     async def __anext__(self) -> stt.SpeechEvent:
-        if self._closed and self._event_queue.empty():
+        evt = await self._event_queue.get()
+        if evt is None:
             raise StopAsyncIteration
 
-        return await self._event_queue.get()
+        return evt
 
 
 def recognize_response_to_speech_event(
     resp: cloud_speech.RecognizeResponse,
 ) -> stt.SpeechEvent:
     result = resp.results[0]
     gg_alts = result.alternatives
     return stt.SpeechEvent(
-        is_final=True,
-        end_of_speech=True,
+        type=stt.SpeechEventType.FINAL_TRANSCRIPT,
         alternatives=[
             stt.SpeechData(
                 language=result.language_code,
                 start_time=alt.words[0].start_offset.seconds if alt.words else 0,
                 end_time=alt.words[-1].end_offset.seconds if alt.words else 0,
                 confidence=alt.confidence,
                 text=alt.transcript,
             )
             for alt in gg_alts
         ],
     )
 
 
-def streaming_recognize_response_to_speech_event(
+def streaming_recognize_response_to_speech_data(
     resp: cloud_speech.StreamingRecognizeResponse,
-) -> stt.SpeechEvent:
+) -> List[stt.SpeechData]:
     result = resp.results[0]
     gg_alts = result.alternatives
-    return stt.SpeechEvent(
-        is_final=result.is_final,
-        # Google STT does not have a separate end_of_speech indicator
-        # so we'll use is_final
-        end_of_speech=result.is_final,
-        alternatives=[
-            stt.SpeechData(
-                language=result.language_code,
-                start_time=alt.words[0].start_offset.seconds if alt.words else 0,
-                end_time=alt.words[-1].end_offset.seconds if alt.words else 0,
-                confidence=alt.confidence,
-                text=alt.transcript,
-            )
-            for alt in gg_alts
-        ],
-    )
+    return [
+        stt.SpeechData(
+            language=result.language_code,
+            start_time=alt.words[0].start_offset.seconds if alt.words else 0,
+            end_time=alt.words[-1].end_offset.seconds if alt.words else 0,
+            confidence=alt.confidence,
+            text=alt.transcript,
+        )
+        for alt in gg_alts
+    ]
```

### Comparing `livekit-plugins-google-0.2.0/livekit/plugins/google/version.py` & `livekit-plugins-google-0.3.dev0/livekit/plugins/google/version.py`

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

### Comparing `livekit-plugins-google-0.2.0/livekit_plugins_google.egg-info/PKG-INFO` & `livekit-plugins-google-0.3.dev0/livekit_plugins_google.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-google
-Version: 0.2.0
+Version: 0.3.dev0
 Summary: Agent Framework plugin for services from Google Cloud
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -25,16 +25,16 @@
 Requires-Dist: google-api-core<3,>=2
 Requires-Dist: google-auth<3,>=2
 Requires-Dist: google-cloud-core<3,>=2
 Requires-Dist: google-cloud-speech<3,>=2
 Requires-Dist: google-cloud-texttospeech<3,>=2
 Requires-Dist: google-cloud-translate<4,>=3
 Requires-Dist: googleapis-common-protos<2,>=1
-Requires-Dist: livekit>=0.9.0
-Requires-Dist: livekit-agents>=0.3.0
+Requires-Dist: livekit>=0.9.2
+Requires-Dist: livekit-agents~=0.5.dev0
 
 # LiveKit Plugins Google
 
 Agent Framework plugin for services from Google Cloud. Currently supporting Google's [Speech-to-Text](https://cloud.google.com/speech-to-text) API.
 
 ## Installation
```

### Comparing `livekit-plugins-google-0.2.0/setup.py` & `livekit-plugins-google-0.3.dev0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 import os
 import pathlib
 
 import setuptools
 import setuptools.command.build_py
 
-
 here = pathlib.Path(__file__).parent.resolve()
 about = {}
 with open(os.path.join(here, "livekit", "plugins", "google", "version.py"), "r") as f:
     exec(f.read(), about)
 
 
 setuptools.setup(
@@ -55,17 +54,19 @@
         "google-api-core >= 2, < 3",
         "google-auth >= 2, < 3",
         "google-cloud-core >= 2, < 3",
         "google-cloud-speech >= 2, < 3",
         "google-cloud-texttospeech >= 2, < 3",
         "google-cloud-translate >= 3, < 4",
         "googleapis-common-protos >= 1, < 2",
-        "livekit >= 0.9.0",
-        "livekit-agents >= 0.3.0",
+        "livekit >= 0.9.2",
+        "livekit-agents~=0.5.dev0",
     ],
-    package_data={},
+    package_data={
+        "livekit.plugins.google": ["py.typed"],
+    },
     project_urls={
         "Documentation": "https://docs.livekit.io",
         "Website": "https://livekit.io/",
         "Source": "https://github.com/livekit/agents",
     },
 )
```

