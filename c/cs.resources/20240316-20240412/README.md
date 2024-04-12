# Comparing `tmp/cs.resources-20240316.tar.gz` & `tmp/cs.resources-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.resources-20240316.tar", last modified: Sat Mar 16 06:11:07 2024, max compression
+gzip compressed data, was "cs.resources-20240412.tar", last modified: Fri Apr 12 04:43:02 2024, max compression
```

## Comparing `cs.resources-20240316.tar` & `cs.resources-20240412.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:11:07.762840 cs.resources-20240316/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-16 06:10:40.000000 cs.resources-20240316/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    11116 2024-03-16 06:11:07.762213 cs.resources-20240316/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    15803 2024-03-16 06:10:49.000000 cs.resources-20240316/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:11:07.758440 cs.resources-20240316/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:11:07.758705 cs.resources-20240316/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:11:07.759889 cs.resources-20240316/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    26776 2024-03-16 06:10:30.000000 cs.resources-20240316/lib/python/cs/resources.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:11:07.761771 cs.resources-20240316/lib/python/cs.resources.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    11116 2024-03-16 06:11:07.000000 cs.resources-20240316/lib/python/cs.resources.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      297 2024-03-16 06:11:07.000000 cs.resources-20240316/lib/python/cs.resources.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 06:11:07.000000 cs.resources-20240316/lib/python/cs.resources.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      212 2024-03-16 06:11:07.000000 cs.resources-20240316/lib/python/cs.resources.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 06:11:07.000000 cs.resources-20240316/lib/python/cs.resources.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    11730 2024-03-16 06:11:06.000000 cs.resources-20240316/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 06:11:07.762935 cs.resources-20240316/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:43:02.148893 cs.resources-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 04:42:35.000000 cs.resources-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17683 2024-04-12 04:43:02.147971 cs.resources-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    16926 2024-04-12 04:42:44.000000 cs.resources-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:43:02.141777 cs.resources-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:43:02.142080 cs.resources-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:43:02.144666 cs.resources-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    27453 2024-04-12 04:42:21.000000 cs.resources-20240412/lib/python/cs/resources.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:43:02.147381 cs.resources-20240412/lib/python/cs.resources.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17683 2024-04-12 04:43:01.000000 cs.resources-20240412/lib/python/cs.resources.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      297 2024-04-12 04:43:02.000000 cs.resources-20240412/lib/python/cs.resources.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 04:43:01.000000 cs.resources-20240412/lib/python/cs.resources.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      210 2024-04-12 04:43:01.000000 cs.resources-20240412/lib/python/cs.resources.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 04:43:01.000000 cs.resources-20240412/lib/python/cs.resources.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    18297 2024-04-12 04:43:00.000000 cs.resources-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 04:43:02.149007 cs.resources-20240412/setup.cfg
```

### Comparing `cs.resources-20240316/PKG-INFO` & `cs.resources-20240412/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,60 @@
-Metadata-Version: 2.1
-Name: cs.resources
-Version: 20240316
-Summary: Resource management classes and functions.
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python2,python3
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
-
 Resource management classes and functions.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+* RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
+* RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
+* MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
+* RunState.__init__: make most parameters keyword only.
 
-## Class `ClosedError(builtins.Exception, builtins.BaseException)`
+## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
-## Class `MultiOpen(MultiOpenMixin, cs.context.ContextManagerMixin)`
+## Class `MultiOpen(MultiOpenMixin)`
 
 Context manager class that manages a single open/close object
 using a MultiOpenMixin.
 
 *Method `MultiOpen.__init__(self, openable, finalise_later=False)`*:
 Initialise: save the `openable` and call the MultiOpenMixin initialiser.
 
+*Method `MultiOpen.shutdown(self)`*:
+Close the associated openable object.
+
+*Method `MultiOpen.startup(self)`*:
+Open the associated openable object.
+
 ## Class `MultiOpenMixin(cs.context.ContextManagerMixin)`
 
 A multithread safe mixin to count open and close calls,
 doing a startup on the first `.open` and shutdown on the last `.close`.
 
 If used as a context manager this mixin calls `open()`/`close()` from
 `__enter__()` and `__exit__()`.
 
-It is recommended subclass implementations do as little as possible
-during `__init__`, and do almost all setup during startup so
-that the class may perform multiple startup/shutdown iterations.
+It is recommended that subclass implementations do as little
+as possible during `__init__`, and do almost all setup during
+startup so that the class may perform multiple startup/shutdown
+iterations.
 
 Classes using this mixin should define a context manager
 method `.startup_shutdown` which does the startup actions
 before yielding and then does the shutdown actions.
 
 Example:
 
     class DatabaseThing(MultiOpenMixin):
         @contextmanager
         def startup_shutdown(self):
             self._db = open_the_database()
-            yield
-            self._db.close()
+            try:
+                yield
+            finally:
+                self._db.close()
     ...
     with DatabaseThing(...) as db_thing:
         ... use db_thing ...
 
 If course, often something like a database open will itself
 be a context manager and the `startup_shutdown` method more
 usually looks like this:
@@ -88,14 +82,88 @@
        ... use db_thing ...
 
 TODO:
 * `subopens`: if true (default false) then `.open` will return
   a proxy object with its own `.closed` attribute set by the
   proxy's `.close`.
 
