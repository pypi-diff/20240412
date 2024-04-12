# Comparing `tmp/nonebot_plugin_ncm-1.6.8.tar.gz` & `tmp/nonebot_plugin_ncm-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ncm-1.6.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_ncm-1.6.9.tar", max compression
```

## Comparing `nonebot_plugin_ncm-1.6.8.tar` & `nonebot_plugin_ncm-1.6.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-11-04 21:02:36.812512 nonebot_plugin_ncm-1.6.8/LICENSE
--rw-r--r--   0        0        0     4693 2023-11-04 21:02:36.812512 nonebot_plugin_ncm-1.6.8/README.md
--rw-r--r--   0        0        0    13806 2023-11-04 21:02:36.812512 nonebot_plugin_ncm-1.6.8/nonebot-plugin-ncm/__init__.py
--rw-r--r--   0        0        0      734 2023-11-04 21:02:36.812512 nonebot_plugin_ncm-1.6.8/nonebot-plugin-ncm/config.py
--rw-r--r--   0        0        0    13059 2023-11-04 21:02:36.812512 nonebot_plugin_ncm-1.6.8/nonebot-plugin-ncm/data_source.py
--rw-r--r--   0        0        0      859 2023-11-04 21:02:36.812512 nonebot_plugin_ncm-1.6.8/pyproject.toml
--rw-r--r--   0        0        0     5901 1970-01-01 00:00:00.000000 nonebot_plugin_ncm-1.6.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-12-03 07:49:56.889148 nonebot_plugin_ncm-1.6.9/LICENSE
+-rw-r--r--   0        0        0     4625 2023-12-03 07:49:56.889148 nonebot_plugin_ncm-1.6.9/README.md
+-rw-r--r--   0        0        0    11814 2023-12-03 07:49:56.889148 nonebot_plugin_ncm-1.6.9/nonebot-plugin-ncm/__init__.py
+-rw-r--r--   0        0        0      660 2023-12-03 07:49:56.889148 nonebot_plugin_ncm-1.6.9/nonebot-plugin-ncm/config.py
+-rw-r--r--   0        0        0    13865 2023-12-03 07:49:56.889148 nonebot_plugin_ncm-1.6.9/nonebot-plugin-ncm/data_source.py
+-rw-r--r--   0        0        0      859 2023-12-03 07:49:56.889148 nonebot_plugin_ncm-1.6.9/pyproject.toml
+-rw-r--r--   0        0        0     5833 1970-01-01 00:00:00.000000 nonebot_plugin_ncm-1.6.9/PKG-INFO
```

### Comparing `nonebot_plugin_ncm-1.6.8/LICENSE` & `nonebot_plugin_ncm-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ncm-1.6.8/README.md` & `nonebot_plugin_ncm-1.6.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,14 @@
 ## 配置文件说明 ⚙️
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | ncm_admin_level | 否 | 1 | 设置命令权限(1:仅限superusers和群主,2:在1的基础上+管理员,3:所有用户) |
 | ncm_ctcode | 否 | 86 | 手机号区域码 |
 | ncm_phone | 是 |   | 网易云绑定的手机号(留空则二维码登录) |
 | ncm_password | 是 |   | 网易云账号密码(留空则短信登录) |
-| ncm_playlist_zip | 否 | False | 是否开启歌单打包上传 |
 | ncm_bitrate | 否 | 320 | 下载码率(单位K) <=96: m4a, >=320:flac, 96< mp3 <320|
 ```
 # 这是示例
 ncm_admin_level=1 # 设置命令权限(1:仅限superusers和群主,2:在1的基础上+管理员,3:所有用户)
 ncm_ctcode="86" # 手机号区域码,默认86
 ncm_phone=  # 手机登录
 ncm_password=  # 密码
```

#### html2text {}

