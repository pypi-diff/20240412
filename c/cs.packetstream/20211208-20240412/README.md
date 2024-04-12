# Comparing `tmp/cs.packetstream-20211208.tar.gz` & `tmp/cs.packetstream-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.packetstream-20211208.tar", last modified: Wed Dec  8 09:50:48 2021, max compression
+gzip compressed data, was "cs.packetstream-20240412.tar", last modified: Fri Apr 12 05:17:43 2024, max compression
```

## Comparing `cs.packetstream-20211208.tar` & `cs.packetstream-20240412.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) staff       (20)        0 2021-12-08 09:50:48.853570 cs.packetstream-20211208/
--rw-rw-r--   0 cameron    (501) staff       (20)        0 2021-12-08 09:50:48.000000 cs.packetstream-20211208/MANIFEST.in
--rw-rw-r--   0 cameron    (501) staff       (20)     4675 2021-12-08 09:50:48.853362 cs.packetstream-20211208/PKG-INFO
--rw-rw-r--   0 cameron    (501) staff       (20)     3887 2021-12-08 09:50:48.000000 cs.packetstream-20211208/README.md
-drwxrwxr-x   0 cameron    (501) staff       (20)        0 2021-12-08 09:50:48.850369 cs.packetstream-20211208/lib/
-drwxrwxr-x   0 cameron    (501) staff       (20)        0 2021-12-08 09:50:48.850538 cs.packetstream-20211208/lib/python/
-drwxrwxr-x   0 cameron    (501) staff       (20)        0 2021-12-08 09:50:48.851256 cs.packetstream-20211208/lib/python/cs/
--rw-r--r--   0 cameron    (501) staff       (20)    21387 2021-12-08 09:50:39.000000 cs.packetstream-20211208/lib/python/cs/packetstream.py
-drwxrwxr-x   0 cameron    (501) staff       (20)        0 2021-12-08 09:50:48.853086 cs.packetstream-20211208/lib/python/cs.packetstream.egg-info/
--rw-rw-r--   0 cameron    (501) staff       (20)     4675 2021-12-08 09:50:48.000000 cs.packetstream-20211208/lib/python/cs.packetstream.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) staff       (20)      309 2021-12-08 09:50:48.000000 cs.packetstream-20211208/lib/python/cs.packetstream.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) staff       (20)        1 2021-12-08 09:50:48.000000 cs.packetstream-20211208/lib/python/cs.packetstream.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) staff       (20)      124 2021-12-08 09:50:48.000000 cs.packetstream-20211208/lib/python/cs.packetstream.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) staff       (20)        3 2021-12-08 09:50:48.000000 cs.packetstream-20211208/lib/python/cs.packetstream.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) staff       (20)       38 2021-12-08 09:50:48.853639 cs.packetstream-20211208/setup.cfg
--rw-rw-r--   0 cameron    (501) staff       (20)     6137 2021-12-08 09:50:48.000000 cs.packetstream-20211208/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:17:43.387333 cs.packetstream-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 05:17:35.000000 cs.packetstream-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     4895 2024-04-12 05:17:43.387066 cs.packetstream-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     4154 2024-04-12 05:17:37.000000 cs.packetstream-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:17:43.383485 cs.packetstream-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:17:43.383762 cs.packetstream-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:17:43.384955 cs.packetstream-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    23413 2024-04-12 05:17:15.000000 cs.packetstream-20240412/lib/python/cs/packetstream.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:17:43.386643 cs.packetstream-20240412/lib/python/cs.packetstream.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     4895 2024-04-12 05:17:42.000000 cs.packetstream-20240412/lib/python/cs.packetstream.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      315 2024-04-12 05:17:43.000000 cs.packetstream-20240412/lib/python/cs.packetstream.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 05:17:42.000000 cs.packetstream-20240412/lib/python/cs.packetstream.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      326 2024-04-12 05:17:43.000000 cs.packetstream-20240412/lib/python/cs.packetstream.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 05:17:43.000000 cs.packetstream-20240412/lib/python/cs.packetstream.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     5660 2024-04-12 05:17:41.000000 cs.packetstream-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 05:17:43.387430 cs.packetstream-20240412/setup.cfg
```

### Comparing `cs.packetstream-20211208/PKG-INFO` & `cs.packetstream-20240412/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,68 @@
 Metadata-Version: 2.1
 Name: cs.packetstream
-Version: 20211208
+Version: 20240412
 Summary: general purpose bidirectional packet stream connection
-Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
-Author: Cameron Simpson
-Author-email: cs@cskk.id.au
+Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Networking
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 A general purpose bidirectional packet stream connection.
 
-*Latest release 20211208*:
-* Packet.__eq__: only test .rq_type if .is_request.
-* Update tests for changes.
+*Latest release 20240412*:
+* PacketConnection: now subclasses MultiOpenMixin, big refactor.
+* PacketConnection.__init__: use @promote to turn the recv parameter into a CornuCopyBuffer.
+* Fix a deadlock.
 
-## Class `Packet(cs.binary.SimpleBinary,types.SimpleNamespace,cs.binary.AbstractBinary,cs.binary.BinaryMixin)`
+## Class `Packet(cs.binary.SimpleBinary)`
 
 A protocol packet.
 
-### Method `Packet.__str__(self)`
-
+*Method `Packet.__str__(self)`*:
 pylint: disable=signature-differs
 
