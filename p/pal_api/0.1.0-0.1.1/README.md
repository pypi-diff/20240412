# Comparing `tmp/pal_api-0.1.0.tar.gz` & `tmp/pal_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pal_api-0.1.0.tar", last modified: Fri Apr 12 17:47:04 2024, max compression
+gzip compressed data, was "pal_api-0.1.1.tar", last modified: Fri Apr 12 18:07:50 2024, max compression
```

## Comparing `pal_api-0.1.0.tar` & `pal_api-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0     1091 2024-04-12 15:51:43.994462 pal_api-0.1.0/LICENSE
--rw-r--r--   0        0        0     2110 2024-04-12 15:51:43.998466 pal_api-0.1.0/README.md
--rw-r--r--   0        0        0      850 2024-04-12 17:47:04.868115 pal_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      100 2024-04-12 15:56:17.140507 pal_api-0.1.0/src/pal_api/__init__.py
--rw-r--r--   0        0        0     4441 2024-04-12 14:41:10.574627 pal_api-0.1.0/src/pal_api/async_client.py
--rw-r--r--   0        0        0     3889 2024-04-11 17:22:07.002250 pal_api-0.1.0/src/pal_api/client.py
--rw-r--r--   0        0        0      132 2024-04-05 16:43:42.519968 pal_api-0.1.0/src/pal_api/errors.py
--rw-r--r--   0        0        0     1687 2024-04-11 17:45:49.037862 pal_api-0.1.0/src/pal_api/models.py
--rw-r--r--   0        0        0        0 2024-04-05 14:27:20.572492 pal_api-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      703 2024-04-12 14:48:31.232880 pal_api-0.1.0/tests/test_async.py
--rw-r--r--   0        0        0      718 2024-04-11 17:41:04.343086 pal_api-0.1.0/tests/test_sync.py
--rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 pal_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-12 18:07:37.532419 pal_api-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2040 2024-04-12 18:07:37.532419 pal_api-0.1.1/README.md
+-rw-r--r--   0        0        0      850 2024-04-12 18:07:50.016438 pal_api-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      100 2024-04-12 18:07:37.532419 pal_api-0.1.1/src/pal_api/__init__.py
+-rw-r--r--   0        0        0     4441 2024-04-12 18:07:37.532419 pal_api-0.1.1/src/pal_api/async_client.py
+-rw-r--r--   0        0        0     3889 2024-04-12 18:07:37.532419 pal_api-0.1.1/src/pal_api/client.py
+-rw-r--r--   0        0        0      132 2024-04-12 18:07:37.532419 pal_api-0.1.1/src/pal_api/errors.py
+-rw-r--r--   0        0        0     1687 2024-04-12 18:07:37.532419 pal_api-0.1.1/src/pal_api/models.py
+-rw-r--r--   0        0        0        0 2024-04-12 18:07:37.532419 pal_api-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 pal_api-0.1.1/PKG-INFO
```

### Comparing `pal_api-0.1.0/LICENSE` & `pal_api-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Charahiro-tan
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Charahiro-tan
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pal_api-0.1.0/README.md` & `pal_api-0.1.1/README.md`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-# pal_api
-API Wrapper for Palworld Dedicated Server  
-### Usage
-_Install_  
-```sh
-pip install pal_api
-### Option ###
-pip install ujson
-```
-_Sync_
-```python
-from pal_api import PalApiClient
-client = PalApiClient(password="password")
-print(client.get_server_info())
-
-# with Context Manager
-with PalApiClient(password="password") as client:
-    print(client.get_server_info())
-```
-_Async_
-```python
-import asyncio
-from pal_api import AsyncPalApiClient
-
-async def main():
-    client = AsyncPalApiClient(password="password")
-    print(await client.get_server_info())
-    await client.close()
-
-asyncio.run(main())
-
-# with Context Manager
-async def main():
-    async with AsyncPalApiClient(password="password") as client:
-        print(await client.get_server_info())
-
-asyncio.run(main())
-```
-_Options and Default Values for the Class_
-|name|class|default|
-|---|---|---|
-|host|str|"localhost"|
-|port|int|8212|
-|username|str|"admin"|
-|password|str||
-|timeout|int|5|
-|session(async only)|aiohttp.ClientSession|None|
-
-_method_
-```python
-get_server_info() -> ServerInfo
-get_player_list() -> PlayerList
-get_server_settings() -> dict
-get_server_metrics() -> ServerMetrics
-announce_message(message: str) -> None
-kick_player(userid: str, message: str = "") -> None
-ban_player(userid: str, message: str = "") -> None
-unban_player(userid: str) -> None
-save_world() -> None
-shutdown_server(waittime: int = 10, message: str | None = None, force: bool = False) -> None
-```
-
-### やってること・その他
-- playerIdが負の数が返ってくることがある -> とりあえず正の数に直してます
-- ログイン中にSteamの名前が返ってくる -> playerIdがNoneのものは除外しています
-- BanするとbanlistにはIDが乗るが、効いてなさそう(コミュニティサーバー未確認)
-- また、間違ったIDを送ってもとりあえずリストには乗る
-- Banするときにメッセージを送れるが、どこに表示されているのか不明
-
-License MIT ©[Charahiro-tan](https://twitter.com/__Charahiro)
+# pal_api
+API Wrapper for Palworld Dedicated Server  
+### Usage
+_Install_  
+```sh
+pip install pal_api
+### Option ###
+pip install ujson
+```
+_Sync_
+```python
+from pal_api import PalApiClient
+client = PalApiClient(password="password")
+print(client.get_server_info())
+
+# with Context Manager
+with PalApiClient(password="password") as client:
+    print(client.get_server_info())
+```
+_Async_
+```python
+import asyncio
+from pal_api import AsyncPalApiClient
+
+async def main():
+    client = AsyncPalApiClient(password="password")
+    print(await client.get_server_info())
+    await client.close()
+
+asyncio.run(main())
+
+# with Context Manager
+async def main():
+    async with AsyncPalApiClient(password="password") as client:
+        print(await client.get_server_info())
+
+asyncio.run(main())
+```
+_Options and Default Values for the Class_
+|name|class|default|
+|---|---|---|
+|host|str|"localhost"|
+|port|int|8212|
+|username|str|"admin"|
+|password|str||
+|timeout|int|5|
+|session(async only)|aiohttp.ClientSession|None|
+
+_method_
+```python
+get_server_info() -> ServerInfo
+get_player_list() -> PlayerList
+get_server_settings() -> dict
+get_server_metrics() -> ServerMetrics
+announce_message(message: str) -> None
+kick_player(userid: str, message: str = "") -> None
+ban_player(userid: str, message: str = "") -> None
+unban_player(userid: str) -> None
+save_world() -> None
+shutdown_server(waittime: int = 10, message: str | None = None, force: bool = False) -> None
+```
+
+### やってること・その他
+- playerIdが負の数が返ってくることがある -> とりあえず正の数に直してます
+- ログイン中にSteamの名前が返ってくる -> playerIdがNoneのものは除外しています
+- BanするとbanlistにはIDが乗るが、効いてなさそう(コミュニティサーバー未確認)
+- また、間違ったIDを送ってもとりあえずリストには乗る
+- Banするときにメッセージを送れるが、どこに表示されているのか不明
+
+License MIT ©[Charahiro-tan](https://twitter.com/__Charahiro)
```

### Comparing `pal_api-0.1.0/pyproject.toml` & `pal_api-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 readme = "README.md"
 dynamic = []
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Natural Language :: Japanese",
     "Programming Language :: Python :: 3",
 ]
-version = "0.1.0"
+version = "0.1.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/Charahiro-tan/pal_api"
```

### Comparing `pal_api-0.1.0/src/pal_api/async_client.py` & `pal_api-0.1.1/src/pal_api/async_client.py`

 * *Files identical despite different names*

### Comparing `pal_api-0.1.0/src/pal_api/client.py` & `pal_api-0.1.1/src/pal_api/client.py`

 * *Files identical despite different names*

### Comparing `pal_api-0.1.0/src/pal_api/models.py` & `pal_api-0.1.1/src/pal_api/models.py`

 * *Files identical despite different names*

### Comparing `pal_api-0.1.0/PKG-INFO` & `pal_api-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pal_api
-Version: 0.1.0
+Version: 0.1.1
 Summary: API Wrapper for Palworld Dedicated Server
 Home-page: https://github.com/Charahiro-tan/pal_api
 Author-Email: Charahiro-tan <charahiro.tan@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python :: 3
```

