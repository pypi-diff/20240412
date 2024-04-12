# Comparing `tmp/cs.result-20240316.tar.gz` & `tmp/cs.result-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.result-20240316.tar", last modified: Sat Mar 16 07:06:14 2024, max compression
+gzip compressed data, was "cs.result-20240412.tar", last modified: Fri Apr 12 04:38:00 2024, max compression
```

## Comparing `cs.result-20240316.tar` & `cs.result-20240412.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:06:14.988539 cs.result-20240316/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-16 07:05:48.000000 cs.result-20240316/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     9584 2024-03-16 07:06:14.988231 cs.result-20240316/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    12684 2024-03-16 07:05:57.000000 cs.result-20240316/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:06:14.984718 cs.result-20240316/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:06:14.984984 cs.result-20240316/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:06:14.986212 cs.result-20240316/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    19139 2024-03-16 07:05:38.000000 cs.result-20240316/lib/python/cs/result.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:06:14.987816 cs.result-20240316/lib/python/cs.result.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     9584 2024-03-16 07:06:14.000000 cs.result-20240316/lib/python/cs.result.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      279 2024-03-16 07:06:14.000000 cs.result-20240316/lib/python/cs.result.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 07:06:14.000000 cs.result-20240316/lib/python/cs.result.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      182 2024-03-16 07:06:14.000000 cs.result-20240316/lib/python/cs.result.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 07:06:14.000000 cs.result-20240316/lib/python/cs.result.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    10155 2024-03-16 07:06:13.000000 cs.result-20240316/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 07:06:14.988625 cs.result-20240316/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:38:00.819628 cs.result-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 04:37:35.000000 cs.result-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    13666 2024-04-12 04:38:00.818812 cs.result-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    12873 2024-04-12 04:37:43.000000 cs.result-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:38:00.815886 cs.result-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:38:00.816108 cs.result-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:38:00.817081 cs.result-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    19485 2024-04-12 03:44:12.000000 cs.result-20240412/lib/python/cs/result.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:38:00.818448 cs.result-20240412/lib/python/cs.result.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    13666 2024-04-12 04:38:00.000000 cs.result-20240412/lib/python/cs.result.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      279 2024-04-12 04:38:00.000000 cs.result-20240412/lib/python/cs.result.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 04:38:00.000000 cs.result-20240412/lib/python/cs.result.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      182 2024-04-12 04:38:00.000000 cs.result-20240412/lib/python/cs.result.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 04:38:00.000000 cs.result-20240412/lib/python/cs.result.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    14246 2024-04-12 04:37:59.000000 cs.result-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 04:38:00.819714 cs.result-20240412/setup.cfg
```

### Comparing `cs.result-20240316/PKG-INFO` & `cs.result-20240412/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,11 @@
-Metadata-Version: 2.1
-Name: cs.result
-Version: 20240316
-Summary: Result and friends: various subclassable classes for deferred delivery of values.
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python2,python3
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
-
 Result and friends: various subclassable classes for deferred delivery of values.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+Result.bg: plumb _foo arguments to cs.threads.bg as foo.
 
 A `Result` is the base class for several callable subclasses
 which will receive values at a later point in time,
 and can also be used standalone without subclassing.
 
 A call to a `Result` will block until the value is received or the `Result` is cancelled,
 which will raise an exception in the caller.
@@ -89,15 +70,15 @@
 Other parameters are passed to `func`.
 
 ## Function `call_in_thread(func, *a, **kw)`
 
 Run `func(*a,**kw)` in a separate `Thread` via the `@in_thread` decorator.
 Return or exception is as for the original function.
 
-## Class `CancellationError(builtins.Exception, builtins.BaseException)`
+## Class `CancellationError(builtins.Exception)`
 
 Raised when accessing `result` or `exc_info` after cancellation.
 
 *Method `CancellationError.__init__(self, message=None, **kw)`*:
 Initialise the `CancellationError`.
 
 The optional `message` parameter (default `"cancelled"`)
@@ -109,31 +90,31 @@
 Decorator to evaluate `func` in a separate `Thread`.
 Return or exception is as for the original function.
 
 This exists to step out of the current `Thread's` thread
 local context, such as a database transaction associated
 with Django's implicit per-`Thread` database context.
 
-## Class `OnDemandFunction(Result, cs.fsm.FSM, cs.gvutils.DOTNodeMixin)`
+## Class `OnDemandFunction(Result)`
 
 Wrap a callable, run it when required.
 