-### Method `Packet.parse(bfr)`
-
-Parse a packet from a buffer.
-
-### Method `Packet.transcribe(self)`
+*Method `Packet.parse(bfr)`*:
+Parse a `Packet` from a buffer.
 
+*Method `Packet.transcribe(self)`*:
 Transcribe this packet.
 
-## Class `PacketConnection`
+## Class `PacketConnection(cs.resources.MultiOpenMixin)`
 
 A bidirectional binary connection for exchanging requests and responses.
 
-### Method `PacketConnection.__init__(self, recv, send, request_handler=None, name=None, packet_grace=None, tick=None)`
-
+*Method `PacketConnection.__init__(self, recv: cs.buffer.CornuCopyBuffer, send, request_handler=None, name=None, packet_grace=None, tick=None, recv_len_func=None, send_len_func=None)`*:
 Initialise the PacketConnection.
 
 Parameters:
 * `recv`: inbound binary stream.
-  If this is an `int` it is taken to be an OS file descriptor,
-  otherwise it should be a `cs.buffer.CornuCopyBuffer`
-  or a file like object with a `read1` or `read` method.
+  This value is automatically promoted to a `cs.buffer.CornuCopyBuffer`
+  by the `CornuCopyBuffer.promote` method.
+* `recv_len_func`: optional function to compute the data
+  length of a received packet; the default watches the offset
+  on the receive stream
 * `send`: outbound binary stream.
   If this is an `int` it is taken to be an OS file descriptor,
-  otherwise it should be a file like object with `.write(bytes)`
+  otherwise it should be a binary file like object with `.write(bytes)`
   and `.flush()` methods.
-  For a file descriptor sending is done via an os.dup() of
-  the supplied descriptor, so the caller remains responsible
-  for closing the original descriptor.
+  This objects _is not closed_ by the `PacketConnection`;
+  the caller has responsibility for that.
+* `send_len_func`: optional function to compute the data
+  length of a sent packet; the default watches the offset
+  on the send stream
 * `packet_grace`:
   default pause in the packet sending worker
   to allow another packet to be queued
   before flushing the output stream.
   Default: `DEFAULT_PACKET_GRACE`s.
   A value of `0` will flush immediately if the queue is empty.
 * `request_handler`: an optional callable accepting
@@ -78,57 +77,50 @@
   An unsuccessful request should raise an exception, which
   will cause a failure response packet.
 * `tick`: optional tick parameter, default `None`.
   If `None`, do nothing.
   If a Boolean, call `tick_fd_2` if true, otherwise do nothing.
   Otherwise `tick` should be a callable accepting a byteslike value.
 
-### Method `PacketConnection.do(self, *a, **kw)`
-
+*Method `PacketConnection.do(self, *a, **kw)`*:
 Wrapper function to check that this instance is not closed.
 
-### Method `PacketConnection.join(self)`
-
+*Method `PacketConnection.join(self)`*:
 Wait for the receive side of the connection to terminate.
 
-### Method `PacketConnection.request(self, *a, **kw)`
-
+*Method `PacketConnection.request(self, *a, **kw)`*:
 Wrapper function to check that this instance is not closed.
 
-### Method `PacketConnection.shutdown(self, *a, **kw)`
-
-Shut down the PacketConnection, optionally blocking for outstanding requests.
-
-Parameters:
-`block`: block for outstanding requests, default False.
-
 ## Class `Request_State(builtins.tuple)`
 
 RequestState(decode_response, result)
 
-### Property `Request_State.decode_response`
-
+*Property `Request_State.decode_response`*:
 Alias for field number 0
 
-### Property `Request_State.result`
-
+*Property `Request_State.result`*:
 Alias for field number 1
 
 ## Function `tick_fd_2(bs)`
 
 A low level tick function to write a short binary tick
 to the standard error file descriptor.
 
 This may be called by the send and receive workers to give
 an indication of activity type.
 
 # Release Log
 
 
 
+*Release 20240412*:
+* PacketConnection: now subclasses MultiOpenMixin, big refactor.
+* PacketConnection.__init__: use @promote to turn the recv parameter into a CornuCopyBuffer.
+* Fix a deadlock.
+
 *Release 20211208*:
 * Packet.__eq__: only test .rq_type if .is_request.
 * Update tests for changes.
 
 *Release 20210306*:
 * Port to new cs.binary.Binary* classes.
 * Some refactors and small fixes.
```

### Comparing `cs.packetstream-20211208/README.md` & `cs.packetstream-20240412/lib/python/cs.packetstream.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,68 @@
+Metadata-Version: 2.1
+Name: cs.packetstream
+Version: 20240412
+Summary: general purpose bidirectional packet stream connection
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python2,python3
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: System :: Networking
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
+
 A general purpose bidirectional packet stream connection.
 
-*Latest release 20211208*:
-* Packet.__eq__: only test .rq_type if .is_request.
-* Update tests for changes.
+*Latest release 20240412*:
+* PacketConnection: now subclasses MultiOpenMixin, big refactor.
+* PacketConnection.__init__: use @promote to turn the recv parameter into a CornuCopyBuffer.
+* Fix a deadlock.
 