```diff
@@ -27,20 +27,19 @@
 qqå· f | å³é­è¯¥ç¨æ·ç§èä¸è½½ | - å½ä»¤å¼å§ç¬¦å·ä¼èªå¨è¯å«
 [`COMMAND_START`](https://v2.nonebot.dev/docs/api/config#Config-
 command_start)é¡¹ ## éç½®æä»¶è¯´æ âï¸ | éç½®é¡¹ | å¿å¡« | é»è®¤å¼
 | è¯´æ | |:-----:|:----:|:----:|:----:| | ncm_admin_level | å¦ | 1 |
 è®¾ç½®å½ä»¤æé(1:ä»ésuperusersåç¾¤ä¸»,2:å¨1çåºç¡ä¸+ç®¡çå,3:
 ææç¨æ·) | | ncm_ctcode | å¦ | 86 | ææºå·åºåç  | | ncm_phone |
 æ¯ | | ç½æäºç»å®çææºå·(çç©ºåäºç»´ç ç»å½) | | ncm_password
-| æ¯ | | ç½æäºè´¦å·å¯ç (çç©ºåç­ä¿¡ç»å½) | | ncm_playlist_zip |
-å¦ | False | æ¯å¦å¼å¯æ­åæåä¸ä¼  | | ncm_bitrate | å¦ | 320 |
-ä¸è½½ç ç(åä½K) <=96: m4a, >=320:flac, 96< mp3 <320| ``` # è¿æ¯ç¤ºä¾
-ncm_admin_level=1 # è®¾ç½®å½ä»¤æé(1:ä»ésuperusersåç¾¤ä¸»,2:
-å¨1çåºç¡ä¸+ç®¡çå,3:ææç¨æ·) ncm_ctcode="86" #
-ææºå·åºåç ,é»è®¤86 ncm_phone= # ææºç»å½ ncm_password= # å¯ç 
-ncm_playlist_zip=False # ä¸ä¼ æ­åæ¶æ¯å¦åç¼© ncm_bitrate: int = 320 #
-ä¸è½½ç ç(åä½K) 96åä»¥ä¸ä¸ºm4a,320åä»¥ä¸ä¸ºflac,ä¸­é´mp3 ``` ##
-åè½åè¡¨ ð - [x] è¯å«/ä¸è½½ ç½æäºåæ² - é¾æ¥ - å¡ç -
-å¡çè½¬å - [x] è¯å«/ä¸è½½ ç½æäºæ­å - é¾æ¥ - å¡ç -
-å¡çè½¬å - [x] ç¹æ­(ç½æäº) - [ ] QQé³ä¹æ æä¸è½½ # é¸£è°¢ -
-[pyncm](https://github.com/greats3an/pyncm) - [nonebot2](https://github.com/
-nonebot/nonebot2)
+| æ¯ | | ç½æäºè´¦å·å¯ç (çç©ºåç­ä¿¡ç»å½) | | ncm_bitrate | å¦ |
+320 | ä¸è½½ç ç(åä½K) <=96: m4a, >=320:flac, 96< mp3 <320| ``` #
+è¿æ¯ç¤ºä¾ ncm_admin_level=1 # è®¾ç½®å½ä»¤æé(1:
+ä»ésuperusersåç¾¤ä¸»,2:å¨1çåºç¡ä¸+ç®¡çå,3:ææç¨æ·)
+ncm_ctcode="86" # ææºå·åºåç ,é»è®¤86 ncm_phone= # ææºç»å½
+ncm_password= # å¯ç  ncm_playlist_zip=False # ä¸ä¼ æ­åæ¶æ¯å¦åç¼©
+ncm_bitrate: int = 320 # ä¸è½½ç ç(åä½K)
+96åä»¥ä¸ä¸ºm4a,320åä»¥ä¸ä¸ºflac,ä¸­é´mp3 ``` ## åè½åè¡¨ ð - [x]
+è¯å«/ä¸è½½ ç½æäºåæ² - é¾æ¥ - å¡ç - å¡çè½¬å - [x] è¯å«/
+ä¸è½½ ç½æäºæ­å - é¾æ¥ - å¡ç - å¡çè½¬å - [x] ç¹æ­(ç½æäº)
+- [ ] QQé³ä¹æ æä¸è½½ # é¸£è°¢ - [pyncm](https://github.com/greats3an/
+pyncm) - [nonebot2](https://github.com/nonebot/nonebot2)
```

### Comparing `nonebot_plugin_ncm-1.6.8/nonebot-plugin-ncm/__init__.py` & `nonebot_plugin_ncm-1.6.9/nonebot-plugin-ncm/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from dataclasses import dataclass
-from pathlib import Path
-from typing import Tuple, Any, Union, Optional, Type, Set, Dict
+from typing import Tuple, Any, Union
 
-import nonebot
 from nonebot import on_regex, on_command, on_message
 from nonebot.adapters.onebot.v11 import (Message, Bot,
                                          MessageSegment,
                                          GroupMessageEvent,
                                          PrivateMessageEvent)
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg, RegexGroup, Arg
+from nonebot.plugin import PluginMetadata
 from nonebot.rule import Rule