+*Property `MultiOpenMixin.MultiOpenMixin_state`*:
+The state object for the mixin,
+something of a hack to avoid providing an `__init__`.
+
+*Method `MultiOpenMixin.close(self, *, enforce_final_close=False, caller_frame=None, unopened_ok=False)`*:
+Decrement the open count.
+If the count goes to zero, call `self.shutdown()` and return its value.
+
+Parameters:
+* `enforce_final_close`: if true, the caller expects this to
+  be the final close for the object and a `RuntimeError` is
+  raised if this is not actually the case.
+* `caller_frame`: used for debugging; the caller may specify
+  this if necessary, otherwise it is computed from
+  `cs.py.stack.caller` when needed. Presently the caller of the
+  final close is recorded to help debugging extra close calls.
+* `unopened_ok`: if true, it is not an error if this is not open.
+  This is intended for closing callbacks which might get called
+  even if the original open never happened.
+  (I'm looking at you, `cs.resources.RunState`.)
+
+*Property `MultiOpenMixin.closed`*:
+Whether this object has been closed.
+Note: False if never opened.
+
+*Method `MultiOpenMixin.is_open(self)`*:
+Test whether this object is open.
+
+*Method `MultiOpenMixin.is_opened(func)`*:
+Decorator to wrap `MultiOpenMixin` proxy object methods which
+should raise if the object is not yet open.
+
+*Method `MultiOpenMixin.join(self)`*:
+Join this object.
+
+Wait for the internal finalise `Condition` (if still not `None`).
+Normally this is notified at the end of the shutdown procedure
+unless the object's `finalise_later` parameter was true.
+
+*Method `MultiOpenMixin.open(self, caller_frame=None)`*:
+Increment the open count.
+On the first `.open` call `self.startup()`.
+
+*Method `MultiOpenMixin.startup_shutdown(self)`*:
+Default context manager form of startup/shutdown - just
+call the distinct `.startup()` and `.shutdown()` methods
+if both are present, do nothing if neither is present.
+
+This supports subclasses always using:
+
+    with super().startup_shutdown():
+
+as an outer wrapper.
+
+The `.startup` check is to support legacy subclasses of
+`MultiOpenMixin` which have separate `startup()` and
+`shutdown()` methods.
+The preferred approach is a single `startup_shutdwn()`
+context manager overriding this method.
+
+The usual form looks like this:
+
+    @contextmanager
+    def startup_shutdown(self):
+        with super().startup_shutdown():
+            ... do some set up ...
+            try:
+                yield
+            finally:
+                ... do some tear down ...
+
+*Method `MultiOpenMixin.tcm_get_state(self)`*:
+Support method for `TrackedClassMixin`.
+
 ## Function `not_closed(func)`
 
 Decorator to wrap methods of objects with a .closed property
 which should raise when self.closed.
 
 ## Function `openif(obj)`
 
@@ -121,15 +189,18 @@
 Parameters:
 * `new_object` is a callable which returns a new object for the Pool.
 * `max_size`: The maximum size of the pool of available objects saved for reuse.
     If omitted or `None`, defaults to 4.
     If 0, no upper limit is applied.
 * `lock`: optional shared Lock; if omitted or `None` a new Lock is allocated
 
-## Class `RunState(cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+*Method `Pool.instance(self)`*:
+Context manager returning an object for use, which is returned to the pool afterwards.
+
+## Class `RunState(cs.threads.HasThreadState)`
 
 A class to track a running task whose cancellation may be requested.
 
 Its purpose is twofold, to provide easily queriable state
 around tasks which can start and stop, and to provide control
 methods to pronounce that a task has started (`.start`),
 should stop (`.cancel`)
@@ -168,32 +239,138 @@
 * `notify_start`: a set of callables called with the `RunState` instance
   to be called whenever `.running` becomes true.
 * `notify_end`: a set of callables called with the `RunState` instance
   to be called whenever `.running` becomes false.
 * `notify_cancel`: a set of callables called with the `RunState` instance
   to be called whenever `.cancel` is called.
 
+*Method `RunState.__bool__(self)`*:
+Return true if the task is running.
+
+*Method `RunState.__enter_exit__(self)`*:
+The `__enter__`/`__exit__` generator function:
+* push this RunState via HasThreadState
+* catch signals
+* start
+* `yield self` => run
+* cancel on exception during run
+* stop
+
+Note that if the `RunState` is already runnings we do not
+do any of that stuff apart from the `yield self` because
+we assume whatever setup should have been done has already
+been done.
+In particular, the `HasThreadState.Thread` factory calls this
+in the "running" state.
+
+*Method `RunState.__nonzero__(self)`*:
+Return true if the task is running.
+
+*Method `RunState.cancel(self)`*:
+Set the cancelled flag; the associated process should notice and stop.
+
+*Property `RunState.cancelled`*:
+Test the .cancelled attribute, including a poll if supplied.
+
+*Method `RunState.catch_signal(self, sig, call_previous=False, handle_signal=None)`*:
+Context manager to catch the signal or signals `sig` and
+cancel this `RunState`.
+Restores the previous handlers on exit.
+Yield a mapping of `sig`=>`old_handler`.
+
+Parameters:
+* `sig`: an `int` signal number or an iterable of signal numbers
+* `call_previous`: optional flag (default `False`)
+  passed to `cs.psutils.signal_handlers`
+
+*Method `RunState.end(self)`*:
+Stop: adjust state, set `stop_time` to now.
+Sets sets `.running` to `False`.
+
+*Method `RunState.handle_signal(self, sig, _)`*:
+`RunState` signal handler: cancel the run state.
+Warn if `self.verbose`.
+
+*Method `RunState.iter(self, it)`*:
+Iterate over `it` while not `self.cancelled`.
+
+*`RunState.perthread_state`*
+
+*Method `RunState.raiseif(self, msg=None, *a)`*:
+Raise `CancellationError` if cancelled.
+This is the concise way to terminate an operation which honour
+`.cancelled` if you're prepared to handle the exception.
+
+Example:
+
+    for item in items:
+        runstate.raiseif()
+        ... process item ...
+
+*Property `RunState.run_time`*:
+Property returning most recent run time (`stop_time-start_time`).
+If still running, use now as the stop time.
+If not started, return `0.0`.
+
+*Property `RunState.running`*:
+Property expressing whether the task is running.
+
+*Method `RunState.start(self, running_ok=False)`*:
+Start: adjust state, set `start_time` to now.
+Sets `.cancelled` to `False` and sets `.running` to `True`.
+
+*Method `RunState.stop(self)`*:
+Stop: adjust state, set `stop_time` to now.
+Sets sets `.running` to `False`.
+
+*Property `RunState.stopped`*:
+Was the process stopped? Running is false and cancelled is true.
+
+*Property `RunState.stopping`*:
+Is the process stopping? Running is true and cancelled is true.
+
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType])`*:
+*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x104ae5d80>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
+*Method `RunStateMixin.cancel(self)`*:
+Call .runstate.cancel().
+
+*Property `RunStateMixin.cancelled`*:
+Test .runstate.cancelled.
+
+*Property `RunStateMixin.running`*:
+Test .runstate.running.
+
+*Property `RunStateMixin.stopped`*:
+Test .runstate.stopped.
+
+*Property `RunStateMixin.stopping`*:
+Test .runstate.stopping.
+
 # Release Log
 
 
 
+*Release 20240412*:
+* RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
+* RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
+* MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
+* RunState.__init__: make most parameters keyword only.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
 MultiOpenMixin: new .is_open() method to test for opens > 0.
 
 *Release 20231221*:
@@ -285,8 +462,7 @@
 *Release 20160827*:
 * BREAKING CHANGE: rename NestingOpenCloseMixin to MultiOpenMixin.
 * New Pool class for generic object reuse.
 * Assorted minor improvements.
 
 *Release 20150115*:
 First PyPI release.
-
```

