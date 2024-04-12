# Comparing `tmp/objr-110.tar.gz` & `tmp/objr-120.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objr-110.tar", last modified: Thu Mar 21 11:49:48 2024, max compression
+gzip compressed data, was "objr-120.tar", last modified: Fri Apr 12 14:51:32 2024, max compression
```

## Comparing `objr-110.tar` & `objr-120.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-03-21 11:49:48.989721 objr-110/
--rw-r--r--   0 bart      (1000) bart      (1000)     1221 2024-03-21 11:49:48.989721 objr-110/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      695 2024-03-20 12:29:47.000000 objr-110/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-03-21 11:49:48.989721 objr-110/objr/
--rw-r--r--   0 bart      (1000) bart      (1000)     1160 2024-03-20 22:31:36.000000 objr-110/objr/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      811 2024-03-20 22:29:20.000000 objr-110/objr/broker.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1523 2024-03-20 15:10:10.000000 objr-110/objr/errors.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4372 2024-03-20 22:32:06.000000 objr-110/objr/handler.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5708 2024-03-20 22:30:08.000000 objr-110/objr/object.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4515 2024-03-20 22:30:19.000000 objr-110/objr/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1170 2024-03-20 22:30:30.000000 objr-110/objr/repeat.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1859 2024-03-20 22:30:43.000000 objr-110/objr/thread.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-03-21 11:49:48.989721 objr-110/objr.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     1221 2024-03-21 11:49:48.000000 objr-110/objr.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      293 2024-03-21 11:49:48.000000 objr-110/objr.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-03-21 11:49:48.000000 objr-110/objr.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-03-21 11:49:48.000000 objr-110/objr.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-03-21 11:49:48.000000 objr-110/objr.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      875 2024-03-21 11:49:39.000000 objr-110/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-03-21 11:49:48.989721 objr-110/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-03-18 12:44:31.000000 objr-110/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:51:32.988106 objr-120/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3989 2024-04-12 14:51:32.988106 objr-120/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     3462 2024-04-12 14:00:10.000000 objr-120/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:51:32.984106 objr-120/objr/
+-rw-r--r--   0 bart      (1000) bart      (1000)      560 2024-04-12 13:30:26.000000 objr-120/objr/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3871 2024-04-12 12:29:51.000000 objr-120/objr/client.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1888 2024-04-12 12:29:51.000000 objr-120/objr/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      941 2024-04-12 12:29:51.000000 objr-120/objr/errors.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      762 2024-04-12 12:29:51.000000 objr-120/objr/event.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1361 2024-04-12 12:29:51.000000 objr-120/objr/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      275 2024-04-12 12:29:51.000000 objr-120/objr/repeater.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1900 2024-04-12 12:29:51.000000 objr-120/objr/thread.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1091 2024-04-12 12:29:51.000000 objr-120/objr/timer.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:51:32.988106 objr-120/objr.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3989 2024-04-12 14:51:32.000000 objr-120/objr.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      335 2024-04-12 14:51:32.000000 objr-120/objr.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 14:51:32.000000 objr-120/objr.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-12 14:51:32.000000 objr-120/objr.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-12 14:51:32.000000 objr-120/objr.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 14:51:32.000000 objr-120/objr.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)      907 2024-04-12 14:04:57.000000 objr-120/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-12 14:51:32.988106 objr-120/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-09 11:10:16.000000 objr-120/setup.py
```

### Comparing `objr-110/objr/handler.py` & `objr-120/objr/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,139 +1,116 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0212,W0613,W0718,E0402,E1102
+# pylint: disable=C,R,W0105,W0718
 
 
-"hander"
+"client"
 
 
-import queue
-import threading
-import _thread
+from objx import Default
 
 
-from .broker import Broker
-from .errors import Errors
-from .object import Default, Object
-from .thread import launch
-
-
-class Event(Default):
-
-    def __init__(self):
-        Default.__init__(self)
-        self._thr    = None
-        self._ready  = threading.Event()
-        self.done    = False
-        self.orig    = None
-        self.result  = []
-        self.txt     = ""
-        self.type    = "event"
-
-    def ready(self):
-        self._ready.set()
-
-    def reply(self, txt):
-        self.result.append(txt)
-
-    def wait(self):
-        if self._thr:
-            self._thr.join()
-        self._ready.wait()
-        return self.result
-
-
-class Handler:
-
-    def __init__(self):
-        self.cbs = Object()
-        self.queue    = queue.Queue()
-        self.stopped  = threading.Event()
-        self.threaded = True
-
-    def callback(self, evt):
-        func = getattr(self.cbs, evt.type, None)
-        if not func:
-            evt.ready()
-            return
-        evt._thr = launch(func, evt)
-
-    def loop(self):
-        while not self.stopped.is_set():
-            try:
-                evt = self.poll()
-                self.callback(evt)
-            except (KeyboardInterrupt, EOFError):
-                _thread.interrupt_main()
-
-    def poll(self):
-        return self.queue.get()
-
-    def put(self, evt):
-        self.queue.put_nowait(evt)
-
-    def register(self, typ, cbs):
-        setattr(self.cbs, typ, cbs)
-
-    def start(self):
-        launch(self.loop)
-
-    def stop(self):
-        self.stopped.set()
+from .command import Command
+from .errors  import later
+from .event   import Event
+from .handler import Handler
 
 
 class Client(Handler):
 