-## Class `OnDemandResult(Result, cs.fsm.FSM, cs.gvutils.DOTNodeMixin)`
+## Class `OnDemandResult(Result)`
 
 Wrap a callable, run it when required.
 
 ## Function `report(LFs)`
 
 Generator which yields completed `Result`s.
 
 This is a generator that yields `Result`s as they complete,
 useful for waiting for a sequence of `Result`s
 that may complete in an arbitrary order.
 
-## Class `Result(cs.fsm.FSM, cs.gvutils.DOTNodeMixin)`
+## Class `Result(cs.fsm.FSM)`
 
 Base class for asynchronous collection of a result.
 This is used to make `Result`, `OnDemandFunction`s, `LateFunction`s
 and other objects with asynchronous termination.
 
 In addition to the methods below, for each state value such
 as `self.PENDING` there is a corresponding attribute `is_pending`
@@ -148,23 +129,154 @@
 * `result`: if not `None`, prefill the `.result` property.
 * `extra`: an optional mapping of extra information to
   associate with the `Result`, useful to provide context
   when collecting the result; the `Result` has a public
   attribute `.extra` which is an `AttrableMapping` to hold
   this information.
 
+*Method `Result.__call__(self, *a, **kw)`*:
+Call the `Result`: wait for it to be ready and then return or raise.
+
+You can optionally supply a callable and arguments,
+in which case `callable(*args,**kwargs)` will be called
+via `Result.call` and the results applied to this `Result`.
+
+Basic example:
+
+    R = Result()
+    ... hand R to something which will fulfil it later ...
+    x = R() # wait for fulfilment - value lands in x
+
+Direct call:
+
+    R = Result()
+    ... pass R to something which wants the result ...
+    # call func(1,2,z=3), save result in R
+    # ready for collection by whatever received R
+    R(func,1,2,z=3)
+
+*Method `Result.bg(self, func, *a, **kw)`*:
+Submit a function to compute the result in a separate `Thread`,
+returning the `Thread`.
+
+Keyword arguments for `cs.threads.bg` may be supplied by
+prefixing their names with an underscore, for example:
+
+    T = R.bg(mainloop, _pre_enter_objects=(S, fs))
+
+This dispatches a `Thread` to run `self.run_func(func,*a,**kw)`
+and as such the `Result` must be in "pending" state,
+and transitions to "running".
+
+*Method `Result.cancel(self)`*:
+Cancel this function.
+If `self.fsm_state` is `PENDING`` or `'CANCELLED'`, return `True`.
+Otherwise return `False` (too late to cancel).
+
+*Property `Result.cancelled`*:
+Test whether this `Result` has been cancelled.
+Obsolete: use `.is_cancelled`.
+
+*Method `Result.empty(self)`*:
+Analogue to `Queue.empty()`.
+
+*Property `Result.exc_info`*:
+The exception information from a completed `Result`.
+This is not available before completion.
+
+*Method `Result.get(self, default=None)`*:
+Wait for readiness; return the result if `self.exc_info` is `None`,
+otherwise `default`.
+
+*Method `Result.join(self)`*:
+Calling the `.join()` method waits for the function to run to
+completion and returns a tuple of `(result,exc_info)`.
+
+On completion the sequence `(result,None)` is returned.
+If an exception occurred computing the result the sequence
+`(None,exc_info)` is returned
+where `exc_info` is a tuple of `(exc_type,exc_value,exc_traceback)`.
+If the function was cancelled the sequence `(None,None)`
+is returned.
+
+*Method `Result.notify(self, notifier: Callable[[ForwardRef('Result')], NoneType])`*:
+After the `Result` completes, call `notifier(self)`.
+
+If the `Result` has already completed this will happen immediately.
+If you'd rather `self` got put on some queue `Q`, supply `Q.put`.
+
+*Property `Result.pending`*:
+Whether the `Result` is pending.
+Obsolete: use `.is_pending`.
+
+*Method `Result.post_notify(self, post_func) -> 'Result'`*:
+Return a secondary `Result` which processes the result of `self`.
+
+After the `self` completes, call `post_func(retval)` where
+`retval` is the result of `self`, and use that to complete
+the secondary `Result`.
+
+Example:
+
+    # submit packet to data stream
+    R = submit_packet()
+    # arrange that when the response is received, decode the response
+    R2 = R.post_notify(lambda response: decode(response))
+    # collect decoded response
+    decoded = R2()
+
+If the `Result` has already completed this will happen immediately.
+
+*Method `Result.put(self, value)`*:
+Store the value. `Queue`-like idiom.
+
+*Method `Result.raise_(self, exc=None)`*:
+Convenience wrapper for `self.exc_info` to store an exception result `exc`.
+If `exc` is omitted or `None`, uses `sys.exc_info()`.
+
+*Property `Result.ready`*:
+True if the `Result` state is `DONE` or `CANCELLED`..
+
+*Property `Result.result`*:
+The result.
+This property is not available before completion.
+
+*Method `Result.run_func(self, func, *a, **kw)`*:
+Fulfil the `Result` by running `func(*a,**kw)`.
+
+*Method `Result.run_func_in_thread(self, func, *a, **kw)`*:
+Fulfil the `Result` by running `func(*a,**kw)`
+in a separate `Thread`.
+
+This exists to step out of the current `Thread's` thread
+local context, such as a database transaction associated
+with Django's implicit per-`Thread` database context.
+
+*Property `Result.state`*:
+The `FSM` state (obsolete).
+Obsolete: use `.fsm_state`.
+
 ## Class `ResultSet(builtins.set)`
 
 A `set` subclass containing `Result`s,
 on which one may iterate as `Result`s complete.
 