-## Class `Packet(cs.binary.SimpleBinary,types.SimpleNamespace,cs.binary.AbstractBinary,cs.binary.BinaryMixin)`
+## Class `Packet(cs.binary.SimpleBinary)`
 
 A protocol packet.
 
-### Method `Packet.__str__(self)`
-
+*Method `Packet.__str__(self)`*:
 pylint: disable=signature-differs
 
-### Method `Packet.parse(bfr)`
-
-Parse a packet from a buffer.
-
-### Method `Packet.transcribe(self)`
+*Method `Packet.parse(bfr)`*:
+Parse a `Packet` from a buffer.
 
+*Method `Packet.transcribe(self)`*:
 Transcribe this packet.
 
-## Class `PacketConnection`
+## Class `PacketConnection(cs.resources.MultiOpenMixin)`
 
 A bidirectional binary connection for exchanging requests and responses.
 
-### Method `PacketConnection.__init__(self, recv, send, request_handler=None, name=None, packet_grace=None, tick=None)`
-
+*Method `PacketConnection.__init__(self, recv: cs.buffer.CornuCopyBuffer, send, request_handler=None, name=None, packet_grace=None, tick=None, recv_len_func=None, send_len_func=None)`*:
 Initialise the PacketConnection.
 
 Parameters:
 * `recv`: inbound binary stream.
-  If this is an `int` it is taken to be an OS file descriptor,
-  otherwise it should be a `cs.buffer.CornuCopyBuffer`
-  or a file like object with a `read1` or `read` method.
+  This value is automatically promoted to a `cs.buffer.CornuCopyBuffer`
+  by the `CornuCopyBuffer.promote` method.
+* `recv_len_func`: optional function to compute the data
+  length of a received packet; the default watches the offset
+  on the receive stream
 * `send`: outbound binary stream.
   If this is an `int` it is taken to be an OS file descriptor,
-  otherwise it should be a file like object with `.write(bytes)`
+  otherwise it should be a binary file like object with `.write(bytes)`
   and `.flush()` methods.
-  For a file descriptor sending is done via an os.dup() of
-  the supplied descriptor, so the caller remains responsible
-  for closing the original descriptor.
+  This objects _is not closed_ by the `PacketConnection`;
+  the caller has responsibility for that.
+* `send_len_func`: optional function to compute the data
+  length of a sent packet; the default watches the offset
+  on the send stream
 * `packet_grace`:
   default pause in the packet sending worker
   to allow another packet to be queued
   before flushing the output stream.
   Default: `DEFAULT_PACKET_GRACE`s.
   A value of `0` will flush immediately if the queue is empty.
 * `request_handler`: an optional callable accepting
@@ -58,57 +77,50 @@
   An unsuccessful request should raise an exception, which
   will cause a failure response packet.
 * `tick`: optional tick parameter, default `None`.
   If `None`, do nothing.
   If a Boolean, call `tick_fd_2` if true, otherwise do nothing.
   Otherwise `tick` should be a callable accepting a byteslike value.
 
-### Method `PacketConnection.do(self, *a, **kw)`
-
+*Method `PacketConnection.do(self, *a, **kw)`*:
 Wrapper function to check that this instance is not closed.
 
-### Method `PacketConnection.join(self)`
-
+*Method `PacketConnection.join(self)`*:
 Wait for the receive side of the connection to terminate.
 
-### Method `PacketConnection.request(self, *a, **kw)`
-
+*Method `PacketConnection.request(self, *a, **kw)`*:
 Wrapper function to check that this instance is not closed.
 
-### Method `PacketConnection.shutdown(self, *a, **kw)`
-
-Shut down the PacketConnection, optionally blocking for outstanding requests.
-
-Parameters:
-`block`: block for outstanding requests, default False.
-
 ## Class `Request_State(builtins.tuple)`
 
 RequestState(decode_response, result)
 
-### Property `Request_State.decode_response`
-
+*Property `Request_State.decode_response`*:
 Alias for field number 0
 
-### Property `Request_State.result`
-
+*Property `Request_State.result`*:
 Alias for field number 1
 
 ## Function `tick_fd_2(bs)`
 
 A low level tick function to write a short binary tick
 to the standard error file descriptor.
 
 This may be called by the send and receive workers to give
 an indication of activity type.
 
 # Release Log
 
 
 
+*Release 20240412*:
+* PacketConnection: now subclasses MultiOpenMixin, big refactor.
+* PacketConnection.__init__: use @promote to turn the recv parameter into a CornuCopyBuffer.
+* Fix a deadlock.
+
 *Release 20211208*:
 * Packet.__eq__: only test .rq_type if .is_request.
 * Update tests for changes.
 
 *Release 20210306*:
 * Port to new cs.binary.Binary* classes.
 * Some refactors and small fixes.
@@ -118,7 +130,8 @@
 * Add a crude packet level activity ticker.
 
 *Release 20190221*:
 DISTINFO requirement updates.
 
 *Release 20181228*:
 Initial PyPI release.
+
```

### Comparing `cs.packetstream-20211208/lib/python/cs/packetstream.py` & `cs.packetstream-20240412/lib/python/cs/packetstream.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,66 +4,78 @@
 # - Cameron Simpson <cs@cskk.id.au> 21aug2015
 #
 
 ''' A general purpose bidirectional packet stream connection.
 '''
 
 from collections import namedtuple
+from contextlib import contextmanager
 import errno
 import os
 import sys
 from time import sleep
 from threading import Lock
