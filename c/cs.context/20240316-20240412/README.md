# Comparing `tmp/cs.context-20240316.tar.gz` & `tmp/cs.context-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.context-20240316.tar", last modified: Sat Mar 16 07:01:16 2024, max compression
+gzip compressed data, was "cs.context-20240412.tar", last modified: Fri Apr 12 02:32:58 2024, max compression
```

## Comparing `cs.context-20240316.tar` & `cs.context-20240412.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:01:16.349720 cs.context-20240316/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-16 07:00:53.000000 cs.context-20240316/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    15925 2024-03-16 07:01:16.349405 cs.context-20240316/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    16004 2024-03-16 07:01:00.000000 cs.context-20240316/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:01:16.346010 cs.context-20240316/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:01:16.346310 cs.context-20240316/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:01:16.347546 cs.context-20240316/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    19772 2024-03-16 07:00:43.000000 cs.context-20240316/lib/python/cs/context.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:01:16.348863 cs.context-20240316/lib/python/cs.context.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    15925 2024-03-16 07:01:15.000000 cs.context-20240316/lib/python/cs.context.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      241 2024-03-16 07:01:16.000000 cs.context-20240316/lib/python/cs.context.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 07:01:15.000000 cs.context-20240316/lib/python/cs.context.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 07:01:16.000000 cs.context-20240316/lib/python/cs.context.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    16274 2024-03-16 07:01:14.000000 cs.context-20240316/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 07:01:16.349836 cs.context-20240316/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:32:58.318375 cs.context-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 02:32:35.000000 cs.context-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    19639 2024-04-12 02:32:58.318046 cs.context-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    18852 2024-04-12 02:32:42.000000 cs.context-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:32:58.312895 cs.context-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:32:58.313181 cs.context-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:32:58.315306 cs.context-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    23359 2024-04-12 02:32:19.000000 cs.context-20240412/lib/python/cs/context.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:32:58.317596 cs.context-20240412/lib/python/cs.context.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    19639 2024-04-12 02:32:57.000000 cs.context-20240412/lib/python/cs.context.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      285 2024-04-12 02:32:58.000000 cs.context-20240412/lib/python/cs.context.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 02:32:57.000000 cs.context-20240412/lib/python/cs.context.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       22 2024-04-12 02:32:58.000000 cs.context-20240412/lib/python/cs.context.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 02:32:58.000000 cs.context-20240412/lib/python/cs.context.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    20026 2024-04-12 02:32:56.000000 cs.context-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 02:32:58.318468 cs.context-20240412/setup.cfg
```

### Comparing `cs.context-20240316/PKG-INFO` & `cs.context-20240412/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.context
-Version: 20240316
+Version: 20240412
 Summary: Assorted context managers.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,28 +15,72 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted context managers.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
-
-## Function `contextif(flag, cmgr_func, *cmgr_args, **cmgr_kwargs)`
+*Latest release 20240412*:
+* contextif: rework to be much easier to use, add new call modes.
+* pushkeys, stackkeys: support update dicts whose keys are not identifier strings i.e. a non **kw call mode.
+* New withif() function returning a context manager even for objects which do not provide one.
+* New withall(iterable-of-context-managers) context manager.
+
+## Function `contextif(cmgr, *cmgr_args, **cmgr_kwargs)`
+
+A context manager to use `cmgr` conditionally,
+with a flexible call signature.
+This yields the context manager if `cmgr` is used or `None`
+if it is not used, allowing the enclosed code to test whether
+the context is active.
 
-A context manager to call `cmgr_func(*cmgr_args,**cmgr_kwargs)`
-if `flag` is true, otherwise to call `nullcontext()`.
+This is to ease uses where the context object is optional
+i.e. `None` if not present. Example from `cs.vt.stream`:
 
-The driving use case is verbosity dependent status lines or
-progress bars, eg:
+    @contextmanager
+    def startup_shutdown(self):
+      """ Open/close `self.local_store` if not `None`.
+      """
+      with super().startup_shutdown():
+        with contextif(self.local_store):
+          with self._packet_connection(self.recv, self.send) as conn:
+            with stackattrs(self, _conn=conn):
+              yield
+
+Here `self.local_store` might be `None` if there's no local
+store to present. We still want a nice nested `with` statement
+during the setup. By using `contextif` we run a context manager
+which behaves correctly when `self.local_store=None`.
+
+The signature is flexible, offering 2 basic modes of use.
+
+Flagged use: `contextif(flag,cmgr,*a,**kw)`: if `flag` is a
+Boolean then it governs whether the context manager `cmgr`
+is used. Historically the driving use case was verbosity
+dependent status lines or progress bars. Example:
 
     from cs.upd import run_task
     with contextif(verbose, run_task, ....) as proxy:
-      ... do stuff, updating proxy if not None ...
+        ... do stuff, updating proxy if not None ...
+
+Unflagged use: `contextif(cmgr,*a,**kw)`: use `cmgr` as the
+flag: if false (eg `None`) then `cmgr` is not used.
+
+Additionally, `cmgr` may be a callable, in which case the
+context manager itself is obtained by calling
+`cmgr,*cmgr_args,**cmgr_kwargs)`. Otherwise `cmgr` is assumed
+to be a context manager already, and it is an error to provide
+`cmgr_args` or `cmgr_kwargs`.
+
+In the `cs.upd` example above, `run_task` is a context manager
+function which pops up an updatable status line, normally
+used as:
+
+    with run_task("doing thing") as proxy:
+        ... do the thing, setting proxy.text as needed ...
 
 ## Class `ContextManagerMixin`
 
 A mixin to provide context manager `__enter__` and `__exit__` methods
 running the first and second steps of a single `__enter_exit__` generator method.
 
 *Note*: the `__enter_exit__` method is _not_ a context manager,
@@ -79,14 +123,38 @@
             except SomeException as e:
                 ... handle e ...
                 exit_result = True
             finally:
                 ... do tear down here ...
             yield exit_result
 