+*Method `ResultSet.__iter__(self)`*:
+Iterating on a `ResultSet` yields `Result`s as they complete.
+
+*Method `ResultSet.wait(self)`*:
+Convenience function to wait for all the `Result`s.
+
 # Release Log
 
 
 
+*Release 20240412*:
+Result.bg: plumb _foo arguments to cs.threads.bg as foo.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240305*:
 Result.__str__: handle early use where __dict__ lacks various entries.
 
 *Release 20231221*:
@@ -256,8 +368,7 @@
 Fix module requirements specification.
 
 *Release 20171030*:
 New Result.bg(func, *a, **kw) method to dispatch function in separate Thread to compute the Result value.
 
 *Release 20170903*:
 rename cs.asynchron to cs.result
-
```

### Comparing `cs.result-20240316/README.md` & `cs.result-20240412/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,29 @@
+Metadata-Version: 2.1
+Name: cs.result
+Version: 20240412
+Summary: Result and friends: various subclassable classes for deferred delivery of values.
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
+
 Result and friends: various subclassable classes for deferred delivery of values.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+Result.bg: plumb _foo arguments to cs.threads.bg as foo.
 
 A `Result` is the base class for several callable subclasses
 which will receive values at a later point in time,
 and can also be used standalone without subclassing.
 
 A call to a `Result` will block until the value is received or the `Result` is cancelled,
 which will raise an exception in the caller.
@@ -70,15 +88,15 @@
 Other parameters are passed to `func`.
 
 ## Function `call_in_thread(func, *a, **kw)`
 
 Run `func(*a,**kw)` in a separate `Thread` via the `@in_thread` decorator.
 Return or exception is as for the original function.
 
-## Class `CancellationError(builtins.Exception, builtins.BaseException)`
+## Class `CancellationError(builtins.Exception)`
 
 Raised when accessing `result` or `exc_info` after cancellation.
 
 *Method `CancellationError.__init__(self, message=None, **kw)`*:
 Initialise the `CancellationError`.
 
 The optional `message` parameter (default `"cancelled"`)
@@ -90,31 +108,31 @@
 Decorator to evaluate `func` in a separate `Thread`.
 Return or exception is as for the original function.
 
 This exists to step out of the current `Thread's` thread
 local context, such as a database transaction associated
 with Django's implicit per-`Thread` database context.
 
-## Class `OnDemandFunction(Result, cs.fsm.FSM, cs.gvutils.DOTNodeMixin)`
+## Class `OnDemandFunction(Result)`
 
 Wrap a callable, run it when required.
 
-## Class `OnDemandResult(Result, cs.fsm.FSM, cs.gvutils.DOTNodeMixin)`
+## Class `OnDemandResult(Result)`
 
 Wrap a callable, run it when required.
 
 ## Function `report(LFs)`
 
 Generator which yields completed `Result`s.
 
 This is a generator that yields `Result`s as they complete,
 useful for waiting for a sequence of `Result`s
 that may complete in an arbitrary order.
 
-## Class `Result(cs.fsm.FSM, cs.gvutils.DOTNodeMixin)`
+## Class `Result(cs.fsm.FSM)`
 
 Base class for asynchronous collection of a result.
 This is used to make `Result`, `OnDemandFunction`s, `LateFunction`s
 and other objects with asynchronous termination.
 
 In addition to the methods below, for each state value such
 as `self.PENDING` there is a corresponding attribute `is_pending`
