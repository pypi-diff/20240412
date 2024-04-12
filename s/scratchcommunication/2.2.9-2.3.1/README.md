# Comparing `tmp/scratchcommunication-2.2.9.tar.gz` & `tmp/scratchcommunication-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.2.9.tar", last modified: Fri Mar  8 09:26:59 2024, max compression
+gzip compressed data, was "scratchcommunication-2.3.1.tar", last modified: Fri Apr 12 17:47:30 2024, max compression
```

## Comparing `scratchcommunication-2.2.9.tar` & `scratchcommunication-2.3.1.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:26:59.156059 scratchcommunication-2.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-03-08 09:26:59.156059 scratchcommunication-2.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:26:59.156059 scratchcommunication-2.2.9/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14674 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/scratchcommunication/cloud_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:26:59.156059 scratchcommunication-2.2.9/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-03-08 09:26:59.000000 scratchcommunication-2.2.9/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-08 09:26:59.000000 scratchcommunication-2.2.9/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 09:26:59.000000 scratchcommunication-2.2.9/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-08 09:26:59.000000 scratchcommunication-2.2.9/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-08 09:26:59.000000 scratchcommunication-2.2.9/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 09:26:59.156059 scratchcommunication-2.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:47:30.243297 scratchcommunication-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-12 17:47:26.000000 scratchcommunication-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11086 2024-04-12 17:47:30.243297 scratchcommunication-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-04-12 17:47:26.000000 scratchcommunication-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:47:30.243297 scratchcommunication-2.3.1/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-12 17:47:26.000000 scratchcommunication-2.3.1/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16890 2024-04-12 17:47:26.000000 scratchcommunication-2.3.1/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-04-12 17:47:26.000000 scratchcommunication-2.3.1/scratchcommunication/cloud_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:47:30.243297 scratchcommunication-2.3.1/scratchcommunication/cloudrequests/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-12 17:47:26.000000 scratchcommunication-2.3.1/scratchcommunication/cloudrequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-12 17:47:26.000000 scratchcommunication-2.3.1/scratchcommunication/cloudrequests/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-04-12 17:47:26.000000 scratchcommunication-2.3.1/scratchcommunication/cloudrequests/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-12 17:47:26.000000 scratchcommunication-2.3.1/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-12 17:47:26.000000 scratchcommunication-2.3.1/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-12 17:47:26.000000 scratchcommunication-2.3.1/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-12 17:47:26.000000 scratchcommunication-2.3.1/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:47:30.243297 scratchcommunication-2.3.1/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11086 2024-04-12 17:47:30.000000 scratchcommunication-2.3.1/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-12 17:47:30.000000 scratchcommunication-2.3.1/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:47:30.000000 scratchcommunication-2.3.1/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 17:47:30.000000 scratchcommunication-2.3.1/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-12 17:47:30.000000 scratchcommunication-2.3.1/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:47:30.243297 scratchcommunication-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-12 17:47:26.000000 scratchcommunication-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:47:30.243297 scratchcommunication-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-12 17:47:26.000000 scratchcommunication-2.3.1/tests/test1.py
```

### Comparing `scratchcommunication-2.2.9/LICENSE` & `scratchcommunication-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.2.9/PKG-INFO` & `scratchcommunication-2.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.2.9
+Version: 2.3.1
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -116,30 +116,32 @@
     project_id = "Your project id here", 
     username = "player1000", # (Optional)
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", # (Optional) Changes the host used for cloud variables.
-    accept_strs = False # (Optional) Allows you to set cloud variables to strings. Only works if cloud host allows it.
+    accept_strs = False, # (Optional) Allows you to set cloud variables to strings. Only works if cloud host allows it.
+    keep_all_events = False # (Optional) Allows you to disable automatic garbage disposal of events. Events can still be manually disposed of. Unrecommended because it will slowly but surely fill up a lot of memory if events aren't disposed of.
 )
 ```
 
 Or you could connect from your session
 
 ```python
 tw_cloud = session.create_turbowarp_cloudconnection(
     project_id = "Your project id here",
     username = None, # (Optional) Will default to your username
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", 
-    accept_strs = False 
+    accept_strs = False,
+    keep_all_events = False
 )
 ```
 
 To shorten it a bit you can also use `scratchcommunication.session.Session.create_tw_cloudconnection` instead of `scratchcommunication.session.Session.create_turbowarp_cloudconnection`.
 
 ## Working with cloud variables
 
@@ -199,14 +201,22 @@
 
 If you want to stop the background thread used for events and variable updates, you can use `scratchcommunication.cloud.CloudConnection.stop_thread`
 
 ```python
 cloud.stop_thread()
 ```
 
+You can also manually dispose of events (which normally happens automatically).
+
+```python
+cloud.garbage_disposal_of_events(
+    force_disposal = False # (Optional) Is needed to be True if automatic garbage disposal is disabled.
+)
+```
+
 If you set `daemon_thread` to `True` when creating the object, the background thread will terminate when your process ends.
 
 # Cloud sockets
 
 Cloud sockets (inspired by sockets) are connections from a scratch project to a python program where both sides can send data to one another and there is even the possibility to add security to the connection using RSA.
 
 ## Creating a cloud socket
```