+*Method `ContextManagerMixin.__enter__(self)`*:
+Run `super().__enter__` (if any)
+then the `__enter__` phase of `self.__enter_exit__()`.
+
+*Method `ContextManagerMixin.__exit__(self, exc_type, exc_value, traceback)`*:
+Run the `__exit__` step of `self.__enter_exit__()`,
+then `super().__exit__` (if any).
+
+*Method `ContextManagerMixin.as_contextmanager(self)`*:
+Run the generator from the `cls` class specific `__enter_exit__`
+method via `self` as a context manager.
+
+Example from `RunState` which subclasses `HasThreadState`,
+both of which are `ContextManagerMixin` subclasses:
+
+    class RunState(HasThreadState):
+        .....
+        def __enter_exit__(self):
+            with HasThreadState.as_contextmanager(self):
+                ... RunState context manager stuff ...
+
+This runs the `HasThreadState` context manager
+around the main `RunState` context manager.
+
 ## Function `pop_cmgr(o, attr)`
 
 Run the `__exit__` phase of a context manager commenced with `push_cmgr`.
 Restore `attr` as it was before `push_cmgr`.
 Return the result of `__exit__`.
 
 ## Function `popattrs(o, attr_names, old_values)`
@@ -143,27 +211,27 @@
     >>> assert not hasattr(obj, 'path')
     >>> assert not isdirpath(dirpath)
 
 ## Function `pushattrs(o, **attr_values)`
 
 The "push" part of `stackattrs`.
 Push `attr_values` onto `o` as attributes,
-return the previous attribute values in a dict.
+return the previous attribute values in a `dict`.
 
 This can be useful in hooks/signals/callbacks,
 where you cannot inline a context manager.
 
-## Function `pushkeys(d, **key_values)`
+## Function `pushkeys(d, kv=None, **kw)`
 
 The "push" part of `stackkeys`.
-Push `key_values` onto `d` as key values.
-return the previous key values in a dict.
+Use the mapping provided as `kv` or `kw` to update `d`.
+Return the previous key values in a `dict`.
 
 This can be useful in hooks/signals/callbacks,
-where you cannot inline a context manager.
+where you cannot inline a context manager using `stackkeys`.
 
 ## Function `reconfigure_file(f, **kw)`
 
 Context manager flavour of `TextIOBase.reconfigure`.
 
 ## Function `setup_cmgr(cmgr)`
 
@@ -226,25 +294,25 @@
 apply a handler which calls both the new handler and the old handler.
 
 ## Function `stackattrs(o, **attr_values)`
 
 Context manager to push new values for the attributes of `o`
 and to restore them afterward.
 Returns a `dict` containing a mapping of the previous attribute values.
-Attributes not present are not present in returned mapping.
+Attributes not present are not present in the returned mapping.
 
 Restoration includes deleting attributes which were not present
 initially.
 
 This makes it easy to adjust temporarily some shared context object
 without having to pass it through the call stack.
 
 See `stackkeys` for a flavour of this for mappings.
 
-See `cs.threads.State` for a convenient wrapper class.
+See `cs.threads.ThreadState` for a convenient wrapper class.
 
 Example of fiddling a programme's "verbose" mode:
 
     >>> class RunModes:
     ...     def __init__(self, verbose=False):
     ...         self.verbose = verbose
     ...
@@ -287,18 +355,19 @@
     >>> print(o.a)
     1
     >>> print(o.b)
     Traceback (most recent call last):
       File "<stdin>", line 1, in <module>
     AttributeError: 'O' object has no attribute 'b'
 
-## Function `stackkeys(d, **key_values)`
+## Function `stackkeys(d, kv=None, **kw)`
 
-Context manager to push new values for the key values of `d`
+A context manager to push new values for the key values of `d`
 and to restore them afterward.
+The new values are provided as `kv` or `kw` as convenient.
 Returns a `dict` containing a mapping of the previous key values.
 Keys not present are not present in the mapping.
 
 Restoration includes deleting key values which were not present
 initially.
 
 This makes it easy to adjust temporarily some shared context object
@@ -367,17 +436,20 @@
 
     @contextmanager
     def my_cmgr_func(...):
         ...
         yield
         ...
 
-then the correct use of `twostep()` is:
+then `my_cmgr_func(...)` returns a context manager instance
+and so the correct use of `twostep()` is like this:
 
-    cmgr_iter = twostep(my_cmgr_func(...))
+    # steps broken out for clarity
+    cmgr = my_cmgr_func(...)
+    cmgr_iter = twostep(cmgr)
     next(cmgr_iter)   # set up
     next(cmgr_iter)   # tear down
 
 and _not_:
 
     cmgr_iter = twostep(my_cmgr_func)
     next(cmgr_iter)   # set up
@@ -394,18 +466,40 @@
             self._cmgr_stepped = twostep(stackattrs(o, setting=foo))
             self._cmgr = next(self._cmgr_stepped)
             return self._cmgr
         def __exit__(self, *_):
             next(self._cmgr_stepped)
             self._cmgr = None
 
+## Function `withall(objs)`
+
+Enter every object `obj` in `obj_list` except those which are `None`
+using `with obj:`, then yield.
+
+## Function `withif(obj)`
+
+Return a context manager for `obj`.
+If `obj` has an `__enter__` attribute, return `obj`
+otherwise return `nullcontext()`.
+
+Example:
+
+    with withif(inner_mapping):
+      ... work with inner_mapping ...
+
 # Release Log
 
 
 
+*Release 20240412*:
+* contextif: rework to be much easier to use, add new call modes.
+* pushkeys, stackkeys: support update dicts whose keys are not identifier strings i.e. a non **kw call mode.
+* New withif() function returning a context manager even for objects which do not provide one.
+* New withall(iterable-of-context-managers) context manager.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240212.1*:
 Minor doc updates.
 
 *Release 20240212*:
```

### Comparing `cs.context-20240316/README.md` & `cs.context-20240412/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,67 @@
 Assorted context managers.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
-
-## Function `contextif(flag, cmgr_func, *cmgr_args, **cmgr_kwargs)`
+*Latest release 20240412*:
+* contextif: rework to be much easier to use, add new call modes.
+* pushkeys, stackkeys: support update dicts whose keys are not identifier strings i.e. a non **kw call mode.
+* New withif() function returning a context manager even for objects which do not provide one.
+* New withall(iterable-of-context-managers) context manager.
+
+## Function `contextif(cmgr, *cmgr_args, **cmgr_kwargs)`
+
+A context manager to use `cmgr` conditionally,
+with a flexible call signature.
+This yields the context manager if `cmgr` is used or `None`
+if it is not used, allowing the enclosed code to test whether
+the context is active.
 