-from pydantic.main import BaseModel
 
-from .data_source import nncm, ncm_config, setting, Q, cmd
 from .config import Config
-from nonebot.plugin import PluginMetadata
+from .data_source import nncm, ncm_config, setting, Q, cmd
 
 __plugin_meta__ = PluginMetadata(
     name="网易云无损音乐下载",
     description="基于go-cqhttp与nonebot2的 网易云无损音乐下载",
     usage=(
         '将网易云歌曲/歌单分享到群聊即可自动解析\n'
         '回复分享消息 + 文字`下载` 即可开始下载歌曲并上传到群文件(需要稍等一会)'
@@ -123,80 +119,50 @@
 @search.got("song", prompt="要点什么歌捏?")
 async def receive_song(bot: Bot,
                        event: Union[GroupMessageEvent, PrivateMessageEvent],
                        song: Message = Arg(),
                        ):
     _id = await nncm.search_song(keyword=song.extract_plain_text(), limit=1)
     message_id = await bot.send(event=event, message=Message(MessageSegment.music(type_="163", id_=_id)))
-    nncm.get_song(message_id=message_id["message_id"], nid=_id, bot_id=bot.self_id)
+    nncm.get_song(message_id=message_id["message_id"], nid=_id)
     # try:
 
     # except ActionFailed as e:
     #    logger.error(e.info)
     #    await search.finish(event=event, message=f"[WARNING]: 网易云卡片消息发送失败: 账号可能被风控")
 
 
 @music_regex.handle()
 async def music_receive(bot: Bot, event: Union[GroupMessageEvent, PrivateMessageEvent],
                         regroup: Tuple[Any, ...] = RegexGroup()):
     nid = regroup[1]
     logger.info(f"已识别NID:{nid}的歌曲")
 
-    nncm.get_song(nid=nid, message_id=event.message_id, bot_id=bot.self_id)
+    nncm.get_song(nid=nid, message_id=event.message_id)
 
 
 @playlist_regex.handle()
 async def music_list_receive(bot: Bot, event: Union[GroupMessageEvent, PrivateMessageEvent],
                              regroup: Tuple[Any, ...] = RegexGroup()):
     lid = regroup[0]
     logger.info(f"已识别LID:{lid}的歌单")
-    nncm.get_playlist(lid=lid, message_id=event.message_id, bot_id=bot.self_id)
+    nncm.get_playlist(lid=lid, message_id=event.message_id)
 
 
 @music_reply.handle()
 async def music_reply_receive(bot: Bot, event: Union[GroupMessageEvent, PrivateMessageEvent]):
     info = nncm.check_message(int(event.dict()["reply"]["message_id"]))
     if info is None:
         return
-    if info["type"] == "song" and await song_is_open(event) and info["bot_id"] == bot.self_id:
+    if info["type"] == "song" and await song_is_open(event):
         await bot.send(event=event, message="少女祈祷中🙏...上传时间较久,请勿重复发送命令")
-        data = await nncm.music_check(info["nid"])
-        if isinstance(data, list):
-            data = data[0]
-        if data:
-            if isinstance(event, GroupMessageEvent):
-                await nncm.upload_group_data_file(event.group_id, data, bot_id=info["bot_id"])
-            elif isinstance(event, PrivateMessageEvent):
-                await nncm.upload_private_data_file(event.user_id, data, bot_id=info["bot_id"])
-        else:
-            logger.error("数据库中未有该音乐地址数据")
-            await bot.send(event=event, message="数据库中未有该音乐地址数据")
-
-    elif info["type"] == "playlist" and await playlist_is_open(event) and info["bot_id"] == bot.self_id:
+        await nncm.music_check(info["nid"], event)
+    elif info["type"] == "playlist" and await playlist_is_open(event):
         await bot.send(event=event, message=info["lmsg"] + "\n下载中,上传时间较久,请勿重复发送命令")
-        not_zips = await nncm.download(ids=info["ids"], lid=info["lid"], is_zip=ncm_config.ncm_playlist_zip)
-        filename = f"{info['lid']}.zip"
-        data = Path.cwd().joinpath("music").joinpath(filename)
-        if ncm_config.ncm_playlist_zip:
-            logger.debug(f"Upload:{filename}")
-            if isinstance(event, GroupMessageEvent):
-                await nncm.upload_group_file(group_id=event.group_id, file=str(data), name=filename,
-                                             bot_id=info["bot_id"])
-            elif isinstance(event, PrivateMessageEvent):
-                await nncm.upload_private_file(user_id=event.user_id, file=str(data), name=filename,
-                                               bot_id=info["bot_id"])
-        else:
-            for i in not_zips:
-                file = i["file"]
-                filename = i["filename"]
-                logger.debug(f"Upload:{filename}")
-                if isinstance(event, GroupMessageEvent):
-                    await nncm.upload_group_file(group_id=event.group_id, file=file, name=filename)
-                elif isinstance(event, PrivateMessageEvent):
-                    await nncm.upload_private_file(user_id=event.user_id, file=file, name=filename)
+        await nncm.music_check(info["ids"], event, info["lid"])
 
 
 @ncm_set.handle()
 async def set_receive(bot: Bot, event: Union[GroupMessageEvent, PrivateMessageEvent],
                       args: Message = CommandArg()):  # 功能设置接收
     logger.debug(f"权限为{event.sender.role}的用户<{event.sender.nickname}>尝试使用命令{cmd}ncm {args}")
     if args:
```

### Comparing `nonebot_plugin_ncm-1.6.8/nonebot-plugin-ncm/data_source.py` & `nonebot_plugin_ncm-1.6.9/nonebot-plugin-ncm/data_source.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-import os
-import zipfile
-from pathlib import Path
-from datetime import datetime
-from typing import Union, List, Optional, Dict
+import asyncio
 import re
-
-import qrcode
 import time
-from aiofile import async_open
+from datetime import datetime
+from pathlib import Path
+from typing import Union, List, Dict, cast
 
-import httpx
 import nonebot
-from nonebot.utils import run_sync
-
-from pyncm import apis, Session, GetCurrentSession, DumpSessionAsString, LoadSessionFromString, SetCurrentSession
-from pyncm.apis.cloudsearch import SONG, USER, PLAYLIST
-
-from nonebot.log import logger
+import qrcode
 from nonebot.adapters.onebot.v11 import (MessageSegment, Message,
                                          ActionFailed, NetworkError, Bot,
                                          GroupMessageEvent, PrivateMessageEvent)
+from nonebot.log import logger
+from nonebot.matcher import current_bot
+from pyncm import apis, GetCurrentSession, DumpSessionAsString, LoadSessionFromString, SetCurrentSession
+from pyncm.apis.cloudsearch import SONG, USER, PLAYLIST
+from tinydb import TinyDB, Query
 
 from .config import ncm_config
-from tinydb import TinyDB, Query
 
 # ============数据库导入=============
 dbPath = Path("db")
 musicPath = Path("music")
 
 if not musicPath.is_dir():
     musicPath.mkdir()
@@ -122,27 +116,60 @@
                 st = self.api.login.GetCurrentLoginStatus()
                 logger.debug(st)
                 self.api.login.WriteLoginInfo(st)
                 self.get_user_info()
                 return True
             time.sleep(1)
 
-    def detail(self, ids: list) -> list:
+    def detail_names(self, ids: List[int]) -> List[str]:
         songs: list = self.api.track.GetTrackDetail(song_ids=ids)["songs"]
         detail = [(data["name"] + "-" + ",".join([names["name"] for names in data["ar"]])) for data in songs]
         return detail
 
-    async def music_check(self, nid: int) -> Union[List[Dict[str, Union[str, int]]], Dict[str, Union[str, int]], None]:
-        nid = int(nid)
-        info = music.search(Q["id"] == nid)
-        if info:
-            path = Path(info[0]["file"])
-            if path.is_file():
-                return info[0]
-        return await self.download(ids=[nid])
+    @logger.catch()
+    def get_detail(self, ids: List[int]):
+        data: list = self.api.track.GetTrackAudio(song_ids=ids, bitrate=ncm_config.ncm_bitrate * 1000)["data"]
+        names: list = self.detail_names(ids)
+        for i in range(len(ids)):
+            data[i]['ncm_name'] = names[i]
+        return data
+
+    async def music_check(self, nid: Union[int, List[int]], event: Union[GroupMessageEvent, PrivateMessageEvent],
+                          lid: int = None):
+        """判断数据库中是否有缓存，有则使用缓存，没有则新下载"""
+        tasks = []
+        if lid:
+            del_nid = []
+            for i in nid:
+                info = music.search(Q["id"] == i)
+                if info:
+                    try:
+                        tasks.append(asyncio.create_task(self.upload_data_file(event=event, data=info[0])))
+                        del_nid.append(i)
+                    except Exception:
+                        continue
+            for j in del_nid:
+                nid.remove(j)
+        else:
+            nid = int(nid)
+            info = music.search(Q["id"] == nid)
+            if info:
+                try:
+                    tasks.append(asyncio.create_task(self.upload_data_file(event=event, data=info[0])))
+                    return
+                except Exception as e:
+                    if isinstance(e, ActionFailed) and e.info.get("retcode") != 10003:
+                        logger.error(e)
+                        return
+        if tasks:
+            await asyncio.gather(*tasks)
+        if nid:
+            if isinstance(nid, int):
+                nid = [nid]
+            await self.start_upload(ids=nid, event=event)
 
     async def search_song(self, keyword: str, limit: int = 1) -> int:  # 搜索歌曲
         res = self.api.cloudsearch.GetSearchResult(keyword=keyword, stype=SONG, limit=limit)
         logger.debug(f"搜索歌曲{keyword},返回结果:{res}")
         if "result" in res.keys():
             data = res["result"]["songs"]
         else:
@@ -161,32 +188,30 @@
         """检查缓存中是否存在解析
         :return:
         """
         flag = ncm_check_cache.search(Q.message_id == message_id)
         return flag[0] if flag else None
 
     @staticmethod
-    def get_song(nid: int, message_id: int, bot_id: str):
+    def get_song(nid: int, message_id: int):
         """解析歌曲id,并且加入缓存
-
-        :param bot_id:
         :param message_id:
         :param nid:
         :return:
         """
         ncm_check_cache.insert({"message_id": message_id,
                                 "type": "song",
                                 "nid": int(nid),
                                 "lid": 0,
                                 "ids": [],
                                 "lmsg": "",
-                                "bot_id": bot_id,
+                                "bot_id": "",
                                 "time": int(time.time())})
 
-    def get_playlist(self, lid: int, message_id: int, bot_id: str):
+    def get_playlist(self, lid: int, message_id: int):
         lid = int(lid)
         data = self.api.playlist.GetPlaylistInfo(lid)
         # logger.info(data)
         if data["code"] == 200:
             raw = data["playlist"]
             tags = ",".join(raw['tags'])
             songs = [int(i['id']) for i in raw['trackIds']]
@@ -194,100 +219,95 @@
                                     "type": "playlist",
                                     "nid": 0,
                                     "lid": lid,
                                     "ids": songs,
                                     "lmsg": f"歌单:{raw['name']}\r\n创建者:{raw['creator']['nickname']}\r\n歌曲总数:{raw['trackCount']}\r\n"
                                             f"标签:{tags}\r\n播放次数:{raw['playCount']}\r\n收藏:{raw['subscribedCount']}\r\n"
                                             f"评论:{raw['commentCount']}\r\n分享:{raw['shareCount']}\r\nListID:{lid}",
-                                    "bot_id": bot_id,
+                                    "bot_id": "",
                                     "time": int(time.time())})
 