### Comparing `scratchcommunication-2.2.9/README.md` & `scratchcommunication-2.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -92,30 +92,32 @@
     project_id = "Your project id here", 
     username = "player1000", # (Optional)
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", # (Optional) Changes the host used for cloud variables.
-    accept_strs = False # (Optional) Allows you to set cloud variables to strings. Only works if cloud host allows it.
+    accept_strs = False, # (Optional) Allows you to set cloud variables to strings. Only works if cloud host allows it.
+    keep_all_events = False # (Optional) Allows you to disable automatic garbage disposal of events. Events can still be manually disposed of. Unrecommended because it will slowly but surely fill up a lot of memory if events aren't disposed of.
 )
 ```
 
 Or you could connect from your session
 
 ```python
 tw_cloud = session.create_turbowarp_cloudconnection(
     project_id = "Your project id here",
     username = None, # (Optional) Will default to your username
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", 
-    accept_strs = False 
+    accept_strs = False,
+    keep_all_events = False
 )
 ```
 
 To shorten it a bit you can also use `scratchcommunication.session.Session.create_tw_cloudconnection` instead of `scratchcommunication.session.Session.create_turbowarp_cloudconnection`.
 
 ## Working with cloud variables
 
@@ -175,14 +177,22 @@
 
 If you want to stop the background thread used for events and variable updates, you can use `scratchcommunication.cloud.CloudConnection.stop_thread`
 
 ```python
 cloud.stop_thread()
 ```
 
+You can also manually dispose of events (which normally happens automatically).
+
+```python
+cloud.garbage_disposal_of_events(
+    force_disposal = False # (Optional) Is needed to be True if automatic garbage disposal is disabled.
+)
+```
+
 If you set `daemon_thread` to `True` when creating the object, the background thread will terminate when your process ends.
 
 # Cloud sockets
 
 Cloud sockets (inspired by sockets) are connections from a scratch project to a python program where both sides can send data to one another and there is even the possibility to add security to the connection using RSA.
 
 ## Creating a cloud socket
```

### Comparing `scratchcommunication-2.2.9/scratchcommunication/cloud.py` & `scratchcommunication-2.3.1/scratchcommunication/cloud.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,60 @@
 from typing import Literal, Union, Any
-from .exceptions import QuickAccessDisabledError, NotSupported, ErrorInEventHandler, StopException
-import json, time, requests, warnings, traceback
+from .exceptions import QuickAccessDisabledError, NotSupported, ErrorInEventHandler, StopException, EventExpiredError
+import json, time, requests, warnings, traceback, secrets, sys
 from websocket import WebSocket
 from func_timeout import StoppableThread
 
 NoneType = type(None)
 CloudConnection = None
 
 class Event:
+    _id : int = None
     value : Union[float, int, bool] = None
     var : str = None
     name : str = None
     project : CloudConnection = None
     def __init__(self, _type: Literal["set", "delete", "connect", "create"], **entries):
         entries["type"] = _type
         self.__dict__.update(entries)
         self._data = None
         self.project = getattr(self, "project")
+        self._id = secrets.randbits(16)
+        
 
     @property
     def data(self):
         if not hasattr(self, "var"):
             raise NotSupported("No setting")
         if not self._data:
-            self._data = list(
-                filter(
-                    lambda x: x["value"] == self.value,
-                    self.project.get_cloud_logs(
-                        project_id=self.project.project_id,
-                        filter_by_name=self.var,
-                        filter_by_name_literal=True,
-                    ),
-                )
-            )[0]
+            try:
+                self._data = list(
+                    filter(
+                        lambda x: x["value"] == self.value,
+                        self.project.get_cloud_logs(
+                            project_id=self.project.project_id,
+                            filter_by_name=self.var,
+                            filter_by_name_literal=True,
+                        ),
+                    )
+                )[self.project.get_age_of_event(self)]
+            except IndexError:
+                raise EventExpiredError("Event expired. (Cannot fetch data from Scratch server)")
         return self._data
 
     @property
     def user(self):
         return self.data["user"]
 
     @property
     def timestamp(self):
         return self.data["timestamp"]
+    
+    def hash(self):
+        return hash(self._id)
 
 
 class CloudConnection:
     """
     Connect to a cloud server and set cloud variables.
     """
     project_id : int