### Comparing `cs.resources-20240316/README.md` & `cs.resources-20240412/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,62 @@
+[project]
+name = "cs.resources"
+description = "Resource management classes and functions."
+authors = [
+    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
+]
+keywords = [
+    "python2",
+    "python3",
+]
+dependencies = [
+    "cs.context>=20240412",
+    "cs.deco>=20240412",
+    "cs.gimmicks>=20240316",
+    "cs.obj>=20220918",
+    "cs.pfx>=20240412",
+    "cs.psutils>=20240316",
+    "cs.py.func>=20230331",
+    "cs.py.stack>=20240412",
+    "cs.result>=20240412",
+    "cs.threads>=20240412",
+    "typeguard",
+]
+classifiers = [
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+]
+version = "20240412"
+
+[project.license]
+text = "GNU General Public License v3 or later (GPLv3+)"
+
+[project.urls]
+URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
+
+[project.readme]
+text = """
 Resource management classes and functions.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+* RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
+* RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
+* MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
+* RunState.__init__: make most parameters keyword only.
 
-## Class `ClosedError(builtins.Exception, builtins.BaseException)`
+## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
-## Class `MultiOpen(MultiOpenMixin, cs.context.ContextManagerMixin)`
+## Class `MultiOpen(MultiOpenMixin)`
 
 Context manager class that manages a single open/close object
 using a MultiOpenMixin.
 
 *Method `MultiOpen.__init__(self, openable, finalise_later=False)`*:
 Initialise: save the `openable` and call the MultiOpenMixin initialiser.
 
@@ -25,30 +70,33 @@
 
 A multithread safe mixin to count open and close calls,
 doing a startup on the first `.open` and shutdown on the last `.close`.
 
 If used as a context manager this mixin calls `open()`/`close()` from
 `__enter__()` and `__exit__()`.
 
-It is recommended subclass implementations do as little as possible
-during `__init__`, and do almost all setup during startup so
-that the class may perform multiple startup/shutdown iterations.
+It is recommended that subclass implementations do as little
+as possible during `__init__`, and do almost all setup during
+startup so that the class may perform multiple startup/shutdown
+iterations.
 
 Classes using this mixin should define a context manager
 method `.startup_shutdown` which does the startup actions
 before yielding and then does the shutdown actions.
 
 Example:
 
     class DatabaseThing(MultiOpenMixin):
         @contextmanager
         def startup_shutdown(self):
             self._db = open_the_database()
-            yield
-            self._db.close()
+            try:
+                yield
+            finally:
+                self._db.close()
     ...
     with DatabaseThing(...) as db_thing:
         ... use db_thing ...
 
 If course, often something like a database open will itself
 be a context manager and the `startup_shutdown` method more
 usually looks like this:
@@ -57,15 +105,15 @@
         def startup_shutdown(self):
             with open_the_database() as db:
                 self._db = db
                 yield
 
 Why not just write a plain context manager class? Because in
 multithreaded or async code one wants to keep the instance
-"open" while any thread is still using it.
+\"open\" while any thread is still using it.
 This mixin lets threads use an instance in overlapping fashion:
 
     db_thing = DatabaseThing(...)
     with db_thing:
         ... kick off threads with access to the db ...
     ...
     thread 1:
@@ -76,14 +124,18 @@
        ... use db_thing ...
 
 TODO:
 * `subopens`: if true (default false) then `.open` will return
   a proxy object with its own `.closed` attribute set by the
   proxy's `.close`.
 
+*Property `MultiOpenMixin.MultiOpenMixin_state`*:
+The state object for the mixin,
+something of a hack to avoid providing an `__init__`.
+
 *Method `MultiOpenMixin.close(self, *, enforce_final_close=False, caller_frame=None, unopened_ok=False)`*:
 Decrement the open count.
 If the count goes to zero, call `self.shutdown()` and return its value.
 
 Parameters:
 * `enforce_final_close`: if true, the caller expects this to
   be the final close for the object and a `RuntimeError` is
@@ -182,15 +234,15 @@
     If omitted or `None`, defaults to 4.
     If 0, no upper limit is applied.
 * `lock`: optional shared Lock; if omitted or `None` a new Lock is allocated
 
 *Method `Pool.instance(self)`*:
 Context manager returning an object for use, which is returned to the pool afterwards.
 
-## Class `RunState(cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+## Class `RunState(cs.threads.HasThreadState)`
 
 A class to track a running task whose cancellation may be requested.
 
 Its purpose is twofold, to provide easily queriable state
 around tasks which can start and stop, and to provide control
 methods to pronounce that a task has started (`.start`),
 should stop (`.cancel`)
@@ -246,15 +298,15 @@
 * stop
 
 Note that if the `RunState` is already runnings we do not
 do any of that stuff apart from the `yield self` because
 we assume whatever setup should have been done has already
 been done.
 In particular, the `HasThreadState.Thread` factory calls this
-in the "running" state.
+in the \"running\" state.
 
 *Method `RunState.__nonzero__(self)`*:
 Return true if the task is running.
 
 *Method `RunState.cancel(self)`*:
 Set the cancelled flag; the associated process should notice and stop.
 
@@ -276,18 +328,23 @@
 Stop: adjust state, set `stop_time` to now.
 Sets sets `.running` to `False`.
 
 *Method `RunState.handle_signal(self, sig, _)`*:
 `RunState` signal handler: cancel the run state.
 Warn if `self.verbose`.
 
+*Method `RunState.iter(self, it)`*:
+Iterate over `it` while not `self.cancelled`.
+
 *`RunState.perthread_state`*
 
 *Method `RunState.raiseif(self, msg=None, *a)`*:
-Raise `CancellationError` is cancelled.
+Raise `CancellationError` if cancelled.
+This is the concise way to terminate an operation which honour
+`.cancelled` if you're prepared to handle the exception.
 
 Example:
 
     for item in items:
         runstate.raiseif()
         ... process item ...
 
@@ -315,15 +372,15 @@
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType])`*:
+*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x104ae5d80>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -342,14 +399,20 @@
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
 # Release Log
 
 
 
+*Release 20240412*:
+* RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
+* RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
+* MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
+* RunState.__init__: make most parameters keyword only.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
 MultiOpenMixin: new .is_open() method to test for opens > 0.
 
 *Release 20231221*:
@@ -398,15 +461,15 @@
 * MultiOpenMixin.startup_shutdown: fix up shutdown logic, was not using a finally clause.
 * MultiOpenMixin: use ContextManagerMixin __enter_exit__ generator method instead of __enter__ and __exit__.
 
 *Release 20210906*:
 MultiOpenMixin: make startup and shutdown optional.
 
 *Release 20210731*:
-RunState: tune the sanity checks around whether the state is "running".
+RunState: tune the sanity checks around whether the state is \"running\".
 
 *Release 20210420*:
 MultiOpenMixin: run startup/shutdown entirely via the new default method @contextmanager(startup_shutdown), paving the way for subclasses to just define their own startup_shutdown context manager methods instead of distinct startup/shutdown methods.
 
 *Release 20201025*:
 MultiOpenMixin.__mo_getstate: dereference self.__dict__ because using AttributeError was pulling a state object from another instance, utterly weird.
 
@@ -432,16 +495,33 @@
 * RunState improvements.
 
 *Release 20171024*:
 * bugfix MultiOpenMixin finalise logic and other small logic fixes and checs
 * new class RunState for tracking or controlling a running task
 
 *Release 20160828*:
-Use "install_requires" instead of "requires" in DISTINFO.
+Use \"install_requires\" instead of \"requires\" in DISTINFO.
 
 *Release 20160827*:
 * BREAKING CHANGE: rename NestingOpenCloseMixin to MultiOpenMixin.
 * New Pool class for generic object reuse.
 * Assorted minor improvements.
 
 *Release 20150115*:
-First PyPI release.
+First PyPI release."""
+content-type = "text/markdown"
+
+[build-system]
+build-backend = "setuptools.build_meta"
+requires = [
+    "setuptools >= 61.2",
+    "trove-classifiers",
+    "wheel",
+]
+
+[tool.setuptools]
+py-modules = [
+    "cs.resources",
+]
+
+[tool.setuptools.package-dir]
+"" = "lib/python"
```

### Comparing `cs.resources-20240316/lib/python/cs/resources.py` & `cs.resources-20240412/lib/python/cs/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,33 +5,34 @@
 #
 
 ''' Resource management classes and functions.
 '''
 
 from collections import defaultdict
 from contextlib import contextmanager
-import sys
-from threading import Condition, Lock, RLock, current_thread, main_thread
+from dataclasses import dataclass, field
+from functools import partial
+from threading import Lock, current_thread, main_thread
 import time
-from typing import Any, Callable, Optional, Tuple, Union
+from typing import Any, Callable, Mapping, Optional, Tuple, Union
 
 from typeguard import typechecked
 
-from cs.context import stackattrs, setup_cmgr, ContextManagerMixin
+from cs.context import contextif, stackattrs, setup_cmgr, ContextManagerMixin
 from cs.deco import default_params
 from cs.gimmicks import error, warning, nullcontext
 from cs.obj import Proxy
 from cs.pfx import pfx_call, pfx_method
 from cs.psutils import signal_handlers
 from cs.py.func import prop