+
+from icontract import ensure
+
 from cs.binary import SimpleBinary, BSUInt, BSData
 from cs.buffer import CornuCopyBuffer
+from cs.context import stackattrs
+from cs.deco import promote
 from cs.excutils import logexc
 from cs.later import Later
 from cs.logutils import debug, warning, error, exception
 from cs.pfx import Pfx, PrePfx, pfx_method
 from cs.predicate import post_condition
+from cs.progress import progressbar
 from cs.queues import IterableQueue
-from cs.resources import not_closed, ClosedError
+from cs.resources import not_closed, ClosedError, MultiOpenMixin, RunState
 from cs.result import Result
 from cs.seq import seq, Seq
 from cs.threads import locked, bg as bg_thread
+from cs.units import BINARY_BYTES_SCALE
 
 def tick_fd_2(bs):
   ''' A low level tick function to write a short binary tick
       to the standard error file descriptor.
 
       This may be called by the send and receive workers to give
       an indication of activity type.
   '''
   os.write(2, bs)
 
-__version__ = '20211208'
+__version__ = '20240412'
 
 DISTINFO = {
     'description':
     "general purpose bidirectional packet stream connection",
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "Topic :: System :: Networking",
     ],
     'install_requires': [
         'cs.binary',
         'cs.buffer',
+        'cs.context',
+        'cs.deco',
+        'cs.progress',
+        'cs.units',
         'cs.excutils',
         'cs.later',
         'cs.logutils',
         'cs.pfx',
         'cs.predicate',
         'cs.queues',
         'cs.resources',
         'cs.result',
         'cs.seq',
         'cs.threads',
+        'icontract',
     ]
 }
 
 # default pause before flush to allow for additional packet data to arrive
 DEFAULT_PACKET_GRACE = 0.01
 
 class Packet(SimpleBinary):
@@ -80,26 +92,29 @@
     return (
         "%s(is_request=%s,channel=%s,tag=%s,flags=0x%02x,payload=%s)" % (
             type(self).__name__, self.is_request, self.channel, self.tag,
             self.flags, payload_s
         )
     )
 
+  def __repr__(self):
+    return str(self)
+
   def __eq__(self, other):
     return (
         bool(self.is_request) == bool(other.is_request)
         and self.channel == other.channel and self.tag == other.tag
         and self.flags == other.flags
         and (not self.is_request or self.rq_type == other.rq_type)
         and self.payload == other.payload
     )
 
   @classmethod
   def parse(cls, bfr):
-    ''' Parse a packet from a buffer.
+    ''' Parse a `Packet` from a buffer.
     '''
     raw_payload = BSData.parse_value(bfr)
     payload_bfr = CornuCopyBuffer([raw_payload])
     self = cls()
     # pylint: disable=attribute-defined-outside-init
     self.tag = BSUInt.parse_value(payload_bfr)
     flags = BSUInt.parse_value(payload_bfr)
@@ -126,57 +141,64 @@
         BSUInt.transcribe_value(
             (0x01 if channel != 0 else 0x00)
             | (0x02 if is_request else 0x00)
             | (self.flags << 2)
         ),
         BSUInt.transcribe_value(channel) if channel != 0 else b'',
         BSUInt.transcribe_value(self.rq_type) if is_request else b'',
-        self.payload
+        self.payload,
     ]
     length = sum(len(bs) for bs in bss)
     # spit out a BSData manually to avoid pointless bytes.join
     yield BSUInt.transcribe_value(length)
     yield bss
 
 Request_State = namedtuple('RequestState', 'decode_response result')
 
 # pylint: disable=too-many-instance-attributes
-class PacketConnection(object):
+class PacketConnection(MultiOpenMixin):
   ''' A bidirectional binary connection for exchanging requests and responses.
   '''
 
   # special packet indicating end of stream
   EOF_Packet = Packet(
       is_request=True, channel=0, tag=0, flags=0, rq_type=0, payload=b''
   )
 
   # pylint: disable=too-many-arguments
+  @promote
   def __init__(
       self,
-      recv,
+      recv: CornuCopyBuffer,
       send,
       request_handler=None,
       name=None,
       packet_grace=None,
-      tick=None
+      tick=None,
+      recv_len_func=None,
+      send_len_func=None,
   ):
     ''' Initialise the PacketConnection.
 
         Parameters:
         * `recv`: inbound binary stream.
-          If this is an `int` it is taken to be an OS file descriptor,
-          otherwise it should be a `cs.buffer.CornuCopyBuffer`
-          or a file like object with a `read1` or `read` method.
+          This value is automatically promoted to a `cs.buffer.CornuCopyBuffer`
+          by the `CornuCopyBuffer.promote` method.
+        * `recv_len_func`: optional function to compute the data
+          length of a received packet; the default watches the offset
+          on the receive stream
         * `send`: outbound binary stream.
           If this is an `int` it is taken to be an OS file descriptor,
-          otherwise it should be a file like object with `.write(bytes)`
+          otherwise it should be a binary file like object with `.write(bytes)`
           and `.flush()` methods.