@@ -154,14 +172,19 @@
     # ready for collection by whatever received R
     R(func,1,2,z=3)
 
 *Method `Result.bg(self, func, *a, **kw)`*:
 Submit a function to compute the result in a separate `Thread`,
 returning the `Thread`.
 
+Keyword arguments for `cs.threads.bg` may be supplied by
+prefixing their names with an underscore, for example:
+
+    T = R.bg(mainloop, _pre_enter_objects=(S, fs))
+
 This dispatches a `Thread` to run `self.run_func(func,*a,**kw)`
 and as such the `Result` must be in "pending" state,
 and transitions to "running".
 
 *Method `Result.cancel(self)`*:
 Cancel this function.
 If `self.fsm_state` is `PENDING`` or `'CANCELLED'`, return `True`.
@@ -189,15 +212,15 @@
 On completion the sequence `(result,None)` is returned.
 If an exception occurred computing the result the sequence
 `(None,exc_info)` is returned
 where `exc_info` is a tuple of `(exc_type,exc_value,exc_traceback)`.
 If the function was cancelled the sequence `(None,None)`
 is returned.
 
-*Method `Result.notify(self, notifier)`*:
+*Method `Result.notify(self, notifier: Callable[[ForwardRef('Result')], NoneType])`*:
 After the `Result` completes, call `notifier(self)`.
 
 If the `Result` has already completed this will happen immediately.
 If you'd rather `self` got put on some queue `Q`, supply `Q.put`.
 
 *Property `Result.pending`*:
 Whether the `Result` is pending.
@@ -261,14 +284,17 @@
 *Method `ResultSet.wait(self)`*:
 Convenience function to wait for all the `Result`s.
 
 # Release Log
 
 
 
+*Release 20240412*:
+Result.bg: plumb _foo arguments to cs.threads.bg as foo.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240305*:
 Result.__str__: handle early use where __dict__ lacks various entries.
 
 *Release 20231221*:
@@ -360,7 +386,8 @@
 Fix module requirements specification.
 
 *Release 20171030*:
 New Result.bg(func, *a, **kw) method to dispatch function in separate Thread to compute the Result value.
 
 *Release 20170903*:
 rename cs.asynchron to cs.result
+
```

### Comparing `cs.result-20240316/lib/python/cs/result.py` & `cs.result-20240412/lib/python/cs/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,34 +51,34 @@
         x = R()     # collect result, will return immediately because
                     # the Result is complete
         print(x)    # print result
 '''
 
 import sys
 from threading import Lock, RLock
+from typing import Callable
 
 from icontract import require
 
 from cs.deco import OBSOLETE
 from cs.fsm import FSM
 from cs.gimmicks import exception, warning
 from cs.mappings import AttrableMapping
 from cs.pfx import pfx_method
 from cs.py.func import funcname, func_a_kw_fmt
 from cs.py3 import Queue, raise3, StringTypes
 from cs.seq import seq, Seq
 from cs.threads import bg as bg_thread
 
-__version__ = '20240316'
+__version__ = '20240412'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
     ],
     'install_requires': [
         'cs.deco',
         'cs.fsm',
         'cs.gimmicks',
         'cs.mappings',
@@ -320,20 +320,33 @@
     else:
       self.result = r
 
   def bg(self, func, *a, **kw):
     ''' Submit a function to compute the result in a separate `Thread`,
         returning the `Thread`.
 
+        Keyword arguments for `cs.threads.bg` may be supplied by
+        prefixing their names with an underscore, for example:
+
+            T = R.bg(mainloop, _pre_enter_objects=(S, fs))
+
         This dispatches a `Thread` to run `self.run_func(func,*a,**kw)`
         and as such the `Result` must be in "pending" state,
         and transitions to "running".
     '''
+    bg_kw = {}
+    for k in list(kw.keys()):
+      if k.startswith('_'):
+        bg_kw[k[1:]] = kw.pop(k)
     return bg_thread(
-        self.run_func, name=self.name, args=[func] + list(a), kwargs=kw
+        self.run_func,
+        name=self.name,
+        args=[func] + list(a),
+        kwargs=kw,
+        **bg_kw,
     )
 
   def run_func_in_thread(self, func, *a, **kw):
     ''' Fulfil the `Result` by running `func(*a,**kw)`
         in a separate `Thread`.
 
         This exists to step out of the current `Thread's` thread
