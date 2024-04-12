# Comparing `tmp/cs.threads-20240316.tar.gz` & `tmp/cs.threads-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.threads-20240316.tar", last modified: Sat Mar 16 07:03:51 2024, max compression
+gzip compressed data, was "cs.threads-20240412.tar", last modified: Fri Apr 12 03:32:19 2024, max compression
```

## Comparing `cs.threads-20240316.tar` & `cs.threads-20240412.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:03:51.973890 cs.threads-20240316/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-16 07:03:25.000000 cs.threads-20240316/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    11263 2024-03-16 07:03:51.973429 cs.threads-20240316/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    16055 2024-03-16 07:03:33.000000 cs.threads-20240316/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:03:51.969504 cs.threads-20240316/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:03:51.969803 cs.threads-20240316/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:03:51.971098 cs.threads-20240316/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    24323 2024-03-16 07:03:15.000000 cs.threads-20240316/lib/python/cs/threads.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:03:51.972926 cs.threads-20240316/lib/python/cs.threads.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    11263 2024-03-16 07:03:51.000000 cs.threads-20240316/lib/python/cs.threads.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      285 2024-03-16 07:03:51.000000 cs.threads-20240316/lib/python/cs.threads.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 07:03:51.000000 cs.threads-20240316/lib/python/cs.threads.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      140 2024-03-16 07:03:51.000000 cs.threads-20240316/lib/python/cs.threads.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 07:03:51.000000 cs.threads-20240316/lib/python/cs.threads.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    11785 2024-03-16 07:03:50.000000 cs.threads-20240316/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 07:03:51.973998 cs.threads-20240316/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 03:32:19.224279 cs.threads-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 03:31:53.000000 cs.threads-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    18084 2024-04-12 03:32:19.223940 cs.threads-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17315 2024-04-12 03:32:01.000000 cs.threads-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 03:32:19.219894 cs.threads-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 03:32:19.220210 cs.threads-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 03:32:19.221620 cs.threads-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    27102 2024-04-12 03:25:42.000000 cs.threads-20240412/lib/python/cs/threads.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 03:32:19.223453 cs.threads-20240412/lib/python/cs.threads.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    18084 2024-04-12 03:32:18.000000 cs.threads-20240412/lib/python/cs.threads.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      285 2024-04-12 03:32:19.000000 cs.threads-20240412/lib/python/cs.threads.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 03:32:18.000000 cs.threads-20240412/lib/python/cs.threads.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      140 2024-04-12 03:32:18.000000 cs.threads-20240412/lib/python/cs.threads.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 03:32:19.000000 cs.threads-20240412/lib/python/cs.threads.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    18608 2024-04-12 03:32:17.000000 cs.threads-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 03:32:19.224381 cs.threads-20240412/setup.cfg
```

### Comparing `cs.threads-20240316/PKG-INFO` & `cs.threads-20240412/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.threads
-Version: 20240316
+Version: 20240412
 Summary: threading and communication/synchronisation conveniences
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,37 +14,74 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Thread related convenience classes and functions.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+* New NRLock, an nonrecursive Lock and associated exception DeadlockError.
+* bg: rename thread_class to thread_factory for clarity.
+* HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
+* HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
 
 ## Class `AdjustableSemaphore`
 
 A semaphore whose value may be tuned after instantiation.
 
-## Function `bg(func, daemon=None, name=None, no_start=False, no_logexc=False, thread_class=None, thread_states=None, args=None, kwargs=None)`
+*Method `AdjustableSemaphore.acquire(self, blocking=True)`*:
+The acquire() method calls the base acquire() method if not blocking.
+If blocking is true, the base acquire() is called inside a lock to
+avoid competing with a reducing adjust().
+
+*Method `AdjustableSemaphore.adjust(self, newvalue)`*:
+Set capacity to `newvalue`
+by calling release() or acquire() an appropriate number of times.
+
+If `newvalue` lowers the semaphore capacity then adjust()
+may block until the overcapacity is released.
+
+*Method `AdjustableSemaphore.adjust_delta(self, delta)`*:
+Adjust capacity by `delta` by calling release() or acquire()
+an appropriate number of times.
+
+If `delta` lowers the semaphore capacity then adjust() may block
+until the overcapacity is released.
+
+*Method `AdjustableSemaphore.release(self)`*:
+Release the semaphore.
+
+## Function `bg(func, *, daemon=None, name=None, no_start=False, no_logexc=False, args=None, kwargs=None, thread_factory=None, pre_enter_objects=None, **tfkw)`
 
 Dispatch the callable `func` in its own `Thread`;
 return the `Thread`.
 
 Parameters:
 * `func`: a callable for the `Thread` target.
+* `args`, `kwargs`: passed to the `Thread` constructor
+* `kwargs`, `kwargs`: passed to the `Thread` constructor
 * `daemon`: optional argument specifying the `.daemon` attribute.
 * `name`: optional argument specifying the `Thread` name,
   default: the name of `func`.
 * `no_logexc`: if false (default `False`), wrap `func` in `@logexc`.
 * `no_start`: optional argument, default `False`.
   If true, do not start the `Thread`.
-* `thread_class`: the `Thread` factory, default `HasThreadState.Thread`
-* `thread_states`: passed tothe  `thread_class` factory
-* `args`, `kwargs`: passed to the `Thread` constructor
+* `pre_enter_objects`: an optional iterable of objects which
+  should be entered using `with`
+
+If `pre_enter_objects` is supplied, these objects will be
+entered before the `Thread` is started and exited when the
+`Thread` target function ends.
+If the `Thread` is _not_ started (`no_start=True`, very
+unusual) then it will be the caller's responsibility to manage
+to entered objects.
+
+## Class `DeadlockError(builtins.RuntimeError)`
+
+Raised by `NRLock` when a lock is attempted from the `Thread` currently holding the lock.
 
 ## Class `HasThreadState(cs.context.ContextManagerMixin)`
 
 A mixin for classes with a `cs.threads.ThreadState` instance as `.state`
 providing a context manager which pushes `current=self` onto that state
 and a `default()` class method returning `cls.perthread_state.current`
 as the default instance of that class.
@@ -58,35 +95,109 @@
 *NOTE*: `HasThreadState.Thread` is a _class_ method whose default
 is to push state for all active `HasThreadState` subclasses.
 Contrast with `HasThreadState.bg` which is an _instance_method
 whose default is to push state for just that instance.
 The top level `cs.threads.bg` function calls `HasThreadState.Thread`
 to obtain its `Thread`.
 
+*Method `HasThreadState.Thread(*, name=None, target, enter_objects=None, **Thread_kw)`*:
+Factory for a `Thread` to push the `.current` state for the
+currently active classes.
+
+The optional parameter `enter_objects` may be used to pass
+an iterable of objects whose contexts should be entered
+using `with obj:`.
+If this is set to `True` that indicates that every "current"
+`HasThreadStates` instance should be entered.
+The default does not enter any object contexts.
+The `HasThreadStates.bg` method defaults to passing
+`enter_objects=(self,)` to enter the context for `self`.
+
+*Method `HasThreadState.__enter_exit__(self)`*:
+Push `self.perthread_state.current=self` as the `Thread` local current instance.
+
+Include `self.__class__` in the set of currently active classes for the duration.
+
+*Method `HasThreadState.bg(self, func, *, enter_objects=None, pre_enter_objects=None, **bg_kw)`*:
+Get a `Thread` using `type(elf).Thread` and start it.
+Return the `Thread`.
+
+The `HasThreadState.Thread` factory duplicates the current `Thread`'s
+`HasThreadState` current objects as current in the new `Thread`.
+Additionally it enters the contexts of various objects using
+`with obj` according to the `enter_objects` parameter.
+
+The value of the optional parameter `enter_objects` governs
+which objects have their context entered using `with obj`
+in the child `Thread` while running `func` as follows:
+- `None`: the default, meaning `(self,)`
+- `False`: no object contexts are entered
+- `True`: all current `HasThreadState` object contexts will be entered
+- an iterable of objects whose contexts will be entered;
+  pass `()` to enter no objects
+
+*Method `HasThreadState.default(factory=None, raise_on_None=False)`*:
+The default instance of this class from `cls.perthread_state.current`.
+
+Parameters:
+* `factory`: optional callable to create an instance of `cls`
+  if `cls.perthread_state.current` is `None` or missing;
+  if `factory` is `True` then `cls` is used as the factory
+* `raise_on_None`: if `cls.perthread_state.current` is `None` or missing
+  and `factory` is false and `raise_on_None` is true,
+  raise a `RuntimeError`;
+  this is primarily a debugging aid
+
+*Method `HasThreadState.get_thread_states(all_classes=None)`*:
+Return a mapping of `class`->*current_instance*`
+for use with `HasThreadState.with_thread_states`
+or `HasThreadState.Thread` or `HasThreadState.bg`.
+
+The default behaviour returns just a mapping for this class,
+expecting the default instance to be responsible for what
+other resources it holds.
+
+There is also a legacy mode for `all_classes=True`
+where the mapping is for all active classes,
+probably best used for `Thread`s spawned outside
+a `HasThreadState` context.
+
+Parameters:
+* `all_classes`: optional flag, default `False`;
+  if true, return a mapping of class to current instance
+  for all `HasThreadState` subclasses with an open instance,
+  otherwise just a mapping from this class to its current instance
+
 ## Function `joinif(T: threading.Thread)`
 
 Call `T.join()` if `T` is not the current `Thread`.
 
 Unlike `threading.Thread.join`, this function is a no-op if
 `T` is the current `Thread.
 
 The use case is situations such as the shutdown phase of the
 `MultiOpenMixin.startup_shutdown` context manager. Because
 the "initial open" startup phase is not necessarily run in
 the same thread as the "final close" shutdown phase, it is
 possible for example for a worker `Thread` to execute the
 shutdown phase and try to join itself. Using this function
