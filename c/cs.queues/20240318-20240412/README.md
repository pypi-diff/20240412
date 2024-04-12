# Comparing `tmp/cs.queues-20240318.tar.gz` & `tmp/cs.queues-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.queues-20240318.tar", last modified: Sun Mar 17 23:30:27 2024, max compression
+gzip compressed data, was "cs.queues-20240412.tar", last modified: Fri Apr 12 04:48:16 2024, max compression
```

## Comparing `cs.queues-20240318.tar` & `cs.queues-20240412.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-17 23:30:27.213608 cs.queues-20240318/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-17 23:30:01.000000 cs.queues-20240318/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     7113 2024-03-17 23:30:27.213304 cs.queues-20240318/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     9474 2024-03-17 23:30:09.000000 cs.queues-20240318/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-17 23:30:27.208428 cs.queues-20240318/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-17 23:30:27.208806 cs.queues-20240318/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-17 23:30:27.210479 cs.queues-20240318/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    20007 2024-03-17 23:29:44.000000 cs.queues-20240318/lib/python/cs/queues.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-17 23:30:27.212815 cs.queues-20240318/lib/python/cs.queues.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     7113 2024-03-17 23:30:26.000000 cs.queues-20240318/lib/python/cs.queues.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      279 2024-03-17 23:30:27.000000 cs.queues-20240318/lib/python/cs.queues.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-17 23:30:26.000000 cs.queues-20240318/lib/python/cs.queues.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      130 2024-03-17 23:30:27.000000 cs.queues-20240318/lib/python/cs.queues.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-17 23:30:27.000000 cs.queues-20240318/lib/python/cs.queues.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     7611 2024-03-17 23:30:25.000000 cs.queues-20240318/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-17 23:30:27.213726 cs.queues-20240318/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:48:16.669554 cs.queues-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 04:47:51.000000 cs.queues-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    11170 2024-04-12 04:48:16.669181 cs.queues-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    10375 2024-04-12 04:47:59.000000 cs.queues-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:48:16.665618 cs.queues-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:48:16.665915 cs.queues-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:48:16.667096 cs.queues-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    21001 2024-04-12 04:45:23.000000 cs.queues-20240412/lib/python/cs/queues.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:48:16.668707 cs.queues-20240412/lib/python/cs.queues.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    11170 2024-04-12 04:48:16.000000 cs.queues-20240412/lib/python/cs.queues.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      279 2024-04-12 04:48:16.000000 cs.queues-20240412/lib/python/cs.queues.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 04:48:16.000000 cs.queues-20240412/lib/python/cs.queues.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      130 2024-04-12 04:48:16.000000 cs.queues-20240412/lib/python/cs.queues.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 04:48:16.000000 cs.queues-20240412/lib/python/cs.queues.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    11668 2024-04-12 04:48:15.000000 cs.queues-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 04:48:16.669650 cs.queues-20240412/setup.cfg
```

### Comparing `cs.queues-20240318/README.md` & `cs.queues-20240412/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,31 @@
+Metadata-Version: 2.1
+Name: cs.queues
+Version: 20240412
+Summary: some Queue subclasses and ducktypes
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python2,python3
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
+
 Queue-like items: iterable queues, channels, etc.
 
-*Latest release 20240318*:
-QueueIterator.put: be more rigorous with the put + item count increment.
+*Latest release 20240412*:
+* QueueIterator: new next_batch and iter_batch methods for collecting items in batches.
+* QueueIterator: bugfix put(), do not hold the lock around the internal Queue.put, can deadlock the corresponding next/get.
 
 ## Class `Channel`
 
 A zero-storage data passage.
 Unlike a `Queue`, `put(item)` blocks waiting for the matching `get()`.
 
 *Method `Channel.__init__(self)`*:
@@ -115,15 +135,15 @@
 Put appends to the queue.
 
 ## `NullQ = <NullQueue:NullQ blocking=False>`
 
 A queue-like object that discards its inputs.
 Calls to `.get()` raise `Queue_Empty`.
 
