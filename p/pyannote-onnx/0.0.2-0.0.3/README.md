# Comparing `tmp/pyannote-onnx-0.0.2.tar.gz` & `tmp/pyannote-onnx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyannote-onnx-0.0.2.tar", last modified: Sat Apr  6 09:37:50 2024, max compression
+gzip compressed data, was "pyannote-onnx-0.0.3.tar", last modified: Fri Apr 12 06:31:44 2024, max compression
```

## Comparing `pyannote-onnx-0.0.2.tar` & `pyannote-onnx-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pengzhendong   (501) staff       (20)        0 2024-04-06 09:37:50.508364 pyannote-onnx-0.0.2/
--rw-r--r--   0 pengzhendong   (501) staff       (20)    11357 2024-04-04 15:32:09.000000 pyannote-onnx-0.0.2/LICENSE
--rw-r--r--   0 pengzhendong   (501) staff       (20)       64 2024-04-06 08:53:56.000000 pyannote-onnx-0.0.2/MANIFEST.in
--rw-r--r--   0 pengzhendong   (501) staff       (20)     1534 2024-04-06 09:37:50.508018 pyannote-onnx-0.0.2/PKG-INFO
--rw-r--r--   0 pengzhendong   (501) staff       (20)     1020 2024-04-06 01:01:05.000000 pyannote-onnx-0.0.2/README.md
-drwxr-xr-x   0 pengzhendong   (501) staff       (20)        0 2024-04-06 09:37:50.501541 pyannote-onnx-0.0.2/pyannote_onnx/
--rw-r--r--   0 pengzhendong   (501) staff       (20)      636 2024-04-04 15:32:09.000000 pyannote-onnx-0.0.2/pyannote_onnx/__init__.py
--rw-r--r--   0 pengzhendong   (501) staff       (20)     1398 2024-04-04 15:32:09.000000 pyannote-onnx-0.0.2/pyannote_onnx/inference_session.py
--rw-r--r--   0 pengzhendong   (501) staff       (20)    12846 2024-04-06 08:51:54.000000 pyannote-onnx-0.0.2/pyannote_onnx/pyannote_onnx.py
--rw-r--r--   0 pengzhendong   (501) staff       (20)  5983836 2024-04-04 15:32:09.000000 pyannote-onnx-0.0.2/pyannote_onnx/segmentation-3.0.onnx
-drwxr-xr-x   0 pengzhendong   (501) staff       (20)        0 2024-04-06 09:37:50.507708 pyannote-onnx-0.0.2/pyannote_onnx.egg-info/
--rw-r--r--   0 pengzhendong   (501) staff       (20)     1534 2024-04-06 09:37:50.000000 pyannote-onnx-0.0.2/pyannote_onnx.egg-info/PKG-INFO
--rw-r--r--   0 pengzhendong   (501) staff       (20)      407 2024-04-06 09:37:50.000000 pyannote-onnx-0.0.2/pyannote_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 pengzhendong   (501) staff       (20)        1 2024-04-06 09:37:50.000000 pyannote-onnx-0.0.2/pyannote_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 pengzhendong   (501) staff       (20)       42 2024-04-06 09:37:50.000000 pyannote-onnx-0.0.2/pyannote_onnx.egg-info/entry_points.txt
--rw-r--r--   0 pengzhendong   (501) staff       (20)       42 2024-04-06 09:37:50.000000 pyannote-onnx-0.0.2/pyannote_onnx.egg-info/requires.txt
--rw-r--r--   0 pengzhendong   (501) staff       (20)       14 2024-04-06 09:37:50.000000 pyannote-onnx-0.0.2/pyannote_onnx.egg-info/top_level.txt
--rw-r--r--   0 pengzhendong   (501) staff       (20)       42 2024-04-06 08:54:53.000000 pyannote-onnx-0.0.2/requirements.txt
--rw-r--r--   0 pengzhendong   (501) staff       (20)       38 2024-04-06 09:37:50.508413 pyannote-onnx-0.0.2/setup.cfg
--rw-r--r--   0 pengzhendong   (501) staff       (20)     1530 2024-04-06 08:54:18.000000 pyannote-onnx-0.0.2/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-12 06:31:44.529967 pyannote-onnx-0.0.3/
+-rw-r--r--   0 admin      (501) staff       (20)    11357 2024-04-12 01:55:28.000000 pyannote-onnx-0.0.3/LICENSE
+-rw-r--r--   0 admin      (501) staff       (20)       64 2024-04-12 01:55:28.000000 pyannote-onnx-0.0.3/MANIFEST.in
+-rw-r--r--   0 admin      (501) staff       (20)     1534 2024-04-12 06:31:44.529719 pyannote-onnx-0.0.3/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     1020 2024-04-12 01:55:28.000000 pyannote-onnx-0.0.3/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-12 06:31:44.525130 pyannote-onnx-0.0.3/pyannote_onnx/
+-rw-r--r--   0 admin      (501) staff       (20)      636 2024-04-12 01:55:28.000000 pyannote-onnx-0.0.3/pyannote_onnx/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1398 2024-04-12 01:55:28.000000 pyannote-onnx-0.0.3/pyannote_onnx/inference_session.py
+-rw-r--r--   0 admin      (501) staff       (20)    13799 2024-04-12 06:29:25.000000 pyannote-onnx-0.0.3/pyannote_onnx/pyannote_onnx.py
+-rw-r--r--   0 admin      (501) staff       (20)  5983836 2024-04-12 01:55:28.000000 pyannote-onnx-0.0.3/pyannote_onnx/segmentation-3.0.onnx
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-12 06:31:44.529433 pyannote-onnx-0.0.3/pyannote_onnx.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1534 2024-04-12 06:31:44.000000 pyannote-onnx-0.0.3/pyannote_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      407 2024-04-12 06:31:44.000000 pyannote-onnx-0.0.3/pyannote_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-04-12 06:31:44.000000 pyannote-onnx-0.0.3/pyannote_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       42 2024-04-12 06:31:44.000000 pyannote-onnx-0.0.3/pyannote_onnx.egg-info/entry_points.txt
+-rw-r--r--   0 admin      (501) staff       (20)       42 2024-04-12 06:31:44.000000 pyannote-onnx-0.0.3/pyannote_onnx.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       14 2024-04-12 06:31:44.000000 pyannote-onnx-0.0.3/pyannote_onnx.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       42 2024-04-12 01:55:28.000000 pyannote-onnx-0.0.3/requirements.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2024-04-12 06:31:44.530010 pyannote-onnx-0.0.3/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1530 2024-04-12 06:30:37.000000 pyannote-onnx-0.0.3/setup.py
```

### Comparing `pyannote-onnx-0.0.2/LICENSE` & `pyannote-onnx-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.2/PKG-INFO` & `pyannote-onnx-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyannote-onnx
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pyannote ONNX
 Home-page: https://github.com/pengzhendong/pyannote-onnx
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `pyannote-onnx-0.0.2/README.md` & `pyannote-onnx-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.2/pyannote_onnx/__init__.py` & `pyannote-onnx-0.0.3/pyannote_onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.2/pyannote_onnx/inference_session.py` & `pyannote-onnx-0.0.3/pyannote_onnx/inference_session.py`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.2/pyannote_onnx/pyannote_onnx.py` & `pyannote-onnx-0.0.3/pyannote_onnx/pyannote_onnx.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,41 +10,68 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from functools import partial
+from itertools import permutations
 from pathlib import Path
 from typing import Union
 
 import librosa
 import numpy as np
 import soundfile as sf
