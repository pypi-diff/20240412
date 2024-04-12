# Comparing `tmp/cs.later-20240305.tar.gz` & `tmp/cs.later-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.later-20240305.tar", last modified: Mon Mar  4 21:52:38 2024, max compression
+gzip compressed data, was "cs.later-20240412.tar", last modified: Fri Apr 12 05:13:24 2024, max compression
```

## Comparing `cs.later-20240305.tar` & `cs.later-20240412.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-04 21:52:38.038842 cs.later-20240305/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-04 21:52:14.000000 cs.later-20240305/MANIFEST.in
--rw-r--r--   0 cameron    (501) cameron    (502)     9714 2024-03-04 21:52:38.038152 cs.later-20240305/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    17595 2024-03-04 21:52:19.000000 cs.later-20240305/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-04 21:52:38.037682 cs.later-20240305/cs.later.egg-info/
--rw-r--r--   0 cameron    (501) cameron    (502)     9714 2024-03-04 21:52:38.000000 cs.later-20240305/cs.later.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      218 2024-03-04 21:52:38.000000 cs.later-20240305/cs.later.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-04 21:52:38.000000 cs.later-20240305/cs.later.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      213 2024-03-04 21:52:38.000000 cs.later-20240305/cs.later.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        4 2024-03-04 21:52:38.000000 cs.later-20240305/cs.later.egg-info/top_level.txt
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-04 21:52:38.032853 cs.later-20240305/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-04 21:52:38.032967 cs.later-20240305/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-04 21:52:38.036463 cs.later-20240305/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    35835 2024-03-04 21:51:59.000000 cs.later-20240305/lib/python/cs/later.py
--rw-rw-r--   0 cameron    (501) cameron    (502)     9854 2024-03-04 21:52:29.000000 cs.later-20240305/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-04 21:52:38.038952 cs.later-20240305/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:13:24.474644 cs.later-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 05:13:08.000000 cs.later-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    18031 2024-04-12 05:13:24.474259 cs.later-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17265 2024-04-12 05:13:13.000000 cs.later-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:13:24.470059 cs.later-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:13:24.470356 cs.later-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:13:24.471769 cs.later-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    35124 2024-04-12 05:12:56.000000 cs.later-20240412/lib/python/cs/later.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:13:24.473757 cs.later-20240412/lib/python/cs.later.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    18031 2024-04-12 05:13:23.000000 cs.later-20240412/lib/python/cs.later.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      273 2024-04-12 05:13:24.000000 cs.later-20240412/lib/python/cs.later.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 05:13:23.000000 cs.later-20240412/lib/python/cs.later.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      234 2024-04-12 05:13:24.000000 cs.later-20240412/lib/python/cs.later.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 05:13:24.000000 cs.later-20240412/lib/python/cs.later.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    18659 2024-04-12 05:13:22.000000 cs.later-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 05:13:24.474747 cs.later-20240412/setup.cfg
```

### Comparing `cs.later-20240305/README.md` & `cs.later-20240412/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Queue functions for execution later in priority and time order.
 
-*Latest release 20240305*:
-Later: new thread_states=True parameter to propagate all HasThreadStates to the LateFUnction Threads; adjust LateFunction to match.
+*Latest release 20240412*:
+Later: new optional default=False parameter, set to true to have the Later push itself as the default for HasThreadStates.
 
 I use `Later` objects for convenient queuing of functions whose
 execution occurs later in a priority order with capacity constraints.
 
 Why not futures?
 I already had this before futures came out,
 I prefer its naming scheme and interface,
@@ -26,15 +26,15 @@
 so to collect the result you just call the `LateFunction`.
 
 ## Function `defer(func, *a, **kw)`
 
 Queue a function using the current default Later.
 Return the `LateFunction`.
 
-## Class `LateFunction(cs.result.Result, cs.fsm.FSM, cs.gvutils.DOTNodeMixin)`
+## Class `LateFunction(cs.result.Result)`
 
 State information about a pending function,
 a subclass of `cs.result.Result`.
 
 A `LateFunction` is callable,
 so a synchronous call can be done like this:
 