-from cs.py.stack import caller, frames as stack_frames, stack_dump
+from cs.py.stack import caller, frames as stack_frames, stack_dump, StackSummary
 from cs.result import CancellationError
-from cs.threads import ThreadState, HasThreadState
+from cs.threads import ThreadState, HasThreadState, NRLock
 
-__version__ = '20240316'
+__version__ = '20240412'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -68,61 +69,59 @@
       )
     return func(self, *a, **kw)
 
   not_closed_wrapper.__name__ = "not_closed_wrapper(%s)" % (func.__name__,)
   return not_closed_wrapper
 
 # pylint: disable=too-few-public-methods,too-many-instance-attributes
-class _mom_state(object):
+@dataclass(slots=True)
+class _MultiOpenMixinOpenCloseState:
 
-  def __init__(self, mom: "MultiOpenMixin"):
-    self.mom = mom
-    self.opened = False
-    self.opens = 0
-    self.opens_from = defaultdict(int)
-    ##self.closed = False # final _close() not yet called
-    self.final_close_from = None
-    self._lock = RLock()
-    self.join_lock = None
-
-  def __repr__(self):
-    return "%s:%r" % (self.__class__.__name__, self.__dict__)
+  mom: "MultiOpenMixin"
+  opened: bool = False
+  opens: int = 0
+  opens_from: Mapping = field(default_factory=lambda: defaultdict(int))
+  final_close_from: StackSummary = None
+  join_lock: Lock = None
+  _teardown: Callable = None
+  _lock: NRLock = field(default_factory=NRLock)
 
   def open(self, caller_frame=None) -> int:
     ''' The open process:
         Bump the opens counter.
         If it goes to 1, run the startup phase of `self.mom.startup_shutdown`.
-        Return the bumped opens counter.
+        Return the incremented opens counter.
     '''
     with self._lock:
       opens = self.opens
       opens += 1
       self.opens = opens
       if caller_frame is not None:
         frame_key = caller_frame.filename, caller_frame.lineno
         self.opens_from[frame_key] += 1
       if opens == 1:
         self.join_lock = Lock()
         self.join_lock.acquire()
         self._teardown = setup_cmgr(self.mom.startup_shutdown())
-      self.opened = True
+        self.opened = True
     return opens
 
   def close(
       self,
       *,
       caller_frame=None,
       enforce_final_close=False,
       unopened_ok=False,
   ) -> Tuple[int, Any]:
     ''' The close process:
         Decrement the opens counter.
         If it goes to 0, run the shutdown phase of `self.mom.startup_shutdown`.
-        Return the bumped opens counter and the return value of the shutdown phase
-        (or `None` if the shutdown was not run).
+        Return a 2-tuple `(opens,retval)` being:
+        - the decremented opens counter
+        - the return value of the shutdown phase or `None` if the shutdown was not run
     '''
     if not self.opened:
       if unopened_ok:
         return None
       raise RuntimeError("%s: close before initial open" % (self,))
     retval = None
     with self._lock:
@@ -131,15 +130,15 @@
         error("%s: UNDERFLOW CLOSE from %s", self, caller())
         error("  final close was from %s", self.final_close_from)
         for frame_key in sorted(self.opens_from.keys()):
           error(
               "  opened from %s %d times", frame_key,
               self.opens_from[frame_key]
           )
-        return retval
+        return opens, retval
       opens -= 1
       self.opens = opens
       if opens == 0:
         ##INACTIVE##self.tcm_dump(MultiOpenMixin)
         self.final_close_from = caller_frame
         teardown, self._teardown = self._teardown, None
         retval = teardown()
@@ -167,30 +166,33 @@
 class MultiOpenMixin(ContextManagerMixin):
   ''' A multithread safe mixin to count open and close calls,
       doing a startup on the first `.open` and shutdown on the last `.close`.
 
       If used as a context manager this mixin calls `open()`/`close()` from
       `__enter__()` and `__exit__()`.
 
-      It is recommended subclass implementations do as little as possible
-      during `__init__`, and do almost all setup during startup so
-      that the class may perform multiple startup/shutdown iterations.
+      It is recommended that subclass implementations do as little
+      as possible during `__init__`, and do almost all setup during
+      startup so that the class may perform multiple startup/shutdown
+      iterations.
 
       Classes using this mixin should define a context manager
       method `.startup_shutdown` which does the startup actions
       before yielding and then does the shutdown actions.
 
       Example:
 
           class DatabaseThing(MultiOpenMixin):
               @contextmanager
               def startup_shutdown(self):
                   self._db = open_the_database()
-                  yield
-                  self._db.close()
+                  try:
+                      yield
+                  finally:
+                      self._db.close()
           ...
           with DatabaseThing(...) as db_thing:
               ... use db_thing ...
 
       If course, often something like a database open will itself
       be a context manager and the `startup_shutdown` method more
       usually looks like this:
@@ -219,39 +221,46 @@
 
       TODO:
       * `subopens`: if true (default false) then `.open` will return
         a proxy object with its own `.closed` attribute set by the
         proxy's `.close`.
   '''
 
-  def __mo_getstate(self):
-    ''' Fetch the state object for the mixin,
-        something of a hack to avoid providing an __init__.
+  _mom_state_lock = Lock()
+
+  @property
+  def MultiOpenMixin_state(self):
+    ''' The state object for the mixin,
+        something of a hack to avoid providing an `__init__`.
     '''
-    # used to be self.__mo_state and catch AttributeError, but
-    # something up the MRO weirds this - suspect the ABC base class
     try:
-      state = self.__dict__['_MultiOpenMixin_state']
+      # the fast path
+      return self.__dict__['_MultiOpenMixin_state']
     except KeyError:
-      state = self.__dict__['_MultiOpenMixin_state'] = _mom_state(self)
-      assert state.opens == 0
-    return state
+      # pylint: disable=protected-access
+      with self.__class__._mom_state_lock:
+        try:
+          state = self.__dict__['_MultiOpenMixin_state']
+        except KeyError:
+          state = self.__dict__['_MultiOpenMixin_state'
+                                ] = _MultiOpenMixinOpenCloseState(self)
+      return state
 
   def tcm_get_state(self):
     ''' Support method for `TrackedClassMixin`.
     '''
-    state = self.__mo_getstate()
+    state = self.MultiOpenMixin_state
     return {'opened': state.opened, 'opens': state.opens}
 
   def __enter_exit__(self):
-    self.open(caller_frame=caller())
+    self.open()
     try:
       yield
     finally:
-      self.close()  ##caller_frame=caller())
+      self.close()
 
   @contextmanager
   def startup_shutdown(self):
     ''' Default context manager form of startup/shutdown - just
         call the distinct `.startup()` and `.shutdown()` methods
         if both are present, do nothing if neither is present.
 
@@ -291,16 +300,16 @@
       if shutdown is not None:
         shutdown()
 
   def open(self, caller_frame=None):
     ''' Increment the open count.
         On the first `.open` call `self.startup()`.
     '''
-    state = self.__mo_getstate()
-    if False:
+    state = self.MultiOpenMixin_state
+    if False:  # pylint: disable=using-constant-test
       if caller_frame is None:
         caller_frame = caller()
       frame_key = caller_frame.filename, caller_frame.lineno
       state.opens_from[frame_key] = state.opens_from.get(frame_key, 0) + 1
     state.open(caller_frame=caller_frame)
     return self
 