-          For a file descriptor sending is done via an os.dup() of
-          the supplied descriptor, so the caller remains responsible
-          for closing the original descriptor.
+          This objects _is not closed_ by the `PacketConnection`;
+          the caller has responsibility for that.
+        * `send_len_func`: optional function to compute the data
+          length of a sent packet; the default watches the offset
+          on the send stream
         * `packet_grace`:
           default pause in the packet sending worker
           to allow another packet to be queued
           before flushing the output stream.
           Default: `DEFAULT_PACKET_GRACE`s.
           A value of `0` will flush immediately if the queue is empty.
         * `request_handler`: an optional callable accepting
@@ -194,157 +216,183 @@
           If `None`, do nothing.
           If a Boolean, call `tick_fd_2` if true, otherwise do nothing.
           Otherwise `tick` should be a callable accepting a byteslike value.
     '''
     if name is None:
       name = str(seq())
     self.name = name
-    if isinstance(recv, int):
-      self._recv = CornuCopyBuffer.from_fd(recv)
-    elif isinstance(recv, CornuCopyBuffer):
-      self._recv = recv
-    else:
-      self._recv = CornuCopyBuffer.from_file(recv)
+    self._recv = recv
     if isinstance(send, int):
-      self._send = os.fdopen(os.dup(send), 'wb')
+      self._send = os.fdopen(send, 'wb')
     else:
       self._send = send
     if packet_grace is None:
       packet_grace = DEFAULT_PACKET_GRACE
     if tick is None:
-      tick = lambda bs: None
+      tick = lambda bs: None  # pylint: disable=unnecessary-lambda-assignment
     elif isinstance(tick, bool):
       if tick:
         tick = tick_fd_2
       else:
-        tick = lambda bs: None
+        tick = lambda bs: None  # pylint: disable=unnecessary-lambda-assignment
+    self._recv_last_offset = 0
+    if recv_len_func is None:
+
+      def recv_len_func(_):
+        ''' The default length of a packet is the length of the _recv.offset change.
+        '''
+        new_offset = self._recv.offset
+        length = new_offset - self._recv_last_offset
+        self._recv_last_offset = new_offset
+        return length
+
+    self._recv_len_func = recv_len_func
+    self._send_last_offset = 0
+    if send_len_func is None:
+
+      def send_len_func(_):
+        ''' The default length of a packet is the length of the _send.offset change.
+        '''
+        new_offset = self._send.offset
+        length = new_offset - self._send_last_offset
+        self._send_last_offset = new_offset
+        return length
+
+    self._send_len_func = send_len_func
     self.packet_grace = packet_grace
     self.request_handler = request_handler
     self.tick = tick
-    # tags of requests in play against the local system
-    self._channel_request_tags = {0: set()}
-    self.notify_recv_eof = set()
-    self.notify_send_eof = set()
-    # LateFunctions for the requests we are performing for the remote system
-    self._running = set()
-    # requests we have outstanding against the remote system
-    self._pending = {0: {}}
-    # sequence of tag numbers
-    # TODO: later, reuse old tags to prevent monotonic growth of tag field
-    self._tag_seq = Seq(1)
-    # work queue for local requests
-    self._later = Later(4, name="%s:Later" % (self,))
-    self._later.open()
-    # dispatch queue of Packets to send
-    self._sendQ = IterableQueue(16)
+    self._pending = None
+    self._runstate = RunState(str(self))
     self._lock = Lock()
-    self.closed = False
-    # debugging: check for reuse of (channel,tag) etc
-    self.__sent = set()
-    self.__send_queued = set()
-    # dispatch Thread to process received packets
-    self._recv_thread = bg_thread(
-        self._receive_loop, name="%s[_receive_loop]" % (self.name,)
-    )
-    # dispatch Thread to send data
-    # primary purpose is to bundle output by deferring flushes
-    self._send_thread = bg_thread(
-        self._send_loop, name="%s[_send]" % (self.name,)
-    )
 
   def __str__(self):
     return "PacketConnection[%s]" % (self.name,)
 
-  @pfx_method
-  def shutdown(self, block=False):
-    ''' Shut down the PacketConnection, optionally blocking for outstanding requests.
-
-        Parameters:
-        `block`: block for outstanding requests, default False.
-    '''
-    with self._lock:
-      if self.closed:
-        # shutdown already called from another thread
-        return
-      # prevent further request submission either local or remote
-      self.closed = True
-    ps = self._pending_states()
-    if ps:
-      warning("PENDING STATES AT SHUTDOWN: %r", ps)
-    # wait for completion of requests we're performing
-    for LF in list(self._running):
-      LF.join()
-    # shut down sender, should trigger shutdown of remote receiver
-    self._sendQ.close(enforce_final_close=True)
-    self._send_thread.join()
-    # we do not wait for the receiver - anyone hanging on outstaning
-    # requests will get them as they come in, and in theory a network
-    # disconnect might leave the receiver hanging anyway
-    self._later.close()
-    if block:
-      self._later.wait()
+  @contextmanager
+  def startup_shutdown(self):
+    with super().startup_shutdown():
+      later = Later(4, name="%s:Later" % (self,))
+      with stackattrs(
+          self,
+          notify_recv_eof=set(),
+          notify_send_eof=set(),
+          # tags of remote requests in play against the local system,
+          # per channel
+          _channel_request_tags={0: set()},
+          # LateFunctions for the requests we are performing for the remote system
+          _running=set(),
+          # requests we have outstanding against the remote system, per channel
+          _pending={0: {}},
+          # sequence of tag numbers
+          # TODO: later, reuse old tags to prevent monotonic growth of tag field?
+          _tag_seq=Seq(1),
+          # work queue for local requests
+          _later=later,
+          # dispatch queue of Packets to send
+          _sendQ=IterableQueue(16),
+          _lock=Lock(),
+          # debugging: check for reuse of (channel,tag) etc
+          _sent=set(),
+          _send_queued=set(),
+      ):
+        with self._later:
+          runstate = self._runstate
+          with runstate:
+            # dispatch Thread to process received packets
+            self._recv_thread = bg_thread(
+                self._receive_loop,
+                name="%s[_receive_loop]" % (self.name,),
+                kwargs=dict(
+                    notify_recv_eof=self.notify_recv_eof, runstate=runstate
+                ),
+            )
+            # dispatch Thread to send data
+            # primary purpose is to bundle output by deferring flushes
+            self._send_thread = bg_thread(
+                self._send_loop,
+                name="%s[_send]" % (self.name,),
+            )
+            yield
+          # block new requests
+          runstate.cancel()
+          # complete accepted but incomplete requests
+          for LF in list(self._running):
+            LF.join()
+        # there should not be any outstanding work
+        later.wait()
+        # close the stream to the remote and wait
+        self._sendQ.close(enforce_final_close=True)
+        self._send_thread.join()
+        # we do not wait for the receiver - anyone hanging on outstanding
+        # requests will get them as they come in, and in theory a network
+        # disconnect might leave the receiver hanging anyway
+        ps = self._pending_states()
+        if ps:
+          warning("PENDING STATES AT SHUTDOWN: %r", ps)
 
   def join(self):
     ''' Wait for the receive side of the connection to terminate.
     '''
     self._recv_thread.join()
 
   def _new_tag(self):
     return next(self._tag_seq)
 
   def _pending_states(self):
     ''' Return a list of ( (channel, tag), Request_State ) for the currently pending requests.
     '''
     states = []
     pending = self._pending
-    for channel, channel_states in sorted(pending.items()):
-      for tag, channel_state in sorted(channel_states.items()):
-        states.append(((channel, tag), channel_state))
+    if pending is not None:
+      for channel, channel_states in sorted(pending.items()):
+        for tag, channel_state in sorted(channel_states.items()):
+          states.append(((channel, tag), channel_state))
     return states
 
   @locked
   def _pending_add(self, channel, tag, state):
-    ''' Record some state against a (channel, tag).
+    ''' Record some state against `(channel,tag)`.
     '''
     pending = self._pending
     if channel not in pending:
       raise ValueError("unknown channel %d" % (channel,))
     channel_info = pending[channel]
     if tag in channel_info:
       raise ValueError("tag %d already pending in channel %d" % (tag, channel))
     self._pending[channel][tag] = state
 
   @locked
   def _pending_pop(self, channel, tag):