-    cmds = Object()
+    "Client"
 
     def __init__(self):
         Handler.__init__(self)
-        self.register("command", self.command)
-        Broker.add(self)
-
-    @staticmethod
-    def add(func):
-        setattr(Client.cmds, func.__name__, func)
+        self.register("command", command)
 
     def announce(self, txt):
+        "announce text."
         self.raw(txt)
 
-    def command(self, evt):
-        parse_cmd(evt)
-        func = getattr(Client.cmds, evt.cmd, None)
-        if func:
-            try:
-                func(evt)
-            except Exception as exc:
-                Errors.add(exc)
-        self.show(evt)
-        evt.ready()
-
     def raw(self, txt):
-        pass
+        "raw output."
 
-    def say(self, channel, txt):
+    def say(self, _channel, txt):
+        "say text in a channel."
         self.raw(txt)
 
     def show(self, evt):
+        "show results into a channel."
         for txt in evt.result:
             self.say(evt.channel, txt)
 
 
 def cmnd(txt, out):
+    "do a command using the provided output function."
     clt = Client()
     clt.raw = out
     evn = Event()
     evn.orig = object.__repr__(clt)
     evn.txt = txt
-    clt.command(evn)
+    command(clt, evn)
     evn.wait()
     return evn
 
+
+def command(bot, evt):
+    "check for and run a command."
+    parse_cmd(evt)
+    func = getattr(Command.cmds, evt.cmd, None)
+    if func:
+        try:
+            func(evt)
+        except Exception as exc:
+            later(exc)
+    bot.show(evt)
+    evt.ready()
+
+
+def laps(seconds, short=True):
+    "show elapsed time."
+    txt = ""
+    nsec = float(seconds)
+    if nsec < 1:
+        return f"{nsec:.2f}s"
+    yea = 365*24*60*60
+    week = 7*24*60*60
+    nday = 24*60*60
+    hour = 60*60
+    minute = 60
+    yeas = int(nsec/yea)
+    nsec -= yeas*yea
+    weeks = int(nsec/week)
+    nsec -= weeks*week
+    nrdays = int(nsec/nday)
+    nsec -= nrdays*nday
+    hours = int(nsec/hour)
+    nsec -= hours*hour
+    minutes = int(nsec/minute)
+    nsec -= int(minute*minutes)
+    sec = int(nsec)
+    if yeas:
+        txt += f"{yeas}y"
+    if weeks:
+        nrdays += weeks * 7
+    if nrdays:
+        txt += f"{nrdays}d"
+    if short and txt:
+        return txt.strip()
+    if hours:
+        txt += f"{hours}h"
+    if minutes:
+        txt += f"{minutes}m"
+    if sec:
+        txt += f"{sec}s"
+    txt = txt.strip()
+    return txt
+
+
 def parse_cmd(obj, txt=None):