-    async def upload_group_data_file(self, group_id: int, data: Dict[str, Union[str, int]], bot_id: str):
-        await self.upload_group_file(group_id=group_id, file=data["file"], name=data["filename"], bot_id=bot_id)
-
-    async def upload_private_data_file(self, user_id: int, data: Dict[str, Union[str, int]], bot_id: str):
-        await self.upload_private_file(user_id=user_id, file=data["file"], name=data["filename"], bot_id=bot_id)
+    async def upload_data_file(self, event: Union[GroupMessageEvent, PrivateMessageEvent],
+                               data: Dict[str, Union[str, int]]):
+        if isinstance(event, GroupMessageEvent):
+            await self.upload_group_file(group_id=event.group_id, file=data["file"], name=data["filename"])
+        elif isinstance(event, PrivateMessageEvent):
+            await self.upload_private_file(user_id=event.user_id, file=data["file"], name=data["filename"])
 
     @staticmethod
-    async def upload_group_file(group_id: int, file: str, name: str, bot_id: str):
+    async def upload_group_file(group_id: int, file: str, name: str):
+        bot: Bot = cast(Bot, current_bot.get())
         try:
-            bot: Bot = nonebot.get_bot(bot_id)
             await bot.upload_group_file(group_id=group_id, file=file, name=name)
         except (ActionFailed, NetworkError) as e:
             logger.error(e)