-    ''' Retrieve and remove the state associated with (channel, tag).
+    ''' Retrieve and remove the state associated with `(channel,tag)`.
     '''
     pending = self._pending
     if channel not in pending:
       raise ValueError("unknown channel %d" % (channel,))
     channel_info = pending[channel]
     if tag not in channel_info:
       raise ValueError("tag %d unknown in channel %d" % (tag, channel))
-    if False and tag == 15:
-      raise RuntimeError("BANG")
+    ##if False and tag == 15:
+    ##  raise RuntimeError("BANG")
     return channel_info.pop(tag)
 
   def _pending_cancel(self):
     ''' Cancel all the pending requests.
     '''
     for chtag, _ in self._pending_states():
       channel, tag = chtag
       warning("%s: cancel pending request %d:%s", self, channel, tag)
       _, result = self._pending_pop(channel, tag)
       result.cancel()
 
   def _queue_packet(self, P):
     sig = (P.channel, P.tag, P.is_request)
-    if sig in self.__send_queued:
+    if sig in self._send_queued:
       raise RuntimeError("requeue of %s: %s" % (sig, P))
-    self.__send_queued.add(sig)
+    self._send_queued.add(sig)
     try:
       self._sendQ.put(P)
     except ClosedError as e:
       warning("%s: packet not sent: %s (P=%s)", self._sendQ, e, P)
 
   def _reject(self, channel, tag, payload=bytes(())):
     ''' Issue a rejection of the specified request.
@@ -380,16 +428,21 @@
             payload=payload
         )
     )
 
   @not_closed
   # pylint: disable=too-many-arguments
   def request(
-      self, rq_type, flags=0, payload=b'', decode_response=None, channel=0
-  ):
+      self,
+      rq_type,
+      flags=0,
+      payload=b'',
+      decode_response=None,
+      channel=0
+  ) -> Result:
     ''' Compose and dispatch a new request, returns a `Result`.
 
         Allocates a new tag, a Result to deliver the response, and
         records the response decode function for use when the
         response arrives.
 
         Parameters:
@@ -404,54 +457,65 @@
 
         The Result will yield an `(ok, flags, payload)` tuple, where:
         * `ok`: whether the request was successful
         * `flags`: the response flags
         * `payload`: the response payload, decoded by decode_response
           if specified
     '''
+    if self._runstate.cancelled:
+      raise ClosedError("shutting down: self.cancelled")
     if rq_type < 0:
       raise ValueError("rq_type may not be negative (%s)" % (rq_type,))
     # reserve type 0 for end-of-requests
     rq_type += 1
     tag = self._new_tag()