-A context manager to call `cmgr_func(*cmgr_args,**cmgr_kwargs)`
-if `flag` is true, otherwise to call `nullcontext()`.
+This is to ease uses where the context object is optional
+i.e. `None` if not present. Example from `cs.vt.stream`:
 
-The driving use case is verbosity dependent status lines or
-progress bars, eg:
+    @contextmanager
+    def startup_shutdown(self):
+      """ Open/close `self.local_store` if not `None`.
+      """
+      with super().startup_shutdown():
+        with contextif(self.local_store):
+          with self._packet_connection(self.recv, self.send) as conn:
+            with stackattrs(self, _conn=conn):
+              yield
+
+Here `self.local_store` might be `None` if there's no local
+store to present. We still want a nice nested `with` statement
+during the setup. By using `contextif` we run a context manager
+which behaves correctly when `self.local_store=None`.
+
+The signature is flexible, offering 2 basic modes of use.
+
+Flagged use: `contextif(flag,cmgr,*a,**kw)`: if `flag` is a
+Boolean then it governs whether the context manager `cmgr`
+is used. Historically the driving use case was verbosity
+dependent status lines or progress bars. Example:
 
     from cs.upd import run_task
     with contextif(verbose, run_task, ....) as proxy:
-      ... do stuff, updating proxy if not None ...
+        ... do stuff, updating proxy if not None ...
+
+Unflagged use: `contextif(cmgr,*a,**kw)`: use `cmgr` as the
+flag: if false (eg `None`) then `cmgr` is not used.
+
+Additionally, `cmgr` may be a callable, in which case the
+context manager itself is obtained by calling
+`cmgr,*cmgr_args,**cmgr_kwargs)`. Otherwise `cmgr` is assumed
+to be a context manager already, and it is an error to provide
+`cmgr_args` or `cmgr_kwargs`.
+
+In the `cs.upd` example above, `run_task` is a context manager
+function which pops up an updatable status line, normally
+used as:
+
+    with run_task("doing thing") as proxy:
+        ... do the thing, setting proxy.text as needed ...
 
 ## Class `ContextManagerMixin`
 
 A mixin to provide context manager `__enter__` and `__exit__` methods
 running the first and second steps of a single `__enter_exit__` generator method.
 
 *Note*: the `__enter_exit__` method is _not_ a context manager,
@@ -148,27 +192,27 @@
     >>> assert not hasattr(obj, 'path')
     >>> assert not isdirpath(dirpath)
 
 ## Function `pushattrs(o, **attr_values)`
 
 The "push" part of `stackattrs`.
 Push `attr_values` onto `o` as attributes,
-return the previous attribute values in a dict.
+return the previous attribute values in a `dict`.
 
 This can be useful in hooks/signals/callbacks,
 where you cannot inline a context manager.
 
-## Function `pushkeys(d, **key_values)`
+## Function `pushkeys(d, kv=None, **kw)`
 
 The "push" part of `stackkeys`.
-Push `key_values` onto `d` as key values.
-return the previous key values in a dict.
+Use the mapping provided as `kv` or `kw` to update `d`.
+Return the previous key values in a `dict`.
 
 This can be useful in hooks/signals/callbacks,
-where you cannot inline a context manager.
+where you cannot inline a context manager using `stackkeys`.
 
 ## Function `reconfigure_file(f, **kw)`
 
 Context manager flavour of `TextIOBase.reconfigure`.
 
 ## Function `setup_cmgr(cmgr)`
 
@@ -231,25 +275,25 @@
 apply a handler which calls both the new handler and the old handler.
 
 ## Function `stackattrs(o, **attr_values)`
 
 Context manager to push new values for the attributes of `o`
 and to restore them afterward.
 Returns a `dict` containing a mapping of the previous attribute values.
-Attributes not present are not present in returned mapping.
+Attributes not present are not present in the returned mapping.
 
 Restoration includes deleting attributes which were not present
 initially.
 
 This makes it easy to adjust temporarily some shared context object
 without having to pass it through the call stack.
 
 See `stackkeys` for a flavour of this for mappings.
 
-See `cs.threads.State` for a convenient wrapper class.
+See `cs.threads.ThreadState` for a convenient wrapper class.
 
 Example of fiddling a programme's "verbose" mode:
 
     >>> class RunModes:
     ...     def __init__(self, verbose=False):
     ...         self.verbose = verbose
     ...
@@ -292,18 +336,19 @@
     >>> print(o.a)
     1
     >>> print(o.b)
     Traceback (most recent call last):
       File "<stdin>", line 1, in <module>
     AttributeError: 'O' object has no attribute 'b'
 
-## Function `stackkeys(d, **key_values)`
+## Function `stackkeys(d, kv=None, **kw)`
 
-Context manager to push new values for the key values of `d`
+A context manager to push new values for the key values of `d`
 and to restore them afterward.
+The new values are provided as `kv` or `kw` as convenient.
 Returns a `dict` containing a mapping of the previous key values.
 Keys not present are not present in the mapping.
 
 Restoration includes deleting key values which were not present
 initially.
 
 This makes it easy to adjust temporarily some shared context object
@@ -372,17 +417,20 @@
 
     @contextmanager
     def my_cmgr_func(...):
         ...
         yield
         ...
 
-then the correct use of `twostep()` is:
+then `my_cmgr_func(...)` returns a context manager instance
+and so the correct use of `twostep()` is like this:
 
-    cmgr_iter = twostep(my_cmgr_func(...))
+    # steps broken out for clarity
+    cmgr = my_cmgr_func(...)
+    cmgr_iter = twostep(cmgr)
     next(cmgr_iter)   # set up
     next(cmgr_iter)   # tear down
 
 and _not_:
 
     cmgr_iter = twostep(my_cmgr_func)
     next(cmgr_iter)   # set up
