# Comparing `tmp/livekit-plugins-deepgram-0.2.0.tar.gz` & `tmp/livekit-plugins-deepgram-0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-plugins-deepgram-0.2.0.tar", last modified: Tue Feb 20 16:16:38 2024, max compression
+gzip compressed data, was "livekit-plugins-deepgram-0.3.dev0.tar", last modified: Thu Apr 11 22:01:22 2024, max compression
```

## Comparing `livekit-plugins-deepgram-0.2.0.tar` & `livekit-plugins-deepgram-0.3.dev0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:38.320552 livekit-plugins-deepgram-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-02-20 16:16:38.320552 livekit-plugins-deepgram-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-20 16:16:28.000000 livekit-plugins-deepgram-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:38.316552 livekit-plugins-deepgram-0.2.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:38.316552 livekit-plugins-deepgram-0.2.0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:38.320552 livekit-plugins-deepgram-0.2.0/livekit/plugins/deepgram/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-20 16:16:28.000000 livekit-plugins-deepgram-0.2.0/livekit/plugins/deepgram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-02-20 16:16:28.000000 livekit-plugins-deepgram-0.2.0/livekit/plugins/deepgram/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-02-20 16:16:28.000000 livekit-plugins-deepgram-0.2.0/livekit/plugins/deepgram/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-20 16:16:28.000000 livekit-plugins-deepgram-0.2.0/livekit/plugins/deepgram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:38.320552 livekit-plugins-deepgram-0.2.0/livekit_plugins_deepgram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-02-20 16:16:38.000000 livekit-plugins-deepgram-0.2.0/livekit_plugins_deepgram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-02-20 16:16:38.000000 livekit-plugins-deepgram-0.2.0/livekit_plugins_deepgram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 16:16:38.000000 livekit-plugins-deepgram-0.2.0/livekit_plugins_deepgram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-20 16:16:38.000000 livekit-plugins-deepgram-0.2.0/livekit_plugins_deepgram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-20 16:16:38.000000 livekit-plugins-deepgram-0.2.0/livekit_plugins_deepgram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-20 16:16:28.000000 livekit-plugins-deepgram-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 16:16:38.320552 livekit-plugins-deepgram-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-02-20 16:16:28.000000 livekit-plugins-deepgram-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:01:22.328751 livekit-plugins-deepgram-0.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-11 22:01:22.328751 livekit-plugins-deepgram-0.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:01:22.324751 livekit-plugins-deepgram-0.3.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:01:22.324751 livekit-plugins-deepgram-0.3.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:01:22.324751 livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16717 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:01:22.328751 livekit-plugins-deepgram-0.3.dev0/livekit_plugins_deepgram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-11 22:01:22.000000 livekit-plugins-deepgram-0.3.dev0/livekit_plugins_deepgram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-11 22:01:22.000000 livekit-plugins-deepgram-0.3.dev0/livekit_plugins_deepgram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:01:22.000000 livekit-plugins-deepgram-0.3.dev0/livekit_plugins_deepgram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 22:01:22.000000 livekit-plugins-deepgram-0.3.dev0/livekit_plugins_deepgram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:01:22.000000 livekit-plugins-deepgram-0.3.dev0/livekit_plugins_deepgram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:01:22.328751 livekit-plugins-deepgram-0.3.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-11 22:01:18.000000 livekit-plugins-deepgram-0.3.dev0/setup.py
```

### Comparing `livekit-plugins-deepgram-0.2.0/PKG-INFO` & `livekit-plugins-deepgram-0.3.dev0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-deepgram
-Version: 0.2.0
+Version: 0.3.dev0
 Summary: Agent Framework plugin for services using DeepGram's API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -13,18 +13,18 @@
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.10.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit>=0.9.0
-Requires-Dist: livekit-agents>=0.3.0
+Requires-Dist: livekit~=0.9
+Requires-Dist: livekit-agents~=0.5.dev0
 Requires-Dist: aiohttp>=3.7.4
 
 # LiveKit Plugins DeepGram
 
 Agent Framework plugin for speech-to-text with [DeepGram](https://deepgram.com/)'s API. Currently supports speech-to-text.
 
 ## Installation
```

### Comparing `livekit-plugins-deepgram-0.2.0/livekit/plugins/deepgram/models.py` & `livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/models.py`

 * *Files identical despite different names*

### Comparing `livekit-plugins-deepgram-0.2.0/livekit/plugins/deepgram/version.py` & `livekit-plugins-deepgram-0.3.dev0/livekit/plugins/deepgram/version.py`

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

### Comparing `livekit-plugins-deepgram-0.2.0/livekit_plugins_deepgram.egg-info/PKG-INFO` & `livekit-plugins-deepgram-0.3.dev0/livekit_plugins_deepgram.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-deepgram
-Version: 0.2.0
+Version: 0.3.dev0
 Summary: Agent Framework plugin for services using DeepGram's API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -13,18 +13,18 @@
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.10.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Requires-Dist: livekit>=0.9.0
-Requires-Dist: livekit-agents>=0.3.0
+Requires-Dist: livekit~=0.9
+Requires-Dist: livekit-agents~=0.5.dev0
 Requires-Dist: aiohttp>=3.7.4
 
 # LiveKit Plugins DeepGram
 
 Agent Framework plugin for speech-to-text with [DeepGram](https://deepgram.com/)'s API. Currently supports speech-to-text.
 
 ## Installation
```

### Comparing `livekit-plugins-deepgram-0.2.0/setup.py` & `livekit-plugins-deepgram-0.3.dev0/setup.py`

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
 with open(os.path.join(here, "livekit", "plugins", "deepgram", "version.py"), "r") as f:
     exec(f.read(), about)
 
 
 setuptools.setup(
@@ -43,20 +42,22 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
-    python_requires=">=3.10.0",  # deepgram-sdk requires 3.10
+    python_requires=">=3.9.0",
     install_requires=[
-        "livekit >= 0.9.0",
-        "livekit-agents >= 0.3.0",
+        "livekit ~= 0.9",
+        "livekit-agents~=0.5.dev0",
         "aiohttp >= 3.7.4",
     ],
-    package_data={},
+    package_data={
+        "livekit.plugins.deepgram": ["py.typed"],
+    },
     project_urls={
         "Documentation": "https://docs.livekit.io",
         "Website": "https://livekit.io/",
         "Source": "https://github.com/livekit/agents",
     },
 )
```