@@ -63,28 +63,27 @@
       exc_type, exc_value, exc_traceback = exc_info
       ...
     else:
       # use `x`, the function result
 
 TODO: .cancel(), timeout for wait().
 
-*Method `LateFunction.__init__(self, func, name=None, retry_delay=None, thread_states=None)`*:
+*Method `LateFunction.__init__(self, func, name=None, retry_delay=None)`*:
 Initialise a `LateFunction`.
 
 Parameters:
 * `func` is the callable for later execution.
 * `name`, if supplied, specifies an identifying name for the `LateFunction`.
 * `retry_local`: time delay before retry of this function on RetryError.
   Default from `later.retry_delay`.
-* `thread_states`: optional thread states passed to `HasThreadState.Thread`
 
 *Method `LateFunction.wait(self)`*:
 Obsolete name for `.join`.
 
-## Class `LatePool`
+## Class `LatePool(cs.context.ContextManagerMixin)`
 
 A context manager after the style of subprocess.Pool
 but with deferred completion.
 
 Example usage:
 
     L = Later(4)    # a 4 thread Later
@@ -95,32 +94,26 @@
     # now we can LP.join() to block for all `LateFunctions`
     #
     # or iterate over LP to collect `LateFunction`s as they complete
     for LF in LP:
       result = LF()
       print(result)
 
-*Method `LatePool.__init__(self, *, later, priority=None, delay=None, when=None, pfx=None, block=False)`*:
+*Method `LatePool.__init__(self, *, later: Optional[inspect._empty] = <function <lambda> at 0x10a2b0160>, priority=None, delay=None, when=None, pfx=None, block=False)`*:
 Initialise the `LatePool`.
 
 Parameters:
 * `later`: optional `Later` instance, default from `Later.default()`
 * `priority`, `delay`, `when`, `name`, `pfx`:
   default values passed to Later.submit.
 * `block`: if true, wait for `LateFunction` completion
-  before leaving __exit__.
+  before leaving `__exit__`.
 
-*Method `LatePool.__enter__(self)`*:
-Entry handler: submit a placeholder function to the queue,
-acquire the "commence" lock, which will be made available
-when the placeholder gets to run.
-
-*Method `LatePool.__exit__(self, exc_type, exc_val, exc_tb)`*:
-Exit handler.
-If .block is true, wait for `LateFunction` completion before return.
+*Method `LatePool.__enter_exit__(self)`*:
+Generator supporting `__enter__` and `__exit__`.
 
 *Method `LatePool.__iter__(self)`*:
 Report completion of the `LateFunction`s.
 
 *Method `LatePool.add(self, LF)`*:
 Add a `LateFunction` to those to be tracked by this LatePool.
 
@@ -129,15 +122,15 @@
 
 *Method `LatePool.join(self)`*:
 Wait for completion of all the `LateFunction`s.
 
 *Method `LatePool.submit(self, func, **params)`*:
 Submit a function using the LatePool's default parameters, overridden by `params`.
 
-## Class `Later(cs.resources.MultiOpenMixin, cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+## Class `Later(cs.resources.MultiOpenMixin, cs.threads.HasThreadState)`
 
 A management class to queue function calls for later execution.
 
 Methods are provided for submitting functions to run ASAP or
 after a delay or after other pending functions. These methods
 return `LateFunction`s, a subclass of `cs.result.Result`.
 
@@ -147,33 +140,29 @@
 completed or even been dispatched.
 Callers may wait for completion and optionally cancel functions.
 
 TODO: __enter__ returns a SubLater, __exit__ closes the SubLater.
 
 TODO: drop global default Later.
 