@@ -399,18 +447,40 @@
             self._cmgr_stepped = twostep(stackattrs(o, setting=foo))
             self._cmgr = next(self._cmgr_stepped)
             return self._cmgr
         def __exit__(self, *_):
             next(self._cmgr_stepped)
             self._cmgr = None
 
+## Function `withall(objs)`
+
+Enter every object `obj` in `obj_list` except those which are `None`
+using `with obj:`, then yield.
+
+## Function `withif(obj)`
+
+Return a context manager for `obj`.
+If `obj` has an `__enter__` attribute, return `obj`
+otherwise return `nullcontext()`.
+
+Example:
+
+    with withif(inner_mapping):
+      ... work with inner_mapping ...
+
 # Release Log
 
 
 
+*Release 20240412*:
+* contextif: rework to be much easier to use, add new call modes.
+* pushkeys, stackkeys: support update dicts whose keys are not identifier strings i.e. a non **kw call mode.
+* New withif() function returning a context manager even for objects which do not provide one.
+* New withall(iterable-of-context-managers) context manager.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240212.1*:
 Minor doc updates.
 
 *Release 20240212*:
```

### Comparing `cs.context-20240316/lib/python/cs/context.py` & `cs.context-20240412/lib/python/cs/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,47 +11,107 @@
 
   @contextmanager
   def nullcontext():
     ''' A simple `nullcontext` for older Pythons
     '''
     yield None
 
-__version__ = '20240316'
+from cs.gimmicks import error
+
+__version__ = '20240412'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
     ],
-    'install_requires': [],
+    'install_requires': ['cs.gimmicks'],
 }
 
 @contextmanager
-def contextif(flag, cmgr_func, *cmgr_args, **cmgr_kwargs):
-  ''' A context manager to call `cmgr_func(*cmgr_args,**cmgr_kwargs)`
-      if `flag` is true, otherwise to call `nullcontext()`.
+def contextif(cmgr, *cmgr_args, **cmgr_kwargs):
+  ''' A context manager to use `cmgr` conditionally,
+      with a flexible call signature.
+      This yields the context manager if `cmgr` is used or `None`
+      if it is not used, allowing the enclosed code to test whether
+      the context is active.
+
+      This is to ease uses where the context object is optional
+      i.e. `None` if not present. Example from `cs.vt.stream`:
 
-      The driving use case is verbosity dependent status lines or
-      progress bars, eg:
+          @contextmanager
+          def startup_shutdown(self):
+            """ Open/close `self.local_store` if not `None`.
+            """
+            with super().startup_shutdown():
+              with contextif(self.local_store):
+                with self._packet_connection(self.recv, self.send) as conn:
+                  with stackattrs(self, _conn=conn):
+                    yield
+
+      Here `self.local_store` might be `None` if there's no local
+      store to present. We still want a nice nested `with` statement
+      during the setup. By using `contextif` we run a context manager
+      which behaves correctly when `self.local_store=None`.
+
+      The signature is flexible, offering 2 basic modes of use.
+
+      Flagged use: `contextif(flag,cmgr,*a,**kw)`: if `flag` is a
+      Boolean then it governs whether the context manager `cmgr`
+      is used. Historically the driving use case was verbosity
+      dependent status lines or progress bars. Example:
 
           from cs.upd import run_task
           with contextif(verbose, run_task, ....) as proxy:
-            ... do stuff, updating proxy if not None ...
+              ... do stuff, updating proxy if not None ...
+
+      Unflagged use: `contextif(cmgr,*a,**kw)`: use `cmgr` as the
+      flag: if false (eg `None`) then `cmgr` is not used.
+
+      Additionally, `cmgr` may be a callable, in which case the
+      context manager itself is obtained by calling
+      `cmgr,*cmgr_args,**cmgr_kwargs)`. Otherwise `cmgr` is assumed
+      to be a context manager already, and it is an error to provide
+      `cmgr_args` or `cmgr_kwargs`.
+
+      In the `cs.upd` example above, `run_task` is a context manager
+      function which pops up an updatable status line, normally
+      used as:
+
+          with run_task("doing thing") as proxy:
+              ... do the thing, setting proxy.text as needed ...
   '''
-  assert isinstance(flag, bool)
-  cmgr = cmgr_func(*cmgr_args, **cmgr_kwargs) if flag else nullcontext()
-  with cmgr as ctxt:
-    yield ctxt
+  if callable(cmgr):
+    flag = True
+  else:
+    if isinstance(cmgr, bool):
+      flag = cmgr
+      cmgr = cmgr_args[0]
+      cmgr_args = cmgr_args[1:]
+    else:
+      flag = bool(cmgr)
+  if flag:
+    if callable(cmgr):
+      cmgr = cmgr(*cmgr_args, **cmgr_kwargs)
+    elif cmgr_args or cmgr_kwargs:
+      raise ValueError(
+          "cmgr %s:%r is not callable but arguments were provided: cmgr_args=%r, cmgr_kwargs=%r"
+          % (cmgr.__class__.__name__, cmgr, cmgr_args, cmgr_kwargs)
+      )
+    with cmgr as ctxt:
+      yield ctxt
+  else:
+    yield
 
 def pushattrs(o, **attr_values):
   ''' The "push" part of `stackattrs`.
       Push `attr_values` onto `o` as attributes,
-      return the previous attribute values in a dict.
+      return the previous attribute values in a `dict`.
 
       This can be useful in hooks/signals/callbacks,
       where you cannot inline a context manager.
   '''
   old_values = {}
   for attr, value in attr_values.items():
     try:
@@ -83,25 +143,25 @@
       setattr(o, attr, old_value)
 
 @contextmanager
 def stackattrs(o, **attr_values):
   ''' Context manager to push new values for the attributes of `o`
       and to restore them afterward.
       Returns a `dict` containing a mapping of the previous attribute values.
-      Attributes not present are not present in returned mapping.
+      Attributes not present are not present in the returned mapping.
 
       Restoration includes deleting attributes which were not present
       initially.
 
       This makes it easy to adjust temporarily some shared context object
       without having to pass it through the call stack.
 
       See `stackkeys` for a flavour of this for mappings.
 
