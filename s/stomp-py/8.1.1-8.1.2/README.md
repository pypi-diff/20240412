# Comparing `tmp/stomp_py-8.1.1.tar.gz` & `tmp/stomp_py-8.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stomp_py-8.1.1.tar", max compression
+gzip compressed data, was "stomp_py-8.1.2.tar", max compression
```

## Comparing `stomp_py-8.1.1.tar` & `stomp_py-8.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11358 2020-01-08 20:24:28.435496 stomp_py-8.1.1/LICENSE
--rw-r--r--   0        0        0     4854 2022-08-01 07:39:51.672854 stomp_py-8.1.1/README.rst
--rw-r--r--   0        0        0     1031 2023-03-11 17:16:41.468918 stomp_py-8.1.1/pyproject.toml
--rw-r--r--   0        0        0     1336 2023-03-11 17:16:41.480919 stomp_py-8.1.1/stomp/__init__.py
--rw-r--r--   0        0        0    20806 2023-03-22 21:16:43.493015 stomp_py-8.1.1/stomp/__main__.py
--rw-r--r--   0        0        0       86 2022-11-13 16:44:23.491555 stomp_py-8.1.1/stomp/adapter/__init__.py
--rw-r--r--   0        0        0     6143 2022-11-13 16:44:23.491555 stomp_py-8.1.1/stomp/adapter/multicast.py
--rw-r--r--   0        0        0    18804 2023-03-11 11:48:42.973118 stomp_py-8.1.1/stomp/adapter/ws.py
--rw-r--r--   0        0        0      277 2022-01-04 23:22:01.024428 stomp_py-8.1.1/stomp/colours.py
--rw-r--r--   0        0        0     8575 2022-11-13 16:44:23.503555 stomp_py-8.1.1/stomp/connect.py
--rw-r--r--   0        0        0      685 2022-11-13 16:44:23.503555 stomp_py-8.1.1/stomp/constants.py
--rw-r--r--   0        0        0      859 2022-01-04 23:22:01.024428 stomp_py-8.1.1/stomp/exception.py
--rw-r--r--   0        0        0    20213 2022-11-13 16:44:23.507556 stomp_py-8.1.1/stomp/listener.py
--rw-r--r--   0        0        0      663 2022-10-22 18:46:40.395770 stomp_py-8.1.1/stomp/logging.py
--rw-r--r--   0        0        0    22859 2023-06-06 20:38:54.908052 stomp_py-8.1.1/stomp/protocol.py
--rw-r--r--   0        0        0    35167 2022-11-13 16:44:23.507556 stomp_py-8.1.1/stomp/transport.py
--rw-r--r--   0        0        0     8521 2022-11-13 16:44:23.511556 stomp_py-8.1.1/stomp/utils.py
--rw-r--r--   0        0        0     5913 1970-01-01 00:00:00.000000 stomp_py-8.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2020-01-08 20:24:28.435496 stomp_py-8.1.2/LICENSE
+-rw-r--r--   0        0        0     4854 2022-08-01 07:39:51.672854 stomp_py-8.1.2/README.rst
+-rw-r--r--   0        0        0     1035 2024-04-12 21:36:40.482887 stomp_py-8.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1336 2023-03-11 17:16:41.480919 stomp_py-8.1.2/stomp/__init__.py
+-rw-r--r--   0        0        0    20806 2023-03-22 21:16:43.493015 stomp_py-8.1.2/stomp/__main__.py
+-rw-r--r--   0        0        0       86 2022-11-13 16:44:23.491555 stomp_py-8.1.2/stomp/adapter/__init__.py
+-rw-r--r--   0        0        0     6143 2022-11-13 16:44:23.491555 stomp_py-8.1.2/stomp/adapter/multicast.py
+-rw-r--r--   0        0        0    19382 2024-04-12 21:20:52.221595 stomp_py-8.1.2/stomp/adapter/ws.py
+-rw-r--r--   0        0        0      277 2022-01-04 23:22:01.024428 stomp_py-8.1.2/stomp/colours.py
+-rw-r--r--   0        0        0     8575 2022-11-13 16:44:23.503555 stomp_py-8.1.2/stomp/connect.py
+-rw-r--r--   0        0        0      685 2022-11-13 16:44:23.503555 stomp_py-8.1.2/stomp/constants.py
+-rw-r--r--   0        0        0      859 2022-01-04 23:22:01.024428 stomp_py-8.1.2/stomp/exception.py
+-rw-r--r--   0        0        0    20213 2022-11-13 16:44:23.507556 stomp_py-8.1.2/stomp/listener.py
+-rw-r--r--   0        0        0      663 2022-10-22 18:46:40.395770 stomp_py-8.1.2/stomp/logging.py
+-rw-r--r--   0        0        0    22759 2023-06-29 21:52:07.284372 stomp_py-8.1.2/stomp/protocol.py
+-rw-r--r--   0        0        0    35189 2024-04-12 21:36:14.356426 stomp_py-8.1.2/stomp/transport.py
+-rw-r--r--   0        0        0     8521 2022-11-13 16:44:23.511556 stomp_py-8.1.2/stomp/utils.py
+-rw-r--r--   0        0        0     5913 1970-01-01 00:00:00.000000 stomp_py-8.1.2/PKG-INFO
```

### Comparing `stomp_py-8.1.1/LICENSE` & `stomp_py-8.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stomp_py-8.1.1/README.rst` & `stomp_py-8.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `stomp_py-8.1.1/pyproject.toml` & `stomp_py-8.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stomp.py"
-version = "8.1.1"
+version = "8.1.2"
 description = "Python STOMP client, supporting versions 1.0, 1.1 and 1.2 of the protocol"
 authors = ["Jason R Briggs <jasonrbriggs@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/jasonrbriggs/stomp.py"
 documentation = "http://jasonrbriggs.github.io/stomp.py/"
 keywords = ["stomp", "messaging", "events", "client"]
@@ -32,9 +32,9 @@
 
 [tool.poetry.scripts]
 stomp = "stomp.__main__:main"
 
 [tool.poetry_bumpversion.file."stomp/__init__.py"]
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `stomp_py-8.1.1/stomp/__init__.py` & `stomp_py-8.1.2/stomp/__init__.py`

 * *Files identical despite different names*

### Comparing `stomp_py-8.1.1/stomp/__main__.py` & `stomp_py-8.1.2/stomp/__main__.py`

 * *Files identical despite different names*

### Comparing `stomp_py-8.1.1/stomp/adapter/multicast.py` & `stomp_py-8.1.2/stomp/adapter/multicast.py`

 * *Files identical despite different names*

### Comparing `stomp_py-8.1.1/stomp/adapter/ws.py` & `stomp_py-8.1.2/stomp/adapter/ws.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         default keepalive options for your OS, or as a tuple of
         values, which also enables keepalive packets, but specifies
         options specific to your OS implementation.
         For linux, supply ("linux", ka_idle, ka_intvl, ka_cnt)
         For macos, supply ("mac", ka_intvl)
     :param str vhost: specify a virtual hostname to provide in the 'host' header of the connection
     :param int recv_bytes: the number of bytes to use when calling recv