-*Method `Later.__init__(self, capacity, name=None, inboundCapacity=0, retry_delay=None, thread_states=True)`*:
+*Method `Later.__init__(self, capacity, name=None, inboundCapacity=0, retry_delay=None, default=False)`*:
 Initialise the Later instance.
 
 Parameters:
 * `capacity`: resource contraint on this Later; if an int, it is used
   to size a Semaphore to constrain the number of dispatched functions
   which may be in play at a time; if not an int it is presumed to be a
   suitable Semaphore-like object, perhaps shared with other subsystems.
 * `name`: optional identifying name for this instance.
 * `inboundCapacity`: if >0, used as a limit on the number of
   undispatched functions that may be queued up; the default is 0 (no
   limit).  Calls to submit functions when the inbound limit is reached
   block until some functions are dispatched.
 * `retry_delay`: time delay for requeued functions.
   Default: `DEFAULT_RETRY_DELAY`.
-* `thread_states`: the default `thread_states` parameter
-  for `LateFunctions`, which is in turn passed to
-  `HasThreadState.Thread`
-  Default: `True`
 
 *Method `Later.__call__(self, func, *a, **kw)`*:
 A Later object can be called with a function and arguments
 with the effect of deferring the function and waiting for
 it to complete, returning its return value.
 
 Example:
@@ -341,15 +330,15 @@
 *Method `Later.ready(self, **kwargs)`*:
 Awful name.
 Return a context manager to block until the `Later` provides a timeslot.
 
 *Method `Later.state(self, new_state, *a)`*:
 Update the state of this Later.
 
-*Method `Later.submit(self, func, priority=None, delay=None, when=None, name=None, pfx=None, LF=None, retry_delay=None, thread_states=None)`*:
+*Method `Later.submit(self, func, priority=None, delay=None, when=None, name=None, pfx=None, LF=None, retry_delay=None)`*:
 Submit the callable `func` for later dispatch.
 Return the corresponding `LateFunction` for result collection.
 
 If the parameter `priority` is not None then use it as the priority
 otherwise use the default priority.
 
 If the parameter `delay` is not None, delay consideration of
@@ -386,23 +375,23 @@
 
 Call the callable `func` with the supplied arguments.
 
 If it raises `RetryError`,
 run `time.sleep(retry_interval)`
 and then call again until it does not raise `RetryError`.
 
-## Class `RetryError(builtins.Exception, builtins.BaseException)`
+## Class `RetryError(builtins.Exception)`
 
 Exception raised by functions which should be resubmitted to the queue.
 
 ## Class `SubLater`
 
 A class for managing a group of deferred tasks using an existing `Later`.
 
-*Method `SubLater.__init__(self, *, later: cs.later.Later)`*:
+*Method `SubLater.__init__(self, *, later: Optional[cs.later.Later] = <function <lambda> at 0x10a2b0160>)`*:
 Initialise the `SubLater` with its parent `Later`.
 
 TODO: accept `discard=False` param to suppress the queue and
 associated checks.
 
 *Method `SubLater.__iter__(self)`*:
 Iteration over the `SubLater`
@@ -426,14 +415,17 @@
 `handler`: an optional callable to be passed each `LateFunction`
 as it completes.
 
 # Release Log
 
 
 
+*Release 20240412*:
+Later: new optional default=False parameter, set to true to have the Later push itself as the default for HasThreadStates.
+
 *Release 20240305*:
 Later: new thread_states=True parameter to propagate all HasThreadStates to the LateFUnction Threads; adjust LateFunction to match.
 
 *Release 20230612*:
 Updates stemming from cs.threads changes.
 
 *Release 20230212.1*:
```

### Comparing `cs.later-20240305/lib/python/cs/later.py` & `cs.later-20240412/lib/python/cs/later.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,35 +39,37 @@
 import sys
 from threading import Lock, Event
 import time
 from typing import Callable, Iterable, Optional
 
 from typeguard import typechecked
 
+from cs.context import ContextManagerMixin
 from cs.deco import OBSOLETE, decorator, default_params
 from cs.excutils import logexc
 import cs.logutils
 from cs.logutils import error, warning, info, debug, ifdebug, exception, D
 from cs.pfx import pfx, pfx_method
 from cs.py.func import funccite, funcname
 from cs.queues import IterableQueue, TimerQueue
 from cs.resources import MultiOpenMixin
 from cs.result import Result, report, after
 from cs.seq import seq
 from cs.threads import ThreadState, HasThreadState
 
