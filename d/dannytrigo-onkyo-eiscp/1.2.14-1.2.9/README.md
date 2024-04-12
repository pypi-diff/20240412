# Comparing `tmp/dannytrigo_onkyo_eiscp-1.2.14.tar.gz` & `tmp/dannytrigo-onkyo-eiscp-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dannytrigo_onkyo_eiscp-1.2.14.tar", last modified: Fri Apr 12 16:35:21 2024, max compression
+gzip compressed data, was "dannytrigo-onkyo-eiscp-1.2.9.tar", last modified: Fri Mar  8 05:04:59 2024, max compression
```

## Comparing `dannytrigo_onkyo_eiscp-1.2.14.tar` & `dannytrigo-onkyo-eiscp-1.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 16:35:21.028791 dannytrigo_onkyo_eiscp-1.2.14/
--rw-rw-rw-   0        0        0     1092 2024-03-05 05:47:48.000000 dannytrigo_onkyo_eiscp-1.2.14/LICENSE
--rw-rw-rw-   0        0        0    10326 2024-04-12 16:35:21.013206 dannytrigo_onkyo_eiscp-1.2.14/PKG-INFO
--rw-rw-rw-   0        0        0     9555 2024-03-05 05:47:48.000000 dannytrigo_onkyo_eiscp-1.2.14/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-12 16:35:21.013206 dannytrigo_onkyo_eiscp-1.2.14/dannytrigo_onkyo_eiscp.egg-info/
--rw-rw-rw-   0        0        0    10326 2024-04-12 16:35:20.000000 dannytrigo_onkyo_eiscp-1.2.14/dannytrigo_onkyo_eiscp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2024-04-12 16:35:20.000000 dannytrigo_onkyo_eiscp-1.2.14/dannytrigo_onkyo_eiscp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 16:35:20.000000 dannytrigo_onkyo_eiscp-1.2.14/dannytrigo_onkyo_eiscp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-12 16:35:20.000000 dannytrigo_onkyo_eiscp-1.2.14/dannytrigo_onkyo_eiscp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 16:35:20.000000 dannytrigo_onkyo_eiscp-1.2.14/dannytrigo_onkyo_eiscp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-12 16:35:20.000000 dannytrigo_onkyo_eiscp-1.2.14/dannytrigo_onkyo_eiscp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 16:35:20.997537 dannytrigo_onkyo_eiscp-1.2.14/eiscp/
--rw-rw-rw-   0        0        0      150 2024-03-19 00:26:52.000000 dannytrigo_onkyo_eiscp-1.2.14/eiscp/__init__.py
--rw-rw-rw-   0        0        0   184623 2024-04-12 16:31:18.000000 dannytrigo_onkyo_eiscp-1.2.14/eiscp/commands.py
--rw-rw-rw-   0        0        0    27848 2024-04-12 16:31:18.000000 dannytrigo_onkyo_eiscp-1.2.14/eiscp/core.py
--rw-rw-rw-   0        0        0     7827 2024-04-12 16:31:18.000000 dannytrigo_onkyo_eiscp-1.2.14/eiscp/script.py
--rw-rw-rw-   0        0        0      929 2024-04-12 16:31:18.000000 dannytrigo_onkyo_eiscp-1.2.14/eiscp/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-12 16:35:21.028791 dannytrigo_onkyo_eiscp-1.2.14/setup.cfg
--rw-rw-rw-   0        0        0     1227 2024-04-12 16:31:18.000000 dannytrigo_onkyo_eiscp-1.2.14/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:35:20.997537 dannytrigo_onkyo_eiscp-1.2.14/tests/
--rw-rw-rw-   0        0        0     1125 2024-04-12 16:31:18.000000 dannytrigo_onkyo_eiscp-1.2.14/tests/test_core.py
+drwxrwxrwx   0        0        0        0 2024-03-08 05:04:59.114818 dannytrigo-onkyo-eiscp-1.2.9/
+-rw-rw-rw-   0        0        0     1092 2024-03-05 05:47:48.000000 dannytrigo-onkyo-eiscp-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0    10325 2024-03-08 05:04:59.107200 dannytrigo-onkyo-eiscp-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9555 2024-03-05 05:47:48.000000 dannytrigo-onkyo-eiscp-1.2.9/README.rst
+drwxrwxrwx   0        0        0        0 2024-03-08 05:04:59.098198 dannytrigo-onkyo-eiscp-1.2.9/dannytrigo_onkyo_eiscp.egg-info/
+-rw-rw-rw-   0        0        0    10325 2024-03-08 05:04:58.000000 dannytrigo-onkyo-eiscp-1.2.9/dannytrigo_onkyo_eiscp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-03-08 05:04:58.000000 dannytrigo-onkyo-eiscp-1.2.9/dannytrigo_onkyo_eiscp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-08 05:04:58.000000 dannytrigo-onkyo-eiscp-1.2.9/dannytrigo_onkyo_eiscp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-03-08 05:04:58.000000 dannytrigo-onkyo-eiscp-1.2.9/dannytrigo_onkyo_eiscp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       42 2024-03-08 05:04:58.000000 dannytrigo-onkyo-eiscp-1.2.9/dannytrigo_onkyo_eiscp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-03-08 05:04:58.000000 dannytrigo-onkyo-eiscp-1.2.9/dannytrigo_onkyo_eiscp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-08 05:04:59.079751 dannytrigo-onkyo-eiscp-1.2.9/eiscp/
+-rw-rw-rw-   0        0        0      150 2024-03-05 05:47:49.000000 dannytrigo-onkyo-eiscp-1.2.9/eiscp/__init__.py
+-rw-rw-rw-   0        0        0   184623 2024-03-05 05:47:49.000000 dannytrigo-onkyo-eiscp-1.2.9/eiscp/commands.py
+-rw-rw-rw-   0        0        0    24320 2024-03-05 05:51:31.000000 dannytrigo-onkyo-eiscp-1.2.9/eiscp/core.py
+-rw-rw-rw-   0        0        0     7262 2024-03-05 05:47:49.000000 dannytrigo-onkyo-eiscp-1.2.9/eiscp/script.py
+-rw-rw-rw-   0        0        0      929 2024-03-05 05:47:49.000000 dannytrigo-onkyo-eiscp-1.2.9/eiscp/utils.py
+-rw-rw-rw-   0        0        0       42 2024-03-08 05:04:59.115831 dannytrigo-onkyo-eiscp-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1226 2024-03-08 05:04:36.000000 dannytrigo-onkyo-eiscp-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-08 05:04:59.088757 dannytrigo-onkyo-eiscp-1.2.9/tests/
+-rw-rw-rw-   0        0        0      401 2024-03-05 05:47:49.000000 dannytrigo-onkyo-eiscp-1.2.9/tests/test_core.py
```

### Comparing `dannytrigo_onkyo_eiscp-1.2.14/LICENSE` & `dannytrigo-onkyo-eiscp-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dannytrigo_onkyo_eiscp-1.2.14/PKG-INFO` & `dannytrigo-onkyo-eiscp-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dannytrigo-onkyo-eiscp
-Version: 1.2.14
+Version: 1.2.9
 Summary: Control Onkyo receivers over ethernet. (dannytrigo fork for bugfix)
 Home-page: https://github.com/dannytrigo/onkyo-eiscp
 Author: Michael Elsdörfer
 Author-email: michael@elsdoerfer.com
 License: MIT
 Platform: any
 Classifier: Topic :: System :: Networking