@@ -323,33 +332,33 @@
           `cs.py.stack.caller` when needed. Presently the caller of the
           final close is recorded to help debugging extra close calls.
         * `unopened_ok`: if true, it is not an error if this is not open.
           This is intended for closing callbacks which might get called
           even if the original open never happened.
           (I'm looking at you, `cs.resources.RunState`.)
     '''
-    state = self.__mo_getstate()
-    if False:
+    state = self.MultiOpenMixin_state
+    if False:  # pylint: disable=using-constant-test
       if caller_frame is None:
         caller_frame = caller()
       frame_key = caller_frame.filename, caller_frame.lineno
       state.opens_from[frame_key] = state.opens_from.get(frame_key, 0) + 1
-    opens, retval = state.close(
+    _, retval = state.close(
         caller_frame=caller_frame,
         enforce_final_close=enforce_final_close,
         unopened_ok=unopened_ok,
     )
     return retval
 
   @property
   def closed(self):
     ''' Whether this object has been closed.
         Note: False if never opened.
     '''
-    state = self.__mo_getstate()
+    state = self.MultiOpenMixin_state
     if state.opens > 0:
       return False
     ##if state.opens < 0:
     ##  raise RuntimeError("OPENS UNDERFLOW: opens < 0: %r" % (state.opens,))
     if not state.opened:
       # never opened, so not totally closed
       return False
@@ -358,20 +367,20 @@
   def join(self):
     ''' Join this object.
 
         Wait for the internal finalise `Condition` (if still not `None`).
         Normally this is notified at the end of the shutdown procedure
         unless the object's `finalise_later` parameter was true.
     '''
-    self.__mo_getstate().join()
+    self.MultiOpenMixin_state.join()
 
   def is_open(self):
     ''' Test whether this object is open.
     '''
-    return self.__mo_getstate().opens > 0
+    return self.MultiOpenMixin_state.opens > 0
 
   @staticmethod
   def is_opened(func):
     ''' Decorator to wrap `MultiOpenMixin` proxy object methods which
         should raise if the object is not yet open.
     '''
 
@@ -554,21 +563,24 @@
   '''
 
   perthread_state = ThreadState()
 
   def __init__(
       self,
       name=None,
+      *,
       signals=None,
       handle_signal=None,
       poll_cancel: Optional[Callable] = None,
       verbose=False,
+      thread_wide=False,
   ):
     self.name = name
     self.verbose = verbose
+    self.thread_wide = thread_wide
     self._started_from = None
     self._signals = tuple(signals) if signals else ()
     self._sigstack = None
     self._sighandler = handle_signal or self.handle_signal
     # core state
     self._running = False
     self._cancelled = False
@@ -610,15 +622,15 @@
         Note that if the `RunState` is already runnings we do not
         do any of that stuff apart from the `yield self` because
         we assume whatever setup should have been done has already
         been done.
         In particular, the `HasThreadState.Thread` factory calls this
         in the "running" state.
     '''
-    with HasThreadState.as_contextmanager(self):
+    with contextif(self.thread_wide, HasThreadState.as_contextmanager, self):
       if self.running:
         # we're already running - do not change states or push signal handlers
         # typical situation is HasThreadState.Thread setting up the "current" RunState
         yield self
       else:
         # if we're not in the main thread we suppress the signal shuffling as well
         in_main = current_thread() is main_thread()
@@ -664,16 +676,14 @@
   @pfx_method
   def start(self, running_ok=False):
     ''' Start: adjust state, set `start_time` to now.
         Sets `.cancelled` to `False` and sets `.running` to `True`.
     '''
     if not running_ok and self.running:
       warning("already running")
-      print("runstate.start(): originally started from:", file=sys.stderr)
-      stack_dump(Fs=self._started_from)
     else:
       self._started_from = stack_frames()
     self.cancelled = False
     self.running = True
 
   def stop(self):
     ''' Stop: adjust state, set `stop_time` to now.
@@ -699,15 +709,17 @@
   @cancelled.setter
   def cancelled(self, cancel_status):
     ''' Set the .cancelled attribute.
     '''
     self._cancelled = cancel_status
 
   def raiseif(self, msg=None, *a):
-    ''' Raise `CancellationError` is cancelled.
+    ''' Raise `CancellationError` if cancelled.
+        This is the concise way to terminate an operation which honour
+        `.cancelled` if you're prepared to handle the exception.
 
         Example:
 
             for item in items:
                 runstate.raiseif()
                 ... process item ...
     '''
@@ -777,14 +789,26 @@
       return 0.0
     if self.running:
       stop_time = time.time()
     else:
       stop_time = self.stop_time
     return max(0, stop_time - start_time)
 
+  def iter(self, it):
+    ''' Iterate over `it` while not `self.cancelled`.
+    '''
+    it = iter(it)
+    while True:
+      if self.cancelled:
+        return
+      try:
+        yield next(it)
+      except StopIteration:
+        return
+
   @contextmanager
   def catch_signal(
       self,
       sig,
       call_previous=False,
       handle_signal=None,
   ):
@@ -811,37 +835,37 @@
         Warn if `self.verbose`.
       '''
     # pylint: disable=expression-not-assigned
     if self.verbose:
       warning("%s: received signal %s, cancelling", self, sig)
     self.cancel()
 
-# use the prevailing RunState or make a fresh one
+# default to the current RunState or make one
 uses_runstate = default_params(
-    runstate=lambda: RunState.default() or RunState()
+    runstate=lambda:
+    (RunState.default(factory=partial(RunState, thread_wide=True)))
 )
 
 class RunStateMixin(object):
   ''' Mixin to provide convenient access to a `RunState`.
 
       Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
   '''
 
+  @uses_runstate
   @typechecked
-  def __init__(self, runstate: Optional[Union[RunState, str]]):
+  def __init__(self, runstate: Union[RunState, str]):
     ''' Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
         Parameters:
         * `runstate`: optional `RunState` instance or name.
           If a `str`, a new `RunState` with that name is allocated.
           If omitted, the default `RunState` is used.
     '''
-    if runstate is None:
-      runstate = RunState(runstate)
-    elif isinstance(runstate, str):
+    if isinstance(runstate, str):
       runstate = RunState(runstate)
     self.runstate = runstate
 
   def cancel(self):
     ''' Call .runstate.cancel().
     '''
     return self.runstate.cancel()
```

### Comparing `cs.resources-20240316/lib/python/cs.resources.egg-info/PKG-INFO` & `cs.resources-20240412/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.resources
-Version: 20240316
+Version: 20240412
 Summary: Resource management classes and functions.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,53 +14,65 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Resource management classes and functions.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+* RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
+* RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
+* MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
+* RunState.__init__: make most parameters keyword only.
 
-## Class `ClosedError(builtins.Exception, builtins.BaseException)`
+## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
-## Class `MultiOpen(MultiOpenMixin, cs.context.ContextManagerMixin)`
+## Class `MultiOpen(MultiOpenMixin)`
 
 Context manager class that manages a single open/close object
 using a MultiOpenMixin.
 
 *Method `MultiOpen.__init__(self, openable, finalise_later=False)`*:
 Initialise: save the `openable` and call the MultiOpenMixin initialiser.
 
+*Method `MultiOpen.shutdown(self)`*:
+Close the associated openable object.
+
+*Method `MultiOpen.startup(self)`*:
+Open the associated openable object.
+
 ## Class `MultiOpenMixin(cs.context.ContextManagerMixin)`
 
 A multithread safe mixin to count open and close calls,
 doing a startup on the first `.open` and shutdown on the last `.close`.
 
 If used as a context manager this mixin calls `open()`/`close()` from
 `__enter__()` and `__exit__()`.
 
-It is recommended subclass implementations do as little as possible
-during `__init__`, and do almost all setup during startup so
-that the class may perform multiple startup/shutdown iterations.
+It is recommended that subclass implementations do as little
+as possible during `__init__`, and do almost all setup during
+startup so that the class may perform multiple startup/shutdown
+iterations.
 
 Classes using this mixin should define a context manager
 method `.startup_shutdown` which does the startup actions
 before yielding and then does the shutdown actions.
 
 Example:
 
     class DatabaseThing(MultiOpenMixin):
         @contextmanager
         def startup_shutdown(self):
             self._db = open_the_database()
-            yield
-            self._db.close()
+            try:
+                yield
+            finally:
+                self._db.close()
     ...
     with DatabaseThing(...) as db_thing:
         ... use db_thing ...
 
 If course, often something like a database open will itself
 be a context manager and the `startup_shutdown` method more
 usually looks like this:
@@ -88,14 +100,88 @@
        ... use db_thing ...
 
 TODO:
 * `subopens`: if true (default false) then `.open` will return
   a proxy object with its own `.closed` attribute set by the
   proxy's `.close`.
 
+*Property `MultiOpenMixin.MultiOpenMixin_state`*:
+The state object for the mixin,
+something of a hack to avoid providing an `__init__`.
+
+*Method `MultiOpenMixin.close(self, *, enforce_final_close=False, caller_frame=None, unopened_ok=False)`*:
+Decrement the open count.
+If the count goes to zero, call `self.shutdown()` and return its value.
+
+Parameters:
+* `enforce_final_close`: if true, the caller expects this to
+  be the final close for the object and a `RuntimeError` is
+  raised if this is not actually the case.
+* `caller_frame`: used for debugging; the caller may specify
+  this if necessary, otherwise it is computed from
+  `cs.py.stack.caller` when needed. Presently the caller of the
+  final close is recorded to help debugging extra close calls.
+* `unopened_ok`: if true, it is not an error if this is not open.
+  This is intended for closing callbacks which might get called
+  even if the original open never happened.
+  (I'm looking at you, `cs.resources.RunState`.)
+
+*Property `MultiOpenMixin.closed`*:
+Whether this object has been closed.
+Note: False if never opened.
+
+*Method `MultiOpenMixin.is_open(self)`*:
+Test whether this object is open.
+
+*Method `MultiOpenMixin.is_opened(func)`*:
+Decorator to wrap `MultiOpenMixin` proxy object methods which
+should raise if the object is not yet open.
+
+*Method `MultiOpenMixin.join(self)`*:
+Join this object.
+
+Wait for the internal finalise `Condition` (if still not `None`).
+Normally this is notified at the end of the shutdown procedure
+unless the object's `finalise_later` parameter was true.
+
+*Method `MultiOpenMixin.open(self, caller_frame=None)`*:
+Increment the open count.
+On the first `.open` call `self.startup()`.
+
+*Method `MultiOpenMixin.startup_shutdown(self)`*:
+Default context manager form of startup/shutdown - just
+call the distinct `.startup()` and `.shutdown()` methods
+if both are present, do nothing if neither is present.
+
+This supports subclasses always using:
+
+    with super().startup_shutdown():
+
+as an outer wrapper.
+
+The `.startup` check is to support legacy subclasses of
+`MultiOpenMixin` which have separate `startup()` and
+`shutdown()` methods.
+The preferred approach is a single `startup_shutdwn()`
+context manager overriding this method.
+
+The usual form looks like this:
+
+    @contextmanager
+    def startup_shutdown(self):
+        with super().startup_shutdown():
+            ... do some set up ...
+            try:
+                yield
+            finally:
+                ... do some tear down ...
+
+*Method `MultiOpenMixin.tcm_get_state(self)`*:
+Support method for `TrackedClassMixin`.
+
 ## Function `not_closed(func)`
 
 Decorator to wrap methods of objects with a .closed property
 which should raise when self.closed.
 
 ## Function `openif(obj)`
 
@@ -121,15 +207,18 @@
 Parameters:
 * `new_object` is a callable which returns a new object for the Pool.
 * `max_size`: The maximum size of the pool of available objects saved for reuse.
     If omitted or `None`, defaults to 4.
     If 0, no upper limit is applied.
 * `lock`: optional shared Lock; if omitted or `None` a new Lock is allocated
 
-## Class `RunState(cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+*Method `Pool.instance(self)`*:
+Context manager returning an object for use, which is returned to the pool afterwards.
+
+## Class `RunState(cs.threads.HasThreadState)`
 
 A class to track a running task whose cancellation may be requested.
 
 Its purpose is twofold, to provide easily queriable state
 around tasks which can start and stop, and to provide control
 methods to pronounce that a task has started (`.start`),
 should stop (`.cancel`)
@@ -168,32 +257,138 @@
 * `notify_start`: a set of callables called with the `RunState` instance
   to be called whenever `.running` becomes true.
 * `notify_end`: a set of callables called with the `RunState` instance
   to be called whenever `.running` becomes false.
 * `notify_cancel`: a set of callables called with the `RunState` instance
   to be called whenever `.cancel` is called.
 
+*Method `RunState.__bool__(self)`*:
+Return true if the task is running.
+
+*Method `RunState.__enter_exit__(self)`*:
+The `__enter__`/`__exit__` generator function:
+* push this RunState via HasThreadState
+* catch signals
+* start
+* `yield self` => run
+* cancel on exception during run
+* stop
+
+Note that if the `RunState` is already runnings we do not
+do any of that stuff apart from the `yield self` because
+we assume whatever setup should have been done has already
+been done.
+In particular, the `HasThreadState.Thread` factory calls this
+in the "running" state.
+
+*Method `RunState.__nonzero__(self)`*:
+Return true if the task is running.
+
+*Method `RunState.cancel(self)`*:
+Set the cancelled flag; the associated process should notice and stop.
+
+*Property `RunState.cancelled`*:
+Test the .cancelled attribute, including a poll if supplied.
+
+*Method `RunState.catch_signal(self, sig, call_previous=False, handle_signal=None)`*:
+Context manager to catch the signal or signals `sig` and
+cancel this `RunState`.
+Restores the previous handlers on exit.
+Yield a mapping of `sig`=>`old_handler`.
+
+Parameters:
+* `sig`: an `int` signal number or an iterable of signal numbers
+* `call_previous`: optional flag (default `False`)
+  passed to `cs.psutils.signal_handlers`
+
+*Method `RunState.end(self)`*:
+Stop: adjust state, set `stop_time` to now.
+Sets sets `.running` to `False`.
+
+*Method `RunState.handle_signal(self, sig, _)`*:
+`RunState` signal handler: cancel the run state.
+Warn if `self.verbose`.
+
+*Method `RunState.iter(self, it)`*:
+Iterate over `it` while not `self.cancelled`.
+
+*`RunState.perthread_state`*
+
+*Method `RunState.raiseif(self, msg=None, *a)`*:
+Raise `CancellationError` if cancelled.
+This is the concise way to terminate an operation which honour
+`.cancelled` if you're prepared to handle the exception.
+
+Example:
+
+    for item in items:
+        runstate.raiseif()
+        ... process item ...
+
+*Property `RunState.run_time`*:
+Property returning most recent run time (`stop_time-start_time`).
+If still running, use now as the stop time.
+If not started, return `0.0`.
+
+*Property `RunState.running`*:
+Property expressing whether the task is running.
+
+*Method `RunState.start(self, running_ok=False)`*:
+Start: adjust state, set `start_time` to now.
+Sets `.cancelled` to `False` and sets `.running` to `True`.
+
+*Method `RunState.stop(self)`*:
+Stop: adjust state, set `stop_time` to now.
+Sets sets `.running` to `False`.
+
+*Property `RunState.stopped`*:
+Was the process stopped? Running is false and cancelled is true.
+
+*Property `RunState.stopping`*:
+Is the process stopping? Running is true and cancelled is true.
+
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType])`*:
+*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x104ae5d80>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
+*Method `RunStateMixin.cancel(self)`*:
+Call .runstate.cancel().
+
+*Property `RunStateMixin.cancelled`*:
+Test .runstate.cancelled.
+
+*Property `RunStateMixin.running`*:
+Test .runstate.running.
+
+*Property `RunStateMixin.stopped`*:
+Test .runstate.stopped.
+
+*Property `RunStateMixin.stopping`*:
+Test .runstate.stopping.
+
 # Release Log
 
 
 
+*Release 20240412*:
+* RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
+* RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
+* MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
+* RunState.__init__: make most parameters keyword only.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
 MultiOpenMixin: new .is_open() method to test for opens > 0.
 
 *Release 20231221*:
```

