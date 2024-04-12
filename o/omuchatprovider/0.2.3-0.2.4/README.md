# Comparing `tmp/omuchatprovider-0.2.3.tar.gz` & `tmp/omuchatprovider-0.2.4.tar.gz`

## Comparing `omuchatprovider-0.2.3.tar` & `omuchatprovider-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/.python-version
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/run.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/.vscode/launch.json
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/.vscode/settings.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/src/omuchatprovider/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/src/omuchatprovider/__main__.py
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/src/omuchatprovider/chatprovider.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/src/omuchatprovider/errors.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/src/omuchatprovider/helper.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/src/omuchatprovider/services/__init__.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/src/omuchatprovider/services/service.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/src/omuchatprovider/services/youtube/__init__.py
--rw-r--r--   0        0        0    29120 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/src/omuchatprovider/services/youtube/youtube.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/src/omuchatprovider/services/youtube/types/__init__.py
--rw-r--r--   0        0        0    14367 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/src/omuchatprovider/services/youtube/types/api.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/src/omuchatprovider/tasks/__init__.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/src/omuchatprovider/tasks/taskprofiler.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/README.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 omuchatprovider-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/.python-version
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/run.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/.vscode/launch.json
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/.vscode/settings.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/__main__.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/chatprovider.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/errors.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/helper.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/services/__init__.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/services/service.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/services/youtube/__init__.py
+-rw-r--r--   0        0        0    29251 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/services/youtube/youtube.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/services/youtube/types/__init__.py
+-rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/services/youtube/types/api.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/tasks/__init__.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/src/omuchatprovider/tasks/taskprofiler.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/README.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 omuchatprovider-0.2.4/PKG-INFO
```

### Comparing `omuchatprovider-0.2.3/src/omuchatprovider/chatprovider.py` & `omuchatprovider-0.2.4/src/omuchatprovider/chatprovider.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,15 @@
 from omuchatprovider.errors import ProviderError
 
 from .services import ChatService, ProviderService, get_services
 
 IDENTIFIER = Identifier("cc.omuchat", "chatprovider")
 APP = App(
     identifier=IDENTIFIER,
-    description="Chat provider for Omu",
     version="0.1.0",
-    authors=["omu"],
-    license="MIT",
-    repository_url="https://github.com/OMUCHAT/provider",
 )
 
 
 client = Client(APP)
 services: dict[str, ProviderService] = {}
 chats: dict[str, ChatService] = {}
```

### Comparing `omuchatprovider-0.2.3/src/omuchatprovider/helper.py` & `omuchatprovider-0.2.4/src/omuchatprovider/helper.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.2.3/src/omuchatprovider/services/service.py` & `omuchatprovider-0.2.4/src/omuchatprovider/services/service.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.2.3/src/omuchatprovider/services/youtube/youtube.py` & `omuchatprovider-0.2.4/src/omuchatprovider/services/youtube/youtube.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from collections import Counter
 from datetime import datetime
 from typing import Dict, List, Mapping, Tuple, TypedDict
 
 import bs4
 from iwashi.visitors.youtube.youtube import Youtube
 from loguru import logger
+from omu.extension.message import MessageType
 from omu.helper import map_optional
 from omuchat.client import Client
 from omuchat.model import (
     MODERATOR,
     OWNER,
     VERIFIED,
     Author,
@@ -50,20 +51,23 @@
 )
 
 
 YOUTUBE_VISITOR = Youtube()
 session = get_session(INFO)
 
 
-class ReactionEvent(TypedDict):
+class ReactionMessage(TypedDict):
     room_id: str
     reactions: Dict[str, int]
 
 
-REACTION_MESSAGE = client.message.create("youtube-reaction", ReactionEvent)
+REACTION_MESSAGE_TYPE = MessageType[ReactionMessage].create_json(
+    identifier=client.app.identifier / "youtube", name="reaction"
+)
+REACTION_MESSAGE = client.message.get(REACTION_MESSAGE_TYPE)
 
 HEADERS = {
     "User-Agent": (
         "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 "
         "(KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36"
     )
 }
@@ -504,57 +508,56 @@
             message = Message(
                 id=data["id"],
                 room_id=self._room.key(),
                 author_id=author.key(),
                 content=message,
                 created_at=created_at,
             )
-            return (message, author)
+            return message, author
         elif "liveChatPaidMessageRenderer" in item:
             data = item["liveChatPaidMessageRenderer"]
             author = self._parse_author(data)
             message = map_optional(data.get("message"), _parse_runs)
             paid = self._parse_paid(data)
             created_at = self._parse_created_at(data)
             message = Message(
                 id=data["id"],
                 room_id=self._room.key(),
                 author_id=author.key(),
                 content=message,
                 paid=paid,
                 created_at=created_at,
             )
-            return (message, author)
+            return message, author
         elif "liveChatMembershipItemRenderer" in item:
             data = item["liveChatMembershipItemRenderer"]
             author = self._parse_author(data)
             created_at = self._parse_created_at(data)
-            logger.info
             component = content.System.of(_parse_runs(data["headerSubtext"]))
             message = Message(
                 id=data["id"],
                 room_id=self._room.key(),
                 author_id=author.key(),
                 content=component,
                 created_at=created_at,
             )
-            return (message, author)
+            return message, author
         elif "liveChatSponsorshipsGiftRedemptionAnnouncementRenderer" in item:
             data = item["liveChatSponsorshipsGiftRedemptionAnnouncementRenderer"]
             author = self._parse_author(data)
             created_at = self._parse_created_at(data)
             component = content.System.of(_parse_runs(data["message"]))
             message = Message(
                 id=data["id"],
                 room_id=self._room.key(),
                 author_id=author.key(),
                 content=component,
                 created_at=created_at,
             )