-__version__ = '20240305'
+__version__ = '20240412'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
     'install_requires': [
+        'cs.context',
         'cs.deco',
         'cs.excutils',
         'cs.logutils',
         'cs.pfx',
         'cs.py.func',
         'cs.queues',
         'cs.resources',
@@ -215,37 +217,35 @@
             ...
           else:
             # use `x`, the function result
 
       TODO: .cancel(), timeout for wait().
   '''
 
-  def __init__(self, func, name=None, retry_delay=None, thread_states=None):
+  def __init__(self, func, name=None, retry_delay=None):
     ''' Initialise a `LateFunction`.
 
         Parameters:
         * `func` is the callable for later execution.
         * `name`, if supplied, specifies an identifying name for the `LateFunction`.
         * `retry_local`: time delay before retry of this function on RetryError.
           Default from `later.retry_delay`.
-        * `thread_states`: optional thread states passed to `HasThreadState.Thread`
     '''
     Result.__init__(self)
     self.func = func
     if name is None:
       name = "LF-%d[%s]" % (seq(), funcname(func))
     if retry_delay is None:
       retry_delay = DEFAULT_RETRY_DELAY
     self.name = name
     self.retry_delay = retry_delay
     # we prepare the Thread now in order to honour the perThread states
     self.thread = HasThreadState.Thread(
         name=name,
         target=partial(self.run_func, func),
-        thread_states=thread_states,
     )
 
   def __str__(self):
     return "%s[%s]" % (type(self).__name__, self.name)
 
   def _resubmit(self):
     ''' Resubmit this function for later execution.
@@ -315,15 +315,15 @@
 
   def __init__(
       self,
       capacity,
       name=None,
       inboundCapacity=0,
       retry_delay=None,
-      thread_states=True,
+      default=False,
   ):
     ''' Initialise the Later instance.
 
         Parameters:
         * `capacity`: resource contraint on this Later; if an int, it is used
           to size a Semaphore to constrain the number of dispatched functions
           which may be in play at a time; if not an int it is presumed to be a
@@ -331,35 +331,31 @@
         * `name`: optional identifying name for this instance.
         * `inboundCapacity`: if >0, used as a limit on the number of
           undispatched functions that may be queued up; the default is 0 (no
           limit).  Calls to submit functions when the inbound limit is reached
           block until some functions are dispatched.
         * `retry_delay`: time delay for requeued functions.
           Default: `DEFAULT_RETRY_DELAY`.
-        * `thread_states`: the default `thread_states` parameter
-          for `LateFunctions`, which is in turn passed to
-          `HasThreadState.Thread`
-          Default: `True`
     '''
     if name is None:
       name = "Later-%d" % (seq(),)
     if ifdebug():
       import inspect  # pylint: disable=import-outside-toplevel
       filename, lineno = inspect.stack()[1][1:3]
       name = "%s[%s:%d]" % (name, filename, lineno)
     debug(
         "Later.__init__(capacity=%s, inboundCapacity=%s, name=%s)", capacity,
         inboundCapacity, name
     )
     if retry_delay is None:
       retry_delay = DEFAULT_RETRY_DELAY
+    self.default = default
     self.capacity = capacity
     self.inboundCapacity = inboundCapacity
     self.retry_delay = retry_delay
-    self.thread_states = thread_states
     self.name = name
     self._lock = Lock()
     self.outstanding = set()  # dispatched but uncompleted LateFunctions
     self.delayed = set()  # unqueued, delayed until specific time
     self.pending = []  # undispatched LateFunctions, a heap
     self.running = set()  # running LateFunctions
     # counter tracking jobs queued or active
@@ -371,15 +367,15 @@
     self.finished_event = None
 
   def __enter_exit__(self):
     ''' Run both the inherited context managers.
     '''
     for _ in zip_longest(
         MultiOpenMixin.__enter_exit__(self),
-        HasThreadState.__enter_exit__(self),
+        HasThreadState.__enter_exit__(self) if self.default else (),
     ):
       yield
 
   @contextmanager
   def startup_shutdown(self):
     with super().startup_shutdown():
       self.finished_event = Event()
@@ -391,15 +387,14 @@
         # - close the request queue
         # - close the TimerQueue if any
         # - close the worker thread pool
         # - dispatch a Thread to wait for completion and fire the
         #   finished_event Event
         # queue final action to mark activity completion
         self.defer(
-            dict(thread_states=False),
             self.finished_event.set,
             _force_submit=True,
         )
         if self._timerQ:
           self._timerQ.close()
           self._timerQ.join()
 
@@ -598,15 +593,15 @@
     name = None
     if isinstance(func, str):
       name = func
       a = list(a)
       func = a.pop(0)
     if a or kw:
       func = partial(func, *a, **kw)
-    LF = LateFunction(func, name=name, thread_states=self.thread_states)
+    LF = LateFunction(func, name=name)
     LF._dispatch()  # pylint: disable=protected-access
     return LF
 
   def ready(self, **kwargs):
     ''' Awful name.
         Return a context manager to block until the `Later` provides a timeslot.
     '''
@@ -620,15 +615,14 @@
       priority=None,
       delay=None,
       when=None,
       name=None,
       pfx=None,  # pylint: disable=redefined-outer-name
       LF=None,
       retry_delay=None,
-      thread_states=None,
   ):
     ''' Submit the callable `func` for later dispatch.
         Return the corresponding `LateFunction` for result collection.
 
         If the parameter `priority` is not None then use it as the priority
         otherwise use the default priority.
 
@@ -653,22 +647,19 @@
       )
     if priority is None:
       priority = self._priority
     elif isinstance(priority, int):
       priority = (priority,)
     if pfx is not None:
       func = pfx.partial(func)
-    if thread_states is None:
-      thread_states = self.thread_states
     if LF is None:
       LF = LateFunction(
           func,
           name=name,
           retry_delay=retry_delay,
-          thread_states=thread_states,
       )
     pri_entry = list(priority)
     pri_entry.append(seq())  # ensure FIFO servicing of equal priorities
     pri_entry.append(LF)
 
     now = time.time()
     if delay is not None:
@@ -1030,15 +1021,15 @@
 
     T = HasThreadState.Thread(
         name="reaper(%s)" % (self,), target=reap, args=(self._queue,)
     )
     T.start()
     return T
 
-class LatePool(object):
+class LatePool(ContextManagerMixin):
   ''' A context manager after the style of subprocess.Pool
       but with deferred completion.
 
       Example usage:
 
           L = Later(4)    # a 4 thread Later
           with LatePool(L) as LP:
@@ -1068,40 +1059,34 @@
     ''' Initialise the `LatePool`.
 
         Parameters:
         * `later`: optional `Later` instance, default from `Later.default()`
         * `priority`, `delay`, `when`, `name`, `pfx`:
           default values passed to Later.submit.
         * `block`: if true, wait for `LateFunction` completion
-          before leaving __exit__.
+          before leaving `__exit__`.
     '''
     self.later = later
     self.parameters = {
         'priority': priority,
         'delay': delay,
         'when': when,
         'pfx': pfx,
     }
     self.block = block
     self.LFs = []
 
-  def __enter__(self):
-    ''' Entry handler: submit a placeholder function to the queue,
-        acquire the "commence" lock, which will be made available
-        when the placeholder gets to run.
-    '''
-    return self
-
-  def __exit__(self, exc_type, exc_val, exc_tb):
-    ''' Exit handler.
-        If .block is true, wait for `LateFunction` completion before return.
+  def __enter_exit__(self):
+    ''' Generator supporting `__enter__` and `__exit__`.
     '''
-    if self.block:
-      self.join()
-    return False
+    try:
+      yield
+    finally:
+      if self.block:
+        self.join()
 
   def add(self, LF):
     ''' Add a `LateFunction` to those to be tracked by this LatePool.
     '''
     self.LFs.append(LF)
 
   def submit(self, func, **params):
```