### Comparing `cs.resources-20240316/pyproject.toml` & `cs.resources-20240412/lib/python/cs.resources.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,78 @@
-[project]
-name = "cs.resources"
-description = "Resource management classes and functions."
-authors = [
-    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
-]
-keywords = [
-    "python2",
-    "python3",
-]
-dependencies = [
-    "cs.context>=20240212.1",
-    "cs.deco>=20240316",
-    "cs.gimmicks>=20240316",
-    "cs.obj>=20220918",
-    "cs.pfx>=20230604",
-    "cs.psutils>=20240211",
-    "cs.py.func>=20230331",
-    "cs.py.stack>=20220918",
-    "cs.result>=20240305",
-    "cs.threads>=20240303",
-    "typeguard",
-]
-classifiers = [
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "Operating System :: OS Independent",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-]
-version = "20240316"
+Metadata-Version: 2.1
+Name: cs.resources
+Version: 20240412
+Summary: Resource management classes and functions.
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python2,python3
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
 
-[project.license]
-text = "GNU General Public License v3 or later (GPLv3+)"
-
-[project.urls]
-URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
-
-[project.readme]
-text = """
 Resource management classes and functions.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+* RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
+* RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
+* MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
+* RunState.__init__: make most parameters keyword only.
 
-## Class `ClosedError(builtins.Exception, builtins.BaseException)`
+## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
-## Class `MultiOpen(MultiOpenMixin, cs.context.ContextManagerMixin)`
+## Class `MultiOpen(MultiOpenMixin)`
 
 Context manager class that manages a single open/close object
 using a MultiOpenMixin.
 
 *Method `MultiOpen.__init__(self, openable, finalise_later=False)`*:
 Initialise: save the `openable` and call the MultiOpenMixin initialiser.
 
+*Method `MultiOpen.shutdown(self)`*:
+Close the associated openable object.
+
+*Method `MultiOpen.startup(self)`*:
+Open the associated openable object.
+
 ## Class `MultiOpenMixin(cs.context.ContextManagerMixin)`
 
 A multithread safe mixin to count open and close calls,
 doing a startup on the first `.open` and shutdown on the last `.close`.
 
 If used as a context manager this mixin calls `open()`/`close()` from
 `__enter__()` and `__exit__()`.
 
-It is recommended subclass implementations do as little as possible
-during `__init__`, and do almost all setup during startup so
-that the class may perform multiple startup/shutdown iterations.
+It is recommended that subclass implementations do as little
+as possible during `__init__`, and do almost all setup during
+startup so that the class may perform multiple startup/shutdown
+iterations.
 
 Classes using this mixin should define a context manager
 method `.startup_shutdown` which does the startup actions
 before yielding and then does the shutdown actions.
 
 Example:
 
     class DatabaseThing(MultiOpenMixin):
         @contextmanager
         def startup_shutdown(self):
             self._db = open_the_database()
-            yield
-            self._db.close()
+            try:
+                yield
+            finally:
+                self._db.close()
     ...
     with DatabaseThing(...) as db_thing:
         ... use db_thing ...
 
 If course, often something like a database open will itself
 be a context manager and the `startup_shutdown` method more
 usually looks like this:
@@ -93,15 +81,15 @@
         def startup_shutdown(self):
             with open_the_database() as db:
                 self._db = db
                 yield
 
 Why not just write a plain context manager class? Because in
 multithreaded or async code one wants to keep the instance
-\"open\" while any thread is still using it.
+"open" while any thread is still using it.
 This mixin lets threads use an instance in overlapping fashion:
 
     db_thing = DatabaseThing(...)
     with db_thing:
         ... kick off threads with access to the db ...
     ...
     thread 1:
@@ -112,14 +100,88 @@
        ... use db_thing ...
 
 TODO:
 * `subopens`: if true (default false) then `.open` will return
   a proxy object with its own `.closed` attribute set by the
   proxy's `.close`.
 
+*Property `MultiOpenMixin.MultiOpenMixin_state`*:
+The state object for the mixin,
+something of a hack to avoid providing an `__init__`.
+
+*Method `MultiOpenMixin.close(self, *, enforce_final_close=False, caller_frame=None, unopened_ok=False)`*:
+Decrement the open count.
+If the count goes to zero, call `self.shutdown()` and return its value.
+
+Parameters:
+* `enforce_final_close`: if true, the caller expects this to
+  be the final close for the object and a `RuntimeError` is
+  raised if this is not actually the case.
+* `caller_frame`: used for debugging; the caller may specify
+  this if necessary, otherwise it is computed from
+  `cs.py.stack.caller` when needed. Presently the caller of the
+  final close is recorded to help debugging extra close calls.
+* `unopened_ok`: if true, it is not an error if this is not open.
+  This is intended for closing callbacks which might get called
+  even if the original open never happened.
+  (I'm looking at you, `cs.resources.RunState`.)
+
+*Property `MultiOpenMixin.closed`*:
+Whether this object has been closed.
+Note: False if never opened.
+
+*Method `MultiOpenMixin.is_open(self)`*:
+Test whether this object is open.
+
+*Method `MultiOpenMixin.is_opened(func)`*:
+Decorator to wrap `MultiOpenMixin` proxy object methods which
+should raise if the object is not yet open.
+
+*Method `MultiOpenMixin.join(self)`*:
+Join this object.
+
+Wait for the internal finalise `Condition` (if still not `None`).
+Normally this is notified at the end of the shutdown procedure
+unless the object's `finalise_later` parameter was true.
+
+*Method `MultiOpenMixin.open(self, caller_frame=None)`*:
+Increment the open count.
+On the first `.open` call `self.startup()`.
+
+*Method `MultiOpenMixin.startup_shutdown(self)`*:
+Default context manager form of startup/shutdown - just
+call the distinct `.startup()` and `.shutdown()` methods
+if both are present, do nothing if neither is present.
+
+This supports subclasses always using:
+
+    with super().startup_shutdown():
+
+as an outer wrapper.
+
+The `.startup` check is to support legacy subclasses of
+`MultiOpenMixin` which have separate `startup()` and
+`shutdown()` methods.
+The preferred approach is a single `startup_shutdwn()`
+context manager overriding this method.
+
+The usual form looks like this:
+
+    @contextmanager
+    def startup_shutdown(self):
+        with super().startup_shutdown():
+            ... do some set up ...
+            try:
+                yield
+            finally:
+                ... do some tear down ...
+
+*Method `MultiOpenMixin.tcm_get_state(self)`*:
+Support method for `TrackedClassMixin`.
+
 ## Function `not_closed(func)`
 
 Decorator to wrap methods of objects with a .closed property
 which should raise when self.closed.
 
 ## Function `openif(obj)`
 
@@ -145,15 +207,18 @@
 Parameters:
 * `new_object` is a callable which returns a new object for the Pool.
 * `max_size`: The maximum size of the pool of available objects saved for reuse.
     If omitted or `None`, defaults to 4.
     If 0, no upper limit is applied.
 * `lock`: optional shared Lock; if omitted or `None` a new Lock is allocated
 
-## Class `RunState(cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+*Method `Pool.instance(self)`*:
+Context manager returning an object for use, which is returned to the pool afterwards.
+
+## Class `RunState(cs.threads.HasThreadState)`
 
 A class to track a running task whose cancellation may be requested.
 
 Its purpose is twofold, to provide easily queriable state
 around tasks which can start and stop, and to provide control
 methods to pronounce that a task has started (`.start`),
 should stop (`.cancel`)
@@ -192,32 +257,138 @@
 * `notify_start`: a set of callables called with the `RunState` instance
   to be called whenever `.running` becomes true.
 * `notify_end`: a set of callables called with the `RunState` instance
   to be called whenever `.running` becomes false.
 * `notify_cancel`: a set of callables called with the `RunState` instance
   to be called whenever `.cancel` is called.
 
+*Method `RunState.__bool__(self)`*:
+Return true if the task is running.
+
+*Method `RunState.__enter_exit__(self)`*:
+The `__enter__`/`__exit__` generator function:
+* push this RunState via HasThreadState
+* catch signals
+* start
+* `yield self` => run
+* cancel on exception during run
+* stop
+
+Note that if the `RunState` is already runnings we do not
+do any of that stuff apart from the `yield self` because
+we assume whatever setup should have been done has already
+been done.
+In particular, the `HasThreadState.Thread` factory calls this
+in the "running" state.
+
+*Method `RunState.__nonzero__(self)`*:
+Return true if the task is running.
+
+*Method `RunState.cancel(self)`*:
+Set the cancelled flag; the associated process should notice and stop.
+
+*Property `RunState.cancelled`*:
+Test the .cancelled attribute, including a poll if supplied.
+
+*Method `RunState.catch_signal(self, sig, call_previous=False, handle_signal=None)`*:
+Context manager to catch the signal or signals `sig` and
+cancel this `RunState`.
+Restores the previous handlers on exit.
+Yield a mapping of `sig`=>`old_handler`.
+
+Parameters:
+* `sig`: an `int` signal number or an iterable of signal numbers
+* `call_previous`: optional flag (default `False`)
+  passed to `cs.psutils.signal_handlers`
+
+*Method `RunState.end(self)`*:
+Stop: adjust state, set `stop_time` to now.
+Sets sets `.running` to `False`.
+
+*Method `RunState.handle_signal(self, sig, _)`*:
+`RunState` signal handler: cancel the run state.
+Warn if `self.verbose`.
+
+*Method `RunState.iter(self, it)`*:
+Iterate over `it` while not `self.cancelled`.
+
+*`RunState.perthread_state`*
+
+*Method `RunState.raiseif(self, msg=None, *a)`*:
+Raise `CancellationError` if cancelled.
+This is the concise way to terminate an operation which honour
+`.cancelled` if you're prepared to handle the exception.
+
+Example:
+
+    for item in items:
+        runstate.raiseif()
+        ... process item ...
+
+*Property `RunState.run_time`*:
+Property returning most recent run time (`stop_time-start_time`).
+If still running, use now as the stop time.
+If not started, return `0.0`.
+
+*Property `RunState.running`*:
+Property expressing whether the task is running.
+
+*Method `RunState.start(self, running_ok=False)`*:
+Start: adjust state, set `start_time` to now.
+Sets `.cancelled` to `False` and sets `.running` to `True`.
+
+*Method `RunState.stop(self)`*:
+Stop: adjust state, set `stop_time` to now.
+Sets sets `.running` to `False`.
+
+*Property `RunState.stopped`*:
+Was the process stopped? Running is false and cancelled is true.
+
+*Property `RunState.stopping`*:
+Is the process stopping? Running is true and cancelled is true.
+
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType])`*:
+*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x104ae5d80>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
+*Method `RunStateMixin.cancel(self)`*:
+Call .runstate.cancel().
+
+*Property `RunStateMixin.cancelled`*:
+Test .runstate.cancelled.
+
+*Property `RunStateMixin.running`*:
+Test .runstate.running.
+
+*Property `RunStateMixin.stopped`*:
+Test .runstate.stopped.
+
+*Property `RunStateMixin.stopping`*:
+Test .runstate.stopping.
+
 # Release Log
 
 
 
+*Release 20240412*:
+* RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
+* RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
+* MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
+* RunState.__init__: make most parameters keyword only.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
 MultiOpenMixin: new .is_open() method to test for opens > 0.
 
 *Release 20231221*:
@@ -266,15 +437,15 @@
 * MultiOpenMixin.startup_shutdown: fix up shutdown logic, was not using a finally clause.
 * MultiOpenMixin: use ContextManagerMixin __enter_exit__ generator method instead of __enter__ and __exit__.
 
 *Release 20210906*:
 MultiOpenMixin: make startup and shutdown optional.
 
 *Release 20210731*:
-RunState: tune the sanity checks around whether the state is \"running\".
+RunState: tune the sanity checks around whether the state is "running".
 
 *Release 20210420*:
 MultiOpenMixin: run startup/shutdown entirely via the new default method @contextmanager(startup_shutdown), paving the way for subclasses to just define their own startup_shutdown context manager methods instead of distinct startup/shutdown methods.
 
 *Release 20201025*:
 MultiOpenMixin.__mo_getstate: dereference self.__dict__ because using AttributeError was pulling a state object from another instance, utterly weird.
 
@@ -300,33 +471,17 @@
 * RunState improvements.
 
 *Release 20171024*:
 * bugfix MultiOpenMixin finalise logic and other small logic fixes and checs
 * new class RunState for tracking or controlling a running task
 
 *Release 20160828*:
-Use \"install_requires\" instead of \"requires\" in DISTINFO.
+Use "install_requires" instead of "requires" in DISTINFO.
 
 *Release 20160827*:
 * BREAKING CHANGE: rename NestingOpenCloseMixin to MultiOpenMixin.
 * New Pool class for generic object reuse.
 * Assorted minor improvements.
 
 *Release 20150115*:
-First PyPI release."""
-content-type = "text/markdown"
-
-[build-system]
-build-backend = "setuptools.build_meta"
-requires = [
-    "setuptools >= 61.2",
-    "trove-classifiers",
-    "wheel",
-]
-
-[tool.setuptools]
-py-modules = [
-    "cs.resources",
-]
+First PyPI release.
 
-[tool.setuptools.package-dir]
-"" = "lib/python"
```

