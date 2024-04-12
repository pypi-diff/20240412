# Comparing `tmp/startrek-1.1.2.tar.gz` & `tmp/startrek-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/startrek-1.1.2.tar", last modified: Wed Mar 13 11:07:19 2024, max compression
+gzip compressed data, was "dist/startrek-1.1.3.tar", last modified: Fri Apr 12 10:36:07 2024, max compression
```

## Comparing `startrek-1.1.2.tar` & `startrek-1.1.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:07:19.000000 startrek-1.1.2/
--rw-r--r--   0 moky       (501) staff       (20)      449 2024-03-13 11:07:19.000000 startrek-1.1.2/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)       25 2021-05-06 07:15:56.000000 startrek-1.1.2/README.md
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-03-13 11:07:19.000000 startrek-1.1.2/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      826 2024-03-13 08:59:41.000000 startrek-1.1.2/setup.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:07:19.000000 startrek-1.1.2/startrek/
--rw-r--r--   0 moky       (501) staff       (20)     2520 2023-01-13 11:45:48.000000 startrek-1.1.2/startrek/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     5463 2024-03-06 13:31:40.000000 startrek-1.1.2/startrek/arrival.py
--rw-r--r--   0 moky       (501) staff       (20)    11425 2024-03-06 13:32:13.000000 startrek-1.1.2/startrek/departure.py
--rw-r--r--   0 moky       (501) staff       (20)     4960 2024-03-06 13:33:03.000000 startrek-1.1.2/startrek/dock.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:07:19.000000 startrek-1.1.2/startrek/fsm/
--rw-r--r--   0 moky       (501) staff       (20)     2056 2023-01-13 04:48:09.000000 startrek-1.1.2/startrek/fsm/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2301 2024-02-26 16:17:15.000000 startrek-1.1.2/startrek/fsm/auto.py
--rw-r--r--   0 moky       (501) staff       (20)     8897 2024-03-06 13:23:59.000000 startrek-1.1.2/startrek/fsm/base.py
--rw-r--r--   0 moky       (501) staff       (20)     5808 2024-03-06 10:33:56.000000 startrek-1.1.2/startrek/fsm/machine.py
--rw-r--r--   0 moky       (501) staff       (20)     5449 2024-02-26 14:47:40.000000 startrek-1.1.2/startrek/fsm/runner.py
--rw-r--r--   0 moky       (501) staff       (20)     4506 2024-03-07 09:23:03.000000 startrek-1.1.2/startrek/fsm/ticker.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:07:19.000000 startrek-1.1.2/startrek/net/
--rw-r--r--   0 moky       (501) staff       (20)     3283 2023-01-13 11:39:06.000000 startrek-1.1.2/startrek/net/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8734 2024-03-13 09:27:10.000000 startrek-1.1.2/startrek/net/channel.py
--rw-r--r--   0 moky       (501) staff       (20)     3366 2024-03-13 09:14:10.000000 startrek-1.1.2/startrek/net/connection.py
--rw-r--r--   0 moky       (501) staff       (20)     3380 2024-03-06 08:44:28.000000 startrek-1.1.2/startrek/net/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     3867 2024-03-06 08:47:09.000000 startrek-1.1.2/startrek/net/hub.py
--rw-r--r--   0 moky       (501) staff       (20)    17022 2024-03-06 16:02:35.000000 startrek-1.1.2/startrek/net/state.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:07:19.000000 startrek-1.1.2/startrek/port/
--rw-r--r--   0 moky       (501) staff       (20)     3722 2024-03-06 09:27:29.000000 startrek-1.1.2/startrek/port/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3100 2024-03-06 14:33:53.000000 startrek-1.1.2/startrek/port/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     4412 2024-03-13 09:17:53.000000 startrek-1.1.2/startrek/port/docker.py
--rw-r--r--   0 moky       (501) staff       (20)     2619 2024-01-26 17:39:19.000000 startrek-1.1.2/startrek/port/gate.py
--rw-r--r--   0 moky       (501) staff       (20)     4127 2024-03-06 09:27:29.000000 startrek-1.1.2/startrek/port/ship.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:07:19.000000 startrek-1.1.2/startrek/socket/
--rw-r--r--   0 moky       (501) staff       (20)     1899 2024-03-06 13:22:07.000000 startrek-1.1.2/startrek/socket/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3757 2024-03-13 08:51:19.000000 startrek-1.1.2/startrek/socket/active_conn.py
--rw-r--r--   0 moky       (501) staff       (20)    10569 2024-03-13 10:11:33.000000 startrek-1.1.2/startrek/socket/base_channel.py
--rw-r--r--   0 moky       (501) staff       (20)    10478 2024-03-13 09:44:44.000000 startrek-1.1.2/startrek/socket/base_conn.py
--rw-r--r--   0 moky       (501) staff       (20)     9744 2024-03-13 09:20:18.000000 startrek-1.1.2/startrek/socket/base_hub.py
--rw-r--r--   0 moky       (501) staff       (20)    10753 2024-03-13 10:00:28.000000 startrek-1.1.2/startrek/stardocker.py
--rw-r--r--   0 moky       (501) staff       (20)    11425 2024-03-13 09:51:25.000000 startrek-1.1.2/startrek/stargate.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:07:19.000000 startrek-1.1.2/startrek/types/
--rw-r--r--   0 moky       (501) staff       (20)     1678 2024-03-06 07:44:45.000000 startrek-1.1.2/startrek/types/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7196 2024-03-06 10:36:46.000000 startrek-1.1.2/startrek/types/mapping.py
--rw-r--r--   0 moky       (501) staff       (20)     3721 2024-03-08 06:09:38.000000 startrek-1.1.2/startrek/types/pair.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:07:19.000000 startrek-1.1.2/startrek.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)      449 2024-03-13 11:07:19.000000 startrek-1.1.2/startrek.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      894 2024-03-13 11:07:19.000000 startrek-1.1.2/startrek.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-03-13 11:07:19.000000 startrek-1.1.2/startrek.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)        9 2024-03-13 11:07:19.000000 startrek-1.1.2/startrek.egg-info/top_level.txt
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/
+-rw-r--r--   0 moky       (501) staff       (20)      449 2024-04-12 10:36:07.000000 startrek-1.1.3/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)       25 2021-05-06 07:15:56.000000 startrek-1.1.3/README.md
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-04-12 10:36:07.000000 startrek-1.1.3/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      826 2024-03-13 14:44:36.000000 startrek-1.1.3/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek/
+-rw-r--r--   0 moky       (501) staff       (20)     2520 2023-01-13 11:45:48.000000 startrek-1.1.3/startrek/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     5463 2024-03-06 13:31:40.000000 startrek-1.1.3/startrek/arrival.py
+-rw-r--r--   0 moky       (501) staff       (20)    11425 2024-03-06 13:32:13.000000 startrek-1.1.3/startrek/departure.py
+-rw-r--r--   0 moky       (501) staff       (20)     4960 2024-03-06 13:33:03.000000 startrek-1.1.3/startrek/dock.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek/fsm/
+-rw-r--r--   0 moky       (501) staff       (20)     2056 2023-01-13 04:48:09.000000 startrek-1.1.3/startrek/fsm/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2301 2024-02-26 16:17:15.000000 startrek-1.1.3/startrek/fsm/auto.py
+-rw-r--r--   0 moky       (501) staff       (20)     8897 2024-03-06 13:23:59.000000 startrek-1.1.3/startrek/fsm/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     5808 2024-03-06 10:33:56.000000 startrek-1.1.3/startrek/fsm/machine.py
+-rw-r--r--   0 moky       (501) staff       (20)     5449 2024-02-26 14:47:40.000000 startrek-1.1.3/startrek/fsm/runner.py
+-rw-r--r--   0 moky       (501) staff       (20)     4506 2024-03-07 09:23:03.000000 startrek-1.1.3/startrek/fsm/ticker.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek/net/
+-rw-r--r--   0 moky       (501) staff       (20)     3283 2023-01-13 11:39:06.000000 startrek-1.1.3/startrek/net/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8734 2024-03-13 09:27:10.000000 startrek-1.1.3/startrek/net/channel.py
+-rw-r--r--   0 moky       (501) staff       (20)     3366 2024-03-13 09:14:10.000000 startrek-1.1.3/startrek/net/connection.py
+-rw-r--r--   0 moky       (501) staff       (20)     3380 2024-03-06 08:44:28.000000 startrek-1.1.3/startrek/net/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     3867 2024-03-06 08:47:09.000000 startrek-1.1.3/startrek/net/hub.py
+-rw-r--r--   0 moky       (501) staff       (20)    17022 2024-03-06 16:02:35.000000 startrek-1.1.3/startrek/net/state.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek/port/
+-rw-r--r--   0 moky       (501) staff       (20)     3722 2024-03-06 09:27:29.000000 startrek-1.1.3/startrek/port/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3100 2024-03-06 14:33:53.000000 startrek-1.1.3/startrek/port/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     4412 2024-03-13 09:17:53.000000 startrek-1.1.3/startrek/port/docker.py
+-rw-r--r--   0 moky       (501) staff       (20)     2619 2024-01-26 17:39:19.000000 startrek-1.1.3/startrek/port/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)     4127 2024-03-06 09:27:29.000000 startrek-1.1.3/startrek/port/ship.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek/socket/
+-rw-r--r--   0 moky       (501) staff       (20)     1899 2024-03-06 13:22:07.000000 startrek-1.1.3/startrek/socket/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4283 2024-03-14 10:29:49.000000 startrek-1.1.3/startrek/socket/active_conn.py
+-rw-r--r--   0 moky       (501) staff       (20)    10666 2024-03-13 15:37:34.000000 startrek-1.1.3/startrek/socket/base_channel.py
+-rw-r--r--   0 moky       (501) staff       (20)    10445 2024-03-13 14:50:15.000000 startrek-1.1.3/startrek/socket/base_conn.py
+-rw-r--r--   0 moky       (501) staff       (20)     9744 2024-03-13 09:20:18.000000 startrek-1.1.3/startrek/socket/base_hub.py
+-rw-r--r--   0 moky       (501) staff       (20)    10723 2024-03-13 14:50:40.000000 startrek-1.1.3/startrek/stardocker.py
+-rw-r--r--   0 moky       (501) staff       (20)    11425 2024-03-13 09:51:25.000000 startrek-1.1.3/startrek/stargate.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek/types/
+-rw-r--r--   0 moky       (501) staff       (20)     1678 2024-03-06 07:44:45.000000 startrek-1.1.3/startrek/types/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7196 2024-03-06 10:36:46.000000 startrek-1.1.3/startrek/types/mapping.py
+-rw-r--r--   0 moky       (501) staff       (20)     3721 2024-03-08 06:09:38.000000 startrek-1.1.3/startrek/types/pair.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)      449 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      894 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)        9 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek.egg-info/top_level.txt
```

### Comparing `startrek-1.1.2/setup.py` & `startrek-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ~~~~~~~~~
 
     Interstellar Transport
 """
 
 from setuptools import setup, find_packages
 
-__version__ = '1.1.2'
+__version__ = '1.1.3'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with open('README.md', 'r') as fh:
     readme = fh.read()
 
 setup(
```

### Comparing `startrek-1.1.2/startrek/__init__.py` & `startrek-1.1.3/startrek/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/arrival.py` & `startrek-1.1.3/startrek/arrival.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/departure.py` & `startrek-1.1.3/startrek/departure.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/dock.py` & `startrek-1.1.3/startrek/dock.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/fsm/__init__.py` & `startrek-1.1.3/startrek/fsm/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/fsm/auto.py` & `startrek-1.1.3/startrek/fsm/auto.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/fsm/base.py` & `startrek-1.1.3/startrek/fsm/base.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/fsm/machine.py` & `startrek-1.1.3/startrek/fsm/machine.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/fsm/runner.py` & `startrek-1.1.3/startrek/fsm/runner.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/fsm/ticker.py` & `startrek-1.1.3/startrek/fsm/ticker.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/net/__init__.py` & `startrek-1.1.3/startrek/net/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/net/channel.py` & `startrek-1.1.3/startrek/net/channel.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/net/connection.py` & `startrek-1.1.3/startrek/net/connection.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/net/delegate.py` & `startrek-1.1.3/startrek/net/delegate.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/net/hub.py` & `startrek-1.1.3/startrek/net/hub.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/net/state.py` & `startrek-1.1.3/startrek/net/state.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/port/__init__.py` & `startrek-1.1.3/startrek/port/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/port/delegate.py` & `startrek-1.1.3/startrek/port/delegate.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/port/docker.py` & `startrek-1.1.3/startrek/port/docker.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/port/gate.py` & `startrek-1.1.3/startrek/port/gate.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/port/ship.py` & `startrek-1.1.3/startrek/port/ship.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/socket/__init__.py` & `startrek-1.1.3/startrek/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/socket/active_conn.py` & `startrek-1.1.3/startrek/socket/active_conn.py`

 * *Files 19% similar despite different names*

```diff
@@ -63,42 +63,46 @@
         # 2. start a background thread to check channel
         self.__daemon.start()
 
     # protected
     def run(self):
         expired = 0
         last_time = 0
-        interval = 16
+        interval = 8
         while not self.closed:
             time.sleep(1.0)
-            #
-            #  1. check time interval
-            #
             now = time.time()
-            if now < (last_time + interval):
-                continue
-            last_time = now
-            if interval < 256:
-                interval *= 2
-            #
-            #  2. check socket channel
-            #
             try:
                 sock = self.channel
                 if sock is None or sock.closed:
+                    # first time to try connecting (last_time == 0)?
+                    # or connection lost, then try to reconnect again.
+                    # check time interval for the trying here
+                    if now < (last_time + interval):
+                        continue
+                    else:
+                        # update last connect time
+                        last_time = now
                     # get new socket channel via hub
                     hub = self.hub
                     assert hub is not None, 'hub not found: %s -> %s' % (self.local_address, self.remote_address)
+                    # try to open a new socket channel from the hub.
+                    # the returned socket channel is opened for connecting,
+                    # but maybe failed,
+                    # so set an expired time to close it after timeout;
+                    # if failed to open a new socket channel,
+                    # then extend the time interval for next trying.
                     sock = self._open_channel(hub=hub)
-                    if sock is None or sock.closed:
-                        print('[Socket] cannot open channel: %s -> %s' % (self.local_address, self.remote_address))
-                    else:
+                    if sock is not None:
                         # connect timeout after 2 minutes
                         expired = now + 128
+                    elif interval < 128:
+                        interval *= 2
                 elif sock.alive:
-                    # socket channel is normal
-                    interval = 16
+                    # socket channel is normal, reset the time interval here.
+                    # this will work when the current connection lost
+                    interval = 8
                 elif 0 < expired < now:
                     # connect timeout
                     sock.close()
             except Exception as error:
                 print('[Socket] active connection error: %s' % error)
```

### Comparing `startrek-1.1.2/startrek/socket/base_channel.py` & `startrek-1.1.3/startrek/socket/base_channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 
 class BaseChannel(AddressPairObject, Channel, ABC):
 
     def __init__(self, remote: Optional[SocketAddress], local: Optional[SocketAddress]):
         super().__init__(remote=remote, local=local)
         # inner socket
         self.__sock: Optional[socket.socket] = None
+        self.__closed = None
         # create socket reader/writer
         self.__reader = self._create_reader()
         self.__writer = self._create_writer()
 
     #
     #   Channel Controller
     #
@@ -177,32 +178,33 @@
 
     def set_socket(self, sock: Optional[socket.socket]):
         """ set inner socket for this channel """
         # 1. replace with new socket
         old = self.__sock
         if sock is not None:
             self.__sock = sock
-        # else:
-        #     self.__sock = None
+            self.__closed = False
+        else:
+            self.__sock = None
+            self.__closed = True
         # 2. close old socket
         if old is not None and old is not sock:
             disconnect_socket(sock=old)
 
     #
     #   Flags
     #
 
     @property  # Override
     def closed(self) -> bool:
-        sock = self.__sock
-        if sock is None:
+        if self.__closed is None:
             # initializing
             return False
-        else:
-            return is_closed(sock=sock)
+        sock = self.sock
+        return sock is None or is_closed(sock=sock)
 
     @property  # Override
     def bound(self) -> bool:
         sock = self.sock
         return sock is not None and is_bound(sock=sock)
 
     @property  # Override
```

### Comparing `startrek-1.1.2/startrek/socket/base_conn.py` & `startrek-1.1.3/startrek/socket/base_conn.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,21 +117,19 @@
 
     #
     #   Flags
     #
 
     @property  # Override
     def closed(self) -> bool:
-        ref = self.__channel_ref
-        if ref is None:
+        if self.__channel_ref is None:
             # initializing
             return False
-        else:
-            channel = ref()
-            return channel is None or channel.closed
+        channel = self.channel
+        return channel is None or channel.closed
 
     @property  # Override
     def bound(self) -> bool:
         channel = self.channel
         return channel is not None and channel.bound
 
     @property  # Override
```

### Comparing `startrek-1.1.2/startrek/socket/base_hub.py` & `startrek-1.1.3/startrek/socket/base_hub.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/stardocker.py` & `startrek-1.1.3/startrek/stardocker.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,21 +106,19 @@
 
     #
     #   Flags
     #
 
     @property  # Override
     def closed(self) -> bool:
-        ref = self.__conn_ref
-        if ref is None:
+        if self.__conn_ref is None:
             # initializing
             return False
-        else:
-            conn = ref()
-            return conn is None or conn.closed
+        conn = self.connection
+        return conn is None or conn.closed
 
     @property  # Override
     def alive(self) -> bool:
         conn = self.connection
         return conn is not None and conn.alive
 
     @property  # Override
```

### Comparing `startrek-1.1.2/startrek/stargate.py` & `startrek-1.1.3/startrek/stargate.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/types/__init__.py` & `startrek-1.1.3/startrek/types/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/types/mapping.py` & `startrek-1.1.3/startrek/types/mapping.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek/types/pair.py` & `startrek-1.1.3/startrek/types/pair.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.2/startrek.egg-info/SOURCES.txt` & `startrek-1.1.3/startrek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