+    "parse a string for a command."
     args = []
     obj.args    = obj.args or []
     obj.cmd     = obj.cmd or ""
     obj.gets    = obj.gets or Default()
     obj.hasmods = obj.hasmod or False
     obj.index   = None
     obj.mod     = obj.mod or ""
@@ -178,21 +155,14 @@
         obj.txt  = obj.cmd or ""
         obj.rest = " ".join(obj.args)
         obj.txt  = obj.cmd + " " + obj.rest
     else:
         obj.txt = obj.cmd or ""
 
 
-"interface"
-
-
-def __dir__():
-    return (
-        'Event',
-        'Handler',
-        'Client',
-        'cmnd',
-        'parse_cmd'
-    )
-
-
-__all__ = __dir__()
+def spl(txt):
+    "split comma separated string into a list."
+    try:
+        res = txt.split(',')
+    except (TypeError, ValueError):
+        res = txt
+    return [x for x in res if x]
```

### Comparing `objr-110/objr/thread.py` & `objr-120/objr/thread.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C,R,W0105,W0718
 
 
-"threads"
+"thread"
 
 
 import queue
 import threading
 import time
 import types
 
 
-from .errors import Errors
+from .errors import later
 
 
 class Thread(threading.Thread):
 
+    "Thread"
+
     def __init__(self, func, thrname, *args, daemon=True, **kwargs):
         super().__init__(None, self.run, thrname, (), {}, daemon=daemon)
         self._result   = None
         self.name      = thrname or name(func)
         self.queue     = queue.Queue()
         self.sleep     = None
         self.starttime = time.time()
@@ -30,54 +32,44 @@
         return self
 
     def __next__(self):
         for k in dir(self):
             yield k
 
     def join(self, timeout=1.0):
+        "join this thread."
         super().join(timeout)
         return self._result
 
     def run(self):
+        "run this thread's payload."
         func, args = self.queue.get()
         try:
             self._result = func(*args)
-        except Exception as exc:
-            Errors.add(exc)
-            if args and "ready" in dir(args[0]):
+        except Exception as ex:
+            later(ex)
+            if args and "Event" in str(type(args[0])):
                 args[0].ready()
 
 
 def launch(func, *args, **kwargs):
+    "launch a thread."
     nme = kwargs.get("name", name(func))
     thread = Thread(func, nme, *args, **kwargs)
     thread.start()
     return thread
 
 
 def name(obj):
+    "return a full qualified name of an object/function/module."
     typ = type(obj)
     if isinstance(typ, types.ModuleType):
         return obj.__name__
     if '__self__' in dir(obj):
         return f'{obj.__self__.__class__.__name__}.{obj.__name__}'
     if '__class__' in dir(obj) and '__name__' in dir(obj):
         return f'{obj.__class__.__name__}.{obj.__name__}'
     if '__class__' in dir(obj):
         return f"{obj.__class__.__module__}.{obj.__class__.__name__}"
     if '__name__' in dir(obj):
         return f'{obj.__class__.__name__}.{obj.__name__}'
     return None
-
-
-"interface"
-
-
-def __dir__():
-    return (
-        'Thread',
-        'launch',
-        'name'
-    )
-
-
-__all__ = __dir__()
```

### Comparing `objr-110/pyproject.toml` & `objr-120/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "objr"
 description = "objects runtime"
-version = "110"
+version = "120"
 authors = [
-    {name = "xobjectz",email = "objx@proton.me"},
+    {name = "Bart Thate",email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
+dependencies = [
+    'objx',
+]
 classifiers = [ 
     'Development Status :: 3 - Alpha',
     'License :: Public Domain',
     'Operating System :: Unix',
     'Programming Language :: Python',
     'Topic :: Utilities'
 ]
```