+from numpy.linalg import norm
 
 from .inference_session import PickableInferenceSession
 
 
 class PyannoteONNX:
     def __init__(self):
         # segmentation-3.0 classes:
         #   1. {no speech}
         #   2. {spk1}
         #   3. {spk2}
         #   4. {spk3}
         #   5. {spk1, spk2}
         #   6. {spk1, spk3}
         #   7. {spk2, spk3}
-        self.num_classes = 7
+        # only keep the first 4 classes
+        #   1. {speech}
+        #   2. {spk1}
+        #   3. {spk2}
+        #   4. {spk3}
+        self.num_classes = 4
         self.sample_rate = 16000
         self.duration = 10 * self.sample_rate
         onnx_model = f"{os.path.dirname(__file__)}/segmentation-3.0.onnx"
         self.session = PickableInferenceSession(onnx_model)
 
     @staticmethod
+    def sample2frame(x):
+        # Conv1d & MaxPool1d & SincNet:
+        #   * https://pytorch.org/docs/stable/generated/torch.nn.Conv1d.html
+        #   * https://pytorch.org/docs/stable/generated/torch.nn.MaxPool1d.html
+        #   * https://github.com/pyannote/pyannote-audio/blob/develop/pyannote/audio/models/blocks/sincnet.py#L50-L71
+        #            kernel_size  stride
+        # Conv1d             251      10
+        # MaxPool1d            3       3
+        # Conv1d               5       1
+        # MaxPool1d            3       3
+        # Conv1d               5       1
+        # MaxPool1d            3       3
+        # (L_{in} - 721) / 270 = L_{out}
+        return (x - 721) // 270
+
+    @staticmethod
+    def frame2sample(x):
+        return (x * 270) + 721
+
+    @staticmethod
     def sliding_window(waveform, window_size, step_size):
         windows = []
         start = 0
         num_samples = len(waveform)
         while start <= num_samples - window_size:
             windows.append((start, start + window_size))
             yield window_size, waveform[start : start + window_size]