-    R = Result()
+    R = Result(f'{self.name}:{tag}')
     self._pending_add(channel, tag, Request_State(decode_response, R))
     self._queue_packet(
         Packet(
             is_request=True,
             channel=channel,
             tag=tag,
             flags=flags,
             rq_type=rq_type,
             payload=payload
         )
     )
     return R
 
   @not_closed
-  def do(self, *a, **kw):
+  def do(self, rq_type, flags=0, payload=b'', decode_response=None, channel=0):
     ''' Synchronous request.
         Submits the request, then calls the `Result` returned from the request.
     '''
-    return self.request(*a, **kw)()
+    return self.request(
+        rq_type,
+        flags=flags,
+        payload=payload,
+        decode_response=decode_response,
+        channel=channel
+    )()
 
   @logexc
   # pylint: disable=too-many-arguments
   def _run_request(self, channel, tag, handler, rq_type, flags, payload):
     ''' Run a request and queue a response packet.
     '''
     with Pfx(
-        "_run_request[channel=%d,tag=%d,rq_type=%d,flags=0x%02x,payload=%s",
+        "_run_request[channel=%d,tag=%d,rq_type=%d,flags=0x%02x,payload=%s]",
         channel, tag, rq_type, flags,
         repr(payload) if len(payload) <= 32 else repr(payload[:32]) + '...'):
       result_flags = 0
       result_payload = b''
       try:
         result = handler(rq_type, flags, payload)