-allows that scenario.
+supports that scenario.
 
 ## Class `LockableMixin`
 
 Trite mixin to control access to an object via its `._lock` attribute.
 Exposes the `._lock` as the property `.lock`.
 Presents a context manager interface for obtaining an object's lock.
 
+*Method `LockableMixin.__exit__(self, exc_type, exc_value, traceback)`*:
+pylint: disable=unused-argument
+
+*Property `LockableMixin.lock`*:
+Return the lock.
+
 ## Function `locked(*da, **dkw)`
 
 A decorator for instance methods that must run within a lock.
 
 Decorator keyword arguments:
 * `initial_timeout`:
   the initial lock attempt timeout;
@@ -121,14 +232,28 @@
   If omitted, all names commencing with a letter are chosen.
 * `initial_timeout`: optional initial lock timeout, default `10.0`s.
 * `lockattr`: optional lock attribute name, default `'_lock'`.
 
 Only attributes satifying `inspect.ismethod` are wrapped
 because `@locked` requires access to the instance `._lock` attribute.
 
+## Class `NRLock`
+
+A nonrecursive lock.
+Attempting to take this lock when it is already held by the current `Thread`
+will raise `DeadlockError`.
+Otherwise this behaves likc `threading.Lock`.
+
+*Method `NRLock.acquire(self, *a, caller_frame=None, **kw)`*:
+Acquire the lock as for `threading.Lock`.
+Raises `DeadlockError` is the lock is already held by the current `Thread`.
+
+*Method `NRLock.locked(self)`*:
+Return the lock status.
+
 ## Class `PriorityLock`
 
 A priority based mutex which is acquired by and released to waiters
 in priority order.
 
 The initialiser sets a default priority, itself defaulting to `0`.
 
@@ -156,15 +281,39 @@
 Initialise the `PriorityLock`.
 
 Parameters:
 * `default_priority`: the default `acquire` priority,
   default `0`.
 * `name`: optional identifying name
 
-## Class `PriorityLockSubLock(PriorityLockSubLock, builtins.tuple)`
+*Method `PriorityLock.__enter__(self)`*:
+Enter the mutex as a context manager at the default priority.
+Returns the new `Lock`.
+
+*Method `PriorityLock.__exit__(self, *_)`*:
+Exit the context manager.
+
+*Method `PriorityLock.acquire(self, priority=None)`*:
+Acquire the mutex with `priority` (default from `default_priority`).
+Return the new `PriorityLockSubLock`.
+
+This blocks behind any higher priority `acquire`s
+or any earlier `acquire`s of the same priority.
+
+*Method `PriorityLock.priority(self, this_priority)`*:
+A context manager with the specified `this_priority`.
+Returns the new `Lock`.
+
+*Method `PriorityLock.release(self)`*:
+Release the mutex.
+
+Internally, this releases the highest priority `Lock`,
+allowing that `acquire`r to go forward.
+
+## Class `PriorityLockSubLock(PriorityLockSubLock)`
 
 The record for the per-`acquire`r `Lock` held by `PriorityLock.acquire`.
 
 ## Class `State(_thread._local)`
 
 A `Thread` local object with attributes
 which can be used as a context manager to stack attribute values.
@@ -176,15 +325,20 @@
     S = ThreadState(verbose=False)
 
     with S(verbose=True) as prev_attrs:
         if S.verbose:
             print("verbose! (formerly verbose=%s)" % prev_attrs['verbose'])
 
 *Method `State.__init__(self, **kw)`*:
-Initiale the `ThreadState`, providing the per-Thread initial values.
+Initiate the `ThreadState`, providing the per-Thread initial values.
+
+*Method `State.__call__(self, **kw)`*:
+Calling a `ThreadState` returns a context manager which stacks some state.
+The context manager yields the previous values
+for the attributes which were stacked.
 
 ## Class `ThreadState(_thread._local)`
 
 A `Thread` local object with attributes
 which can be used as a context manager to stack attribute values.
 
 Example:
@@ -194,26 +348,37 @@
     S = ThreadState(verbose=False)
 
     with S(verbose=True) as prev_attrs:
         if S.verbose:
             print("verbose! (formerly verbose=%s)" % prev_attrs['verbose'])
 
 *Method `ThreadState.__init__(self, **kw)`*:
-Initiale the `ThreadState`, providing the per-Thread initial values.
+Initiate the `ThreadState`, providing the per-Thread initial values.
+
+*Method `ThreadState.__call__(self, **kw)`*:
+Calling a `ThreadState` returns a context manager which stacks some state.
+The context manager yields the previous values
+for the attributes which were stacked.
 
 ## Function `via(cmanager, func, *a, **kw)`
 
 Return a callable that calls the supplied `func` inside a
 with statement using the context manager `cmanager`.
 This intended use case is aimed at deferred function calls.
 
 # Release Log
 
 
 
+*Release 20240412*:
+* New NRLock, an nonrecursive Lock and associated exception DeadlockError.
+* bg: rename thread_class to thread_factory for clarity.
+* HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
+* HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240303*:
 * HasThreadState: rename thread_states() to get_thread_states().
 * HasThreadState.get_thread_states: some logic fixes.
```

### Comparing `cs.threads-20240316/README.md` & `cs.threads-20240412/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Thread related convenience classes and functions.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+* New NRLock, an nonrecursive Lock and associated exception DeadlockError.
+* bg: rename thread_class to thread_factory for clarity.
+* HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
+* HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
 
 ## Class `AdjustableSemaphore`
 
 A semaphore whose value may be tuned after instantiation.
 
 *Method `AdjustableSemaphore.acquire(self, blocking=True)`*:
 The acquire() method calls the base acquire() method if not blocking.
@@ -25,30 +28,42 @@
 
 If `delta` lowers the semaphore capacity then adjust() may block
 until the overcapacity is released.
 
 *Method `AdjustableSemaphore.release(self)`*:
 Release the semaphore.
 
-## Function `bg(func, daemon=None, name=None, no_start=False, no_logexc=False, thread_class=None, thread_states=None, args=None, kwargs=None)`
+## Function `bg(func, *, daemon=None, name=None, no_start=False, no_logexc=False, args=None, kwargs=None, thread_factory=None, pre_enter_objects=None, **tfkw)`
 
 Dispatch the callable `func` in its own `Thread`;
 return the `Thread`.
 
 Parameters:
 * `func`: a callable for the `Thread` target.
+* `args`, `kwargs`: passed to the `Thread` constructor
+* `kwargs`, `kwargs`: passed to the `Thread` constructor
 * `daemon`: optional argument specifying the `.daemon` attribute.
 * `name`: optional argument specifying the `Thread` name,
   default: the name of `func`.
 * `no_logexc`: if false (default `False`), wrap `func` in `@logexc`.
 * `no_start`: optional argument, default `False`.
   If true, do not start the `Thread`.