@@ -53,45 +80,53 @@
         if num_samples < window_size or (num_samples - window_size) % step_size > 0:
             last_window = waveform[start:]
             last_window_size = len(last_window)
             if last_window_size < window_size:
                 last_window = np.pad(last_window, (0, window_size - last_window_size))
             yield last_window_size, last_window
 
+    @staticmethod
+    def reorder(x, y):
+        perms = [np.array(perm).T for perm in permutations(y.T)]
+        diffs = np.sum(
+            np.abs(np.sum(np.array(perms)[:, : x.shape[0], :] - x, axis=1)), axis=1
+        )
+        return perms[np.argmin(diffs)]
+
     def __call__(self, x, step=5.0, return_chunk=False):
-        # Conv1d & MaxPool1d & SincNet:
-        #   * https://pytorch.org/docs/stable/generated/torch.nn.Conv1d.html
-        #   * https://pytorch.org/docs/stable/generated/torch.nn.MaxPool1d.html
-        #   * https://github.com/pyannote/pyannote-audio/blob/develop/pyannote/audio/models/blocks/sincnet.py#L50-L71
-        #            kernel_size  stride
-        # Conv1d             251      10
-        # MaxPool1d            3       3
-        # Conv1d               5       1
-        # MaxPool1d            3       3
-        # Conv1d               5       1
-        # MaxPool1d            3       3
-        # (L_{in} - 721) / 270 = L_{out}
         step = int(step * self.sample_rate)
         # overlap: [0.5 * duration, 0.9 * duration]
         step = max(min(step, 0.9 * self.duration // 10), self.duration // 2)
-        overlap = (self.duration - step - 721) // 270
+        overlap = self.sample2frame(self.duration - step)
         overlap_chunk = np.zeros((overlap, self.num_classes))
         windows = list(self.sliding_window(x, self.duration, step))
         for idx, (window_size, window) in enumerate(windows):
-            ort_outs = self.session.run(None, {"input": window[None, None, :]})[0][0]
-            ort_outs = np.exp(ort_outs)
-            # aggregate
+            ort_outs = np.exp(
+                self.session.run(None, {"input": window[None, None, :]})[0][0]
+            )
+            # https://herve.niderb.fr/fastpages/2022/10/23/One-speaker-segmentation-model-to-rule-them-all
+            # reorder the speakers and aggregate
+            ort_outs = np.concatenate(
+                (
+                    1 - ort_outs[:, :1],  # speech probabilities
+                    self.reorder(
+                        overlap_chunk[:, 1 : self.num_classes],
+                        ort_outs[:, 1 : self.num_classes],
+                    ),  # speaker probabilities
+                ),
+                axis=1,
+            )
             if idx != 0:
                 ort_outs[:overlap, :] = (ort_outs[:overlap, :] + overlap_chunk) / 2
             if idx != len(windows) - 1:
                 overlap_chunk = ort_outs[-overlap:, :]
                 ort_outs = ort_outs[:-overlap, :]
             else:
                 # crop
-                ort_outs = ort_outs[: (window_size - 721) // 270, :]
+                ort_outs = ort_outs[: self.sample2frame(window_size), :]
 
             if return_chunk:
                 yield ort_outs
             else:
                 for out in ort_outs:
                     yield out
 
@@ -195,36 +230,33 @@
             raise ValueError(
                 "More than one dimension in audio."
                 "Are you trying to process audio with 2 channels?"
             )
         if sr / len(wav) > 31.25:
             raise ValueError("Input audio is too short.")
 
-        window_size_samples = 270
         min_speech_samples = sr * min_speech_duration_ms // 1000
-        max_speech_samples = (
-            sr * max_speech_duration_s - window_size_samples - 2 * speech_pad_samples
-        )
+        max_speech_samples = sr * max_speech_duration_s - 2 * speech_pad_samples
         min_silence_samples = sr * min_silence_duration_ms // 1000
         min_silence_samples_at_max_speech = sr * 98 // 1000
 
         current_speech = {}
         neg_threshold = threshold - 0.15
         triggered = False
         # to save potential segment end (and tolerate some silence)
         temp_end = 0
         # to save potential segment limits in case of maximum segment size reached
         prev_end = 0
         next_start = 0
 
         idx = 0
         current_samples = 721
-        for output in self(wav):
+        for outupt in self(wav):
+            speech_prob = outupt[0]
             current_samples += 270
-            speech_prob = 1 - output[0]
             # current frame is speech
             if speech_prob >= threshold:
                 if temp_end > 0 and next_start < prev_end:
                     next_start = current_samples
                 temp_end = 0
                 if not triggered:
                     triggered = True
@@ -293,24 +325,23 @@
     def get_num_speakers(
         self,
         wav_path: Union[str, Path],
         threshold: float = 0.5,
         min_speech_duration_ms: float = 100,
     ):
         """
-        Get the max number of speakers of each sliding windows (10 seconds)
-        It may not work if there are two or three speakers in different windows
+        Get the max number of speakers
         """
         wav, sr = librosa.load(wav_path, sr=self.sample_rate)
         if len(wav.shape) > 1:
             raise ValueError(
                 "More than one dimension in audio."
                 "Are you trying to process audio with 2 channels?"
             )
         if sr / len(wav) > 31.25:
             raise ValueError("Input audio is too short.")
 
-        outputs = np.array(list(self(wav)))
-        speech_frames = np.sum(outputs[:, 1:4] > threshold, axis=0)
-        speech_duration_ms = (speech_frames * 270 + 721) * 1000 / sr
+        outputs = np.array(list(self(wav)))[:, 1 : self.num_classes]
+        speech_frames = np.sum(outputs > threshold, axis=0)
+        speech_duration_ms = self.frame2sample(speech_frames) * 1000 / sr
         num_speakers = np.sum(speech_duration_ms > min_speech_duration_ms)
         return num_speakers
```

### Comparing `pyannote-onnx-0.0.2/pyannote_onnx/segmentation-3.0.onnx` & `pyannote-onnx-0.0.3/pyannote_onnx/segmentation-3.0.onnx`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.2/pyannote_onnx.egg-info/PKG-INFO` & `pyannote-onnx-0.0.3/pyannote_onnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyannote-onnx
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pyannote ONNX
 Home-page: https://github.com/pengzhendong/pyannote-onnx
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `pyannote-onnx-0.0.2/setup.py` & `pyannote-onnx-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     long_description = fin.read()
 
 with open("requirements.txt", encoding="utf-8") as f:
     requirements = f.readlines()
 
 setup(
     name="pyannote-onnx",
-    version=os.getenv("BUILD_VERSION") or "0.0.2",
+    version=os.getenv("BUILD_VERSION") or "0.0.3",
     author="Zhendong Peng",
     author_email="pzd17@tsinghua.org.cn",
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="Pyannote ONNX",
     url="https://github.com/pengzhendong/pyannote-onnx",
     packages=find_packages(),
```