+    :param bool binary_mode: if true, then send binary data frames (opcode 0x2) rather than text data frames (opcode 0x1)
     """
 
     def __init__(self,
                  host_and_ports=None,
                  prefer_localhost=True,
                  try_loopback_connect=True,
                  reconnect_sleep_initial=0.1,
@@ -91,15 +92,16 @@
                  vhost=None,
                  auto_decode=True,
                  encoding="utf-8",
                  recv_bytes=1024,
                  is_eol_fc=is_eol_default,
                  bind_host_port=None,
                  ws_path=None,
-                 header=None):
+                 header=None,
+                 binary_mode=False):
         BaseTransport.__init__(self, auto_decode, encoding, is_eol_fc)
 
         if host_and_ports is None:
             logging.debug("no hosts_and_ports specified, adding default localhost")
             host_and_ports = [("localhost", 61613)]
 
         sorted_host_and_ports = []
@@ -136,14 +138,15 @@
 
         self.__reconnect_sleep_initial = reconnect_sleep_initial
         self.__reconnect_sleep_increase = reconnect_sleep_increase
         self.__reconnect_sleep_jitter = reconnect_sleep_jitter
         self.__reconnect_sleep_max = reconnect_sleep_max
         self.__reconnect_attempts_max = reconnect_attempts_max
         self.__timeout = timeout
+        self.__binary_mode = binary_mode
 
         self.socket = None
         self.__socket_semaphore = threading.BoundedSemaphore(1)
         self.current_host_and_port = None
         self.vhost = vhost
         self.ws_path = ws_path
         self.header = header
@@ -195,28 +198,34 @@
     def send(self, encoded_frame):
         """
         :param bytes encoded_frame:
         """
         if self.socket is not None:
             try:
                 with self.__socket_semaphore:
-                    self.socket.send(encoded_frame)
+                    if self.__binary_mode:
+                        opcode = websocket.ABNF.OPCODE_BINARY
+                    else:
+                        opcode = websocket.ABNF.OPCODE_TEXT
+
+                    self.socket.send(encoded_frame, opcode)
             except Exception:
                 _, e, _ = sys.exc_info()
                 logging.error("error sending frame", exc_info=True)
                 raise e
         else:
             raise NotConnectedException()
 
     def receive(self):
         """
         :rtype: bytes
         """
         try:
-            return self.socket.recv().encode()
+            opcode, data = self.socket.recv_data()
+            return data
         except socket.error:
             _, e, _ = sys.exc_info()
             if get_errno(e) in (errno.EAGAIN, errno.EINTR):
                 logging.debug("socket read interrupted, restarting")
                 raise InterruptedException()
             if self.is_connected():
                 raise
@@ -319,20 +328,21 @@
 
                     if self.__need_ssl():
                         scheme = "wss"
                     else:
                         scheme = "ws"
                     self.socket = websocket.create_connection(
                         f"{scheme}://{host_and_port[0]}:{host_and_port[1]}{path}",
+                        timeout=self.__timeout,
                         header=self.header,
                         sslopt=self.get_ssl()
                     )
                     logging.info("established connection to host %s, port %s", host_and_port[0], host_and_port[1])
                     break
-                except (OSError, AssertionError) as exc:
+                except (OSError, AssertionError, websocket._exceptions.WebSocketException) as exc:
                     self.socket = None
                     connect_count += 1
                     logging.warning("Could not connect to host %s, port %s: %s", host_and_port[0], host_and_port[1],
                                     str(exc), exc_info=logging.verbose)
 
             if self.socket is None:
                 sleep_duration = (min(self.__reconnect_sleep_max,
@@ -432,16 +442,17 @@
                  auto_decode=True,
                  encoding="utf-8",
                  auto_content_length=True,
                  heart_beat_receive_scale=1.5,
                  bind_host_port=None,
                  ws=None,
                  ws_path=None,
-                 header=None):
+                 header=None,
+                 binary_mode=False):
         transport = WSTransport(host_and_ports, prefer_localhost, try_loopback_connect,
                               reconnect_sleep_initial, reconnect_sleep_increase, reconnect_sleep_jitter,
                               reconnect_sleep_max, reconnect_attempts_max, timeout,
                               keepalive, vhost, auto_decode, encoding, bind_host_port=bind_host_port,
-                              header=header, ws_path=ws_path)
+                              header=header, ws_path=ws_path, binary_mode=binary_mode)
         BaseConnection.__init__(self, transport)
         Protocol12.__init__(self, transport, heartbeats, auto_content_length,
                             heart_beat_receive_scale=heart_beat_receive_scale)
```

### Comparing `stomp_py-8.1.1/stomp/connect.py` & `stomp_py-8.1.2/stomp/connect.py`

 * *Files identical despite different names*

### Comparing `stomp_py-8.1.1/stomp/constants.py` & `stomp_py-8.1.2/stomp/constants.py`

 * *Files identical despite different names*

### Comparing `stomp_py-8.1.1/stomp/exception.py` & `stomp_py-8.1.2/stomp/exception.py`

 * *Files identical despite different names*

### Comparing `stomp_py-8.1.1/stomp/listener.py` & `stomp_py-8.1.2/stomp/listener.py`

 * *Files identical despite different names*

### Comparing `stomp_py-8.1.1/stomp/logging.py` & `stomp_py-8.1.2/stomp/logging.py`

 * *Files identical despite different names*

### Comparing `stomp_py-8.1.1/stomp/protocol.py` & `stomp_py-8.1.2/stomp/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,16 +322,14 @@
         """
         cmd = CMD_CONNECT if with_connect_command else CMD_STOMP
         headers = utils.merge_headers([headers, keyword_headers])
         headers[HDR_ACCEPT_VERSION] = self.version
 
         if self.transport.vhost:
             headers[HDR_HOST] = self.transport.vhost