-* `thread_class`: the `Thread` factory, default `HasThreadState.Thread`
-* `thread_states`: passed tothe  `thread_class` factory
-* `args`, `kwargs`: passed to the `Thread` constructor
+* `pre_enter_objects`: an optional iterable of objects which
+  should be entered using `with`
+
+If `pre_enter_objects` is supplied, these objects will be
+entered before the `Thread` is started and exited when the
+`Thread` target function ends.
+If the `Thread` is _not_ started (`no_start=True`, very
+unusual) then it will be the caller's responsibility to manage
+to entered objects.
+
+## Class `DeadlockError(builtins.RuntimeError)`
+
+Raised by `NRLock` when a lock is attempted from the `Thread` currently holding the lock.
 
 ## Class `HasThreadState(cs.context.ContextManagerMixin)`
 
 A mixin for classes with a `cs.threads.ThreadState` instance as `.state`
 providing a context manager which pushes `current=self` onto that state
 and a `default()` class method returning `cls.perthread_state.current`
 as the default instance of that class.
@@ -62,55 +77,49 @@
 *NOTE*: `HasThreadState.Thread` is a _class_ method whose default
 is to push state for all active `HasThreadState` subclasses.
 Contrast with `HasThreadState.bg` which is an _instance_method
 whose default is to push state for just that instance.
 The top level `cs.threads.bg` function calls `HasThreadState.Thread`
 to obtain its `Thread`.
 
-*Method `HasThreadState.Thread(*Thread_a, target, thread_states=None, **Thread_kw)`*:
-Class factory for a `Thread` to push the `.current` state for this class.
-
-The optional parameter `thread_states`
-may be used to pass an explicit mapping of `type`->`instance`
-of thread states to use;
-the default states come from `HasThreadState.get_thread_states()`.
-The values of this mapping are iterated over and used as context managers.
-
-A boolean value may also be passed meaning:
-* `False`: do not apply any thread states
-* `True`: apply the default thread states
-
-Note: the default `thread_states` does a `with current:`
-for this class' `current` instance (if any) so that the
-`Thread` holds it open until completed.
-For some worker threads such as `MultiOpenMixin`s consuming
-a queue of tasks this may be undesirable if the instance
-shutdown phase includes a close-and-drain for the queue -
-because the `Thread` holds the instance open, the shutdown
-phase never arrives.
-In this case, pass `thread_states=False` to this call.
+*Method `HasThreadState.Thread(*, name=None, target, enter_objects=None, **Thread_kw)`*:
+Factory for a `Thread` to push the `.current` state for the
+currently active classes.
+
+The optional parameter `enter_objects` may be used to pass
+an iterable of objects whose contexts should be entered
+using `with obj:`.
+If this is set to `True` that indicates that every "current"
+`HasThreadStates` instance should be entered.
+The default does not enter any object contexts.
+The `HasThreadStates.bg` method defaults to passing
+`enter_objects=(self,)` to enter the context for `self`.
 
 *Method `HasThreadState.__enter_exit__(self)`*:
 Push `self.perthread_state.current=self` as the `Thread` local current instance.
 
 Include `self.__class__` in the set of currently active classes for the duration.
 
-*Method `HasThreadState.bg(self, func, *bg_a, thread_states=None, **bg_kw)`*:
-Get a `Thread` using `self.Thread` and start it.
+*Method `HasThreadState.bg(self, func, *, enter_objects=None, pre_enter_objects=None, **bg_kw)`*:
+Get a `Thread` using `type(elf).Thread` and start it.
 Return the `Thread`.
 
-Note: the default `thread_states` is `{type(self): self}`
-in order to arranges a `with self:` so that the `Thread`
-holds it open until completed.
-For some worker threads such as `MultiOpenMixin`s consuming
-a queue of tasks this may be undesirable if the instance
-shutdown phase includes a close-and-drain for the queue -
-because the `Thread` holds the instance open, the shutdown
-phase never arrives.
-In this case, pass `thread_states=False` to this call.
+The `HasThreadState.Thread` factory duplicates the current `Thread`'s
+`HasThreadState` current objects as current in the new `Thread`.
+Additionally it enters the contexts of various objects using
+`with obj` according to the `enter_objects` parameter.
+
+The value of the optional parameter `enter_objects` governs
+which objects have their context entered using `with obj`
+in the child `Thread` while running `func` as follows:
+- `None`: the default, meaning `(self,)`
+- `False`: no object contexts are entered
+- `True`: all current `HasThreadState` object contexts will be entered
+- an iterable of objects whose contexts will be entered;
+  pass `()` to enter no objects
 
 *Method `HasThreadState.default(factory=None, raise_on_None=False)`*:
 The default instance of this class from `cls.perthread_state.current`.
 
 Parameters:
 * `factory`: optional callable to create an instance of `cls`
   if `cls.perthread_state.current` is `None` or missing;
@@ -136,34 +145,28 @@
 
 Parameters:
 * `all_classes`: optional flag, default `False`;
   if true, return a mapping of class to current instance
   for all `HasThreadState` subclasses with an open instance,
   otherwise just a mapping from this class to its current instance
 
-*Method `HasThreadState.with_thread_states(thread_states: Optional[Mapping[type, Any]] = None)`*:
-Context manager to push all the current objects from `thread_states`
-by calling each as a context manager.
-
-The default `thread_states` comes from `HasThreadState.get_thread_states()`.
-
 ## Function `joinif(T: threading.Thread)`
 
 Call `T.join()` if `T` is not the current `Thread`.
 
 Unlike `threading.Thread.join`, this function is a no-op if
 `T` is the current `Thread.
 
 The use case is situations such as the shutdown phase of the
 `MultiOpenMixin.startup_shutdown` context manager. Because
 the "initial open" startup phase is not necessarily run in
 the same thread as the "final close" shutdown phase, it is
 possible for example for a worker `Thread` to execute the
 shutdown phase and try to join itself. Using this function
-allows that scenario.
+supports that scenario.
 
 ## Class `LockableMixin`
 
 Trite mixin to control access to an object via its `._lock` attribute.
 Exposes the `._lock` as the property `.lock`.
 Presents a context manager interface for obtaining an object's lock.
 
@@ -211,14 +214,28 @@
   If omitted, all names commencing with a letter are chosen.
 * `initial_timeout`: optional initial lock timeout, default `10.0`s.
 * `lockattr`: optional lock attribute name, default `'_lock'`.
 
 Only attributes satifying `inspect.ismethod` are wrapped
 because `@locked` requires access to the instance `._lock` attribute.
 
+## Class `NRLock`
+
+A nonrecursive lock.
+Attempting to take this lock when it is already held by the current `Thread`
+will raise `DeadlockError`.
+Otherwise this behaves likc `threading.Lock`.
+
+*Method `NRLock.acquire(self, *a, caller_frame=None, **kw)`*:
+Acquire the lock as for `threading.Lock`.
+Raises `DeadlockError` is the lock is already held by the current `Thread`.
+
+*Method `NRLock.locked(self)`*:
+Return the lock status.
+
 ## Class `PriorityLock`
 
 A priority based mutex which is acquired by and released to waiters
 in priority order.
 
 The initialiser sets a default priority, itself defaulting to `0`.
 
@@ -270,15 +287,15 @@
 
 *Method `PriorityLock.release(self)`*:
 Release the mutex.
 
 Internally, this releases the highest priority `Lock`,
 allowing that `acquire`r to go forward.
 
-## Class `PriorityLockSubLock(PriorityLockSubLock, builtins.tuple)`
+## Class `PriorityLockSubLock(PriorityLockSubLock)`
 
 The record for the per-`acquire`r `Lock` held by `PriorityLock.acquire`.
 
 ## Class `State(_thread._local)`
 
 A `Thread` local object with attributes
 which can be used as a context manager to stack attribute values.
@@ -290,15 +307,15 @@
     S = ThreadState(verbose=False)
 
     with S(verbose=True) as prev_attrs:
         if S.verbose:
             print("verbose! (formerly verbose=%s)" % prev_attrs['verbose'])
 
 *Method `State.__init__(self, **kw)`*:
-Initiale the `ThreadState`, providing the per-Thread initial values.
+Initiate the `ThreadState`, providing the per-Thread initial values.
 
 *Method `State.__call__(self, **kw)`*:
 Calling a `ThreadState` returns a context manager which stacks some state.
 The context manager yields the previous values
 for the attributes which were stacked.
 
 ## Class `ThreadState(_thread._local)`
@@ -313,15 +330,15 @@
     S = ThreadState(verbose=False)
 
     with S(verbose=True) as prev_attrs:
         if S.verbose:
             print("verbose! (formerly verbose=%s)" % prev_attrs['verbose'])
 
 *Method `ThreadState.__init__(self, **kw)`*:
-Initiale the `ThreadState`, providing the per-Thread initial values.
+Initiate the `ThreadState`, providing the per-Thread initial values.
 
 *Method `ThreadState.__call__(self, **kw)`*:
 Calling a `ThreadState` returns a context manager which stacks some state.
 The context manager yields the previous values
 for the attributes which were stacked.
 
 ## Function `via(cmanager, func, *a, **kw)`
@@ -330,14 +347,20 @@
 with statement using the context manager `cmanager`.
 This intended use case is aimed at deferred function calls.
 
 # Release Log
 
 
 
+*Release 20240412*:
+* New NRLock, an nonrecursive Lock and associated exception DeadlockError.
+* bg: rename thread_class to thread_factory for clarity.
+* HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
+* HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240303*:
 * HasThreadState: rename thread_states() to get_thread_states().
 * HasThreadState.get_thread_states: some logic fixes.
```

