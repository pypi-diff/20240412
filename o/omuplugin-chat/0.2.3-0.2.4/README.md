# Comparing `tmp/omuplugin_chat-0.2.3.tar.gz` & `tmp/omuplugin_chat-0.2.4.tar.gz`

## Comparing `omuplugin_chat-0.2.3.tar` & `omuplugin_chat-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.3/.python-version
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.3/src/omuplugin_chat/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.3/src/omuplugin_chat/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.3/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.3/README.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.4/.python-version
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.4/src/omuplugin_chat/__init__.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.4/src/omuplugin_chat/plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.4/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.4/README.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.4/PKG-INFO
```

### Comparing `omuplugin_chat-0.2.3/src/omuplugin_chat/plugin.py` & `omuplugin_chat-0.2.4/src/omuplugin_chat/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,19 +13,15 @@
     PROVIDER_TABLE,
     ROOM_TABLE,
 )
 from omuchat.model.channel import Channel
 
 app = App(
     IDENTIFIER,
-    description="",
     version="0.1.0",
-    authors=["omu"],
-    license="MIT",
-    repository_url="https://github.com/OMUCHAT",
 )
 address = Address("127.0.0.1", 26423)
 client = OmuClient(app, address=address)
 
 
 messages = client.tables.get(MESSAGE_TABLE)
 authors = client.tables.get(AUTHOR_TABLE)
@@ -37,27 +33,27 @@
 
 
 @client.endpoints.bind(endpoint_type=CREATE_CHANNEL_TREE_ENDPOINT)
 async def create_channel_tree(url: str) -> List[Channel]:
     results = await iwashi.visit(url)
     if results is None:
         return []
-    channels: List[Channel] = []
+    found_channels: List[Channel] = []
     services = await providers.fetch_items()
     for result in results.to_list():
         for provider in services.values():
             if provider.id == "misskey":
                 continue
             if re.search(provider.regex, result.url) is None:
                 continue
-            channels.append(
+            found_channels.append(
                 Channel(
                     provider_id=provider.key(),
                     id=result.url,
                     url=result.url,
                     name=result.title or result.site_name or result.url,
                     description=result.description or "",
                     active=True,
                     icon_url=result.profile_picture or "",
                 )
             )
-    return channels
+    return found_channels
```

### Comparing `omuplugin_chat-0.2.3/pyproject.toml` & `omuplugin_chat-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuplugin_chat"
-version = "0.2.3"
+version = "0.2.4"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["omuchat>=0.1.9"]
 readme = "README.md"
 requires-python = ">= 3.12"
```