-## Class `NullQueue(cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
+## Class `NullQueue(cs.resources.MultiOpenMixin)`
 
 A queue-like object that discards its inputs.
 Calls to `.get()` raise `Queue_Empty`.
 
 *Method `NullQueue.__init__(self, blocking=False, name=None)`*:
 Initialise the `NullQueue`.
 
@@ -141,15 +161,15 @@
 
 *Method `NullQueue.shutdown(self)`*:
 Shut down the queue.
 
 *Method `NullQueue.startup(self)`*:
 Start the queue.
 
-## Class `PushQueue(cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
+## Class `PushQueue(cs.resources.MultiOpenMixin)`
 
 A puttable object which looks like an iterable `Queue`.
 
 In this base class,
 calling `.put(item)` calls `functor` supplied at initialisation
 to trigger a function on data arrival
 whose iterable of results are put onto the output queue.
@@ -173,15 +193,15 @@
 
 *Method `PushQueue.put(self, *a, **kw)`*:
 Wrapper function to check that this instance is not closed.
 
 *Method `PushQueue.startup_shutdown(self)`*:
 Open/close the output queue.
 
-## Class `QueueIterator(cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
+## Class `QueueIterator(cs.resources.MultiOpenMixin)`
 
 A `QueueIterator` is a wrapper for a `Queue` (or ducktype) which
 presents an iterator interface to collect items.
 It does not offer the `.get` or `.get_nowait` methods.
 
 *Method `QueueIterator.__iter__(self)`*:
 Iterable interface for the queue.
@@ -189,21 +209,34 @@
 *Method `QueueIterator.__next__(self)`*:
 Return the next item from the queue.
 If the queue is closed, raise `StopIteration`.
 
 *Method `QueueIterator.empty(self)`*:
 Test if the queue is empty.
 
+*Method `QueueIterator.iter_batch(self, batch_size=1024)`*:
+A generator which yields batches of items from the queue.
+
 *Method `QueueIterator.join(self)`*:
 Wait for the queue items to complete.
 
 *Method `QueueIterator.next(self)`*:
 Return the next item from the queue.
 If the queue is closed, raise `StopIteration`.
 
+*Method `QueueIterator.next_batch(self, batch_size=1024, block_once=False)`*:
+Obtain a batch of immediately available items from the queue.
+Up to `batch_size` items will be obtained, default 1024.
+Return a list of the items.
+If the queue is empty an empty list is returned.
+If the queue is not empty, continue collecting items until
+the queue is empty or the batch size is reached.
+If `block_once` is true, wait for the first item;
+this mode never returns an empty list except at the end of the iterator.
+
 *Method `QueueIterator.put(self, *a, **kw)`*:
 Wrapper function to check that this instance is not closed.
 
 *Method `QueueIterator.startup_shutdown(self)`*:
 `MultiOpenMixin` support; puts the sentinel onto the underlying queue
 on the final close.
 
@@ -228,14 +261,18 @@
 *Method `TimerQueue.join(self)`*:
 Wait for the main loop thread to finish.
 
 # Release Log
 
 
 
+*Release 20240412*:
+* QueueIterator: new next_batch and iter_batch methods for collecting items in batches.
+* QueueIterator: bugfix put(), do not hold the lock around the internal Queue.put, can deadlock the corresponding next/get.
+
 *Release 20240318*:
 QueueIterator.put: be more rigorous with the put + item count increment.
 
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240305*:
@@ -308,7 +345,8 @@
 * Many bugfixes and internal changes.
 
 *Release 20150115*:
 More PyPI metadata fixups.
 
 *Release 20150111*:
 Initial PyPI release.
+
```

### Comparing `cs.queues-20240318/lib/python/cs/queues.py` & `cs.queues-20240412/lib/python/cs/queues.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 from cs.logutils import exception, warning, debug
 from cs.obj import Sentinel
 from cs.pfx import Pfx, PfxCallInfo
 from cs.py3 import Queue, PriorityQueue, Queue_Empty
 from cs.resources import MultiOpenMixin, not_closed, ClosedError
 from cs.seq import seq, unrepeated
 