```

### Comparing `dannytrigo_onkyo_eiscp-1.2.14/README.rst` & `dannytrigo-onkyo-eiscp-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `dannytrigo_onkyo_eiscp-1.2.14/dannytrigo_onkyo_eiscp.egg-info/PKG-INFO` & `dannytrigo-onkyo-eiscp-1.2.9/dannytrigo_onkyo_eiscp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dannytrigo-onkyo-eiscp
-Version: 1.2.14
+Version: 1.2.9
 Summary: Control Onkyo receivers over ethernet. (dannytrigo fork for bugfix)
 Home-page: https://github.com/dannytrigo/onkyo-eiscp
 Author: Michael Elsdörfer
 Author-email: michael@elsdoerfer.com
 License: MIT
 Platform: any
 Classifier: Topic :: System :: Networking
```

### Comparing `dannytrigo_onkyo_eiscp-1.2.14/eiscp/commands.py` & `dannytrigo-onkyo-eiscp-1.2.9/eiscp/commands.py`

 * *Files identical despite different names*

### Comparing `dannytrigo_onkyo_eiscp-1.2.14/eiscp/core.py` & `dannytrigo-onkyo-eiscp-1.2.9/eiscp/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import re
 import struct
 import time
 import socket, select
 import threading
 import xmltodict
 import json
@@ -12,17 +11,14 @@
     import Queue as queue
 import netifaces
 from collections import namedtuple
 
 from . import commands
 from .utils import ValueRange, format_nri_list
 