### Comparing `cs.threads-20240316/lib/python/cs/threads.py` & `cs.threads-20240412/lib/python/cs/threads.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,30 +10,36 @@
 from collections import defaultdict, namedtuple
 from contextlib import contextmanager
 from heapq import heappush, heappop
 from inspect import ismethod
 import sys
 from threading import (
     current_thread,
+    Lock,
     Semaphore,
     Thread as builtin_Thread,
-    Lock,
     local as thread_local,
 )
-from typing import Any, Mapping, Optional
 
-from cs.context import ContextManagerMixin, stackattrs, stackset
+from cs.context import (
+    ContextManagerMixin,
+    stackattrs,
+    stackset,
+    twostep,
+    withall,
+)
 from cs.deco import decorator
 from cs.excutils import logexc, transmute
 from cs.gimmicks import error, warning
 from cs.pfx import Pfx  # prefix
 from cs.py.func import funcname, prop
+from cs.py.stack import caller
 from cs.seq import Seq
 
-__version__ = '20240316'
+__version__ = '20240412'
 
 DISTINFO = {
     'description':
     "threading and communication/synchronisation conveniences",
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
@@ -62,15 +68,15 @@
 
           with S(verbose=True) as prev_attrs:
               if S.verbose:
                   print("verbose! (formerly verbose=%s)" % prev_attrs['verbose'])
   '''
 
   def __init__(self, **kw):
-    ''' Initiale the `ThreadState`, providing the per-Thread initial values.
+    ''' Initiate the `ThreadState`, providing the per-Thread initial values.
     '''
     thread_local.__init__(self)
     for k, v in kw.items():
       setattr(self, k, v)
 
   def __str__(self):
     return "%s(%s)" % (
@@ -199,161 +205,197 @@
         # just the current instance of the calling class
         currency = {
             cls: getattr(getattr(cls, cls.THREAD_STATE_ATTR, 'current'), None)
         }
     return currency
 
   @classmethod
-  @contextmanager
-  def with_thread_states(
-      cls, thread_states: Optional[Mapping[type, Any]] = None
+  def Thread(
+      cls,
+      *,
+      name=None,
+      target,
+      enter_objects=None,
+      **Thread_kw,
   ):
-    ''' Context manager to push all the current objects from `thread_states`
-        by calling each as a context manager.
+    ''' Factory for a `Thread` to push the `.current` state for the
+        currently active classes.
 
-        The default `thread_states` comes from `HasThreadState.get_thread_states()`.
+        The optional parameter `enter_objects` may be used to pass
+        an iterable of objects whose contexts should be entered
+        using `with obj:`.
+        If this is set to `True` that indicates that every "current"
+        `HasThreadStates` instance should be entered.
+        The default does not enter any object contexts.
+        The `HasThreadStates.bg` method defaults to passing
+        `enter_objects=(self,)` to enter the context for `self`.
     '''
-    if thread_states is None or isinstance(thread_states, bool):
-      thread_states = cls.get_thread_states(all_classes=thread_states)
-    if not thread_states:
-      yield
+    if name is None:
+      name = funcname(target)
+    if enter_objects is True:
+      # the bool True means enter all the state objects, marked as for-with
+      enter_tuples = (
+          (
+              getattr(
+                  getattr(htscls, htscls.THREAD_STATE_ATTR), 'current', None
+              ), True
+          ) for htscls in HasThreadState._HasThreadState_classes
+      )
     else:
-      state_iter = iter(list(thread_states.values()))
+      enter_tuples = (
+          # all the current objects, marked as not-for-with
+          [
+              (
+                  getattr(
+                      getattr(htscls, htscls.THREAD_STATE_ATTR), 'current',
+                      None
+                  ), False
+              ) for htscls in HasThreadState._HasThreadState_classes
+          ] +
+          # the enter_objects, marked as for-with
+          [(obj, True) for obj in enter_objects or ()]
+      )
+    enter_it = iter(enter_tuples)
 
-      def with_thread_states_pusher():
-        try:
-          htsobj = next(state_iter)
-        except StopIteration:
-          yield
+    def with_enter_objects():
+      ''' A recursive context manager to enter all the contexts
+          implied by `enter_it`.
+          For each `(enter_obj,for_with)` in `enter_it`, if `for_with`
+          is true, enter the object using `with enter_obj:` otherwise
+          enter using: `with enter_object.per_thread_state(current=enter_obj)`.
+      '''
+      try:
+        enter_obj, for_with = next(enter_it)
+      except StopIteration:
+        yield
+      else:
+        if enter_obj is None:
+          # no current object, skip to the next one
+          yield from with_enter_objects()
         else:
-          if htsobj is None:
-            # no current object, skip to the next class
-            yield from with_thread_states_pusher()
+          if for_with:
+            print("WITH enter_obj", enter_obj)
+            with enter_obj:
+              yield from with_enter_objects()
           else:
-            with htsobj:
-              yield from with_thread_states_pusher()
+            thread_state = getattr(enter_obj, enter_obj.THREAD_STATE_ATTR)
+            with thread_state(curret=enter_obj):
+              yield from with_enter_objects()
+
+    def target_wrapper(*a, **kw):
+      ''' Wrapper for the `Thread.target` to push the current states
+          from `enter_it` in the new Thread before running the `target`.
+      '''
+      with contextmanager(with_enter_objects)():
+        return target(*a, **kw)
 
-      yield from with_thread_states_pusher()
+    return builtin_Thread(name=name, target=target_wrapper, **Thread_kw)
 
-  @classmethod
-  def Thread(cls, *Thread_a, target, thread_states=None, **Thread_kw):
-    ''' Class factory for a `Thread` to push the `.current` state for this class.
-
-        The optional parameter `thread_states`
-        may be used to pass an explicit mapping of `type`->`instance`
-        of thread states to use;
-        the default states come from `HasThreadState.get_thread_states()`.
-        The values of this mapping are iterated over and used as context managers.
-
-        A boolean value may also be passed meaning:
-        * `False`: do not apply any thread states
-        * `True`: apply the default thread states
-
-        Note: the default `thread_states` does a `with current:`
-        for this class' `current` instance (if any) so that the
-        `Thread` holds it open until completed.
-        For some worker threads such as `MultiOpenMixin`s consuming
-        a queue of tasks this may be undesirable if the instance
-        shutdown phase includes a close-and-drain for the queue -
-        because the `Thread` holds the instance open, the shutdown
-        phase never arrives.
-        In this case, pass `thread_states=False` to this call.
-    '''
-    # snapshot the .current states in the source Thread
-    if thread_states is None:
-      thread_states = False
-    if isinstance(thread_states, bool):
-      thread_states = cls.get_thread_states(all_classes=thread_states)
-    if thread_states:
-
-      def target_wrapper(*a, **kw):
-        ''' Wrapper for the `Thread.target` to push the source `.current`
-            states in the new Thread before running the target.
-        '''
-        with cls.with_thread_states(thread_states):
-          return target(*a, **kw)
-    else:
-      # no state to prepare, eschew the wrapper
-      target_wrapper = target
-
-    return builtin_Thread(*Thread_a, target=target_wrapper, **Thread_kw)
-
-  def bg(self, func, *bg_a, thread_states=None, **bg_kw):
-    ''' Get a `Thread` using `self.Thread` and start it.
+  def bg(self, func, *, enter_objects=None, pre_enter_objects=None, **bg_kw):
+    ''' Get a `Thread` using `type(elf).Thread` and start it.
         Return the `Thread`.
 
-        Note: the default `thread_states` is `{type(self): self}`
-        in order to arranges a `with self:` so that the `Thread`
-        holds it open until completed.
-        For some worker threads such as `MultiOpenMixin`s consuming
-        a queue of tasks this may be undesirable if the instance
-        shutdown phase includes a close-and-drain for the queue -
-        because the `Thread` holds the instance open, the shutdown
-        phase never arrives.
-        In this case, pass `thread_states=False` to this call.
+        The `HasThreadState.Thread` factory duplicates the current `Thread`'s
+        `HasThreadState` current objects as current in the new `Thread`.
+        Additionally it enters the contexts of various objects using
+        `with obj` according to the `enter_objects` parameter.
+
+        The value of the optional parameter `enter_objects` governs
+        which objects have their context entered using `with obj`
+        in the child `Thread` while running `func` as follows:
+        - `None`: the default, meaning `(self,)`
+        - `False`: no object contexts are entered
+        - `True`: all current `HasThreadState` object contexts will be entered
+        - an iterable of objects whose contexts will be entered;
+          pass `()` to enter no objects
     '''
     cls = type(self)
-    if thread_states is None:
-      thread_states = {cls: self}
+    if enter_objects is None:
+      enter_objects = (self,)
     return bg(
-        func, *bg_a, thread_states=thread_states, thread_class=cls, **bg_kw
+        func,
+        thread_factory=cls.Thread,
+        enter_objects=enter_objects,
+        **bg_kw,
     )
 
 # pylint: disable=too-many-arguments
 def bg(
     func,
+    *,
     daemon=None,
     name=None,
     no_start=False,
     no_logexc=False,
-    thread_class=None,
-    thread_states=None,
     args=None,
     kwargs=None,
+    thread_factory=None,
+    pre_enter_objects=None,
+    **tfkw,
 ):
   ''' Dispatch the callable `func` in its own `Thread`;
       return the `Thread`.
 
       Parameters:
       * `func`: a callable for the `Thread` target.
+      * `args`, `kwargs`: passed to the `Thread` constructor
+      * `kwargs`, `kwargs`: passed to the `Thread` constructor
       * `daemon`: optional argument specifying the `.daemon` attribute.
       * `name`: optional argument specifying the `Thread` name,
         default: the name of `func`.
       * `no_logexc`: if false (default `False`), wrap `func` in `@logexc`.
       * `no_start`: optional argument, default `False`.
         If true, do not start the `Thread`.
-      * `thread_class`: the `Thread` factory, default `HasThreadState.Thread`
-      * `thread_states`: passed tothe  `thread_class` factory
-      * `args`, `kwargs`: passed to the `Thread` constructor
+      * `pre_enter_objects`: an optional iterable of objects which
+        should be entered using `with`
+
+      If `pre_enter_objects` is supplied, these objects will be
+      entered before the `Thread` is started and exited when the
+      `Thread` target function ends.
+      If the `Thread` is _not_ started (`no_start=True`, very
+      unusual) then it will be the caller's responsibility to manage
+      to entered objects.
   '''
   if name is None:
     name = funcname(func)
   if args is None:
     args = ()
   if kwargs is None:
     kwargs = {}
-  if thread_class is None:
-    thread_class = HasThreadState.Thread
-
+  if thread_factory is None:
+    thread_factory = HasThreadState.Thread
   ##thread_prefix = prefix() + ': ' + name
   thread_prefix = name
+  preopen_close_it = None
 
   def thread_body():
-    with Pfx(thread_prefix):
-      return func(*args, **kwargs)
+    ''' Establish a basic `Pfx` context for the target `func`.
+    '''
+    try:
+      with Pfx("Thread:%d:%s", current_thread().ident, thread_prefix):
+        return func(*args, **kwargs)
+    finally:
+      if preopen_close_it is not None:
+        # do the closes
+        next(preopen_close_it)
 
-  T = thread_class(
+  T = thread_factory(
       name=thread_prefix,
       target=thread_body,
-      thread_states=thread_states,
+      **tfkw,
   )
   if not no_logexc:
     func = logexc(func)
   if daemon is not None:
     T.daemon = daemon
+  if pre_enter_objects:
+    # prepare a context manager to open all the pre_enter_objects
+    preopen_close_it = twostep(withall(pre_enter_objects))
+    # do the opens
+    next(preopen_close_it)
   if not no_start:
     T.start()
   return T
 
 def joinif(T: builtin_Thread):
   ''' Call `T.join()` if `T` is not the current `Thread`.
 
@@ -362,15 +404,15 @@
 
       The use case is situations such as the shutdown phase of the
       `MultiOpenMixin.startup_shutdown` context manager. Because
       the "initial open" startup phase is not necessarily run in
       the same thread as the "final close" shutdown phase, it is
       possible for example for a worker `Thread` to execute the
       shutdown phase and try to join itself. Using this function
-      allows that scenario.
+      supports that scenario.
   '''
   if T is not current_thread():
     T.join()
 
 class AdjustableSemaphore(object):
   ''' A semaphore whose value may be tuned after instantiation.
   '''
@@ -731,10 +773,67 @@
     if ismethod(method):
       setattr(
           cls, name,
           locked(method, initial_timeout=initial_timeout, lockattr=lockattr)
       )
   return cls
 
+class DeadlockError(RuntimeError):
+  ''' Raised by `NRLock` when a lock is attempted from the `Thread` currently holding the lock.
+  '''
+
+class NRLock:
+  ''' A nonrecursive lock.
+      Attempting to take this lock when it is already held by the current `Thread`
+      will raise `DeadlockError`.
+      Otherwise this behaves likc `threading.Lock`.
+  '''
+
+  __slots__ = ('_lock', '_lock_thread', '_locked_by')
+
+  def __init__(self):
+    self._lock = Lock()
+    self._lock_thread = None
+    self._locked_by = None
+
+  def __repr__(self):
+    return (
+        f'{self.__class__.__name__}:{self._lock}:{self._lock_thread}:{self._locked_by}'
+        if self.locked() else f'{self.__class__.__name__}:{self._lock}'
+    )
+
+  def locked(self):
+    ''' Return the lock status.
+    '''
+    return self._lock.locked()
+
+  def acquire(self, *a, caller_frame=None, **kw):
+    ''' Acquire the lock as for `threading.Lock`.
+        Raises `DeadlockError` is the lock is already held by the current `Thread`.
+    '''
+    lock = self._lock
+    if lock.locked() and current_thread() is self._lock_thread:
+      raise DeadlockError('lock already held by current Thread')
+    acquired = lock.acquire(*a, **kw)
+    if acquired:
+      if caller_frame is None:
+        caller_frame = caller()
+      self._lock_thread = current_thread()
+      self._locked_by = caller_frame
+    return acquired
+
+  def release(self):
+    self._lock.release()
+    self._lock_thread = None
+    self._locked_by = None
+
+  def __enter__(self):
+    acquired = self.acquire(caller_frame=caller())
+    assert acquired
+    return acquired
+
+  def __exit__(self, *_):
+    self.release()
+
 if __name__ == '__main__':
   import cs.threads_tests
   cs.threads_tests.selftest(sys.argv)
```

### Comparing `cs.threads-20240316/lib/python/cs.threads.egg-info/PKG-INFO` & `cs.threads-20240412/lib/python/cs.threads.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.threads
-Version: 20240316
+Version: 20240412
 Summary: threading and communication/synchronisation conveniences
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,37 +14,74 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Thread related convenience classes and functions.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+* New NRLock, an nonrecursive Lock and associated exception DeadlockError.
+* bg: rename thread_class to thread_factory for clarity.
+* HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
+* HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
 
 ## Class `AdjustableSemaphore`
 
 A semaphore whose value may be tuned after instantiation.
 
-## Function `bg(func, daemon=None, name=None, no_start=False, no_logexc=False, thread_class=None, thread_states=None, args=None, kwargs=None)`
+*Method `AdjustableSemaphore.acquire(self, blocking=True)`*:
+The acquire() method calls the base acquire() method if not blocking.
+If blocking is true, the base acquire() is called inside a lock to
+avoid competing with a reducing adjust().
+
+*Method `AdjustableSemaphore.adjust(self, newvalue)`*:
+Set capacity to `newvalue`
+by calling release() or acquire() an appropriate number of times.
+
+If `newvalue` lowers the semaphore capacity then adjust()
+may block until the overcapacity is released.
+
+*Method `AdjustableSemaphore.adjust_delta(self, delta)`*:
+Adjust capacity by `delta` by calling release() or acquire()
+an appropriate number of times.
+
+If `delta` lowers the semaphore capacity then adjust() may block
+until the overcapacity is released.
+
+*Method `AdjustableSemaphore.release(self)`*:
+Release the semaphore.
+
+## Function `bg(func, *, daemon=None, name=None, no_start=False, no_logexc=False, args=None, kwargs=None, thread_factory=None, pre_enter_objects=None, **tfkw)`
 
 Dispatch the callable `func` in its own `Thread`;
 return the `Thread`.
 
 Parameters:
 * `func`: a callable for the `Thread` target.
+* `args`, `kwargs`: passed to the `Thread` constructor
+* `kwargs`, `kwargs`: passed to the `Thread` constructor
 * `daemon`: optional argument specifying the `.daemon` attribute.
 * `name`: optional argument specifying the `Thread` name,
   default: the name of `func`.
 * `no_logexc`: if false (default `False`), wrap `func` in `@logexc`.
 * `no_start`: optional argument, default `False`.
   If true, do not start the `Thread`.
-* `thread_class`: the `Thread` factory, default `HasThreadState.Thread`
-* `thread_states`: passed tothe  `thread_class` factory
-* `args`, `kwargs`: passed to the `Thread` constructor
+* `pre_enter_objects`: an optional iterable of objects which
+  should be entered using `with`
+
+If `pre_enter_objects` is supplied, these objects will be
+entered before the `Thread` is started and exited when the
+`Thread` target function ends.
+If the `Thread` is _not_ started (`no_start=True`, very
+unusual) then it will be the caller's responsibility to manage
+to entered objects.
+
+## Class `DeadlockError(builtins.RuntimeError)`
+
+Raised by `NRLock` when a lock is attempted from the `Thread` currently holding the lock.
 
 ## Class `HasThreadState(cs.context.ContextManagerMixin)`
 
 A mixin for classes with a `cs.threads.ThreadState` instance as `.state`
 providing a context manager which pushes `current=self` onto that state
 and a `default()` class method returning `cls.perthread_state.current`
 as the default instance of that class.
@@ -58,35 +95,109 @@
 *NOTE*: `HasThreadState.Thread` is a _class_ method whose default
 is to push state for all active `HasThreadState` subclasses.
 Contrast with `HasThreadState.bg` which is an _instance_method
 whose default is to push state for just that instance.
 The top level `cs.threads.bg` function calls `HasThreadState.Thread`
 to obtain its `Thread`.
 
+*Method `HasThreadState.Thread(*, name=None, target, enter_objects=None, **Thread_kw)`*:
+Factory for a `Thread` to push the `.current` state for the
+currently active classes.
+
+The optional parameter `enter_objects` may be used to pass
+an iterable of objects whose contexts should be entered
+using `with obj:`.
+If this is set to `True` that indicates that every "current"
+`HasThreadStates` instance should be entered.
+The default does not enter any object contexts.
+The `HasThreadStates.bg` method defaults to passing
+`enter_objects=(self,)` to enter the context for `self`.
+
+*Method `HasThreadState.__enter_exit__(self)`*:
+Push `self.perthread_state.current=self` as the `Thread` local current instance.
+
+Include `self.__class__` in the set of currently active classes for the duration.
+
+*Method `HasThreadState.bg(self, func, *, enter_objects=None, pre_enter_objects=None, **bg_kw)`*:
+Get a `Thread` using `type(elf).Thread` and start it.
+Return the `Thread`.
+
+The `HasThreadState.Thread` factory duplicates the current `Thread`'s
+`HasThreadState` current objects as current in the new `Thread`.
+Additionally it enters the contexts of various objects using
+`with obj` according to the `enter_objects` parameter.
+
+The value of the optional parameter `enter_objects` governs
+which objects have their context entered using `with obj`
+in the child `Thread` while running `func` as follows:
+- `None`: the default, meaning `(self,)`
+- `False`: no object contexts are entered
+- `True`: all current `HasThreadState` object contexts will be entered
+- an iterable of objects whose contexts will be entered;
+  pass `()` to enter no objects
+
+*Method `HasThreadState.default(factory=None, raise_on_None=False)`*:
+The default instance of this class from `cls.perthread_state.current`.
+
+Parameters:
+* `factory`: optional callable to create an instance of `cls`
+  if `cls.perthread_state.current` is `None` or missing;
+  if `factory` is `True` then `cls` is used as the factory
+* `raise_on_None`: if `cls.perthread_state.current` is `None` or missing
+  and `factory` is false and `raise_on_None` is true,
+  raise a `RuntimeError`;
+  this is primarily a debugging aid
+
+*Method `HasThreadState.get_thread_states(all_classes=None)`*:
+Return a mapping of `class`->*current_instance*`
+for use with `HasThreadState.with_thread_states`
+or `HasThreadState.Thread` or `HasThreadState.bg`.
+
+The default behaviour returns just a mapping for this class,
+expecting the default instance to be responsible for what
+other resources it holds.
+
+There is also a legacy mode for `all_classes=True`
+where the mapping is for all active classes,
+probably best used for `Thread`s spawned outside
+a `HasThreadState` context.
+
+Parameters:
+* `all_classes`: optional flag, default `False`;
+  if true, return a mapping of class to current instance
+  for all `HasThreadState` subclasses with an open instance,
+  otherwise just a mapping from this class to its current instance
+
 ## Function `joinif(T: threading.Thread)`
 
 Call `T.join()` if `T` is not the current `Thread`.
 
 Unlike `threading.Thread.join`, this function is a no-op if
 `T` is the current `Thread.
 
 The use case is situations such as the shutdown phase of the
 `MultiOpenMixin.startup_shutdown` context manager. Because
 the "initial open" startup phase is not necessarily run in
 the same thread as the "final close" shutdown phase, it is
 possible for example for a worker `Thread` to execute the
 shutdown phase and try to join itself. Using this function
-allows that scenario.
+supports that scenario.
 
 ## Class `LockableMixin`
 
 Trite mixin to control access to an object via its `._lock` attribute.
 Exposes the `._lock` as the property `.lock`.
 Presents a context manager interface for obtaining an object's lock.
 
+*Method `LockableMixin.__exit__(self, exc_type, exc_value, traceback)`*:
+pylint: disable=unused-argument
+
+*Property `LockableMixin.lock`*:
+Return the lock.
+
 ## Function `locked(*da, **dkw)`
 
 A decorator for instance methods that must run within a lock.
 
 Decorator keyword arguments:
 * `initial_timeout`:
   the initial lock attempt timeout;
@@ -121,14 +232,28 @@
   If omitted, all names commencing with a letter are chosen.
 * `initial_timeout`: optional initial lock timeout, default `10.0`s.
 * `lockattr`: optional lock attribute name, default `'_lock'`.
 
 Only attributes satifying `inspect.ismethod` are wrapped
 because `@locked` requires access to the instance `._lock` attribute.
 
+## Class `NRLock`
+
+A nonrecursive lock.
+Attempting to take this lock when it is already held by the current `Thread`
+will raise `DeadlockError`.
+Otherwise this behaves likc `threading.Lock`.
+
+*Method `NRLock.acquire(self, *a, caller_frame=None, **kw)`*:
+Acquire the lock as for `threading.Lock`.
+Raises `DeadlockError` is the lock is already held by the current `Thread`.
+
+*Method `NRLock.locked(self)`*:
+Return the lock status.
+
 ## Class `PriorityLock`
 
 A priority based mutex which is acquired by and released to waiters
 in priority order.
 
 The initialiser sets a default priority, itself defaulting to `0`.
 
@@ -156,15 +281,39 @@
 Initialise the `PriorityLock`.
 
 Parameters:
 * `default_priority`: the default `acquire` priority,
   default `0`.
 * `name`: optional identifying name
 
-## Class `PriorityLockSubLock(PriorityLockSubLock, builtins.tuple)`
+*Method `PriorityLock.__enter__(self)`*:
+Enter the mutex as a context manager at the default priority.
+Returns the new `Lock`.
+
+*Method `PriorityLock.__exit__(self, *_)`*:
+Exit the context manager.
+
+*Method `PriorityLock.acquire(self, priority=None)`*:
+Acquire the mutex with `priority` (default from `default_priority`).
+Return the new `PriorityLockSubLock`.
+
+This blocks behind any higher priority `acquire`s
+or any earlier `acquire`s of the same priority.
+
+*Method `PriorityLock.priority(self, this_priority)`*:
+A context manager with the specified `this_priority`.
+Returns the new `Lock`.
+
+*Method `PriorityLock.release(self)`*:
+Release the mutex.
+
+Internally, this releases the highest priority `Lock`,
+allowing that `acquire`r to go forward.
+
+## Class `PriorityLockSubLock(PriorityLockSubLock)`
 
 The record for the per-`acquire`r `Lock` held by `PriorityLock.acquire`.
 
 ## Class `State(_thread._local)`
 
 A `Thread` local object with attributes
 which can be used as a context manager to stack attribute values.
@@ -176,15 +325,20 @@
     S = ThreadState(verbose=False)
 
     with S(verbose=True) as prev_attrs:
         if S.verbose:
             print("verbose! (formerly verbose=%s)" % prev_attrs['verbose'])
 
 *Method `State.__init__(self, **kw)`*:
-Initiale the `ThreadState`, providing the per-Thread initial values.
+Initiate the `ThreadState`, providing the per-Thread initial values.
+
+*Method `State.__call__(self, **kw)`*:
+Calling a `ThreadState` returns a context manager which stacks some state.
+The context manager yields the previous values
+for the attributes which were stacked.
 
 ## Class `ThreadState(_thread._local)`
 
 A `Thread` local object with attributes
 which can be used as a context manager to stack attribute values.
 
 Example:
@@ -194,26 +348,37 @@
     S = ThreadState(verbose=False)
 
     with S(verbose=True) as prev_attrs:
         if S.verbose:
             print("verbose! (formerly verbose=%s)" % prev_attrs['verbose'])
 
 *Method `ThreadState.__init__(self, **kw)`*:
-Initiale the `ThreadState`, providing the per-Thread initial values.
+Initiate the `ThreadState`, providing the per-Thread initial values.
+
+*Method `ThreadState.__call__(self, **kw)`*:
+Calling a `ThreadState` returns a context manager which stacks some state.
+The context manager yields the previous values
+for the attributes which were stacked.
 
 ## Function `via(cmanager, func, *a, **kw)`
 
 Return a callable that calls the supplied `func` inside a
 with statement using the context manager `cmanager`.
 This intended use case is aimed at deferred function calls.
 
 # Release Log
 
 
 
+*Release 20240412*:
+* New NRLock, an nonrecursive Lock and associated exception DeadlockError.
+* bg: rename thread_class to thread_factory for clarity.
+* HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
+* HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240303*:
 * HasThreadState: rename thread_states() to get_thread_states().
 * HasThreadState.get_thread_states: some logic fixes.
```

### Comparing `cs.threads-20240316/pyproject.toml` & `cs.threads-20240412/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -5,66 +5,103 @@
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python2",
     "python3",
 ]
 dependencies = [
-    "cs.context>=20240316",
-    "cs.deco>=20240316",
+    "cs.context>=20240412",
+    "cs.deco>=20240412",
     "cs.excutils>=20230212.1",
     "cs.gimmicks>=20240316",
-    "cs.pfx>=20230604",
+    "cs.pfx>=20240412",
     "cs.py.func>=20230331",
     "cs.seq>=20221118",
 ]
 classifiers = [
     "Programming Language :: Python",
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
 Thread related convenience classes and functions.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+* New NRLock, an nonrecursive Lock and associated exception DeadlockError.
+* bg: rename thread_class to thread_factory for clarity.
+* HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
+* HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
 
 ## Class `AdjustableSemaphore`
 
 A semaphore whose value may be tuned after instantiation.
 
-## Function `bg(func, daemon=None, name=None, no_start=False, no_logexc=False, thread_class=None, thread_states=None, args=None, kwargs=None)`
+*Method `AdjustableSemaphore.acquire(self, blocking=True)`*:
+The acquire() method calls the base acquire() method if not blocking.
+If blocking is true, the base acquire() is called inside a lock to
+avoid competing with a reducing adjust().
+
+*Method `AdjustableSemaphore.adjust(self, newvalue)`*:
+Set capacity to `newvalue`
+by calling release() or acquire() an appropriate number of times.
+
+If `newvalue` lowers the semaphore capacity then adjust()
+may block until the overcapacity is released.
+
+*Method `AdjustableSemaphore.adjust_delta(self, delta)`*:
+Adjust capacity by `delta` by calling release() or acquire()
+an appropriate number of times.
+
+If `delta` lowers the semaphore capacity then adjust() may block
+until the overcapacity is released.
+
+*Method `AdjustableSemaphore.release(self)`*:
+Release the semaphore.
+
+## Function `bg(func, *, daemon=None, name=None, no_start=False, no_logexc=False, args=None, kwargs=None, thread_factory=None, pre_enter_objects=None, **tfkw)`
 
 Dispatch the callable `func` in its own `Thread`;
 return the `Thread`.
 
 Parameters:
 * `func`: a callable for the `Thread` target.
+* `args`, `kwargs`: passed to the `Thread` constructor
+* `kwargs`, `kwargs`: passed to the `Thread` constructor
 * `daemon`: optional argument specifying the `.daemon` attribute.
 * `name`: optional argument specifying the `Thread` name,
   default: the name of `func`.
 * `no_logexc`: if false (default `False`), wrap `func` in `@logexc`.
 * `no_start`: optional argument, default `False`.
   If true, do not start the `Thread`.
-* `thread_class`: the `Thread` factory, default `HasThreadState.Thread`
-* `thread_states`: passed tothe  `thread_class` factory
-* `args`, `kwargs`: passed to the `Thread` constructor
+* `pre_enter_objects`: an optional iterable of objects which
+  should be entered using `with`
+
+If `pre_enter_objects` is supplied, these objects will be
+entered before the `Thread` is started and exited when the
+`Thread` target function ends.
+If the `Thread` is _not_ started (`no_start=True`, very
+unusual) then it will be the caller's responsibility to manage
+to entered objects.
+
+## Class `DeadlockError(builtins.RuntimeError)`
+
+Raised by `NRLock` when a lock is attempted from the `Thread` currently holding the lock.
 
 ## Class `HasThreadState(cs.context.ContextManagerMixin)`
 
 A mixin for classes with a `cs.threads.ThreadState` instance as `.state`
 providing a context manager which pushes `current=self` onto that state
 and a `default()` class method returning `cls.perthread_state.current`
 as the default instance of that class.
@@ -78,35 +115,109 @@
 *NOTE*: `HasThreadState.Thread` is a _class_ method whose default
 is to push state for all active `HasThreadState` subclasses.
 Contrast with `HasThreadState.bg` which is an _instance_method
 whose default is to push state for just that instance.
 The top level `cs.threads.bg` function calls `HasThreadState.Thread`
 to obtain its `Thread`.
 
+*Method `HasThreadState.Thread(*, name=None, target, enter_objects=None, **Thread_kw)`*:
+Factory for a `Thread` to push the `.current` state for the
+currently active classes.
+
+The optional parameter `enter_objects` may be used to pass
+an iterable of objects whose contexts should be entered
+using `with obj:`.
+If this is set to `True` that indicates that every \"current\"
+`HasThreadStates` instance should be entered.
+The default does not enter any object contexts.
+The `HasThreadStates.bg` method defaults to passing
+`enter_objects=(self,)` to enter the context for `self`.
+
+*Method `HasThreadState.__enter_exit__(self)`*:
+Push `self.perthread_state.current=self` as the `Thread` local current instance.
+
+Include `self.__class__` in the set of currently active classes for the duration.
+
+*Method `HasThreadState.bg(self, func, *, enter_objects=None, pre_enter_objects=None, **bg_kw)`*:
+Get a `Thread` using `type(elf).Thread` and start it.
+Return the `Thread`.
+
+The `HasThreadState.Thread` factory duplicates the current `Thread`'s
+`HasThreadState` current objects as current in the new `Thread`.
+Additionally it enters the contexts of various objects using
+`with obj` according to the `enter_objects` parameter.
+
+The value of the optional parameter `enter_objects` governs
+which objects have their context entered using `with obj`
+in the child `Thread` while running `func` as follows:
+- `None`: the default, meaning `(self,)`
+- `False`: no object contexts are entered
+- `True`: all current `HasThreadState` object contexts will be entered
+- an iterable of objects whose contexts will be entered;
+  pass `()` to enter no objects
+
+*Method `HasThreadState.default(factory=None, raise_on_None=False)`*:
+The default instance of this class from `cls.perthread_state.current`.
+
+Parameters:
+* `factory`: optional callable to create an instance of `cls`
+  if `cls.perthread_state.current` is `None` or missing;
+  if `factory` is `True` then `cls` is used as the factory
+* `raise_on_None`: if `cls.perthread_state.current` is `None` or missing
+  and `factory` is false and `raise_on_None` is true,
+  raise a `RuntimeError`;
+  this is primarily a debugging aid
+
+*Method `HasThreadState.get_thread_states(all_classes=None)`*:
+Return a mapping of `class`->*current_instance*`
+for use with `HasThreadState.with_thread_states`
+or `HasThreadState.Thread` or `HasThreadState.bg`.
+
+The default behaviour returns just a mapping for this class,
+expecting the default instance to be responsible for what
+other resources it holds.
+
+There is also a legacy mode for `all_classes=True`
+where the mapping is for all active classes,
+probably best used for `Thread`s spawned outside
+a `HasThreadState` context.
+
+Parameters:
+* `all_classes`: optional flag, default `False`;
+  if true, return a mapping of class to current instance
+  for all `HasThreadState` subclasses with an open instance,
+  otherwise just a mapping from this class to its current instance
+
 ## Function `joinif(T: threading.Thread)`
 
 Call `T.join()` if `T` is not the current `Thread`.
 
 Unlike `threading.Thread.join`, this function is a no-op if
 `T` is the current `Thread.
 
 The use case is situations such as the shutdown phase of the
 `MultiOpenMixin.startup_shutdown` context manager. Because
 the \"initial open\" startup phase is not necessarily run in
 the same thread as the \"final close\" shutdown phase, it is
 possible for example for a worker `Thread` to execute the
 shutdown phase and try to join itself. Using this function
-allows that scenario.
+supports that scenario.
 
 ## Class `LockableMixin`
 
 Trite mixin to control access to an object via its `._lock` attribute.
 Exposes the `._lock` as the property `.lock`.
 Presents a context manager interface for obtaining an object's lock.
 
+*Method `LockableMixin.__exit__(self, exc_type, exc_value, traceback)`*:
+pylint: disable=unused-argument
+
+*Property `LockableMixin.lock`*:
+Return the lock.
+
 ## Function `locked(*da, **dkw)`
 
 A decorator for instance methods that must run within a lock.
 
 Decorator keyword arguments:
 * `initial_timeout`:
   the initial lock attempt timeout;
@@ -141,14 +252,28 @@
   If omitted, all names commencing with a letter are chosen.
 * `initial_timeout`: optional initial lock timeout, default `10.0`s.
 * `lockattr`: optional lock attribute name, default `'_lock'`.
 
 Only attributes satifying `inspect.ismethod` are wrapped
 because `@locked` requires access to the instance `._lock` attribute.
 
+## Class `NRLock`
+
+A nonrecursive lock.
+Attempting to take this lock when it is already held by the current `Thread`
+will raise `DeadlockError`.
+Otherwise this behaves likc `threading.Lock`.
+
+*Method `NRLock.acquire(self, *a, caller_frame=None, **kw)`*:
+Acquire the lock as for `threading.Lock`.
+Raises `DeadlockError` is the lock is already held by the current `Thread`.
+
+*Method `NRLock.locked(self)`*:
+Return the lock status.
+
 ## Class `PriorityLock`
 
 A priority based mutex which is acquired by and released to waiters
 in priority order.
 
 The initialiser sets a default priority, itself defaulting to `0`.
 
@@ -176,15 +301,39 @@
 Initialise the `PriorityLock`.
 
 Parameters:
 * `default_priority`: the default `acquire` priority,
   default `0`.
 * `name`: optional identifying name
 
-## Class `PriorityLockSubLock(PriorityLockSubLock, builtins.tuple)`
+*Method `PriorityLock.__enter__(self)`*:
+Enter the mutex as a context manager at the default priority.
+Returns the new `Lock`.
+
+*Method `PriorityLock.__exit__(self, *_)`*:
+Exit the context manager.
+
+*Method `PriorityLock.acquire(self, priority=None)`*:
+Acquire the mutex with `priority` (default from `default_priority`).
+Return the new `PriorityLockSubLock`.
+
+This blocks behind any higher priority `acquire`s
+or any earlier `acquire`s of the same priority.
+
+*Method `PriorityLock.priority(self, this_priority)`*:
+A context manager with the specified `this_priority`.
+Returns the new `Lock`.
+
+*Method `PriorityLock.release(self)`*:
+Release the mutex.
+
+Internally, this releases the highest priority `Lock`,
+allowing that `acquire`r to go forward.
+
+## Class `PriorityLockSubLock(PriorityLockSubLock)`
 
 The record for the per-`acquire`r `Lock` held by `PriorityLock.acquire`.
 
 ## Class `State(_thread._local)`
 
 A `Thread` local object with attributes
 which can be used as a context manager to stack attribute values.
@@ -196,15 +345,20 @@
     S = ThreadState(verbose=False)
 
     with S(verbose=True) as prev_attrs:
         if S.verbose:
             print(\"verbose! (formerly verbose=%s)\" % prev_attrs['verbose'])
 
 *Method `State.__init__(self, **kw)`*:
-Initiale the `ThreadState`, providing the per-Thread initial values.
+Initiate the `ThreadState`, providing the per-Thread initial values.
+
+*Method `State.__call__(self, **kw)`*:
+Calling a `ThreadState` returns a context manager which stacks some state.
+The context manager yields the previous values
+for the attributes which were stacked.
 
 ## Class `ThreadState(_thread._local)`
 
 A `Thread` local object with attributes
 which can be used as a context manager to stack attribute values.
 
 Example:
@@ -214,26 +368,37 @@
     S = ThreadState(verbose=False)
 
     with S(verbose=True) as prev_attrs:
         if S.verbose:
             print(\"verbose! (formerly verbose=%s)\" % prev_attrs['verbose'])
 
 *Method `ThreadState.__init__(self, **kw)`*:
-Initiale the `ThreadState`, providing the per-Thread initial values.
+Initiate the `ThreadState`, providing the per-Thread initial values.
+
+*Method `ThreadState.__call__(self, **kw)`*:
+Calling a `ThreadState` returns a context manager which stacks some state.
+The context manager yields the previous values
+for the attributes which were stacked.
 
 ## Function `via(cmanager, func, *a, **kw)`
 
 Return a callable that calls the supplied `func` inside a
 with statement using the context manager `cmanager`.
 This intended use case is aimed at deferred function calls.
 
 # Release Log
 
 
 
+*Release 20240412*:
+* New NRLock, an nonrecursive Lock and associated exception DeadlockError.
+* bg: rename thread_class to thread_factory for clarity.
+* HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
+* HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240303*:
 * HasThreadState: rename thread_states() to get_thread_states().
 * HasThreadState.get_thread_states: some logic fixes.
```