-      See `cs.threads.State` for a convenient wrapper class.
+      See `cs.threads.ThreadState` for a convenient wrapper class.
 
       Example of fiddling a programme's "verbose" mode:
 
           >>> class RunModes:
           ...     def __init__(self, verbose=False):
           ...         self.verbose = verbose
           ...
@@ -150,24 +210,28 @@
   '''
   old_values = pushattrs(o, **attr_values)
   try:
     yield old_values
   finally:
     popattrs(o, attr_values.keys(), old_values)
 
-def pushkeys(d, **key_values):
+def pushkeys(d, kv=None, **kw):
   ''' The "push" part of `stackkeys`.
-      Push `key_values` onto `d` as key values.
-      return the previous key values in a dict.
+      Use the mapping provided as `kv` or `kw` to update `d`.
+      Return the previous key values in a `dict`.
 
       This can be useful in hooks/signals/callbacks,
-      where you cannot inline a context manager.
+      where you cannot inline a context manager using `stackkeys`.
   '''
+  if kv is None:
+    kv = kw
+  elif kw:
+    raise ValueError("pushkeys: only one of kv or kw may be provided")
   old_values = {}
-  for key, value in key_values.items():
+  for key, value in kv.items():
     try:
       old_value = d[key]
     except KeyError:
       pass
     else:
       old_values[key] = old_value
     d[key] = value
@@ -189,17 +253,18 @@
         del d[key]
       except KeyError:
         pass
     else:
       d[key] = old_value
 
 @contextmanager
-def stackkeys(d, **key_values):
-  ''' Context manager to push new values for the key values of `d`
+def stackkeys(d, kv=None, **kw):
+  ''' A context manager to push new values for the key values of `d`
       and to restore them afterward.
+      The new values are provided as `kv` or `kw` as convenient.
       Returns a `dict` containing a mapping of the previous key values.
       Keys not present are not present in the mapping.
 
       Restoration includes deleting key values which were not present
       initially.
 
       This makes it easy to adjust temporarily some shared context object
@@ -233,19 +298,20 @@
           ...
           log_entry: global_context = {'parent': {'parent': None, 'desc': 'high level entry', 'when': ...}}
           {'parent': {'parent': None, 'desc': 'high level entry', 'when': ...}, 'desc': 'low level event', 'when': ...}
           >>> log_entry("another standalone entry")    #doctest: +ELLIPSIS
           log_entry: global_context = {'parent': None}
           {'parent': None, 'desc': 'another standalone entry', 'when': ...}
   '''
-  old_values = pushkeys(d, **key_values)
+  old_values = pushkeys(d, kv, **kw)
+  kv = kv or kw
   try:
     yield old_values
   finally:
-    popkeys(d, key_values.keys(), old_values)
+    popkeys(d, kv.keys(), old_values)
 
 @contextmanager
 def stackset(s, element, lock=None):
   ''' Context manager to add `element` to the set `s` and remove it on return.
       The element is neither added nor removed if it is already present.
   '''
   if element in s:
@@ -290,17 +356,20 @@
 
           @contextmanager
           def my_cmgr_func(...):
               ...
               yield
               ...
 
-      then the correct use of `twostep()` is:
+      then `my_cmgr_func(...)` returns a context manager instance
+      and so the correct use of `twostep()` is like this:
 
-          cmgr_iter = twostep(my_cmgr_func(...))
+          # steps broken out for clarity
+          cmgr = my_cmgr_func(...)
+          cmgr_iter = twostep(cmgr)
           next(cmgr_iter)   # set up
           next(cmgr_iter)   # tear down
 
       and _not_:
 
           cmgr_iter = twostep(my_cmgr_func)
           next(cmgr_iter)   # set up
@@ -446,14 +515,15 @@
       If the optional `additional` argument is true,
       apply a handler which calls both the new handler and the old handler.
   '''
   stacked_signals = {}
   if additional:
     new_handler = handler
 
+    # pylint: disable=function-redefined
     def handler(sig, frame):
       old_handler = stacked_signals[sig]
       new_handler(sig, frame)
       if old_handler:
         old_handler(sig, frame)
 
   if isinstance(signums, int):
@@ -577,27 +647,64 @@
                     with HasThreadState.as_contextmanager(self):
                         ... RunState context manager stuff ...
 
         This runs the `HasThreadState` context manager
         around the main `RunState` context manager.
     '''
     eegen = cls.__enter_exit__(self)
-    entered = next(eegen)
+    try:
+      entered = next(eegen)
+    except StopIteration as e:
+      error("expected enter value from next(eegen): %s", e)
+      return
     try:
       yield entered
     except Exception as e:  # pylint: disable=broad-exception-caught
       exit_result = eegen.throw(type(e), e, e.__traceback__)
       if not exit_result:
         raise
     else:
       try:
         exit_result = next(eegen)
       except StopIteration:
         pass
 
+def withif(obj):
+  ''' Return a context manager for `obj`.
+      If `obj` has an `__enter__` attribute, return `obj`
+      otherwise return `nullcontext()`.
+
+      Example:
+
+          with withif(inner_mapping):
+            ... work with inner_mapping ...
+  '''
+  if hasattr(obj, '__enter__'):
+    return obj
+  return nullcontext()
+
+def _withall(obj_it):
+  ''' A generator to enter every object `obj` from the iterator
+      `obj_it` using `with obj:`, then yield.
+  '''
+  try:
+    obj = next(obj_it)
+  except StopIteration:
+    yield
+  else:
+    with obj:
+      yield from _withall(obj_it)
+
+@contextmanager
+def withall(objs):
+  ''' Enter every object `obj` in `obj_list` except those which are `None`
+      using `with obj:`, then yield.
+  '''
+  yield from _withall(obj for obj in objs if obj is not None)
+
 @contextmanager
 def reconfigure_file(f, **kw):
   ''' Context manager flavour of `TextIOBase.reconfigure`.
   '''
   old = {k: getattr(f, k) for k in kw}
   try:
     f.reconfigure(**kw)
```

### Comparing `cs.context-20240316/lib/python/cs.context.egg-info/PKG-INFO` & `cs.context-20240412/lib/python/cs.context.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.context
-Version: 20240316
+Version: 20240412
 Summary: Assorted context managers.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,28 +15,72 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted context managers.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