@@ -431,15 +444,15 @@
     if self.is_cancelled:
       raise CancellationError(self)
     result, exc_info = self.join()
     if exc_info:
       raise3(*exc_info)
     return result
 
-  def notify(self, notifier):
+  def notify(self, notifier: Callable[["Result"], None]):
     ''' After the `Result` completes, call `notifier(self)`.
 
         If the `Result` has already completed this will happen immediately.
         If you'd rather `self` got put on some queue `Q`, supply `Q.put`.
     '''
 
     # TODO: adjust all users of .notify() to use fsm_callback and
```

### Comparing `cs.result-20240316/pyproject.toml` & `cs.result-20240412/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -5,49 +5,48 @@
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python2",
     "python3",
 ]
 dependencies = [
-    "cs.deco>=20240316",
+    "cs.deco>=20240412",
     "cs.fsm>=20240316",
     "cs.gimmicks>=20240316",
     "cs.mappings>=20231129",
-    "cs.pfx>=20230604",
+    "cs.pfx>=20240412",
     "cs.py.func>=20230331",
     "cs.py3>=20220523",
     "cs.seq>=20221118",
-    "cs.threads>=20240316",
+    "cs.threads>=20240412",
     "icontract",
 ]
 classifiers = [
     "Programming Language :: Python",
-    "Programming Language :: Python :: 2",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20240316"
+version = "20240412"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Result and friends: various subclassable classes for deferred delivery of values.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+Result.bg: plumb _foo arguments to cs.threads.bg as foo.
 
 A `Result` is the base class for several callable subclasses
 which will receive values at a later point in time,
 and can also be used standalone without subclassing.
 
 A call to a `Result` will block until the value is received or the `Result` is cancelled,
 which will raise an exception in the caller.
@@ -112,15 +111,15 @@
 Other parameters are passed to `func`.
 
 ## Function `call_in_thread(func, *a, **kw)`
 
 Run `func(*a,**kw)` in a separate `Thread` via the `@in_thread` decorator.
 Return or exception is as for the original function.
 
-## Class `CancellationError(builtins.Exception, builtins.BaseException)`
+## Class `CancellationError(builtins.Exception)`
 
 Raised when accessing `result` or `exc_info` after cancellation.
 
 *Method `CancellationError.__init__(self, message=None, **kw)`*:
 Initialise the `CancellationError`.
 
 The optional `message` parameter (default `\"cancelled\"`)
@@ -132,31 +131,31 @@
 Decorator to evaluate `func` in a separate `Thread`.
 Return or exception is as for the original function.
 
 This exists to step out of the current `Thread's` thread
 local context, such as a database transaction associated
 with Django's implicit per-`Thread` database context.
 
-## Class `OnDemandFunction(Result, cs.fsm.FSM, cs.gvutils.DOTNodeMixin)`
+## Class `OnDemandFunction(Result)`
 
 Wrap a callable, run it when required.
 
-## Class `OnDemandResult(Result, cs.fsm.FSM, cs.gvutils.DOTNodeMixin)`
+## Class `OnDemandResult(Result)`
 
 Wrap a callable, run it when required.
 
 ## Function `report(LFs)`
 
 Generator which yields completed `Result`s.
 
 This is a generator that yields `Result`s as they complete,
 useful for waiting for a sequence of `Result`s
 that may complete in an arbitrary order.
 
-## Class `Result(cs.fsm.FSM, cs.gvutils.DOTNodeMixin)`
+## Class `Result(cs.fsm.FSM)`
 
 Base class for asynchronous collection of a result.
 This is used to make `Result`, `OnDemandFunction`s, `LateFunction`s
 and other objects with asynchronous termination.
 
 In addition to the methods below, for each state value such
 as `self.PENDING` there is a corresponding attribute `is_pending`
@@ -171,23 +170,154 @@
 * `result`: if not `None`, prefill the `.result` property.
 * `extra`: an optional mapping of extra information to
   associate with the `Result`, useful to provide context
   when collecting the result; the `Result` has a public
   attribute `.extra` which is an `AttrableMapping` to hold
   this information.
 
+*Method `Result.__call__(self, *a, **kw)`*:
+Call the `Result`: wait for it to be ready and then return or raise.
+
+You can optionally supply a callable and arguments,
+in which case `callable(*args,**kwargs)` will be called
+via `Result.call` and the results applied to this `Result`.
+
+Basic example:
+
+    R = Result()
+    ... hand R to something which will fulfil it later ...
+    x = R() # wait for fulfilment - value lands in x
+
+Direct call:
+
+    R = Result()
+    ... pass R to something which wants the result ...
+    # call func(1,2,z=3), save result in R
+    # ready for collection by whatever received R
+    R(func,1,2,z=3)
+
+*Method `Result.bg(self, func, *a, **kw)`*:
+Submit a function to compute the result in a separate `Thread`,
+returning the `Thread`.
+
+Keyword arguments for `cs.threads.bg` may be supplied by
+prefixing their names with an underscore, for example:
+
+    T = R.bg(mainloop, _pre_enter_objects=(S, fs))
+
+This dispatches a `Thread` to run `self.run_func(func,*a,**kw)`
+and as such the `Result` must be in \"pending\" state,
+and transitions to \"running\".
+
+*Method `Result.cancel(self)`*:
+Cancel this function.
+If `self.fsm_state` is `PENDING`` or `'CANCELLED'`, return `True`.
+Otherwise return `False` (too late to cancel).
+
+*Property `Result.cancelled`*:
+Test whether this `Result` has been cancelled.
+Obsolete: use `.is_cancelled`.
+
+*Method `Result.empty(self)`*:
+Analogue to `Queue.empty()`.
+
+*Property `Result.exc_info`*:
+The exception information from a completed `Result`.
+This is not available before completion.
+
+*Method `Result.get(self, default=None)`*:
+Wait for readiness; return the result if `self.exc_info` is `None`,
+otherwise `default`.
+
+*Method `Result.join(self)`*:
+Calling the `.join()` method waits for the function to run to
+completion and returns a tuple of `(result,exc_info)`.
+
+On completion the sequence `(result,None)` is returned.
+If an exception occurred computing the result the sequence
+`(None,exc_info)` is returned
+where `exc_info` is a tuple of `(exc_type,exc_value,exc_traceback)`.
+If the function was cancelled the sequence `(None,None)`
+is returned.
+
+*Method `Result.notify(self, notifier: Callable[[ForwardRef('Result')], NoneType])`*:
+After the `Result` completes, call `notifier(self)`.
+
+If the `Result` has already completed this will happen immediately.
+If you'd rather `self` got put on some queue `Q`, supply `Q.put`.
+
+*Property `Result.pending`*:
+Whether the `Result` is pending.
+Obsolete: use `.is_pending`.
+
+*Method `Result.post_notify(self, post_func) -> 'Result'`*:
+Return a secondary `Result` which processes the result of `self`.
+
+After the `self` completes, call `post_func(retval)` where
+`retval` is the result of `self`, and use that to complete
+the secondary `Result`.
+
+Example:
+
+    # submit packet to data stream
+    R = submit_packet()
+    # arrange that when the response is received, decode the response
+    R2 = R.post_notify(lambda response: decode(response))
+    # collect decoded response
+    decoded = R2()
+
+If the `Result` has already completed this will happen immediately.
+
+*Method `Result.put(self, value)`*:
+Store the value. `Queue`-like idiom.
+
+*Method `Result.raise_(self, exc=None)`*:
+Convenience wrapper for `self.exc_info` to store an exception result `exc`.
+If `exc` is omitted or `None`, uses `sys.exc_info()`.
+
+*Property `Result.ready`*:
+True if the `Result` state is `DONE` or `CANCELLED`..
+
+*Property `Result.result`*:
+The result.
+This property is not available before completion.
+
+*Method `Result.run_func(self, func, *a, **kw)`*:
+Fulfil the `Result` by running `func(*a,**kw)`.
+
+*Method `Result.run_func_in_thread(self, func, *a, **kw)`*:
+Fulfil the `Result` by running `func(*a,**kw)`
+in a separate `Thread`.
+
+This exists to step out of the current `Thread's` thread
+local context, such as a database transaction associated
+with Django's implicit per-`Thread` database context.
+
+*Property `Result.state`*:
+The `FSM` state (obsolete).
+Obsolete: use `.fsm_state`.
+
 ## Class `ResultSet(builtins.set)`
 
 A `set` subclass containing `Result`s,
 on which one may iterate as `Result`s complete.
 
+*Method `ResultSet.__iter__(self)`*:
+Iterating on a `ResultSet` yields `Result`s as they complete.
+
+*Method `ResultSet.wait(self)`*:
+Convenience function to wait for all the `Result`s.
+
 # Release Log
 
 
 
+*Release 20240412*:
+Result.bg: plumb _foo arguments to cs.threads.bg as foo.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240305*:
 Result.__str__: handle early use where __dict__ lacks various entries.
 
 *Release 20231221*:
```