-        if result is not None:
+        if result is None:
+          # no meaningful result - return the default (0,b'')
+          pass
+        else:
           if isinstance(result, int):
             result_flags = result
           elif isinstance(result, bytes):
             result_payload = result
           elif isinstance(result, str):
             result_payload = result.encode(
                 encoding='utf-8', errors='xmlcharrefreplace'
@@ -462,153 +526,159 @@
         exception("exception: %s", e)
         self._reject(channel, tag, "exception during handler")
       else:
         self._respond(channel, tag, result_flags, result_payload)
       self._channel_request_tags[channel].remove(tag)
 
   # pylint: disable=too-many-branches,too-many-statements,too-many-locals
-  def _receive_loop(self):
+  @logexc
+  @pfx_method
+  @ensure(lambda self: self._recv is None)
+  def _receive_loop(self, *, notify_recv_eof: set, runstate: RunState):
     ''' Receive packets from upstream, decode into requests and responses.
     '''
-    XX = self.tick
-    with PrePfx("_RECEIVE [%s]", self):
-      with post_condition(("_recv is None", lambda: self._recv is None)):
-        while True:
+    ##XX = self.tick
+    for packet in progressbar(
+        Packet.scan(self._recv),
+        label=f'<= {self.name}',
+        units_scale=BINARY_BYTES_SCALE,
+        itemlenfunc=self._recv_len_func,
+    ):
+      if packet == self.EOF_Packet:
+        break
+      channel = packet.channel
+      tag = packet.tag
+      flags = packet.flags
+      payload = packet.payload
+      if packet.is_request:
+        # request from upstream client
+        with Pfx("request[%d:%d]", channel, tag):
+          if self.request_handler is None:
+            # we are only a client, not a server
+            self._reject(channel, tag, "no request handler")
+          elif runstate.cancelled:
+            # we are shutting down, no new work accepted
+            self._reject(channel, tag, "rejecting request: runstate.cancelled")
+          else:
+            requests = self._channel_request_tags
+            if channel not in requests:
+              # unknown channel
+              self._reject(channel, tag, "unknown channel %d")
+            elif tag in self._channel_request_tags[channel]:
+              self._reject(
+                  channel, tag,
+                  "channel %d: tag already in use: %d" % (channel, tag)
+              )
+            else:
+              # payload for requests is the request enum and data
+              rq_type = packet.rq_type
+              if rq_type == 0:
+                # magic EOF rq_type - must be malformed (!=EOF_Packet)
+                error("malformed EOF packet received: %s", packet)
+                break
+              # normalise rq_type
+              rq_type -= 1
+              requests[channel].add(tag)
+              # queue the work function and track it
+              LF = self._later.defer(
+                  self._run_request, channel, tag, self.request_handler,
+                  rq_type, flags, payload
+              )
+              self._running.add(LF)
+              LF.notify(self._running.remove)
+      else:
+        # response to a previous request from us
+        with Pfx("response[%d:%d]", channel, tag):
+          # response: get state of matching pending request, remove state
           try:
-            XX(b'<')
-            packet = Packet.parse(self._recv)
-          except EOFError:
-            break
-          if packet == self.EOF_Packet:
-            break
-          channel = packet.channel
-          tag = packet.tag
-          flags = packet.flags
-          payload = packet.payload
-          if packet.is_request:
-            # request from upstream client
-            with Pfx("request[%d:%d]", channel, tag):
-              if self.closed:
-                debug("rejecting request: closed")
-                # NB: no rejection packet sent since sender also closed
-              elif self.request_handler is None:
-                self._reject(channel, tag, "no request handler")
-              else:
-                requests = self._channel_request_tags
-                if channel not in requests:
-                  # unknown channel
-                  self._reject(channel, tag, "unknown channel %d")
-                elif tag in self._channel_request_tags[channel]:
-                  self._reject(
-                      channel, tag,
-                      "channel %d: tag already in use: %d" % (channel, tag)
-                  )
-                else:
-                  # payload for requests is the request enum and data
-                  rq_type = packet.rq_type
-                  if rq_type == 0:
-                    # magic EOF rq_type - must be malformed (!=EOF_Packet)
-                    error("malformed EOF packet received: %s", packet)
-                    break
-                  # normalise rq_type
-                  rq_type -= 1
-                  requests[channel].add(tag)
-                  # queue the work function and track it
-                  LF = self._later.defer(
-                      self._run_request, channel, tag, self.request_handler,
-                      rq_type, flags, payload
-                  )
-                  self._running.add(LF)
-                  LF.notify(self._running.remove)
+            rq_state = self._pending_pop(channel, tag)
+          except ValueError as e:
+            # no such pending pair - response to unknown request
+            error("%d.%d: response to unknown request: %s", channel, tag, e)
           else:
-            with Pfx("response[%d:%d]", channel, tag):
-              # response: get state of matching pending request, remove state
-              try:
-                rq_state = self._pending_pop(channel, tag)
-              except ValueError as e:
-                # no such pending pair - response to unknown request
-                error(
-                    "%d.%d: response to unknown request: %s", channel, tag, e
-                )
+            decode_response, R = rq_state
+            # first flag is "ok"
+            ok = (flags & 0x01) != 0
+            flags >>= 1
+            payload = packet.payload
+            if ok:
+              # successful reply
+              # return (True, flags, decoded-response)
+              if decode_response is None:
+                # return payload bytes unchanged
+                R.result = (True, flags, payload)
               else:
-                decode_response, R = rq_state
-                # first flag is "ok"
-                ok = (flags & 0x01) != 0
-                flags >>= 1
-                payload = packet.payload
-                if ok:
-                  # successful reply
-                  # return (True, flags, decoded-response)
-                  if decode_response is None:
-                    # return payload bytes unchanged
-                    R.result = (True, flags, payload)
-                  else:
-                    # decode payload
-                    try:
-                      result = decode_response(flags, payload)
-                    except Exception:  # pylint: disable=broad-except
-                      R.exc_info = sys.exc_info()
-                    else:
-                      R.result = (True, flags, result)
+                # decode payload
+                try:
+                  result = decode_response(flags, payload)
+                except Exception:  # pylint: disable=broad-except
+                  R.exc_info = sys.exc_info()
                 else:
-                  # unsuccessful: return (False, other-flags, payload-bytes)
-                  R.result = (False, flags, payload)
-        # end of received packets: cancel any outstanding requests
-        self._pending_cancel()
-        # alert any listeners of receive EOF
-        for notify in self.notify_recv_eof:
-          notify(self)
-        self._recv = None
-        self.shutdown()
+                  R.result = (True, flags, result)
+            else:
+              # unsuccessful: return (False, other-flags, payload-bytes)
+              R.result = (False, flags, payload)
+    # end of received packets: cancel any outstanding requests
+    self._pending_cancel()
+    # alert any listeners of receive EOF
+    for notify in notify_recv_eof:
+      notify(self)
+    self._recv = None
 
   # pylint: disable=too-many-branches
+  @logexc
   def _send_loop(self):
     ''' Send packets upstream.
         Write every packet directly to self._send.
         Flush whenever the queue is empty.
     '''
-    XX = self.tick
-    ##with Pfx("%s._send", self):
+    ##XX = self.tick
     with PrePfx("_SEND [%s]", self):
       with post_condition(("_send is None", lambda: self._send is None)):
         fp = self._send
         Q = self._sendQ
         grace = self.packet_grace
-        for P in Q:
+        for P in progressbar(
+            Q,
+            label=f'=> {self.name}',
+            units_scale=BINARY_BYTES_SCALE,
+            itemlenfunc=len,
+        ):
           sig = (P.channel, P.tag, P.is_request)
-          if sig in self.__sent:
+          if sig in self._sent:
             raise RuntimeError("second send of %s" % (P,))
-          self.__sent.add(sig)
+          self._sent.add(sig)
           try:
-            XX(b'>')
+            ##XX(b'>')
             for bs in P.transcribe_flat():
               fp.write(bs)
             if Q.empty():
               # no immediately ready further packets: flush the output buffer
               if grace > 0:
                 # allow a little time for further Packets to queue
-                XX(b'Sg')
+                ##XX(b'Sg')
                 sleep(grace)
                 if Q.empty():
                   # still nothing
-                  XX(b'F')
+                  ##XX(b'F')
                   fp.flush()
               else:
-                XX(b'F')
+                ##XX(b'F')
                 fp.flush()
           except OSError as e:
             if e.errno == errno.EPIPE:
               warning("remote end closed")
               break
             raise
+        # send EOF packet to remote receiver and close self._send
         try:
-          XX(b'>EOF')
+          ##XX(b'>EOF')
           for bs in self.EOF_Packet.transcribe_flat():
             fp.write(bs)
-          fp.close()
+          fp.flush()
         except (OSError, IOError) as e:
           if e.errno == errno.EPIPE:
             debug("remote end closed: %s", e)
           elif e.errno == errno.EBADF:
             warning("local end closed: %s", e)
           else:
             raise
```