-##from cs.debug import Lock, RLock, Thread
-
-__version__ = '20240318'
+__version__ = '20240412'
 
 DISTINFO = {
     'description':
     "some Queue subclasses and ducktypes",
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
@@ -59,15 +57,15 @@
     self.name = name
     self.finalise_later = True
     self.sentinel = Sentinel(
         "%s:%s:SENTINEL" % (self.__class__.__name__, name)
     )
     # count of non-sentinel items
     self._item_count = 0
-    self._lock = Lock()
+    self.__lock = Lock()
 
   def __str__(self):
     return "%s(%r:q=%s)" % (type(self).__name__, self.name, self.q)
 
   @not_closed
   def put(self, item, *args, **kw):
     ''' Put `item` onto the queue.
@@ -76,16 +74,16 @@
     '''
     if self.closed:
       with PfxCallInfo():
         warning("%r.put: all closed: item=%s", self, item)
       raise ClosedError("QueueIterator closed")
     if item is self.sentinel:
       raise ValueError("put(sentinel)")
-    with self._lock:
-      self._put(item, *args, **kw)
+    self._put(item, *args, **kw)
+    with self.__lock:
       self._item_count += 1
 
   def _put(self, item, *args, **kw):
     ''' Direct call to `self.q.put()` with no checks.
     '''
     return self.q.put(item, *args, **kw)
 
@@ -115,18 +113,18 @@
       warning("%s: Queue_Empty: %s", self, e)
       self._put(self.sentinel)
       # pylint: disable=raise-missing-from
       raise StopIteration("Queue_Empty: %s" % (e,))
     if item is self.sentinel:
       # sentinel consumed (clients won't see it, so we must)
       self.q.task_done()
-      # put the sentinel back for other iterators
+      # put the sentinel back for other consumers
       self._put(self.sentinel)
       raise StopIteration("SENTINEL")
-    with self._lock:
+    with self.__lock:
       self._item_count -= 1
     return item
 
   next = __next__
 
   def _get(self):
     ''' Calls the inner queue's `.get` via `.__next__`; can break other users' iterators.
@@ -149,14 +147,43 @@
     self.q.task_done()
 
   def join(self):
     ''' Wait for the queue items to complete.
     '''
     self.q.join()
 
+  def next_batch(self, batch_size=1024, block_once=False):
+    ''' Obtain a batch of immediately available items from the queue.
+        Up to `batch_size` items will be obtained, default 1024.
+        Return a list of the items.
+        If the queue is empty an empty list is returned.
+        If the queue is not empty, continue collecting items until
+        the queue is empty or the batch size is reached.
+        If `block_once` is true, wait for the first item;
+        this mode never returns an empty list except at the end of the iterator.
+    '''
+    batch = []
+    try:
+      if block_once:
+        batch.append(next(self))
+      while len(batch) < batch_size and not self.empty():
+        batch.append(next(self))
+    except StopIteration:
+      pass
+    return batch
+
+  def iter_batch(self, batch_size=1024):
+    ''' A generator which yields batches of items from the queue.
+    '''
+    while True:
+      batch = self.next_batch(batch_size=batch_size, block_once=True)
+      if not batch:
+        return
+      yield batch
+
 def IterableQueue(capacity=0, name=None):
   ''' Factory to create an iterable queue.
       Note that the returned queue is already open
       and needs a close.
   '''
   return QueueIterator(Queue(capacity), name=name).open()
```

### Comparing `cs.queues-20240318/pyproject.toml` & `cs.queues-20240412/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -8,52 +8,76 @@
     "python2",
     "python3",
 ]
 dependencies = [
     "cs.lex>=20240316",
     "cs.logutils>=20230212",
     "cs.obj>=20220918",
-    "cs.pfx>=20230604",
+    "cs.pfx>=20240412",
     "cs.py3>=20220523",
-    "cs.resources>=20240316",
+    "cs.resources>=20240412",
     "cs.seq>=20221118",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 2",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20240318"
+version = "20240412"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Queue-like items: iterable queues, channels, etc.
 
-*Latest release 20240318*:
-QueueIterator.put: be more rigorous with the put + item count increment.
+*Latest release 20240412*:
+* QueueIterator: new next_batch and iter_batch methods for collecting items in batches.
+* QueueIterator: bugfix put(), do not hold the lock around the internal Queue.put, can deadlock the corresponding next/get.
 
 ## Class `Channel`
 
 A zero-storage data passage.
 Unlike a `Queue`, `put(item)` blocks waiting for the matching `get()`.
 
 *Method `Channel.__init__(self)`*:
 pylint: disable=consider-using-with
 
+*Method `Channel.__call__(self, *a)`*:
+Call the `Channel`.
+With no arguments, do a `.get()`.
+With an argument, do a `.put()`.
+
+*Method `Channel.__iter__(self)`*:
+A `Channel` is iterable.
+
+*Method `Channel.__next__(self)`*:
+`next(Channel)` calls `Channel.get()`.
+
+*Method `Channel.__str__(self)`*:
+pylint: disable=consider-using-with
+
+*Method `Channel.close(self)`*:
+Close the `Channel`, preventing further `put()`s.
+
+*Method `Channel.get(self, *a, **kw)`*:
+Wrapper function to check that this instance is not closed.
+
+*Method `Channel.put(self, *a, **kw)`*:
+Wrapper function to check that this instance is not closed.
+
 ## Function `get_batch(q, max_batch=128, *, poll_delay=0.01)`
 
 Get up to `max_batch` closely spaced items from the queue `q`.
 Return the batch. Raise `Queue_Empty` if the first `q.get()` raises.
 
 Block until the first item arrives. While the batch's size is
 less that `max_batch` and there is another item available
@@ -98,33 +122,74 @@
 
     >>> items = [1, 2, 3, 1, 2, 5]
     >>> list(ListQueue(items))
     [1, 2, 3, 1, 2, 5]
     >>> list(ListQueue(items, unique=True))
     [1, 2, 3, 5]
 
+*Method `ListQueue.__bool__(self)`*:
+A `ListQueue` looks a bit like a container,
+and is false when empty.
+
+*Method `ListQueue.__iter__(self)`*:
+A `ListQueue` is iterable.
+
+*Method `ListQueue.__next__(self)`*:
+Iteration gets from the queue.
+
+*Method `ListQueue.append(self, item)`*:
+Append an item to the queue, aka `put`.
+
+*Method `ListQueue.extend(self, items)`*:
+Convenient/performant queue-lots-of-items.
+
+*Method `ListQueue.get(self)`*:
+Get pops from the start of the list.
+
+*Method `ListQueue.insert(self, index, item)`*:
+Insert `item` at `index` in the queue.
+
+*Method `ListQueue.prepend(self, items, offset=0)`*:
+Insert `items` at `offset` (default `0`, the front of the queue).
+
+*Method `ListQueue.put(self, item)`*:
+Put appends to the queue.
+
 ## `NullQ = <NullQueue:NullQ blocking=False>`
 
 A queue-like object that discards its inputs.
 Calls to `.get()` raise `Queue_Empty`.
 
-## Class `NullQueue(cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
+## Class `NullQueue(cs.resources.MultiOpenMixin)`
 
 A queue-like object that discards its inputs.
 Calls to `.get()` raise `Queue_Empty`.
 
 *Method `NullQueue.__init__(self, blocking=False, name=None)`*:
 Initialise the `NullQueue`.
 
 Parameters:
 * `blocking`: optional; if true, calls to `.get()` block until
   `.shutdown()`; default: `False`.
 * `name`: optional name for this `NullQueue`.
 
-## Class `PushQueue(cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
+*Method `NullQueue.get(self)`*:
+Get the next value. Always raises `Queue_Empty`.
+If `.blocking,` delay until `.shutdown()`.
+
+*Method `NullQueue.put(self, item)`*:
+Put a value onto the queue; it is discarded.
+
+*Method `NullQueue.shutdown(self)`*:
+Shut down the queue.
+
+*Method `NullQueue.startup(self)`*:
+Start the queue.
+
+## Class `PushQueue(cs.resources.MultiOpenMixin)`
 
 A puttable object which looks like an iterable `Queue`.
 
 In this base class,
 calling `.put(item)` calls `functor` supplied at initialisation
 to trigger a function on data arrival
 whose iterable of results are put onto the output queue.
@@ -142,29 +207,92 @@
 Parameters:
 * `functor` is a one-to-many function which accepts a single
   item of input and returns an iterable of outputs; it may be a
   generator. These outputs are passed to `outQ.put` individually as
   received.
 * `outQ` is a `MultiOpenMixin` which accepts via its `.put()` method.
 
-## Class `QueueIterator(cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
+*Method `PushQueue.put(self, *a, **kw)`*:
+Wrapper function to check that this instance is not closed.
+
+*Method `PushQueue.startup_shutdown(self)`*:
+Open/close the output queue.
+
+## Class `QueueIterator(cs.resources.MultiOpenMixin)`
 
 A `QueueIterator` is a wrapper for a `Queue` (or ducktype) which
 presents an iterator interface to collect items.
 It does not offer the `.get` or `.get_nowait` methods.
 
+*Method `QueueIterator.__iter__(self)`*:
+Iterable interface for the queue.
+
+*Method `QueueIterator.__next__(self)`*:
+Return the next item from the queue.
+If the queue is closed, raise `StopIteration`.
+
+*Method `QueueIterator.empty(self)`*:
+Test if the queue is empty.
+
+*Method `QueueIterator.iter_batch(self, batch_size=1024)`*:
+A generator which yields batches of items from the queue.
+
+*Method `QueueIterator.join(self)`*:
+Wait for the queue items to complete.
+
+*Method `QueueIterator.next(self)`*:
+Return the next item from the queue.
+If the queue is closed, raise `StopIteration`.
+
+*Method `QueueIterator.next_batch(self, batch_size=1024, block_once=False)`*:
+Obtain a batch of immediately available items from the queue.
+Up to `batch_size` items will be obtained, default 1024.
+Return a list of the items.
+If the queue is empty an empty list is returned.
+If the queue is not empty, continue collecting items until
+the queue is empty or the batch size is reached.
+If `block_once` is true, wait for the first item;
+this mode never returns an empty list except at the end of the iterator.
+
+*Method `QueueIterator.put(self, *a, **kw)`*:
+Wrapper function to check that this instance is not closed.
+
+*Method `QueueIterator.startup_shutdown(self)`*:
+`MultiOpenMixin` support; puts the sentinel onto the underlying queue
+on the final close.
+
+*Method `QueueIterator.task_done(self)`*:
+Report that an item has been processed.
+
 ## Class `TimerQueue`
 
 Class to run a lot of \"in the future\" jobs without using a bazillion
 Timer threads.
 
+*Method `TimerQueue.add(self, when, func)`*:
+Queue a new job to be called at 'when'.
+'func' is the job function, typically made with `functools.partial`.
+
+*Method `TimerQueue.close(self, cancel=False)`*:
+Close the `TimerQueue`. This forbids further job submissions.
+If `cancel` is supplied and true, cancel all pending jobs.
+Note: it is still necessary to call `TimerQueue.join()` to
+wait for all pending jobs.
+
+*Method `TimerQueue.join(self)`*:
+Wait for the main loop thread to finish.
+
 # Release Log
 
 
 
+*Release 20240412*:
+* QueueIterator: new next_batch and iter_batch methods for collecting items in batches.
+* QueueIterator: bugfix put(), do not hold the lock around the internal Queue.put, can deadlock the corresponding next/get.
+
 *Release 20240318*:
 QueueIterator.put: be more rigorous with the put + item count increment.
 
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240305*:
```

