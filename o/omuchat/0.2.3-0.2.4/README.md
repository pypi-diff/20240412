# Comparing `tmp/omuchat-0.2.3.tar.gz` & `tmp/omuchat-0.2.4.tar.gz`

## Comparing `omuchat-0.2.3.tar` & `omuchat-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuchat-0.2.3/.python-version
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuchat-0.2.3/.vscode/settings.json
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 omuchat-0.2.3/example/chatlogger.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/__init__.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/chat.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/client.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/event/__init__.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/event/event.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/event/event_types.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/model/__init__.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/model/author.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/model/channel.py
--rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/model/content.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/model/gift.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/model/message.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/model/paid.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/model/provider.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/model/role.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 omuchat-0.2.3/src/omuchat/model/room.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omuchat-0.2.3/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 omuchat-0.2.3/README.md
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 omuchat-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 omuchat-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuchat-0.2.4/.python-version
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuchat-0.2.4/.vscode/settings.json
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 omuchat-0.2.4/example/chatlogger.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/__init__.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/chat.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/client.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/event/__init__.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/event/event.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/event/event_types.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/__init__.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/author.py
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/channel.py
+-rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/content.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/gift.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/message.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/paid.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/provider.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/role.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 omuchat-0.2.4/src/omuchat/model/room.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omuchat-0.2.4/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 omuchat-0.2.4/README.md
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 omuchat-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 omuchat-0.2.4/PKG-INFO
```

### Comparing `omuchat-0.2.3/src/omuchat/chat.py` & `omuchat-0.2.4/src/omuchat/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     IDENTIFIER,
     "rooms",
     Room,
 )
 CREATE_CHANNEL_TREE_ENDPOINT = EndpointType[str, List[Channel]].create_json(
     IDENTIFIER,
     "create_channel_tree",
-    response_serializer=Serializer.model(Channel).array(),
+    response_serializer=Serializer.model(Channel).to_array(),
 )
 
 
 class Chat:
     def __init__(
         self,
         client: Client,
```

### Comparing `omuchat-0.2.3/src/omuchat/client.py` & `omuchat-0.2.4/src/omuchat/client.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.3/src/omuchat/event/event.py` & `omuchat-0.2.4/src/omuchat/event/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     from omuchat.client import Client
 
 type EventHandler[**P] = Callable[P, Coroutine[None, None, None]]
 
 
 @dataclass(frozen=True)
 class EventSource[**P]:
-    subscribe: Callable[[EventHandler[P], Client]]
-    unsubscribe: Callable[[EventHandler[P], Client]]
+    subscribe: Callable[[EventHandler[P], Client], None]
+    unsubscribe: Callable[[EventHandler[P], Client], None]
 
 
 class ListenerEvent[**P](EventSource[P]):
     def __init__(self, get_listener: Callable[[Client], EventEmitter[P]]):
         super().__init__(self._subscribe, self._unsubscribe)
         self.get_listener = get_listener
 
@@ -66,15 +66,16 @@
             lambda table: table.listeners.remove,
         )
         self.clear = ListenerEvent(
             lambda client: get_table(client).listeners.clear,
         )
         self.wrappers = {}
 
-    def _create_batch_wrapper(self, emit: EventHandler[[T]]):
+    @staticmethod
+    def _create_batch_wrapper(emit: EventHandler[[T]]):
         async def wrapper(items: Mapping[str, T]):
             for item in items.values():
                 await emit(item)
 
         return wrapper
 
     def _create_batch_subscriber(
```

### Comparing `omuchat-0.2.3/src/omuchat/event/event_types.py` & `omuchat-0.2.4/src/omuchat/event/event_types.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.3/src/omuchat/model/author.py` & `omuchat-0.2.4/src/omuchat/model/author.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.3/src/omuchat/model/channel.py` & `omuchat-0.2.4/src/omuchat/model/channel.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.3/src/omuchat/model/content.py` & `omuchat-0.2.4/src/omuchat/model/content.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.3/src/omuchat/model/gift.py` & `omuchat-0.2.4/src/omuchat/model/gift.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.3/src/omuchat/model/message.py` & `omuchat-0.2.4/src/omuchat/model/message.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.3/src/omuchat/model/paid.py` & `omuchat-0.2.4/src/omuchat/model/paid.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.3/src/omuchat/model/provider.py` & `omuchat-0.2.4/src/omuchat/model/provider.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.3/src/omuchat/model/role.py` & `omuchat-0.2.4/src/omuchat/model/role.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.3/src/omuchat/model/room.py` & `omuchat-0.2.4/src/omuchat/model/room.py`

 * *Files identical despite different names*