-            return (message, author)
+            return message, author
         elif "liveChatSponsorshipsGiftPurchaseAnnouncementRenderer" in item:
             data = item["liveChatSponsorshipsGiftPurchaseAnnouncementRenderer"]
             author = self._parse_author(data)
             created_at = self._parse_created_at(data)
             header = data["header"]["liveChatSponsorshipsHeaderRenderer"]
             component = content.System.of(_parse_runs(header["primaryText"]))
 
@@ -572,15 +575,15 @@
                 id=data["id"],
                 room_id=self._room.key(),
                 author_id=author.key(),
                 content=component,
                 created_at=created_at,
                 gifts=[gift],
             )
-            return (message, author)
+            return message, author
         elif "liveChatPlaceholderItemRenderer" in item:
             """
             item["liveChatPlaceholderItemRenderer"] = {'id': 'ChwKGkNJdml3ZUg0aDRRREZSTEV3Z1FkWUlJTkNR', 'timestampUsec': '1706714981296711'}}
             """
         elif "liveChatPaidStickerRenderer" in item:
             data = item["liveChatPaidStickerRenderer"]
             author = self._parse_author(data)
@@ -598,18 +601,18 @@
             message = Message(
                 id=data["id"],
                 room_id=self._room.key(),
                 author_id=author.key(),
                 gifts=[sticker],
                 created_at=created_at,
             )
-            return (message, author)
+            return message, author
         else:
             raise ProviderError(f"Unknown message type: {list(item.keys())} {item=}")
-        return (None, None)
+        return None, None
 
     async def process_deleted_item(self, item: api.MarkChatItemAsDeletedActionData):
         message = await self.client.chat.messages.get(
             f"{self._room.key()}#{item["targetItemId"]}"
         )
         if message:
             await self.client.chat.messages.remove(message)
@@ -635,15 +638,15 @@
                         reaction["unicodeEmojiId"]: reaction["reactionCount"]
                         for reaction in bucket.get("reactionsData", [])
                     }
                 )
         if not reaction_counts:
             return
         await REACTION_MESSAGE.broadcast(
-            ReactionEvent(
+            ReactionMessage(
                 room_id=self._room.key(),
                 reactions=dict(reaction_counts),
             ),
         )
 
     def _parse_author(self, message: api.LiveChatMessageRenderer) -> Author:
         name = message.get("authorName", {}).get("simpleText")
```

### Comparing `omuchatprovider-0.2.3/src/omuchatprovider/services/youtube/types/api.py` & `omuchatprovider-0.2.4/src/omuchatprovider/services/youtube/types/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -212,56 +212,36 @@
     authorName: SimpleText
     authorPhoto: Thumbnails
     authorBadges: NotRequired[List[AuthorBadge]]
     message: Runs
 
 
 class LiveChatTextMessageRenderer(LiveChatMessageRenderer):
-    id: str
-    timestampUsec: str
-    authorExternalChannelId: str
-    authorName: SimpleText
-    authorPhoto: Thumbnails
-    message: Runs
-    authorBadges: NotRequired[List[AuthorBadge]]
     contextMenuEndpoint: ContextMenuEndpoint
     contextMenuAccessibility: Accessibility
 
 
 class LiveChatPaidMessageRenderer(LiveChatMessageRenderer):
-    id: str
-    timestampUsec: str
-    authorName: SimpleText
-    authorPhoto: Thumbnails
     purchaseAmountText: SimpleText
-    message: Runs
     headerBackgroundColor: int
     headerTextColor: int
     bodyBackgroundColor: int
     bodyTextColor: int
-    authorExternalChannelId: str
     authorNameTextColor: int
     contextMenuEndpoint: ContextMenuEndpoint
     timestampColor: int
     contextMenuAccessibility: Accessibility
     trackingParams: str
-    authorBadges: NotRequired[List[AuthorBadge]]
     textInputBackgroundColor: int
     creatorHeartButton: CreatorHeartButton
     isV2Style: bool
 
 
 class LiveChatPaidStickerRenderer(LiveChatMessageRenderer):
-    id: str
-    timestampUsec: str
-    authorName: SimpleText
-    authorPhoto: Thumbnails
     sticker: Image
-    authorExternalChannelId: str
-    authorBadges: NotRequired[List[AuthorBadge]]
     purchaseAmountText: SimpleText
     contextMenuEndpoint: ContextMenuEndpoint
     contextMenuAccessibility: Accessibility
     trackingParams: str
 
 
 class LiveChatMembershipItemRenderer(LiveChatMessageRenderer):
@@ -387,17 +367,14 @@
             "header": {
 
             }
         }
     }
     """
 
-    id: str
-    timestampUsec: str
-    authorExternalChannelId: str
     header: LiveChatSponsorshipsGiftPurchaseAnnouncementRendererHeader
 
 
 class MessageItemData(TypedDict):
     liveChatTextMessageRenderer: NotRequired[LiveChatTextMessageRenderer]
     liveChatPaidMessageRenderer: NotRequired[LiveChatPaidMessageRenderer]
     liveChatPaidStickerRenderer: NotRequired[LiveChatPaidStickerRenderer]
```

### Comparing `omuchatprovider-0.2.3/src/omuchatprovider/tasks/taskprofiler.py` & `omuchatprovider-0.2.4/src/omuchatprovider/tasks/taskprofiler.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.2.3/pyproject.toml` & `omuchatprovider-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuchatprovider"
-version = "0.2.3"
+version = "0.2.4"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = [
     "aiohttp>=3.9.1",
     "beautifulsoup4>=4.12.2",
```