-BUFFER_SIZE = 64 * 1024
-_LOGGER = logging.getLogger(__name__)
-
 
 class ISCPMessage(object):
     """Deals with formatting and parsing data wrapped in an ISCP
     containers. The docs say:
 
         ISCP (Integra Serial Control Protocol) consists of three
         command characters and parameter character(s) of variable
@@ -184,15 +180,15 @@
             # Split arguments by comma or space
             arguments = [norm(a) for a in re.split(r'[ ,]', arguments)]
         else:
             # Split command part by space or dot
             parts = [norm(c) for c in re.split(command_sep, command)]
             if len(parts) >= 3:
                 zone, command = parts[:2]
-                arguments = parts[2:]
+                arguments = parts[3:]
             elif len(parts) == 2:
                 zone = default_zone
                 command = parts[0]
                 arguments = parts[1:]
             else:
                 raise ValueError('Need at least command and argument')
 
@@ -242,50 +238,47 @@
             else:
                 raise ValueError('"{}" is not a valid argument for command '
                                 '"{}" in zone "{}"'.format(argument, command, zone))
 
     return '{}{}'.format(prefix, value)
 
 
-def iscp_to_command(iscp_message, with_zone=False):
-    def __iscp_to_command(iscp_message):
-        for zone, zone_cmds in commands.COMMANDS.items():
-            # For now, ISCP commands are always three characters, which
-            # makes this easy.
-            command, args = iscp_message[:3], iscp_message[3:]
-            if command in zone_cmds:
-                if args in zone_cmds[command]['values']:
-                    return zone, zone_cmds[command]['name'], \
-                           zone_cmds[command]['values'][args]['name']
+def iscp_to_command(iscp_message):
+    for zone, zone_cmds in commands.COMMANDS.items():
+        # For now, ISCP commands are always three characters, which
+        # makes this easy.
+        command, args = iscp_message[:3], iscp_message[3:]
+        if command in zone_cmds:
+            if args in zone_cmds[command]['values']:
+                return zone_cmds[command]['name'], \
+                       zone_cmds[command]['values'][args]['name']
+            else:
+                match = re.match('[+-]?[0-9a-f]+$', args, re.IGNORECASE)
+                if match:
+                    return zone_cmds[command]['name'], \
+                             int(args, 16)
                 else:
-                    match = re.match('[+-]?[0-9a-f]+$', args, re.IGNORECASE)
-                    if match:
-                        return zone, zone_cmds[command]['name'], int(args, 16)
-                    else:
-                        return zone, zone_cmds[command]['name'], args
-        else:
-            raise ValueError(
-                'Cannot convert ISCP message to command: {}'.format(iscp_message))
-    zone, ret_cmd, args = __iscp_to_command(iscp_message)
-    return (zone, ret_cmd, args) if with_zone else (ret_cmd, args)
+                    return zone_cmds[command]['name'], args
+
+    else:
+        raise ValueError(
+            'Cannot convert ISCP message to command: {}'.format(iscp_message))
+
 
 def filter_for_message(getter_func, msg):
     """Helper that calls ``getter_func`` until a matching message
     is found, or the timeout occurs. Matching means the same commands
     group, i.e. for sent message MVLUP we would accept MVL13
     in response."""
     start = time.time()
     while True:
         candidate = getter_func(0.05)
         # It seems ISCP commands are always three characters.
         if candidate and candidate[:3] == msg[:3]:
             return candidate
-        elif candidate and candidate[:3] == 'MDI' and msg[:3] == 'MGS':
-            # the MGS command for grouping multiroom audio, returns an MDI message, not MGS
-            return candidate
 
         # exception for HDMI-CEC commands (CTV) since they don't provide any response/confirmation
         if "CTV" in msg[:3]:
             return msg
         
         # The protocol docs claim that a response  should arrive
         # within *50ms or the communication has failed*. In my tests,
@@ -307,50 +300,18 @@
         (?P<model_name>[^/]*)/
         (?P<iscp_port>\d{5})/
         (?P<area_code>\w{2})/
         (?P<identifier>.{0,12})
     ''', response.strip(), re.VERBOSE).groupdict()
     return info
 
-class MessageBuffer:
-    """A receive buffer for eISCP packets to avoid partial receipt"""
-
-    def __init__(self, buffer_size):
-        self.buffer_size = buffer_size
-        self.buffer = b''
-
-    def reset(self):
-        """Reset the buffer"""
-        self.buffer = b''
-
-    @property
-    def available(self):
-        """Bytes remaining in the buffer"""
-        return self.buffer_size - len(self.buffer)
-
-    def recv(self, data: bytes):
-        """Add received bytes to the buffer"""
-        self.buffer += data
-
-    def get_message(self):
-        """Return a message if one is available in the buffer, otherwise return None"""
-        if len(self.buffer) >= 16:
-            header = eISCPPacket.parse_header(self.buffer[:16])
-            if len(self.buffer) >= header.data_size + 16:
-                packet = ISCPMessage.parse(self.buffer[16:header.data_size + 16].decode())
-                # Remove the processed message from the remaining buffer
-                self.buffer = self.buffer[16 + header.data_size:]
-                return packet
-        return None
-
-
 class eISCP(object):
     """Implements the eISCP interface to Onkyo receivers.
 