-            bot: Bot = nonebot.get_bot(bot_id)
             if isinstance(e, ActionFailed) and e.info["wording"] == "server" \
                                                                     " requires unsupported ftn upload":
                 await bot.send_group_msg(group_id=group_id, message=Message(MessageSegment.text(
                     "[ERROR]  文件上传失败\r\n[原因]  机器人缺少上传文件的权限\r\n[解决办法]  "
                     "请将机器人设置为管理员或者允许群员上传文件")))
             elif isinstance(e, NetworkError):
                 await bot.send_group_msg(group_id=group_id,
                                          message=Message(MessageSegment.text("[ERROR]文件上传失败\r\n[原因]  "
                                                                              "上传超时(一般来说还在传,建议等待五分钟)")))
 
     @staticmethod
-    async def upload_private_file(user_id: int, file: str, name: str, bot_id: str):
+    async def upload_private_file(user_id: int, file: str, name: str):
+        bot: Bot = cast(Bot, current_bot.get())
         try:
-            bot: Bot = nonebot.get_bot(bot_id)
             await bot.upload_private_file(user_id=user_id, file=file, name=name)
         except (ActionFailed, NetworkError) as e:
             logger.error(e)
             if isinstance(e, NetworkError):
-                bot: Bot = nonebot.get_bot(bot_id)
-                await  bot.send_private_msg(user_id=user_id, message=Message(MessageSegment.text(
+                await bot.send_private_msg(user_id=user_id, message=Message(MessageSegment.text(
                     "[ERROR]  文件上传失败\r\n[原因]  上传超时(一般来说还在传,建议等待五分钟)")))
 
-    @run_sync
-    def get_zip(self, lid: int, filenames: list):
-        zip_file_new = f'{lid}.zip'
-        with zipfile.ZipFile(str(Path.cwd().joinpath("music").joinpath(zip_file_new)), 'w', zipfile.ZIP_DEFLATED) as z:
-            for f in filenames:
-                z.write(str(f), f.name)
-        return zip_file_new
+    # @run_sync
+    # def get_zip(self, lid: int, filenames: list):
+    #     zip_file_new = f'{lid}.zip'
+    #     with zipfile.ZipFile(str(Path.cwd().joinpath("music").joinpath(zip_file_new)), 'w', zipfile.ZIP_DEFLATED) as z:
+    #         for f in filenames:
+    #             z.write(str(f), f.name)
+    #     return zip_file_new
+    async def upload(self, data: dict, fr: str, event: Union[GroupMessageEvent, PrivateMessageEvent]):
+        if data["code"] == 404:
+            logger.error("未从网易云读取到下载地址")
+            return None
+        url = data["url"]
+        nid = data["id"]
+        filename = f"{data['ncm_name']}.{data['type']}"
+        filename = re.sub('[\/:*?"<>|]', '-', filename)
+        bot = cast(Bot, current_bot.get())
+        download_ret: Dict[str, str] = await bot.download_file(url=url)
+        file = download_ret["file"]
+        cf = {
+            "id": int(nid),
+            "file": str(file),  # 获取文件位置
+            "filename": filename,  # 获取文件名
+            "from": fr,  # 判断来自单曲还是歌单
+            "time": datetime.now().strftime("%Y-%m-%d %H:%M:%S")  # 获取时间
+        }
+        info = music.search(Q["id"] == nid)
+        if info:  # 数据库储存
+            music.update(cf, Q["id"] == nid)
+        else:
+            music.insert(cf)
+        logger.debug(f"Download:{filename}")
+        await self.upload_data_file(event=event, data=cf)
 
-    async def download(self, ids: List[int], lid: int = 0, is_zip=False) -> Optional[List[Dict[str, Union[str, int]]]]:
+    async def start_upload(self, ids: List[int], event: Union[GroupMessageEvent, PrivateMessageEvent]):
         """一般地 320k及以上即 flac, 320k及以下即 mp3,96k及以下即 m4a
         """
-        data: list = self.api.track.GetTrackAudio(song_ids=ids, bitrate=ncm_config.ncm_bitrate * 1000)["data"]
-        name: list = self.detail(ids)
-        filenames = []
-        not_zips = []
+        data: list = self.get_detail(ids)
         for i in range(len(ids)):
-            if data[i]["code"] == 404:
-                logger.error("未从网易云读取到下载地址")
-                return None
-            url = data[i]["url"]
-            nid = data[i]["id"]
-            filename = f"{name[i]}.{data[i]['type']}"
-            filename = re.sub('[\/:*?"<>|]', '-', filename)
-            file = Path.cwd().joinpath("music").joinpath(filename)
-            config = {
-                "id": int(nid),
-                "file": str(file),  # 获取文件位置
-                "filename": filename,  # 获取文件名
-                "from": "song" if len(ids) == 1 else "list",  # 判断来自单曲还是歌单
-                "time": datetime.now().strftime("%Y-%m-%d %H:%M:%S")  # 获取时间
-            }
-            filenames.append(file)
-            not_zips.append(config)
-            info = music.search(Q["id"] == nid)
-            if info:  # 数据库储存
-                music.update(config, Q["id"] == nid)
-            else:
-                music.insert(config)
-            async with httpx.AsyncClient() as client:  # 下载歌曲
-                async with client.stream("GET", url=url) as r:
-                    async with async_open(file, 'wb') as out_file:
-                        async for chunk in r.aiter_bytes():
-                            await out_file.write(chunk)
-            logger.debug(f"Download:{filename}")
-        if is_zip:
-            await self.get_zip(lid=lid, filenames=filenames)
-        return not_zips
+            await self.upload(data[i], "song" if len(ids) == 1 else "list", event)
+
+        # if is_zip:
+        #     await self.get_zip(lid=lid, filenames=filenames)
+        # return not_zips
 
 
 nncm = Ncm()
 info = ncm_user_cache.search(Q.uid == "user")
 if info:
     logger.info("检测到缓存，自动加载用户")
     nncm.load_user(info[0]['session'])
```

### Comparing `nonebot_plugin_ncm-1.6.8/pyproject.toml` & `nonebot_plugin_ncm-1.6.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-ncm"
-version = "1.6.8"
+version = "1.6.9"
 description = "基于go-cqhttp与nonebot2的 网易云 无损音乐下载"
 license = "Apache License 2.0"
 authors = ["kitUIN <kulujun@gmail.com>"]
 maintainers = ["kitUIN <kulujun@gmail.com>", "Kurokitu"]
 readme = "README.md"
 packages = [
     { include = "nonebot-plugin-ncm" }
```

### Comparing `nonebot_plugin_ncm-1.6.8/PKG-INFO` & `nonebot_plugin_ncm-1.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ncm
-Version: 1.6.8
+Version: 1.6.9
 Summary: 基于go-cqhttp与nonebot2的 网易云 无损音乐下载
 Home-page: https://github.com/kitUIN/nonebot-plugin-ncm
 License: Apache-2.0
 Keywords: netease-cloud-music,netease,go-cqhttp,nonebot2
 Author: kitUIN
 Author-email: kulujun@gmail.com
 Maintainer: kitUIN
@@ -130,15 +130,14 @@
 ## 配置文件说明 ⚙️
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | ncm_admin_level | 否 | 1 | 设置命令权限(1:仅限superusers和群主,2:在1的基础上+管理员,3:所有用户) |
 | ncm_ctcode | 否 | 86 | 手机号区域码 |
 | ncm_phone | 是 |   | 网易云绑定的手机号(留空则二维码登录) |
 | ncm_password | 是 |   | 网易云账号密码(留空则短信登录) |
-| ncm_playlist_zip | 否 | False | 是否开启歌单打包上传 |
 | ncm_bitrate | 否 | 320 | 下载码率(单位K) <=96: m4a, >=320:flac, 96< mp3 <320|
 ```
 # 这是示例
 ncm_admin_level=1 # 设置命令权限(1:仅限superusers和群主,2:在1的基础上+管理员,3:所有用户)
 ncm_ctcode="86" # 手机号区域码,默认86
 ncm_phone=  # 手机登录
 ncm_password=  # 密码
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ncm Version: 1.6.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-ncm Version: 1.6.9 Summary:
 åºäºgo-cqhttpä¸nonebot2ç ç½æäº æ æé³ä¹ä¸è½½ Home-page: https://
 github.com/kitUIN/nonebot-plugin-ncm License: Apache-2.0 Keywords: netease-
 cloud-music,netease,go-cqhttp,nonebot2 Author: kitUIN Author-email:
 kulujun@gmail.com Maintainer: kitUIN Maintainer-email: kulujun@gmail.com
 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
@@ -44,20 +44,19 @@
 qqå· f | å³é­è¯¥ç¨æ·ç§èä¸è½½ | - å½ä»¤å¼å§ç¬¦å·ä¼èªå¨è¯å«
 [`COMMAND_START`](https://v2.nonebot.dev/docs/api/config#Config-
 command_start)é¡¹ ## éç½®æä»¶è¯´æ âï¸ | éç½®é¡¹ | å¿å¡« | é»è®¤å¼
 | è¯´æ | |:-----:|:----:|:----:|:----:| | ncm_admin_level | å¦ | 1 |
 è®¾ç½®å½ä»¤æé(1:ä»ésuperusersåç¾¤ä¸»,2:å¨1çåºç¡ä¸+ç®¡çå,3:
 ææç¨æ·) | | ncm_ctcode | å¦ | 86 | ææºå·åºåç  | | ncm_phone |
 æ¯ | | ç½æäºç»å®çææºå·(çç©ºåäºç»´ç ç»å½) | | ncm_password
-| æ¯ | | ç½æäºè´¦å·å¯ç (çç©ºåç­ä¿¡ç»å½) | | ncm_playlist_zip |
-å¦ | False | æ¯å¦å¼å¯æ­åæåä¸ä¼  | | ncm_bitrate | å¦ | 320 |
-ä¸è½½ç ç(åä½K) <=96: m4a, >=320:flac, 96< mp3 <320| ``` # è¿æ¯ç¤ºä¾
-ncm_admin_level=1 # è®¾ç½®å½ä»¤æé(1:ä»ésuperusersåç¾¤ä¸»,2:
-å¨1çåºç¡ä¸+ç®¡çå,3:ææç¨æ·) ncm_ctcode="86" #
-ææºå·åºåç ,é»è®¤86 ncm_phone= # ææºç»å½ ncm_password= # å¯ç 
-ncm_playlist_zip=False # ä¸ä¼ æ­åæ¶æ¯å¦åç¼© ncm_bitrate: int = 320 #
-ä¸è½½ç ç(åä½K) 96åä»¥ä¸ä¸ºm4a,320åä»¥ä¸ä¸ºflac,ä¸­é´mp3 ``` ##
-åè½åè¡¨ ð - [x] è¯å«/ä¸è½½ ç½æäºåæ² - é¾æ¥ - å¡ç -
-å¡çè½¬å - [x] è¯å«/ä¸è½½ ç½æäºæ­å - é¾æ¥ - å¡ç -
-å¡çè½¬å - [x] ç¹æ­(ç½æäº) - [ ] QQé³ä¹æ æä¸è½½ # é¸£è°¢ -
-[pyncm](https://github.com/greats3an/pyncm) - [nonebot2](https://github.com/
-nonebot/nonebot2)
+| æ¯ | | ç½æäºè´¦å·å¯ç (çç©ºåç­ä¿¡ç»å½) | | ncm_bitrate | å¦ |
+320 | ä¸è½½ç ç(åä½K) <=96: m4a, >=320:flac, 96< mp3 <320| ``` #
+è¿æ¯ç¤ºä¾ ncm_admin_level=1 # è®¾ç½®å½ä»¤æé(1:
+ä»ésuperusersåç¾¤ä¸»,2:å¨1çåºç¡ä¸+ç®¡çå,3:ææç¨æ·)
+ncm_ctcode="86" # ææºå·åºåç ,é»è®¤86 ncm_phone= # ææºç»å½
+ncm_password= # å¯ç  ncm_playlist_zip=False # ä¸ä¼ æ­åæ¶æ¯å¦åç¼©
+ncm_bitrate: int = 320 # ä¸è½½ç ç(åä½K)
+96åä»¥ä¸ä¸ºm4a,320åä»¥ä¸ä¸ºflac,ä¸­é´mp3 ``` ## åè½åè¡¨ ð - [x]
+è¯å«/ä¸è½½ ç½æäºåæ² - é¾æ¥ - å¡ç - å¡çè½¬å - [x] è¯å«/
+ä¸è½½ ç½æäºæ­å - é¾æ¥ - å¡ç - å¡çè½¬å - [x] ç¹æ­(ç½æäº)
+- [ ] QQé³ä¹æ æä¸è½½ # é¸£è°¢ - [pyncm](https://github.com/greats3an/
+pyncm) - [nonebot2](https://github.com/nonebot/nonebot2)
```