-
-## Function `contextif(flag, cmgr_func, *cmgr_args, **cmgr_kwargs)`
+*Latest release 20240412*:
+* contextif: rework to be much easier to use, add new call modes.
+* pushkeys, stackkeys: support update dicts whose keys are not identifier strings i.e. a non **kw call mode.
+* New withif() function returning a context manager even for objects which do not provide one.
+* New withall(iterable-of-context-managers) context manager.
+
+## Function `contextif(cmgr, *cmgr_args, **cmgr_kwargs)`
+
+A context manager to use `cmgr` conditionally,
+with a flexible call signature.
+This yields the context manager if `cmgr` is used or `None`
+if it is not used, allowing the enclosed code to test whether
+the context is active.
 
-A context manager to call `cmgr_func(*cmgr_args,**cmgr_kwargs)`
-if `flag` is true, otherwise to call `nullcontext()`.
+This is to ease uses where the context object is optional
+i.e. `None` if not present. Example from `cs.vt.stream`:
 
-The driving use case is verbosity dependent status lines or
-progress bars, eg:
+    @contextmanager
+    def startup_shutdown(self):
+      """ Open/close `self.local_store` if not `None`.
+      """
+      with super().startup_shutdown():
+        with contextif(self.local_store):
+          with self._packet_connection(self.recv, self.send) as conn:
+            with stackattrs(self, _conn=conn):
+              yield
+
+Here `self.local_store` might be `None` if there's no local
+store to present. We still want a nice nested `with` statement
+during the setup. By using `contextif` we run a context manager
+which behaves correctly when `self.local_store=None`.
+
+The signature is flexible, offering 2 basic modes of use.
+
+Flagged use: `contextif(flag,cmgr,*a,**kw)`: if `flag` is a
+Boolean then it governs whether the context manager `cmgr`
+is used. Historically the driving use case was verbosity
+dependent status lines or progress bars. Example:
 
     from cs.upd import run_task
     with contextif(verbose, run_task, ....) as proxy:
-      ... do stuff, updating proxy if not None ...
+        ... do stuff, updating proxy if not None ...
+
+Unflagged use: `contextif(cmgr,*a,**kw)`: use `cmgr` as the
+flag: if false (eg `None`) then `cmgr` is not used.
+
+Additionally, `cmgr` may be a callable, in which case the
+context manager itself is obtained by calling
+`cmgr,*cmgr_args,**cmgr_kwargs)`. Otherwise `cmgr` is assumed
+to be a context manager already, and it is an error to provide
+`cmgr_args` or `cmgr_kwargs`.
+
+In the `cs.upd` example above, `run_task` is a context manager
+function which pops up an updatable status line, normally
+used as:
+
+    with run_task("doing thing") as proxy:
+        ... do the thing, setting proxy.text as needed ...
 
 ## Class `ContextManagerMixin`
 
 A mixin to provide context manager `__enter__` and `__exit__` methods
 running the first and second steps of a single `__enter_exit__` generator method.
 
 *Note*: the `__enter_exit__` method is _not_ a context manager,
@@ -79,14 +123,38 @@
             except SomeException as e:
                 ... handle e ...
                 exit_result = True
             finally:
                 ... do tear down here ...
             yield exit_result
 
+*Method `ContextManagerMixin.__enter__(self)`*:
+Run `super().__enter__` (if any)
+then the `__enter__` phase of `self.__enter_exit__()`.
+
+*Method `ContextManagerMixin.__exit__(self, exc_type, exc_value, traceback)`*:
+Run the `__exit__` step of `self.__enter_exit__()`,
+then `super().__exit__` (if any).
+
+*Method `ContextManagerMixin.as_contextmanager(self)`*:
+Run the generator from the `cls` class specific `__enter_exit__`
+method via `self` as a context manager.
+
+Example from `RunState` which subclasses `HasThreadState`,
+both of which are `ContextManagerMixin` subclasses:
+
+    class RunState(HasThreadState):
+        .....
+        def __enter_exit__(self):
+            with HasThreadState.as_contextmanager(self):
+                ... RunState context manager stuff ...
+
+This runs the `HasThreadState` context manager
+around the main `RunState` context manager.
+
 ## Function `pop_cmgr(o, attr)`
 
 Run the `__exit__` phase of a context manager commenced with `push_cmgr`.
 Restore `attr` as it was before `push_cmgr`.
 Return the result of `__exit__`.
 
 ## Function `popattrs(o, attr_names, old_values)`
@@ -143,27 +211,27 @@
     >>> assert not hasattr(obj, 'path')
     >>> assert not isdirpath(dirpath)
 
 ## Function `pushattrs(o, **attr_values)`
 
 The "push" part of `stackattrs`.
 Push `attr_values` onto `o` as attributes,
-return the previous attribute values in a dict.
+return the previous attribute values in a `dict`.
 
 This can be useful in hooks/signals/callbacks,
 where you cannot inline a context manager.
 
-## Function `pushkeys(d, **key_values)`
+## Function `pushkeys(d, kv=None, **kw)`
 
 The "push" part of `stackkeys`.
-Push `key_values` onto `d` as key values.
-return the previous key values in a dict.
+Use the mapping provided as `kv` or `kw` to update `d`.
+Return the previous key values in a `dict`.
 
 This can be useful in hooks/signals/callbacks,
-where you cannot inline a context manager.
+where you cannot inline a context manager using `stackkeys`.
 
 ## Function `reconfigure_file(f, **kw)`
 
 Context manager flavour of `TextIOBase.reconfigure`.
 
 ## Function `setup_cmgr(cmgr)`
 
@@ -226,25 +294,25 @@
 apply a handler which calls both the new handler and the old handler.
 
 ## Function `stackattrs(o, **attr_values)`
 
 Context manager to push new values for the attributes of `o`
 and to restore them afterward.
 Returns a `dict` containing a mapping of the previous attribute values.
-Attributes not present are not present in returned mapping.
+Attributes not present are not present in the returned mapping.
 
 Restoration includes deleting attributes which were not present
 initially.
 
 This makes it easy to adjust temporarily some shared context object
 without having to pass it through the call stack.
 
 See `stackkeys` for a flavour of this for mappings.
 