-    This uses a blocking interface. The remote end will regularly
+    This uses a blocking interface. The remote end will regularily
     send unsolicited status updates. You need to manually call
     ``get_message`` to query those.
 
     You may want to look at the :meth:`Receiver` class instead, which
     uses a background thread.
     """
     ONKYO_PORT = 60128
@@ -406,15 +367,14 @@
         return list(found_receivers.values())
 
     def __init__(self, host, port=60128):
         self.host = host
         self.port = port
         self._info = None
         self._nri = None
-        self._message_buffer = MessageBuffer(BUFFER_SIZE)
 
         self.command_socket = None
 
     @property
     def model_name(self):
         if self.info and self.info.get('model_name'):
             return self.info['model_name']
@@ -510,30 +470,21 @@
             if item.get("band") is not None:
                 key = item.pop("band")
                 info[key] = item
         return info
 
     def _ensure_socket_connected(self):
         if self.command_socket is None:
-            _LOGGER.info(f"Connecting to {self.host}:{self.port}")
-            try:
-                self.command_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-                self.command_socket.settimeout(self.CONNECT_TIMEOUT)
-                self.command_socket.connect((self.host, self.port))
-                self.command_socket.setblocking(0)
-                self._message_buffer.reset()
-                _LOGGER.debug(f"Connected")
-            except OSError as error:
-                _LOGGER.error("Failed to connect", error)
-                self.disconnect()
-                raise error
+            self.command_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            self.command_socket.settimeout(self.CONNECT_TIMEOUT)
+            self.command_socket.connect((self.host, self.port))
+            self.command_socket.setblocking(0)
 
     def disconnect(self):
         try:
-            _LOGGER.info("Closed command socket")
             self.command_socket.close()
         except:
             pass
         self.command_socket = None
 
     def __enter__(self):
         self._ensure_socket_connected()
@@ -554,35 +505,29 @@
 
     def get(self, timeout=0.1):
         """Return the next message sent by the receiver, or, after
         ``timeout`` has passed, return ``None``.
         """
         self._ensure_socket_connected()
 
-        # There might already be another message in the buffer
-        msg = self._message_buffer.get_message()
-        if msg:
-            return msg
-
         ready = select.select([self.command_socket], [], [], timeout or 0)
         if ready[0]:
-            try:
-                data = self.command_socket.recv(self._message_buffer.available)
-                self._message_buffer.recv(data)
-                if len(data) == 0:
-                    _LOGGER.error(f"Received no data on socket. Disconnecting")
-                    # We have very likely been disconnected
-                    eISCP.disconnect(self)
-                    return None
-                _LOGGER.info(f"Received {len(data)} bytes")
-                return self._message_buffer.get_message()
-            except OSError as error:
-                _LOGGER.error("Disconnected from receiver", error)
+            header_bytes = self.command_socket.recv(16)
+            if len(header_bytes) == 0:
+                # We have very likely been disconnected
                 eISCP.disconnect(self)
-        return None
+                return None
+            header = eISCPPacket.parse_header(header_bytes)
+            body = b''
+            while len(body) < header.data_size:
+                ready = select.select([self.command_socket], [], [], timeout or 0)
+                if not ready[0]:
+                    return None
+                body += self.command_socket.recv(header.data_size - len(body))
+            return ISCPMessage.parse(body.decode())
 
     def raw(self, iscp_message):
         """Send a low-level ISCP message, like ``MVL50``, and wait
         for a response.
 
         While the protocol is designed to acknowledge each message with
         a response, there is no fool-proof way to differentiate those
@@ -619,33 +564,14 @@
         """Turn the receiver power on."""
         return self.command('power', 'on')
 
     def power_off(self):
         """Turn the receiver power off."""
         return self.command('power', 'off')
 