@@ -58,27 +67,34 @@
     values : dict
     events : dict
     cloud_host : str
     accept_strs : bool
     wait_until : Union[float, int]
     receive_from_websocket : bool
     data_reception : Any
+    event_order : dict[Union[float, int, bool], dict[Event, int]]
+    processed_events : list[Event]
+    keep_all_events : bool
     def __init__(
         self,
         *,
         project_id : int,
         session = None,
         username : str = None,
         quickaccess : bool = False,
         reconnect : bool = True,
         receive_from_websocket : bool = True,
         warning_type : type[Warning] = ErrorInEventHandler,
         daemon_thread : bool = False,
-        connect : bool = True
+        connect : bool = True,
+        keep_all_events : bool = False
     ):
+        self.keep_all_events = keep_all_events
+        self.event_order = {}
+        self.processed_events = []
         self.thread_running = True
         self.warning_type = warning_type
         self.project_id = project_id
         self.session = session
         self.username = username if username is not None else session.username
         self.quickaccess = quickaccess
         self.reconnect = reconnect
@@ -134,14 +150,15 @@
         try:
             self.websocket = WebSocket()
             self.websocket.connect(
                 "wss://clouddata.scratch.mit.edu",
                 cookie="scratchsessionsid=" + self.session.session_id + ";",
                 origin="https://scratch.mit.edu",
                 enable_multithread=True,
+                timeout=5
             )
             self.handshake()
             self.emit_event("connect", timestamp=time.time())
         except Exception as e:
             if retry == 1:
                 raise ConnectionError(
                     f"There was an error while connecting to the cloud server."
@@ -296,14 +313,15 @@
         self.set_variable(name=item, value=value)
 
     def receive_new_data(self, first : bool = False) -> dict:
         """
         Use for receiving new cloud data.
         """
         data = [json.loads(j) for j in self.websocket.recv().split("\n") if j]
+        
         for i in data:
             i["var"] = i["name"]
             i["name"] = i["name"].replace("☁ ", "", 1)
             method = i.pop("method")
             if not first:
                 self.emit_event(method, **i)
             if method == "set":
@@ -312,40 +330,73 @@
 
     def receive_data(self):
         """
         Use for receiving cloud data.
         """
         while self.thread_running:
             try:
-                self._connect()
                 self.receive_new_data(first=True)
                 break
-            except Exception:
+            except TimeoutError:
                 pass
+            except Exception:
+                self._connect()
         while self.thread_running:
             try:
                 self.receive_new_data()
+            except TimeoutError:
+                pass
             except Exception:
+                self._connect()
                 while self.thread_running:
                     try:
-                        self._connect()
                         self.receive_new_data(first=True)
                         break
-                    except Exception:
+                    except TimeoutError:
                         pass
+                    except Exception:
+                        self._connect()
+                    
+    def get_age_of_event(self, event : Event) -> int:
+        """
+        Do not use.
+        """
+        try:
+            return len(self.event_order.get(event.value, {})) - self.event_order.get(event.value, {})[event] - 1
+        except KeyError:
+            raise ValueError("No such event")
 
     def emit_event(self, event : Union[Literal["set", "delete", "connect", "create"], Event], **entries) -> int:
         """
         Use for emitting events. Returns how many handlers could handle the event.
         """
         data = event if isinstance(event, Event) else Event(event, **entries)
         data.project = self
         if isinstance(event, Event):
             event = event.type
-        return self._emit_event(event, data) + self._emit_event("any", data)
+        if not self.event_order.get(data.value):
+            self.event_order[data.value] = {}
+        self.event_order[data.value][data] = len(self.event_order[data.value])
+        amount = self._emit_event(event, data) + self._emit_event("any", data)
+        self.processed_events.append(data)
+        if not self.keep_all_events:
+            self.garbage_disposal_of_events()
+        return amount
+    
+    def garbage_disposal_of_events(self, force_disposal : bool = False) -> int:
+        """
+        Dispose of all unused events
+        """
+        if self.keep_all_events and not force_disposal:
+            warnings.warn("Attempted to dispose of all events with keep_all_events enabled. Try to set force_disposal=True in order to force garbage disposal.", UserWarning)
+            return
+        for event in self.processed_events.copy():
+            if sys.getrefcount(event) <= 5:
+                self.processed_events.remove(event)
+                self.event_order.get(event.value).pop(event)
 
     def _emit_event(self, event : Literal["set", "delete", "connect", "create", "any"], data : Event) -> int:
         """
         Don't use this.
         """
         amount = 0
         if not event in self.events:
@@ -376,34 +427,35 @@
         return wrapper
 
 
 class TwCloudConnection(CloudConnection):
     def __init__(
         self, 
         *, 
-        project_id : int, 
+        project_id : str, 
         username : str = "player1000", 
         quickaccess : bool = False, 
         reconnect : bool = True, 
         receive_from_websocket : bool = True, 
         warning_type : type[Warning] = ErrorInEventHandler,
         daemon_thread : bool = False, 
         cloud_host : str = "wss://clouddata.turbowarp.org/", 
-        accept_strs : bool = False
+        accept_strs : bool = False,
+        keep_all_events : bool = False
     ):
         super().__init__(
-            self,
             project_id=project_id, 
             username=username,
             quickaccess=quickaccess,
             reconnect=reconnect,
             receive_from_websocket=receive_from_websocket,
             warning_type=warning_type,
             daemon_thread=daemon_thread,
-            connect=False
+            connect=False,
+            keep_all_events=keep_all_events
         )
         self.cloud_host = cloud_host
         self.accept_strs = accept_strs
         self._connect()
         if not self.receive_from_websocket:
             while True:
                 try:
@@ -415,15 +467,15 @@
         self.data_reception.start()
 
     def _connect(self, *, cloud_host = None, retry : int = 10):
         try:
             if cloud_host is not None:
                 self.cloud_host = cloud_host
             self.websocket = WebSocket()
-            self.websocket.connect(self.cloud_host, enable_multithread=True, timeout=10)
+            self.websocket.connect(self.cloud_host, enable_multithread=True, timeout=5)
             self.handshake()
             self.emit_event("connect")
         except Exception as e:
             if retry == 1:
                 raise ConnectionError(
                     f"There was an error while connecting to the cloud server."
                 ) from e
@@ -438,8 +490,8 @@
         Use for detecting if a value can be used for cloud variables.
         """
         try:
             float(value)
         except Exception as e:
             if self.accept_strs and isinstance(value, str):
                 return
-            raise ValueError("Bad value for cloud variables.") from e
+            raise ValueError("Bad value for cloud variables.") from e
```

### Comparing `scratchcommunication-2.2.9/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.3.1/scratchcommunication/cloud_socket.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.2.9/scratchcommunication/security.py` & `scratchcommunication-2.3.1/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.2.9/scratchcommunication/session.py` & `scratchcommunication-2.3.1/scratchcommunication/session.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.2.9/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.3.1/scratchcommunication.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.2.9
+Version: 2.3.1
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -116,30 +116,32 @@
     project_id = "Your project id here", 
     username = "player1000", # (Optional)
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", # (Optional) Changes the host used for cloud variables.
-    accept_strs = False # (Optional) Allows you to set cloud variables to strings. Only works if cloud host allows it.
+    accept_strs = False, # (Optional) Allows you to set cloud variables to strings. Only works if cloud host allows it.
+    keep_all_events = False # (Optional) Allows you to disable automatic garbage disposal of events. Events can still be manually disposed of. Unrecommended because it will slowly but surely fill up a lot of memory if events aren't disposed of.
 )
 ```
 
 Or you could connect from your session
 
 ```python
 tw_cloud = session.create_turbowarp_cloudconnection(
     project_id = "Your project id here",
     username = None, # (Optional) Will default to your username
     quickaccess = False, 
     reconnect = True, 
     receive_from_websocket = True, 
     warning_type = ErrorInEventHandler, 
     cloud_host = "wss://clouddata.turbowarp.org/", 
-    accept_strs = False 
+    accept_strs = False,
+    keep_all_events = False
 )
 ```
 
 To shorten it a bit you can also use `scratchcommunication.session.Session.create_tw_cloudconnection` instead of `scratchcommunication.session.Session.create_turbowarp_cloudconnection`.
 
 ## Working with cloud variables
 
@@ -199,14 +201,22 @@
 
 If you want to stop the background thread used for events and variable updates, you can use `scratchcommunication.cloud.CloudConnection.stop_thread`
 
 ```python
 cloud.stop_thread()
 ```
 
+You can also manually dispose of events (which normally happens automatically).
+
+```python
+cloud.garbage_disposal_of_events(
+    force_disposal = False # (Optional) Is needed to be True if automatic garbage disposal is disabled.
+)
+```
+
 If you set `daemon_thread` to `True` when creating the object, the background thread will terminate when your process ends.
 
 # Cloud sockets
 
 Cloud sockets (inspired by sockets) are connections from a scratch project to a python program where both sides can send data to one another and there is even the possibility to add security to the connection using RSA.
 
 ## Creating a cloud socket
```

### Comparing `scratchcommunication-2.2.9/setup.py` & `scratchcommunication-2.3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='scratchcommunication',
-    version='2.2.9',
+    version='2.3.1',
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/thecommcraft/scratchcommunication',
     packages=find_packages(exclude=[]),
```