-See `cs.threads.State` for a convenient wrapper class.
+See `cs.threads.ThreadState` for a convenient wrapper class.
 
 Example of fiddling a programme's "verbose" mode:
 
     >>> class RunModes:
     ...     def __init__(self, verbose=False):
     ...         self.verbose = verbose
     ...
@@ -287,18 +355,19 @@
     >>> print(o.a)
     1
     >>> print(o.b)
     Traceback (most recent call last):
       File "<stdin>", line 1, in <module>
     AttributeError: 'O' object has no attribute 'b'
 
-## Function `stackkeys(d, **key_values)`
+## Function `stackkeys(d, kv=None, **kw)`
 
-Context manager to push new values for the key values of `d`
+A context manager to push new values for the key values of `d`
 and to restore them afterward.
+The new values are provided as `kv` or `kw` as convenient.
 Returns a `dict` containing a mapping of the previous key values.
 Keys not present are not present in the mapping.
 
 Restoration includes deleting key values which were not present
 initially.
 
 This makes it easy to adjust temporarily some shared context object
@@ -367,17 +436,20 @@
 
     @contextmanager
     def my_cmgr_func(...):
         ...
         yield
         ...
 
-then the correct use of `twostep()` is:
+then `my_cmgr_func(...)` returns a context manager instance
+and so the correct use of `twostep()` is like this:
 
-    cmgr_iter = twostep(my_cmgr_func(...))
+    # steps broken out for clarity
+    cmgr = my_cmgr_func(...)
+    cmgr_iter = twostep(cmgr)
     next(cmgr_iter)   # set up
     next(cmgr_iter)   # tear down
 
 and _not_:
 
     cmgr_iter = twostep(my_cmgr_func)
     next(cmgr_iter)   # set up
@@ -394,18 +466,40 @@
             self._cmgr_stepped = twostep(stackattrs(o, setting=foo))
             self._cmgr = next(self._cmgr_stepped)
             return self._cmgr
         def __exit__(self, *_):
             next(self._cmgr_stepped)
             self._cmgr = None
 
+## Function `withall(objs)`
+
+Enter every object `obj` in `obj_list` except those which are `None`
+using `with obj:`, then yield.
+
+## Function `withif(obj)`
+
+Return a context manager for `obj`.
+If `obj` has an `__enter__` attribute, return `obj`
+otherwise return `nullcontext()`.
+
+Example:
+
+    with withif(inner_mapping):
+      ... work with inner_mapping ...
+
 # Release Log
 
 
 
+*Release 20240412*:
+* contextif: rework to be much easier to use, add new call modes.
+* pushkeys, stackkeys: support update dicts whose keys are not identifier strings i.e. a non **kw call mode.
+* New withif() function returning a context manager even for objects which do not provide one.
+* New withall(iterable-of-context-managers) context manager.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240212.1*:
 Minor doc updates.
 
 *Release 20240212*:
```

### Comparing `cs.context-20240316/pyproject.toml` & `cs.context-20240412/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,51 +4,97 @@
 authors = [
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python2",
     "python3",
 ]
-dependencies = []
+dependencies = [
+    "cs.gimmicks>=20240316",
+]
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
-version = "20240316"
+version = "20240412"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Assorted context managers.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
-
-## Function `contextif(flag, cmgr_func, *cmgr_args, **cmgr_kwargs)`
+*Latest release 20240412*:
+* contextif: rework to be much easier to use, add new call modes.
+* pushkeys, stackkeys: support update dicts whose keys are not identifier strings i.e. a non **kw call mode.
+* New withif() function returning a context manager even for objects which do not provide one.
+* New withall(iterable-of-context-managers) context manager.
+
+## Function `contextif(cmgr, *cmgr_args, **cmgr_kwargs)`
+
+A context manager to use `cmgr` conditionally,
+with a flexible call signature.
+This yields the context manager if `cmgr` is used or `None`
+if it is not used, allowing the enclosed code to test whether
+the context is active.
 
-A context manager to call `cmgr_func(*cmgr_args,**cmgr_kwargs)`
-if `flag` is true, otherwise to call `nullcontext()`.
+This is to ease uses where the context object is optional
+i.e. `None` if not present. Example from `cs.vt.stream`:
 
-The driving use case is verbosity dependent status lines or
-progress bars, eg:
+    @contextmanager
+    def startup_shutdown(self):
+      \"\"\" Open/close `self.local_store` if not `None`.
+      \"\"\"
+      with super().startup_shutdown():
+        with contextif(self.local_store):
+          with self._packet_connection(self.recv, self.send) as conn:
+            with stackattrs(self, _conn=conn):
+              yield
+
+Here `self.local_store` might be `None` if there's no local
+store to present. We still want a nice nested `with` statement
+during the setup. By using `contextif` we run a context manager
+which behaves correctly when `self.local_store=None`.
+
+The signature is flexible, offering 2 basic modes of use.
+
+Flagged use: `contextif(flag,cmgr,*a,**kw)`: if `flag` is a
+Boolean then it governs whether the context manager `cmgr`
+is used. Historically the driving use case was verbosity
+dependent status lines or progress bars. Example:
 
     from cs.upd import run_task
     with contextif(verbose, run_task, ....) as proxy:
-      ... do stuff, updating proxy if not None ...
+        ... do stuff, updating proxy if not None ...
+
+Unflagged use: `contextif(cmgr,*a,**kw)`: use `cmgr` as the
+flag: if false (eg `None`) then `cmgr` is not used.
+
+Additionally, `cmgr` may be a callable, in which case the
+context manager itself is obtained by calling
+`cmgr,*cmgr_args,**cmgr_kwargs)`. Otherwise `cmgr` is assumed
+to be a context manager already, and it is an error to provide
+`cmgr_args` or `cmgr_kwargs`.
+
+In the `cs.upd` example above, `run_task` is a context manager
+function which pops up an updatable status line, normally
+used as:
+
+    with run_task(\"doing thing\") as proxy:
+        ... do the thing, setting proxy.text as needed ...
 
 ## Class `ContextManagerMixin`
 
 A mixin to provide context manager `__enter__` and `__exit__` methods
 running the first and second steps of a single `__enter_exit__` generator method.
 
 *Note*: the `__enter_exit__` method is _not_ a context manager,
@@ -91,14 +137,38 @@
             except SomeException as e:
                 ... handle e ...
                 exit_result = True
             finally:
                 ... do tear down here ...
             yield exit_result
 
+*Method `ContextManagerMixin.__enter__(self)`*:
+Run `super().__enter__` (if any)
+then the `__enter__` phase of `self.__enter_exit__()`.
+
+*Method `ContextManagerMixin.__exit__(self, exc_type, exc_value, traceback)`*:
+Run the `__exit__` step of `self.__enter_exit__()`,
+then `super().__exit__` (if any).
+
+*Method `ContextManagerMixin.as_contextmanager(self)`*:
+Run the generator from the `cls` class specific `__enter_exit__`
+method via `self` as a context manager.
+
+Example from `RunState` which subclasses `HasThreadState`,
+both of which are `ContextManagerMixin` subclasses:
+
+    class RunState(HasThreadState):
+        .....
+        def __enter_exit__(self):
+            with HasThreadState.as_contextmanager(self):
+                ... RunState context manager stuff ...
+
+This runs the `HasThreadState` context manager
+around the main `RunState` context manager.
+
 ## Function `pop_cmgr(o, attr)`
 
 Run the `__exit__` phase of a context manager commenced with `push_cmgr`.
 Restore `attr` as it was before `push_cmgr`.
 Return the result of `__exit__`.
 
 ## Function `popattrs(o, attr_names, old_values)`
@@ -155,27 +225,27 @@
     >>> assert not hasattr(obj, 'path')
     >>> assert not isdirpath(dirpath)
 
 ## Function `pushattrs(o, **attr_values)`
 
 The \"push\" part of `stackattrs`.
 Push `attr_values` onto `o` as attributes,
-return the previous attribute values in a dict.
+return the previous attribute values in a `dict`.
 
 This can be useful in hooks/signals/callbacks,
 where you cannot inline a context manager.
 
-## Function `pushkeys(d, **key_values)`
+## Function `pushkeys(d, kv=None, **kw)`
 
 The \"push\" part of `stackkeys`.
-Push `key_values` onto `d` as key values.
-return the previous key values in a dict.
+Use the mapping provided as `kv` or `kw` to update `d`.
+Return the previous key values in a `dict`.
 
 This can be useful in hooks/signals/callbacks,
-where you cannot inline a context manager.
+where you cannot inline a context manager using `stackkeys`.
 
 ## Function `reconfigure_file(f, **kw)`
 
 Context manager flavour of `TextIOBase.reconfigure`.
 
 ## Function `setup_cmgr(cmgr)`
 
@@ -238,25 +308,25 @@
 apply a handler which calls both the new handler and the old handler.
 
 ## Function `stackattrs(o, **attr_values)`
 
 Context manager to push new values for the attributes of `o`
 and to restore them afterward.
 Returns a `dict` containing a mapping of the previous attribute values.
-Attributes not present are not present in returned mapping.
+Attributes not present are not present in the returned mapping.
 
 Restoration includes deleting attributes which were not present
 initially.
 
 This makes it easy to adjust temporarily some shared context object
 without having to pass it through the call stack.
 
 See `stackkeys` for a flavour of this for mappings.
 
-See `cs.threads.State` for a convenient wrapper class.
+See `cs.threads.ThreadState` for a convenient wrapper class.
 
 Example of fiddling a programme's \"verbose\" mode:
 
     >>> class RunModes:
     ...     def __init__(self, verbose=False):
     ...         self.verbose = verbose
     ...
@@ -299,18 +369,19 @@
     >>> print(o.a)
     1
     >>> print(o.b)
     Traceback (most recent call last):
       File \"<stdin>\", line 1, in <module>
     AttributeError: 'O' object has no attribute 'b'
 
-## Function `stackkeys(d, **key_values)`
+## Function `stackkeys(d, kv=None, **kw)`
 
-Context manager to push new values for the key values of `d`
+A context manager to push new values for the key values of `d`
 and to restore them afterward.
+The new values are provided as `kv` or `kw` as convenient.
 Returns a `dict` containing a mapping of the previous key values.
 Keys not present are not present in the mapping.
 
 Restoration includes deleting key values which were not present
 initially.
 
 This makes it easy to adjust temporarily some shared context object
@@ -379,17 +450,20 @@
 
     @contextmanager
     def my_cmgr_func(...):
         ...
         yield
         ...
 
-then the correct use of `twostep()` is:
+then `my_cmgr_func(...)` returns a context manager instance
+and so the correct use of `twostep()` is like this:
 
-    cmgr_iter = twostep(my_cmgr_func(...))
+    # steps broken out for clarity
+    cmgr = my_cmgr_func(...)
+    cmgr_iter = twostep(cmgr)
     next(cmgr_iter)   # set up
     next(cmgr_iter)   # tear down
 
 and _not_:
 
     cmgr_iter = twostep(my_cmgr_func)
     next(cmgr_iter)   # set up
@@ -406,18 +480,40 @@
             self._cmgr_stepped = twostep(stackattrs(o, setting=foo))
             self._cmgr = next(self._cmgr_stepped)
             return self._cmgr
         def __exit__(self, *_):
             next(self._cmgr_stepped)
             self._cmgr = None
 
+## Function `withall(objs)`
+
+Enter every object `obj` in `obj_list` except those which are `None`
+using `with obj:`, then yield.
+
+## Function `withif(obj)`
+
+Return a context manager for `obj`.
+If `obj` has an `__enter__` attribute, return `obj`
+otherwise return `nullcontext()`.
+
+Example:
+
+    with withif(inner_mapping):
+      ... work with inner_mapping ...
+
 # Release Log
 
 
 
+*Release 20240412*:
+* contextif: rework to be much easier to use, add new call modes.
+* pushkeys, stackkeys: support update dicts whose keys are not identifier strings i.e. a non **kw call mode.
+* New withif() function returning a context manager even for objects which do not provide one.
+* New withall(iterable-of-context-managers) context manager.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240212.1*:
 Minor doc updates.
 
 *Release 20240212*:
```