-    def group_with(self, otherIDs=[]):
-        """Create a multiroom audio / flareconnect group with the supplied device IDs.
-        Calling this without arguments or an empty list stops the multiroom audio / flareconnect group.
-        Calling this method twice with the same arguments does not generate a response from the receiver, thus causing a timeout on the message."""
-        if otherIDs:
-            # check if the supplied deviceIDs are all strings
-            for ID in otherIDs:
-                if type(ID) != str:
-                    raise ValueError('group_with needs a list object, with each device identifier as a string')
-            # construct a MGS message with a list of the device IDs
-            message='MGS<mgs zone="1"><groupid>1</groupid><maxdelay>500</maxdelay><devices>' + \
-                '<device id="%s" zoneid="1"/>'%(self.identifier) + \
-                ''.join(['<device id="%s" zoneid="1"/>'%(ID) for ID in otherIDs]) + \
-                '</devices></mgs>'
-        else:
-            # No other devices specified. Create an empty group, which stops the multiroom audio / flareconnect
-            message='MGS<mgs zone="1"><groupid>0</groupid></mgs>'
-        return self.raw(message)
-
     def get_nri(self):
         """Return NRI info as dict."""
         data = self.command("dock.receiver-information=query")[1]
         if data:
             data = xmltodict.parse(data, attr_prefix="")
             data = data.get("response").get("device")
             # Cast OrderedDict to dict
```

### Comparing `dannytrigo_onkyo_eiscp-1.2.14/eiscp/script.py` & `dannytrigo-onkyo-eiscp-1.2.9/eiscp/script.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 '''Control Onkyo A/V receivers.
 
 Usage:
   %(program_name)s [--host <host>] [--port <port>]
   %(prog_n_space)s [--all] [--name <name>] [--id <identifier>]
   %(prog_n_space)s [--verbose | -v]... [--quiet | -q]... <command>...
   %(program_name)s --discover
-  %(program_name)s [--host <host>] [--group_with <otherhost> ...] 
   %(program_name)s --help-commands [<zone> <command>]
   %(program_name)s -h | --help
 
 Selecting the receiver:
 
   --host, -t <host>     Connect to this host
   --port, -p <port>     Connect to this port
@@ -28,19 +27,14 @@
   --help-commands       List available commands.
 
 Examples:
   %(program_name)s power=on source=pc volume=75
     Turn receiver on, select "PC" source, set volume to 75.
   %(program_name)s zone2.power=standby
     To execute a command for zone that isn't the main one.
-  %(program_name)s --host 192.168.1.15 --group_with "0009B0E4B723" "0009B0E4B724"
-    Setup multiroom audio using Flareconnect. The <host> receiver is source, all receiver IDs supplied for <otherhost> join the <host> in a Flareconnect group.
-    Use the --discover option to get the receiver IDs.
-  %(program_name)s --host 192.168.1.15 --group_with
-    Stop the multiroom audio group / flareconnect.
 '''
 
 import sys
 import os
 import docopt
 import re
 
@@ -114,17 +108,14 @@
                              if options['--id'] in r.identifier]
             else:
                 receivers = list(receivers)[:1]
         if not receivers:
             print('No receivers found.')
             return 1
 
-    if options['--group_with']:
-        receivers[0].group_with(options['<otherhost>'])
-
     # List of commands to execute - deal with special shortcut case
     to_execute = options['<command>']
 
     # Execute commands
     model_names = [r.model_name for r in receivers]
     regex = re.compile('^[A-Z]+[\+\-]*([0-9]*[A-Z]*)*$')
     for receiver in receivers:
```

### Comparing `dannytrigo_onkyo_eiscp-1.2.14/eiscp/utils.py` & `dannytrigo-onkyo-eiscp-1.2.9/eiscp/utils.py`

 * *Files identical despite different names*

### Comparing `dannytrigo_onkyo_eiscp-1.2.14/setup.py` & `dannytrigo-onkyo-eiscp-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 here = os.path.dirname(os.path.abspath(__file__))
 f = open(os.path.join(here, 'README.rst'))
 long_description = f.read().strip()
 f.close()
 
 setup(
     name='dannytrigo-onkyo-eiscp',
-    version='1.2.14',
+    version='1.2.9',
     url='https://github.com/dannytrigo/onkyo-eiscp',
     license='MIT',
     author='Michael Elsdörfer',
     author_email='michael@elsdoerfer.com',
     description='Control Onkyo receivers over ethernet. (dannytrigo fork for bugfix)',
     long_description=long_description,
     packages = find_packages(exclude=('tests*',)),
```