-        else:
-            headers[HDR_HOST] = "/"
 
         if username is not None:
             headers[HDR_LOGIN] = username
 
         if passcode is not None:
             headers[HDR_PASSCODE] = passcode
 
@@ -514,16 +512,14 @@
         cmd = CMD_CONNECT if with_connect_command else CMD_STOMP
         headers = utils.merge_headers([headers, keyword_headers])
         headers[HDR_ACCEPT_VERSION] = self.version
         headers[HDR_HOST] = self.transport.current_host_and_port[0]
 
         if self.transport.vhost:
             headers[HDR_HOST] = self.transport.vhost
-        else:
-            headers[HDR_HOST] = "/"
 
         if username is not None:
             headers[HDR_LOGIN] = username
 
         if passcode is not None:
             headers[HDR_PASSCODE] = passcode
```

### Comparing `stomp_py-8.1.1/stomp/transport.py` & `stomp_py-8.1.2/stomp/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
                 except exception.InterruptedException:
                     logging.debug("socket read interrupted, restarting")
                     continue
             except Exception:
                 logging.debug("socket read error", exc_info=logging.verbose)
                 c = b""
             if c is None or len(c) == 0:
-                logging.debug("nothing received, raising CCE")
+                logging.debug("nothing received, raising ConnectionClosedException")
                 raise exception.ConnectionClosedException()
             if self.__is_eol(c) and not self.__recvbuf and not fastbuf.tell():
                 #
                 # EOL to an empty receive buffer: treat as heartbeat.
                 # Note that this may misdetect an optional EOL at end of frame as heartbeat in case the
                 # previous receive() got a complete frame whose NUL at end of frame happened to be the
                 # last byte of that read. But that should be harmless in practice.
```

### Comparing `stomp_py-8.1.1/stomp/utils.py` & `stomp_py-8.1.2/stomp/utils.py`

 * *Files identical despite different names*

### Comparing `stomp_py-8.1.1/PKG-INFO` & `stomp_py-8.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stomp-py
-Version: 8.1.1
+Version: 8.1.2
 Summary: Python STOMP client, supporting versions 1.0, 1.1 and 1.2 of the protocol
 Home-page: https://github.com/jasonrbriggs/stomp.py
 License: Apache-2.0
 Keywords: stomp,messaging,events,client
 Author: Jason R Briggs
 Author-email: jasonrbriggs@gmail.com
 Requires-Python: >=3.7,<4.0
```

